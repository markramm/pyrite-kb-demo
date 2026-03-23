---
id: outer-space-and-security-holes
title: outer space and security holes
type: writing
writing_type: rre-post
date: 1997-12-07
url: http://commons.somewhere.com:80/rre/1997/outer.space.and.security.html
coauthors: []
key_concepts: []
importance: 7
research_status: partial
tags:
  - administrative
  - auto-imported
  - education
  - forwarded-content
  - international
  - internet-policy
  - labor
  - law
  - libraries
  - media
  - military
  - rre
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/outer.space.and.security.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20001018075401/http://commons.somewhere.com/rre/) | **Most Recent Article: Tue, 17 Oct 2000** |

# outer space and security holes

```
[It seemed appropriate for these four messages to appear in the same
issue of the venerable Risks Digest.  Two of them concern problems with
computer code from earth being sent into outer space, and the other two
concern computer code from outer space trashing your computer on earth.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Tue, 9 Dec 1997 13:48:08 -0800 (PST)
From: risks@csl.sri.com

RISKS-LIST: Risks-Forum Digest  Tuesday 9 December 1997  Volume 19 : Issue 49

---

Date: Sunday, December 07, 1997 6:47 PM
From: Mike Jones <mbj@MICROSOFT.com>
Subject: What really happened on Mars Rover Pathfinder

The Mars Pathfinder mission was widely proclaimed as "flawless" in the early
days after its July 4th, 1997 landing on the Martian surface.  Successes
included its unconventional "landing" -- bouncing onto the Martian surface
surrounded by airbags, deploying the Sojourner rover, and gathering and
transmitting voluminous data back to Earth, including the panoramic pictures
that were such a hit on the Web.  But a few days into the mission, not long
after Pathfinder started gathering meteorological data, the spacecraft began
experiencing total system resets, each resulting in losses of data.  The
press reported these failures in terms such as "software glitches" and "the
computer was trying to do too many things at once".

This week at the IEEE Real-Time Systems Symposium I heard a fascinating
keynote address by David Wilner, Chief Technical Officer of Wind River
Systems.  Wind River makes VxWorks, the real-time embedded systems kernel
that was used in the Mars Pathfinder mission.  In his talk, he explained in
detail the actual software problems that caused the total system resets of
the Pathfinder spacecraft, how they were diagnosed, and how they were
solved.  I wanted to share his story with each of you.

VxWorks provides preemptive priority scheduling of threads.  Tasks on the
Pathfinder spacecraft were executed as threads with priorities that were
assigned in the usual manner reflecting the relative urgency of these tasks.

Pathfinder contained an "information bus", which you can think of as a
shared memory area used for passing information between different components
of the spacecraft.  A bus management task ran frequently with high priority
to move certain kinds of data in and out of the information bus.  Access to
the bus was synchronized with mutual exclusion locks (mutexes).

The meteorological data gathering task ran as an infrequent, low priority
thread, and used the information bus to publish its data.  When publishing
its data, it would acquire a mutex, do writes to the bus, and release the
mutex.  If an interrupt caused the information bus thread to be scheduled
while this mutex was held, and if the information bus thread then attempted
to acquire this same mutex in order to retrieve published data, this would
cause it to block on the mutex, waiting until the meteorological thread
released the mutex before it could continue.  The spacecraft also contained
a communications task that ran with medium priority.

Most of the time this combination worked fine.  However, very infrequently
it was possible for an interrupt to occur that caused the (medium priority)
communications task to be scheduled during the short interval while the
(high priority) information bus thread was blocked waiting for the (low
priority) meteorological data thread.  In this case, the long-running
communications task, having higher priority than the meteorological task,
would prevent it from running, consequently preventing the blocked
information bus task from running.  After some time had passed, a watchdog
timer would go off, notice that the data bus task had not been executed for
some time, conclude that something had gone drastically wrong, and initiate
a total system reset.

This scenario is a classic case of priority inversion.

HOW WAS THIS DEBUGGED?

VxWorks can be run in a mode where it records a total trace of all
interesting system events, including context switches, uses of
synchronization objects, and interrupts.  After the failure, JPL engineers
spent hours and hours running the system on the exact spacecraft replica in
their lab with tracing turned on, attempting to replicate the precise
conditions under which they believed that the reset occurred.  Early in the
morning, after all but one engineer had gone home, the engineer finally
reproduced a system reset on the replica.  Analysis of the trace revealed
the priority inversion.

HOW WAS THE PROBLEM CORRECTED?

When created, a VxWorks mutex object accepts a boolean parameter that
indicates whether priority inheritance should be performed by the mutex.
The mutex in question had been initialized with the parameter off; had it
been on, the low-priority meteorological thread would have inherited the
priority of the high-priority data bus thread blocked on it while it held
the mutex, causing it be scheduled with higher priority than the
medium-priority communications task, thus preventing the priority inversion.
Once diagnosed, it was clear to the JPL engineers that using priority
inheritance would prevent the resets they were seeing.

VxWorks contains a C language interpreter intended to allow developers to
type in C expressions and functions to be executed on the fly during system
debugging.  The JPL engineers fortuitously decided to launch the spacecraft
with this feature still enabled.  By coding convention, the initialization
parameter for the mutex in question (and those for two others which could
have caused the same problem) were stored in global variables, whose
addresses were in symbol tables also included in the launch software, and
available to the C interpreter.  A short C program was uploaded to the
spacecraft, which when interpreted, changed the values of these variables
from FALSE to TRUE.  No more system resets occurred.

ANALYSIS AND LESSONS

First and foremost, diagnosing this problem as a black box would have been
impossible.  Only detailed traces of actual system behavior enabled the
faulty execution sequence to be captured and identified.

Secondly, leaving the "debugging" facilities in the system saved the day.
Without the ability to modify the system in the field, the problem could not
have been corrected.

Finally, the engineer's initial analysis that "the data bus task executes
very frequently and is time-critical -- we shouldn't spend the extra time in
it to perform priority inheritance" was exactly wrong.  It is precisely in
such time critical and important situations where correctness is essential,
even at some additional performance cost.

HUMAN NATURE, DEADLINE PRESSURES

David told us that the JPL engineers later confessed that one or two system
resets had occurred in their months of pre-flight testing.  They had never
been reproducible or explainable, and so the engineers, in a very
human-nature response of denial, decided that they probably weren't
important, using the rationale "it was probably caused by a hardware
glitch".

Part of it too was the engineers' focus.  They were extremely focused on
ensuring the quality and flawless operation of the landing software.  Should
it have failed, the mission would have been lost.  It is entirely
understandable for the engineers to discount occasional glitches in the
less-critical land-mission software, particularly given that a spacecraft
reset was a viable recovery strategy at that phase of the mission.

THE IMPORTANCE OF GOOD THEORY/ALGORITHMS

David also said that some of the real heroes of the situation were some
people from CMU who had published a paper he'd heard presented many years
ago who first identified the priority inversion problem and proposed the
solution.  He apologized for not remembering the precise details of the
paper or who wrote it.  Bringing things full circle, it turns out that the
three authors of this result were all in the room, and at the end of the
talk were encouraged by the program chair to stand and be acknowledged.
They were Lui Sha, John Lehoczky, and Raj Rajkumar.  When was the last time
you saw a room of people cheer a group of computer science theorists for
their significant practical contribution to advancing human knowledge? :-)
It was quite a moment.

POSTLUDE

For the record, the paper was:

L. Sha, R. Rajkumar, and J. P. Lehoczky. Priority Inheritance Protocols: An
Approach to Real-Time Synchronization. In IEEE Transactions on Computers,
vol. 39, pp. 1175-1185, Sep. 1990.

---

Date: Tue, 9 Dec 1997 22:25:43 +0100
From: "Philip N. Gross" <philg@bart.nl>
Subject: Potential software nightmare for International Space Station

After reading the 8 Dec 1997 *Aviation Week and Space Technology* cover
story <http://www.aviationweek.com/aviation/avi_stor.htm>, I have grave
doubts about the software stability of the enormously complex International
Space Station.  A few months of testing in a simulated environment and up
goes 3.5 million lines of code, developed by independent teams dispersed
worldwide.  The low-tech Mir with its straightforward computer failures may
one day be day be remembered nostalgically.  [PGN Excerpting:]

  The initial power-on testing of the U.S. Laboratory Module began at
  Marshall in early November 1997 and is planned to last into early 1998.
  Although the Lab Module is not to be launched until the fifth shuttle
  assembly flight, set for May 1999, it has the potential of affecting ISS
  launch scheduling much earlier because the Lab will be the electronic hub
  of the station and its software must be tested at Kennedy in connection
  with the two assembly flight payloads that precede it.  This critical
  Multiple Element Integrated Test (MEIT), set between September-December
  1998, will link the ISS software and hardware for shuttle assembly flights
  3A, 4A and 5A, requiring that software be developed well in advance of
  these tests.  The MEIT requirements, combined with training requirements
  for the first ISS crew, are creating a "huge tidal wave of software" [...]- The hardware to be linked includes the Z-1 truss carrying electrical and
    fluid systems; the massive U.S. Photovoltaic Module power system, and
    simulated Node-1 avionics.- There are at least 3.5 million lines of code from multiple U.S., Russian,
      European, Canadian and Japanese contractors, ``the most diverse software
      of any aerospace program ever conceived.''- ``Everything is interrelated.  One thing affects the other and we have
        some very complex integrated schedules.  Software clearly has the
        potential for delaying the launch of the Laboratory Module and subsequent
        flights.''

      ---

      Date: 28 Nov 1997 03:21:42 GMT
      From: "braz" <braz@mnw.net>
      Subject: Beware of HTML Mail

      I received a spam mail today that was rather sinister.  Many spams that I
      receive request that you click on the hyperlink to go to their site.  This
      one, however, was much different.  I am running IE4.0, and I simply
      highlighted the new message in my mailbox, and clicked on the subject to
      read it.  It immediately downloaded and initialized a java applet that took
      control of my browser, opened a session to their site as I sat in amazement.
      I then quickly (out of fear) stopped the connection to that site, went back
      to the mail message and viewed the source to see what was in it. Here is the
      first few lines of the mail - I numbered the lines so they won't be
      interpreted as HTML/E-mail here:

      1. <html>
      2. <head>
      3. <title>webtour</title>
      4. </head>
      5. <body>
      6. <applet
       7.    code=sitewalk.class
       8.    codebase=http://www.netinstrument.com/applet
       9.    name=sitewalk
      10.    width=2
       11.   height=2 >
      12. <param name="page1" value="jpg, , 300, 200, 4000, ,
      start-http://www.netinstrument.com/email2.htm, -, -, -, -, -, -, -, -, -, ">
      (line 12 repeated for various links at their site)

      I never really cared much about the spam I received, because it was really
      non-intrusive for the most part. This, however, was scary. It took control
      of my IE4 Browser, and forced me to their site. Who knows what the sites web
      pages do if you let it run its course.

      Net users, beware. The risks of simply receiving spam have just skyrocketed.
      Turn off auto-preview mode, and look at the source of the message prior to
      opening the mail item.  I never cared about this before, but I really feel
      violated in some weird electronic sense.

      Tom Brazil <braz@mnw.net>

      ---

      Date: Sat, 6 Dec 1997 17:46:31 +1100
      From: Geoffrey King <geoff@austlii.edu.au>
      Subject: Microsoft, CNET, BUGTRAQ and the 'land' attack (Milunovic, R-19.48)

      I wish to point out the RISKS of relying on poorly researched media reports
      for information about security ...

      The previous issue of RISKS contained a report passed on from the CNET news
      service about the 'land' attack. The CNET report which appears at
      <http://www.news.com/News/Item/0%2C4%2C17009%2C00.html> carries a date of 4
      Dec 1997 at 5pm PST.

      For a start, the way in which the article was written indicates a general
      misunderstanding of the bug and the possible exploitation thereof.

      More seriously, the article also appears some 14 days after the first
      posting (including exploit code) of the 'land' vulnerability to the BUGTRAQ
      list. But todays "news" does coincide quite nicely with the announcement
      that Microsoft would release patches. And please also note that the
      statement of "Jason Grams, a product manager at Microsoft", that
      "[o]bviously, this isn't a Microsoft-only problem, it's a pretty big
      problem" is not entirely accurate. There are a number of operating systems
      which are not vulnerable to this attack, including current releases of
      Linux, Solaris, Irix, OS/2 and others ... other vendors, including CISCO,
      acted immediately to warn of and patch vulnerabilities in their products.

      Wired News published an excellent article as early as 21 Nov 1997.
      <http://www.wired.com/news/news/technology/story/8707.html>

      While I'm writing about this particular problem, I might also quote from a
      Microsoft executive asked recently about the possibility that the Internet
      Explorer 'res://' bug and the Pentium bug could be combined.

          "It's not as simple as sitting down at an IE4 machine. We've
          tried it on several [machines] and we get a crash but that's
          it, which is certainly not a security hole," he said.

          <http://www.wired.com/news/news/technology/story/8429.html>

      Is that really acceptable coming from a major OS vendor?

      A demonstration of the exploitation of the 'res://' Internet Explorer bug in
      combination with the recently discussed Pentium bug is available at
      <http://www.ee.surrey.ac.uk/Personal/L.Wood/IE4res/> [WARNING: this
      demonstration may crash your machine].

      And here's a quote from a Microsoft technical note about security risks in
      Windows95 file and print sharing:

          "The SMBCLIENT Samba network client allows users to send illegal
          networking commands over the network. At this time, the Samba
          client is the only known SMBCLIENT that does not filter out such
          illegal commands. SMBCLIENT users do not automatically gain access
          to the Windows 95 drive; these users must know the exact steps to
          send these illegal commands."

          <http://premium.microsoft.com/support/kb/articles/q128/0/79.asp>

          Glossary: Samba <http://samba.anu.edu.au/> is an implementation of
                    the SMB protocols to allow UNIX servers to be used in a
                    Microsoft environment, as both servers and clients.

      Does anybody here want to volunteer for a trip to Seattle to explain to the
      Microsoft 'engineers' that client-server security mechanisms probably
      shouldn't rely on the good behaviour of the clients ??

      It looks to me like it might be time to encourage a little more genetic
      diversity in operating systems ... let's not build the world around this sort
      of nonsense ...

      Hmmm ... and does anybody here still think todays "news" is news ??

      Geoffrey King <www.homosapiens.org>, Australasian Legal Information Institutea
      Faculty of Law, University of Technology, Sydney  +61(2) 9514 3176

      ---

      End of RISKS-FORUM Digest 19.49 

      ---

      Standard Risks reuse disclaimer:

        Reused without explicit authorization under blanket 
        permission granted for all Risks-Forum Digest materials.  
        The author(s), the RISKS moderator, and the ACM have no 
        connection with this reuse.
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20001018075401/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20001018075401/mailto:webmaster@somewhere.com). |