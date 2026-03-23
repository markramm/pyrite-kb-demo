---
id: hci-and-airplane-crashes
title: HCI and airplane crashes
type: writing
writing_type: rre-post
date: 1995-12-20
url: http://commons.somewhere.com:80/rre/1996/HCI.and.airplane.crashes.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - media
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1996/HCI.and.airplane.crashes.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009051610/http://www.somewhere.com/)

  

# HCI and airplane crashes

```
---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Tue, 7 May 1996 18:05:03 -0700 (PDT)
From: risks@csl.sri.com
Subject: RISKS DIGEST 18.10

RISKS-LIST: Risks-Forum Digest  Tuesday 7 May 1996  Volume 18 : Issue 10

---

Date: Tue, 7 May 1996 23:29:07 +0200
From: ladkin@TechFak.Uni-Bielefeld.DE
Subject: The Cali and Puerto Plata B757 Crashes

On December 20, 1995, American Airlines flight 965 (AA965), a B757-223
serial number N651AA, crashed into mountains on approach to Cali, Colombia.
This was the first B757 fatal accident in a decade and a half of service,
and I believe the first jet accident for AA in about the same length of time.

On February 6, 1996, a B757 of Birgenair, registration TC-GEN, crashed
into the ocean off Puerto Plata, Dominican Republic, shortly after takeoff.
This was the second fatal B757 accident.

The US National Transportation Safety Board is `participating fully' in each
of the investigations. Statements and documents concerning the accidents
released by the Columbian and Dominican Republic agencies are available from
the NTSB. Statements on Cali were released on 28 Dec 1995 and Feb 15 1996,
and the `docket' (containing the factual reports of the `specialty groups'
of investigators) has been released recently. Statements on the Puerto Plata
accident were released Feb 7, Mar 1 and Mar 18 1996.  Final reports for
neither are yet available.

Contrary to the impression given by some recent articles in the
non-specialist press, neither findings nor causes nor causal factors have
yet been officially determined in either investigation. However, the factual
reports so far indicate to me that the human-computer interface could be
involved in both accident sequences.  These airplanes have a safety record
amongst the best of any type in regular airline use - many B757 and B767
aircraft have been flying for a decade and a half in the fleets of airlines
all over the world, and there have only been three fatal accidents (the
first, to a Lauda Air B767, is thought to have been due to an unrecoverable
technical failure alone).  After 16 years of exemplary safe use, one should
therefore not be too hasty to `blame the computer' or its interface.  Here
are some comments on both accidents.

Cali:

Happened on approach to the airport, which is aligned along a relatively
narrow valley with high mountains to either side. Because of benign weather
conditions, the pilots were offered a `straight in' approach (to land in the
direction they were flying) rather than to fly beyond, turn, and land in the
opposite direction (the more usual procedure). They were not familiar with
the `new' approach. During the approach procedures, the pilots were confused
about exactly where they were in relation to the arrival procedure charts.
They had passed a specific radio beacon (VOR) called Tulua, which is the
start of the arrival procedure. It seems that they were not aware that they
had done so, entered this fix into the Flight Management Computer (FMC), and
didn't immediately notice that the aircraft had begun to turn back to the
Tulua VOR. This turn began a quick sequence of events that led to impact
with a mountain (a CFIT, Controlled Flight Into Terrain accident) about
3,000ft below the summit. A Ground Proximity Warning System warning sounded
about 9 seconds before impact, initiated recovery procedures (full power,
maximum angle of climb, retract any draggy control surfaces that are
deployed).  The crew didn't retract the speed brakes (manually controlled),
which is a necessary part of the escape procedure.

The actual manoeuvers that led to impact were that of turning towards
a specified VOR, and turning towards a specified heading. Both were
initiated by the crew. The former was apparently accomplished with the
FMS, the latter with the autopilot.  Small airplanes such as my Piper
Archer have autopilots capable of such manoeuvers. The pilot flying
must command either, as happened at Cali. However, the more
sophisticated FMC requires more attention than a simple autopilot when
entering fixes, and investigators are paying attention to the role the
FMC-pilot interaction played.

The question that arises is what exactly played a causal role. There is a
known HCI phenomenon that when something is `not right', it takes more time
and attention to `debug' the situation when more sophisticated devices are
involved than when simpler ones are being used.  However, there were also
other, human, procedural problems. The December 28 statement noted that
there was no indication of descent checklist procedures being performed by
the crew, and no indication of an arrival or approach procedures briefing.
Also, it is a basic rule of flying that you know where you are at all times.
These pilots didn't, at a crucial phase of flight, even though they had
reputations for conscientiousness (see the Operational Factors/Human
Performance factual report).

Their confusion may have been aided also by some of the pilot-controller
discourse about the route for which they were cleared. (However, there
was no evidence of `language difficulty', as this is usually understood.)

Puerto Plata:

The captain's airspeed indicator (ASI) was observed to be failed on takeoff.
This is not an event that requires emergency handling.  The captain asked
the copilot to call out the significant airspeeds for takeoff (called V1 and
V2, also normal procedure) and took off as normal.  He then called for the
center autopilot to be switched on. His own airspeed indicator showed higher
and higher airspeeds as the aircraft climbed, even though the actual
airspeed of the aircraft (as recorded by ground radar) was much lower. The
first officer observed that his ASI showed marked decrease in airspeed, and
the pilots became confused over which ASIs were failed (the captain thought
at one point that they'd both failed). The aircraft apparently stalled and
the pilots did not succeed in recovering before hitting the ocean.

The DR/NTSB factual statement noted that the behavior of the aircraft was
consistent with the captain's pitot being blocked. The airplane had been
sitting on the ground for many days in the tropics without the pitots being
covered (there is no procedural requirement for this, but pilots and
mechanics all know that insects love pitots).  The pitot is a tube facing
into the airstream receiving air pressure facing in the direction of flight,
and a related static port receives (roughly) ambient air pressure. The
difference between the two is used to drive the ASIs in all aircraft. If the
pitot is blocked, then pitot pressure remains roughly constant and ambient
air pressure decreases as the aircraft climbs, leading to greater difference
between pitot pressure and static pressure, and thus to greater `indicated'
airspeed on the ASI.

The copilot has a separate pitot-static system. The pitot-static readings on
the B757 are fed into the left (for the captain's system) and right (for the
copilot's) Air Data Computers, and thence to the CRT display instruments for
the respective positions.  There is a third pitot-static system that is
purely mechanical (and therefore `traditional'). Normally, pilots of all
airplanes are also trained to use `alternative source' if a pitot-static
system fails. `Alternative source' on the B757 is to switch the displays so
that the captain's ASI reads from the right ADC and the first officer's from
the left ADC. Also, the `glass' ASIs should be checked against the
mechanical `backup'. There is no evidence that either `alternate source' was
used during the accident flight, or that either instrument was checked
against the backup, even when the captain falsely thought that both his and
the first officer's ASIs had failed.

David Learmount asserted in Flight International (27 Mar - 2 April) that the
central autopilot gets its data from `the' ADC. He must have meant to say
from the left (captain's) ADC. Supposing this is the case, the autopilot
would react to the (false) increasing airspeed indication by raising the
nose, to attempt to reduce `airspeed'.  Continuing to do so, since the false
`airspeed' continued to increase with increasing altitude, the airplane
would radically lose (real) airspeed, and eventually stall, which appears to
be what happened.  I have not yet been able to verify Learmount's (modified)
assertion with the NTSB or Boeing engineers. The question arises, why would
the captain switch on the center autopilot if his ASI had failed and he knew
it got its data from the same ADC?  Anecdotal information (a colleague with
access to a B757 operations manual, another who is a B757 pilot) suggests
that this might not be information that one could expect to be at the front
of every B757 pilot's mind.  These two situations (center AP gets data from
left ADC; this information not in the mental foreground when dealing with
ASI problems) may thus have played a causal role in the accident. (I
emphasise again that I have not yet confirmed either situation.) This could
be categorised as an HCI issue.  As at Cali, there were other apparent
procedural failures: failure to switch to `alternate source'; failure to
check against the standby mechanical instrument. Performance of either would
have avoided the accident: as Learmount says, the pilots lost control of a
flyable airplane.

Further Commentary:

Maybe one can see in these accidents two known and often-observed HCI
effects of automation, which I shall call Complacency and Complexity.  The
Complacency effect is that use of (normally reliable) automation can lead to
reduced awareness of the state of the system.  The Complexity effect is that
increased automation makes some straightforward tasks more complex and
interdependent. The effects are distinct, but both have the consequence that
it becomes harder to figure out what's going on when something is wrong. As
a discussion point, let me propose that the greater role at Cali seems to
have been played by the Complacency effect, with some Complexity effect; and
that at Puerto Plata by the Complexity effect alone.  For the answers, we'll
have to wait until the final reports.

Finally, I don't regard either accident as giving grounds for concern about
the role of automation in itself. But the reports might yield insights into
and improvements to the procedures for dealing with certain forms of
automation. One always hopes to learn from the tragedies.

The text of the official statements referred to above, as well as other
pertinent documents, may be found in the sections on these accidents in the
hypertext Compendium `Computer-Related Incidents and Accidents to Commercial
Airplanes' under
   http://www.techfak.uni-bielefeld.de/~ladkin/

Peter Ladkin

---

End of RISKS-FORUM Digest 18.10

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009051610/http://www.somewhere.com/)