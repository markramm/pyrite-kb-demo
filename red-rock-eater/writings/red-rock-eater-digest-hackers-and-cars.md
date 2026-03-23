---
id: red-rock-eater-digest-hackers-and-cars
title: Red Rock Eater Digest - hackers and cars
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/2001/RRE.hackers.and.cars.html
importance: 6
research_status: partial
tags:
  - cognitive-science
  - environment
  - health
  - international
  - military
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/2001/RRE.hackers.and.cars.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20010917040238/http://commons.somewhere.com/rre/) | **Most Recent Article: Sun, 16 Sep 2001** |

```
[The world is full of exceedingly smart people who know all about the
subject matter of their profession, be it medicine, transportation,
or what-have-you, who are now wandering into the world of computers.
These people are smart enough to make computers work in some narrow
sense, but in many cases they are not acculturated enough into the
world of computers to avoid severe design errors, particularly in the
area of security.  The fact that many people in the computer industry
commit the same errors, whether through ignorance, arrogance, or
deadlines, doesn't help either.  The problem can be funny when
it affects other people, but it stops being funny once we imagine
automobiles on the highway being attacked with scripts.  The enclosed
message is forwarded by permission, and has been reformatted to 70
columns and slightly edited.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
You are welcome to send the message along to others but please do not use
the "redirect" option.  For information about RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html

---

Date: Mon, 25 Jun 2001 17:39:34 -0600
From: << a long-time RRE subscriber who prefers to remain anonymous >>

Very interesting article/paper.  I work for << well, let's just say
he knows what he's talking about -- PA >>.  As a result, I have an
anecdote and a particular point which may be of interest to you.

Client Anecdote:

        High-end vehicles (automobiles) contain three electrical
busses: one for the engine and drivetrain (requiring real-time
mechanisms), one for non-driveline-related controls (e.g. climate,
locks, window controls), and one for entertainment/non-critical
systems.  There are numerous variations one these (see SAE, Intel,
and Motorola for gory details) but the basic situation is that (IMO)
it's apppropriate to characterize them as fast, medium, and slow,
or critical, important, and who-cares.  At the moment, most vehicles
have only the fast and medium busses, and they're not interconnected
at the data and control-message level.

While discussing the evolution of these systems with vehicle engineers
at a large mfr., it came out that they intended to interconnect these
three systems in such a way that it would be possible to transfer
data and control messages from one bus to another.  My background
as a software designer and part-time system security geek led me
to suggest to them several scenarios in which such a system might be
intentionally hacked.  Their responses were frightening, to say the
least.  Roughly, here is what they said:

* o First - no one can (is capable) of doing that* o Two - even if they were, why would they? -or- Why would they want to?* o Three - even if they could and did, we can build unhackable systems.

These were very bright guys, mind you, who clearly had real talent
in designing automotive systems, but the gap between what they
thought and the mind of the average hacker (and I use that term
in the classical sense of "someone who mungs technology for kicks")
was astonishing.  We pointed out that ignition systems were already
being hacked to improve performance.  "But that's different!" they
replied, without being able to muster a reasonable explanation of the
"differences".  We pointed out that the fast and medium busses were
basically Ethernet-style mechanisms and therefore subject to similar
problems.  "Oh", they said after a few minutes thought, "but it's
not like that at all.  Ours is simpler."  Doh!

In a few more minutes we (one of the original architects of the
TCP/IP protocol and I) were able to conjure up several likely lines of
attack, all of which were deemed non-implementable by the automotive
engineers despite their having not a single general-purpose-software
expert among them.  They were literally unable to conceive of
the hacking possibilities they were about to offer us.  The closest
they got to admitting they had a problem was to suggest that they
would solve their bus data security problem by en/decrypting all the
packets.  Right...and how much more processing power would you need
for that, even assuming you could get enc/dec hardware fast enough to
run a modern engine?

In retrospect, I'm sure the conversation was just as frustrating for
them as it was for us.  It never occurred to them that *some kinds of
data are intrinsically valuable* and that software people as a class
tend to want to poke at things for *no other reason* than that it's
fun.

Point:

        Intelligent Traffic Systems seem to me to be yet another
attempt to replace human initiated first order errors (driving
mistakes) with human-initiated second order errors (software
problems).  In addition, the infrastructures typically described
eliminate three types of alternative transport: motorcyles,
motorscooters, and human-powered vehicles.  In Western US cities
especially, motor-driven cycles are practical on a year-round basis
and lower population densities make the construction of dedicated
bicycle trails afforable.  In Alburquerque, NM, for instance, they've
paved many of the access paths along the storm drains and irrigation
system, thus making it possible to ride tens of miles without
venturing onto surface streets.

Fortunately, we live in a nation that can't even get traffic light
sensors to detect a 500# motorcycle, so I'm not too worried about ITS
being deployed any time soon.
```