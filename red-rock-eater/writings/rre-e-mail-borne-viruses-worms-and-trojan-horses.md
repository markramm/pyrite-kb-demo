---
id: rre-e-mail-borne-viruses-worms-and-trojan-horses
title: "[RRE]e-mail borne viruses, worms, and Trojan horses"
type: writing
writing_type: rre-post
date: 1999-06-17
url: http://commons.somewhere.com:80/rre/1999/RRE.e-mail.borne.viruses.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - rre
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1999/RRE.e-mail.borne.viruses.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991008065129/http://www.somewhere.com/)

  

# [RRE]e-mail borne viruses, worms, and Trojan horses

```
[I am astonished that the whole global economy is becoming dependent on
a technology that is so fundamentally shoddy.  Not only is it offensive
from an engineer standpoint, it is also a serious political matter: if
we decide to build our economic system on top of technology that is so
completely open to attack then we might as well establish a world-wide
military dictatorship right now, because that's going to be the only
way to prevent civilization from being overwhelmed by barbarians.
Bruce Schneier's message is forwarded by permission and reformatted.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html
or send a message to requests@lists.gseis.ucla.edu with Subject: info rre

---

Date: Thu, 17 Jun 1999 08:01:29 -0700 (PDT)
From: risks@csl.sri.com

RISKS-LIST: Risks-Forum Digest  Thursday 17 June 1999  Volume 20 : Issue 45

---

Date: Tue, 15 Jun 1999 16:48:25 -0500
From: Bruce Schneier <schneier@counterpane.com>
Subject: Risks of e-mail borne viruses, worms, and Trojan horses"

Looking back from the future, 1999 will have been a pivotal year for
malicious software: viruses, worms, and Trojan horses (collectively
known as "malware").  It's not more malware; we've already seen
thousands.  It's not Internet malware; we've seen those before, tool.
But this is the first year we've seen malware that uses e-mail to
propagate over the Internet and tunnel through firewalls.  And it's a
really big deal.

Viruses and worms survive by reproducing on new computers.  Before
the Internet, computers communicated was through floppy disks.  Hence,
most viruses propagated on floppy disks, and sometimes on computer
bulletin board systems (BBSs).

There are some obvious effects of floppies as a vector.  First,
malware propagates slowly.  One computer shares a disk with another
which shares a disk with five more, and over the course of weeks
or months a virus turns into an epidemic.  Or maybe someone puts a
virus-infected program on a bulletin board, and thousands get infected
in a week or two.

Second, it's easy to block disk-borne malware.  Most anti-virus
programs can automatically scan all floppy disks.  Malware is blocked
at the gate.  BBSs can still be a problem, but many computer users are
trained never to download software from a BBS.  Even so, anti-virus
software can automatically scan new files for malware.

And third, anti-viral software can easily deal with the problem.  It's
easy to write software to block malware you know about.  You simply
have the anti-virus scanner search for bit strings that signify the
virus (called a "signature") and then execute the automatic program
to delete the virus and restore normalcy.  This deletion routine is
unique per virus, but it is not hard to develop.  Anti-viral software
has tens of thousands of signatures, each tuned to a particular virus.
Companies release them within a day of learning of a new virus.  And
as long as viruses propagate slowly, this is good enough.  My software
automatically updates itself once a month.  Until 1999, that was
enough.

What's new in 1999 is e-mail propagation of malware.  These programs
-- the Melissa virus and its variants, Worm.ExploreZip worm and its
inevitable variants, etc. -- arrive via e-mail and use e-mail features
in modern software to replicate themselves across the network.
They mail themselves to people known to the infected host, enticing
the recipients to open or run them.  They don't propagate over weeks
and months; they propagate in seconds.  Anti-viral software cannot
possibly keep up.

And e-mail is everywhere.  It runs over Internet connections that
block everything else.  It tunnels through all firewalls.  Everyone
uses it.

It's easy to point fingers at Microsoft.  Melissa uses features
in Microsoft Word (and variants used Excel) to automatically e-mail
itself to others, and Melissa and Worm.ExploreZip make use of the
automatic mail features of Microsoft Outlook.  Microsoft is certainly
to blame for creating the powerful macro capabilities of Word and
Excel, blurring the distinction between executable files (which can
be dangerous) and data files (which, before now, were safe).  They
will be to blame when Outlook 2000, which supports HTML, makes it
possible for users to be attacked by HTML-based malware simply by
opening an e-mail.  Microsoft set the security state-of-the-art back
25 years with DOS, and they have continued that legacy to this day.
They certainly have a lot to answer for, but the meta-problem is more
subtle.

One problem is the permissive nature of the Internet and the
computers attached to it.  As long as a program has the ability to do
anything on the computer it is running on, malware will be incredibly
dangerous.  Just as firewalls protect different computers on the same
network, we're going to need something similar to protect different
processes running on the same computer.

This cannot be stopped at the firewall.  This type of malware tunnels
through a firewall using e-mail, and then pops up on the inside and
does damage.  So far the examples have been mild, but they represent
a proof of concept.  And the effectiveness of firewalls will diminish
as we open up more services (e-mail, web, etc.), as we add increasingly
complex applications on the internal net, and as crackers catch on.
This "tunnel-inside-and-play" technique will only get worse.

And anti-virus software can't help much.  If a virus can infect 1.2
million computers (one estimate of Melissa infections) in the hours
before a fix is released, that's a lot of damage.  What if the code
took pains to hide itself, so that a virus won't be discovered for a
couple of days.  What if a worm just targeted an individual; it would
delete itself off any computer whose userID didn't match a certain
reference?  How long would it take before that one is discovered?
What if it e-mailed a copy of the user's login script (most contain
passwords) to an anonymous e-mail box before self-erasing?  What if it
automatically encrypted outgoing copies of itself with PGP or S/MIME?
Or signed itself; signing keys are often left lying around the system.
Even a few minutes of thinking about this yields some pretty scary
possibilities.

It's impossible to push the problem off onto users with "do you
trust this message/macro/application" messages.  Sure, it's unwise to
run executables from strangers, but both Melissa and Worm.ExploreZip
arrive pretending to be friends and associates of the recipient.
Worm.ExploreZip even replied to real subject lines.  Users can't make
good security decisions under ideal conditions; they don't stand a
chance against a virus capable of social engineering.

What we're seeing here is the convergence of several problems: the
permissiveness of networks, interconnections between applications
on modern operating systems, e-mail as a vector to tunnel through
network defenses and as a means to spread extremely rapidly, and
the traditional naivete of users.  Simple patches won't fix this.
There are some interesting technologies on the horizon that try to
mimic the body's own immune system to automatically deal with unknown
malware, but I am not very optimistic about them.  Sure they'll
catch some things, but it will always be possible to design malware
specifically to defeat the immune systems.  A large distributed system
that communicates at the speed of light is going to have to accept the
reality of viral affections at the speed of light.  Unless security is
designed into the system from the bottom up, we're constantly going to
be fighting a holding action.

Melissa:
http://www.zdnet.com/zdnn/stories/news/0,4586,2233116,00.html
http://www.zdnet.com/zdnn/stories/news/0,4586,2234121,00.html

Worm.ExploreZip
http://www.zdnet.com/zdnn/stories/news/0,4586,2274306,00.html
http://www.wired.com/news/news/politics/story/20160.html
http://www.symantec.com/press/1999/n990614d.html

Bruce Schneier, President, Counterpane Systems     Phone: 612-823-1098
101 E Minnehaha Parkway, Minneapolis, MN  55419      Fax: 612-823-1590
           Free crypto newsletter.  See:  http://www.counterpane.com

---

End of RISKS-FORUM Digest 20.45 

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991008065129/http://www.somewhere.com/)
