---
id: end-to-end-philosophy-endangered
title: End-to-end philosophy endangered
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1996/End-to-end.philosophy.en.html
coauthors: []
key_concepts: []
importance: 6
research_status: partial
tags:
  - auto-imported
  - community-networking
  - cryptography
  - government-info
  - internet-policy
  - privacy
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1996/End-to-end.philosophy.en.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991019002520/http://www.somewhere.com/)

  

# End-to-end philosophy endangered

```
---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date:	03/28/96 01:54:16 EST (03/28/96 02:35:38 EST) 03/28/96 02:35:40
From:	"David P. Reed" <dpreed@reed.com> @ uucp
Subject:	End-to-end philosophy endangered

Friends -

I'd like to call your attention to a situation where misguided
politics (of the "ends-justify-means" sort) threatens one of the
fundamental principles of Internet architecture, in a way that seems
like a slippery slope.  I do not normally take public stands of a
political nature, and I do not participate much in Internet
architecture anymore, but I'd like to call your attention to a very
severe perversion of the Internet architectural philosophy that is
being carried out in the name of political and commercial expediency.

No matter what you believe about the issues raised by the
Communications Decency Act, I expect that you will agree that the
mechanism to carry out such a discussion or implement a resolution is
in the agreements and protocols between end users of the network, not
in the groups that design and deploy the internal routers and
protocols that they implement.  I hope you will join in and make
suggestions as to the appropriate process to use to discourage the use
of inappropriate architectural changes to the fundamental routing
architecture of the net to achieve political policy goals.

As you know, I am one of the authors, along with Saltzer and Clark, of
the paper "End-to-end arguments in decentralized computer systems",
which first characterized in writing the primary approach to the
Internet's architecture since it was conceived, which approach
arguably has been one of the reasons for its exponential growth.  This
philosophy - avoid building special functionality into the net
internals solely to enforce an end-to-end policy - has led to the
simplicity, low cost, and radical scalability of the Internet.  One of
the consequences is that IP routers do not enforce policies on a
packet-by-packet basis, so routers can be extremely simple beasts,
compared to the complex beasts that characterize even the simplest
telephone central office switch.  End-to-end policies are implemented
by intelligence at the ends (today, the PCs and servers that
communicate over the many consolidated networks that make up the
Internet).

I just read in Inter@ctive weekly that Livingston announced an "Exon
box" - a router that is designed to enable ISPs to restrict access to
"indecent sites" or unrated sites unless an "adult" enters an
authorization code when opening a session to enable the router to
transmit packets to the site.

The scam seems to be that Livingston has colluded with Senator Exon's
staff to propose a "solution" to enable ISP's to implement parental
controls.  Exon's staff is using the announced solution as an example
to demonstrate how simply ISPs can enforce local community standards
and parental controls, thus supporting interpretations of the CDA
requiring all access providers to include such capability in their
boxes.  Exon's staff is quoted as encouraging ISP's to install such
functionality into the routers that serve as access points for nets.

Since I use an Ascend P50 ISDN router to make frequent, short,
bandwidth-on-demand ISDN connections from my "Family LAN" to an Ascend
multi-line ISDN router at my commercial Internet Service Provider, I
am worried that this model is completely unworkable for me, and for
others that will eventually use such a practical system.  My family
has minor children and adults who all happily access the Internet.  My
ISP has no clue whatsoever whether a child or adult has initiated the
call, and in fact, if my child and I are both on different computers
in different rooms, it is quite silly to imagine that the Ascend
router at the ISP can figure out if it is me or my child generating
each packet.

It is appalling to me that Livingston, which has some responsibility
as a router provider to assist in the orderly growth of the net, is
pandering to Exon's complete misunderstanding of how the Internet is
built.  I would hope that Ascend, with its much larger share of the
ISP market, and other router companies such as Cisco and Bay Networks,
would take a principled and likely popular position that the "Exon
box" is not the way to go about this.  I would hope that ISP's would
in general avoid use of Livingston's products, and also refuse to cave
into Exon's pressure.  I believe, though I may be wrong, that
Livingston has contributed to the RADIUS technology that many ISP's
use to manage dialup access charging in a way that is consistent with
ethe end-to-end philosophy, but any credit they are due is overwhelmed
by the Exon box insanity.

I do work to protect my children from inappropriate material, but
pressure from Senators to mandate technically flawed solutions, and
opportunistic, poorly thought-through technologies from companies like
Livingston are not helpful.

If you agree, please join me in attempting to call off any tendency
for other router vendors and protocol designers to develop Exon box
features.  It would seem that the appropriate place for content
restrictions, such as "parental controls", are in the end-to-end
agreements between content providers and their users, not in the
internal switching architecture of the net.  

- David
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991019002520/http://www.somewhere.com/)