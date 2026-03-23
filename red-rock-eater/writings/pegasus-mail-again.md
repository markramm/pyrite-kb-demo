---
id: pegasus-mail-again
title: Pegasus mail again
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1997/Pegasus.mail.again.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - administrative
  - auto-imported
  - forwarded-content
  - government-info
  - international
  - internet-policy
  - law
  - libraries
  - rre
  - rre-post
  - telecommunications
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/Pegasus.mail.again.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991004203858/http://www.somewhere.com/)

  

# Pegasus mail again

```
[Note that the second of these messages, which is highly recommended, was
sent on Wednesday, New Zealand time.  No sooner did David Harris, highly
principled software developer, add features to Pegasus Mail that made it
easy to detect spam sent with his program than the US Government, in the
very CIAC alert whose URL I provided in a message the other day, declared
Pegasus to be spam software, leading many people to set their mail filters
to reject all messages that are sent with it.  Likewise, when Sanford
Wallace and his partners announced that they were setting up a company to
create a spam-friendly Internet backbone, anti-spammers started calling
people whose names are similar to those of Wallace's partners, and people
whose company names are similar to Wallace's, on the telephone at 4AM.
(Source: news.com.)  Fortunately those people happen to hate spam as much
as anybody.  Still, damage was done to the cause.  Lesson to be learned:
In the war against spam, it is really important to Get Your Facts Straight.
You shouldn't let that stop you from reporting suspicious spam messages
to the appropriate authorities, however.  Just stick with the facts that
you know for sure (e.g., that you received a particular message and found
it suspicious), and that will be plenty.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date sent:        Thu, 20 Nov 1997 21:20:45 +1200
From:             David Harris 
Send reply to:    Pegasus Mail Announcements 
Organization:     Pegasus Mail, Dunedin, New Zealand
Subject:          Impending release of WinPMail v2.55
To:               PM-NEWS@UA1VM.UA.EDU

Within the next 72 hours, we will be releasing Pegasus Mail for Windows
v2.55: this version will be identical to the current formal v2.54 release
except that it will not generate headers in outgoing messages that
identify the message as having been sent using Pegasus Mail. 

I deeply regret having to take this step, since some of the headers we
have removed are valuable diagnostic tools for us; but the simple reality
here is that through ignorance, many people have begun associating Pegasus
Mail with spam and that is simply not a tenable position for us. It is
patently unreasonable to have millions of legitimate Pegasus Mail users
handicapped by the antisocial actions of a tiny fraction of one percent of
the userbase, and even worse, by the ignorance of people who should know
better but have not taken the time to become properly-informed. Note that
Pegasus Mail WILL continue to generate its spam-identification "X-
Distribution:" headers, so filtering schemes based on these reasonable
mechanisms will continue to work. 

What really burns me up most about this whole issue is the way that I keep
getting victimized through trying to be a responsible developer. 
Statistics we have gathered on spam indicate that nearly as many spams are
sent with Eudora and Netscape respectively as are sent with Pegasus Mail,
yet you don't see ISPs refusing to pass mail from them... I'm tired of
being the whipping boy for a problem that is social in nature, not
technical.  Spam is not currently illegal, and there's basically nothing
anyone can do about it until it becomes illegal. 

We strongly urge all current v2.54 users to download v2.55 when it becomes
available, so that they will not be affected by the maverick filtering
actions of a few ill-informed people. 

Cheers!

-- David --

------------------ David Harris -+- Pegasus Mail

---

  Box 5451, Dunedin, New Zealand | e-mail: David.Harris@pmail.gen.nz
           Phone: +64 3 453-6880 | Fax: +64 3 453-6612

Thought for the day:
    Erotic (adj): using a feather as a sex aid.
    Kinky (adj):  using the whole duck.

Date sent:        Wed, 26 Nov 1997 01:52:34 +1200
From:             David Harris <David.Harris@pmail.gen.nz>
Send reply to:    Pegasus Mail Announcments <PM-NEWS@UA1VM.UA.EDU>
Organization:     Pegasus Mail, Dunedin, New Zealand
Subject:          Pegasus Mail for Windows v2.55
To:               PM-NEWS@UA1VM.UA.EDU

Pegasus Mail for Windows v2.55 is now available from the following sites:

Via FTP:
        risc.ua.edu, in /pegasus  (North America)
        ftp.let.rug.nl in /pegasus  (Europe)
        ftp.usm.maine.edu, in /pub/network/pegasus  (North America)
        pegasus.topnz.ac.nz, in /pegasus  (South Pacific)

If using a web browser, use these URLs:
        http://risc.ua.edu/pegasus
        http://www.let.rug.nl/pegasus
        ftp://ftp.usm.maine.edu/pub/network/pegasus
        ftp://pegasus.topnz.ac.nz/pegasus

Both 16- and 32-bit versions are available: the filenames are
WINPM255.EXE for the 16-bit version, and W32-255.EXE for the 32-bit
version.V2.55 is identical to the v2.54 release except that it no longer
generates the following headers in outgoing Internet mail:

   X-Mailer: Pegasus Mail [version]
   Comments: Authenticated sender is <pop3address>

The reason these headers have been removed is because some Internet
Service Providers and System Administrators have begun using them to
reject or filter out mail in the mistaken belief that Pegasus Mail is a
package designed for the distribution of "spam" (unsolicited bulk
commercial e-mail). Clearly we cannot tolerate a situation where Pegasus
Mail and its users are victimized through ignorance - the viability of the
program could be in question if such indiscriminate rejection were
permitted to occur.

A part of the basis for this discrimination is a recent bulletin from CIAC
(the U.S. Department of Energy's Computer Incident Alert service) in which
Pegasus Mail was erroneously described as a bulk mail package. The author
of that bulletin has now indicated that this was an error and that he will
reissue the bulletin. Unfortunately, the damage has largely been done.

We believe that the amount of mail affected by this kind of descriminatory
filtering is very small at present, but are releasing v2.55 as a means of
circumventing the problem where it arises. If you are not currently having
any problems with rejection of your mail (the likely scenario for the vast
majority of users) then v2.55 gains you no advantages over v2.54 and you
need not download it.

To say that I am angry and upset that it should be necessary for me to make
this release is a terrific understatement - especially since I am currently
the ONLY major e-mail developer with a strong anti-spam stance. It seems
preposterous and ironic to me that I alone seem to have been singled out in
this way.

Now that spam has done me and my users real, personal damage, my
loathing of it, and the people who so blithely dump it on the Internet
without any concern for whom they may inconvenience or hurt has deepened,
as has my resolve to find ways of doing what I can to combat it. But I
stress that I believe firmly that spam is a social problem and cannot be
overcome by technical means - it can only be dealt with through the normal
channel of social regulation, the law.

It is my hope that this will only be a temporary measure, and that I will
be able to restore the X-Mailer header in particular in an upcoming
revision, once this issue has been properly resolved. Pegasus Mail has
carried its X-Mailer header proudly to all parts of the world for nearly
eight years now, and I feel a profound loss at removing it.

I appreciate the expressions of support I have received from my userbase in
response to my previous postings on this matter - I apologise if many of
you did not receive a personal response, but I was essentially overwhelmed
by the volume. In light of this, although I am deeply appreciative of your
solicitude, I would ask that you do not send me supportive messages for
this announcement - I really, really need to get on and start doing some
real work again, having effectively wasted more than a week struggling with
these issues.

Once again, my thanks to all for their ongoing support and for
understanding the reasons why I have had to take such an unusual and
painful step in making this release.

-- David Harris --
Author/Owner, Pegasus Mail System.

------------------ David Harris -+- Pegasus Mail --------------------------
  Box 5451, Dunedin, New Zealand | e-mail: David.Harris@pmail.gen.nz
           Phone: +64 3 453-6880 | Fax: +64 3 453-6612

Real newspaper headlines from US Papers:
   "State to punish duck violators".
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991004203858/http://www.somewhere.com/)