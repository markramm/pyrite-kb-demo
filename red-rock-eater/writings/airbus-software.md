---
id: airbus-software
title: Airbus software
type: writing
writing_type: rre-post
date: 1995-03-15
url: http://commons.somewhere.com:80/rre/1995/Airbus.software.html
coauthors: []
key_concepts: []
importance: 4
research_status: partial
tags:
  - forwarded-content
  - internet-culture
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1995/Airbus.software.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991002122938/http://www.somewhere.com/)

  

# Airbus software

```
Subject: RISKS DIGEST 16.92

RISKS-LIST: RISKS-FORUM Digest  Thursday 16 March 1995  Volume 16 : Issue 92

---

Date: 15 Mar 1995 15:56:26 +0000
From: Les Hatton <les_hatton@prqa.co.uk>
Subject: A340 shenanigans

The BBC news at 08.30 reported a slight problem which occurred on the
morning of 15 Mar 1995 with the ultra high-tech, packed full of software
and therefore utterly wonderful Airbus A340.

Apparently on the final part of its approach to Gatwick, both the pilots
screens went blank, to be replaced by a polite little message saying "Please
wait ...".  Somewhat unnerved, the pilots requested that the plane turn
left, but it turned right instead.  They then tried to get it to adopt a 3
degree approach to the runway, but it chose a 9 degree plummet instead.  At
this point, from the report, they appeared to gain manual control and landed
safely.  It is not clear who will pick up the dry-cleaning bill.

Vis a vis this sort of thing, I was at a talk recently, given by the CAA (UK
Civil Aviation Authority), at which it was stated that in the past
generation of civil aircraft, most of the software problems were reported in
the Flight Management System.  Not surprisingly, this was the most complex
part of the aircraft software system.  Not any more it isn't.  During the
talk, it was also admitted that the newer generation of aircraft such as the
A340, other software systems including active systems were "at least as
complicated".  So what next ?
 I suppose it follows on nicely from the story in the October 1994 Risks
whereby a Japanese Air Force T-4 jet trainer ejected one of its pilots.
Perhaps it didn't like him.  :-)

Les Hatton, Ph.D. C.Eng, Director of Research & Engineering, Programming
Research Ltd, England   les_hatton@prqa.co.uk    +44 (0) 1 932 888 080

---

End of RISKS-FORUM Digest 16.92 

---

Date: Wed, 22 Mar 95 14:56:20 PST
From: RISKS Forum <risks@csl.sri.com>
Subject: RISKS DIGEST 16.96

RISKS-LIST: RISKS-FORUM Digest  Weds 22 March 1995  Volume 16 : Issue 96

---

Date: Wed, 22 Mar 1995 19:50:56 +0100
From: ladkin@techfak.uni-bielefeld.de
Subject: Re: A340 incident at Heathrow (Hatton, RISKS-16.92)

Les Hatton reports in RISKS-16.92 on an incident involving an Airbus A340 on
a trip from Japan to London Heathrow. The aircraft is one of the
A320/330/340 (also A319/321) family of Airbuses, some of whose primary
flight control systems are computer-controlled (that is, the pilots
control-stick movements are input to a computer that guides the control
systems).  The A340 is a very long-haul aircraft, capable of flying the very
longest routes without refueling (it holds the world record for length of
route flown without refuelling, for normally-equipped civil transport
aircraft).  The incident is of greatest significance for RISKS readers
because it is the first time that an accident report on an A320/330/340
series aircraft specifically cites software and hardware reliability as the
main problem.

The incident concerned a Virgin A340 at Heathrow on 19 September 1994 (cf.
the incorrect info reported by Hatton). A short article by Christian Wolmar
appeared in The Independent newspaper, one of Britain's major dailies, on
Wednesday March 15, 1995. After talking to Christian, I obtained a copy of
AAIB (Britain's Air Accident Investigation Board) Bulletin No. 3/95, the
report on the incident.

I'll spoil the tale for everyone by giving the punchlines first: the
description of the problem areas identified during the incident, and the
report's conclusion, the `Safety Recommendation 95-1'.  [during quotes, my
editorial comments and elisions are contained within square parentheses such
as these. PBL.]

[begin quote]

Problem Areas

The AAIB identified and investigated the following problem areas: RTF [radio
communication] phraseology; ATC [air traffic control] vectors and ILS
[instrument landing system] performance; fuel quantity indications; double
Flight Management Guidance System (FMGS) failure and aircraft type
certification.

[end quote]

The radio phraseology can be ignored by RISKS readers.  ATC vector problems
had to do with capturing the `glideslope', the radio beam angled up into the
sky from the end of the runway, down which an aircraft flies in order to
land, under instrument conditions.  The aircraft at one point encountered a
`false glideslope' at about 9\deg at 5 miles from touchdown and 4,800ft
altitude caused by a `shallow sidelobe' of the ILS. Such problems are known
(glideslope is assured for between 1.35\deg and 5.25\deg in the UK) and the
airplane wouldn't have got there had it not been vectored there by ATC - but
one hastens to add that normally this is not a problem. Just in this
case....see below. All the other problems concern the on-board computers,
and the AAIB has written to the JAA (Joint Aviation Authority, which does
for Europe what the FAA does for the USA) to determine if the JAA was "aware
of some of the more significant shortcomings of the A340's fuel and flight
management systems before the type certificate was granted".

[begin quote]

Safety Recommendation.

It is recommended that the reliability of the Airbus A340 FMGS and the fuel
management system should be reviewed to ensure that modified software and
hardware required to achieve a significant improvement in reliability should
be introduced as quickly as possible and the subsequent system performance
closely monitored.

[end quote]

Here is why they made this recommendation:

[begin quote]

Autopilot and Flight Director heading performance

The reason for the wrong response of the autopilot and one flight director
to the left turn demand was a software error [...] [This error] was known to
Airbus Industrie and corrective measures for this and several other software
deficiencies were contained in [...] standard L-5 that has been issued and
incorporated in most A340s on the UK register.

Fuel Quantity indications

In July 1994 Airbus Industrie issed an Operations Engineering Bulletin on
the subject of fuel quantity indication. [The bulletin gives detailed
descriptions of anomalies, when they occur, and how to take them into
account.]  Action pending by Airbus Industrie to correct fuel quantity
errors involves the installation of five additional fuel probes in each
inner tank and software standard 6.0. Action to correct CG control errors
[the center of gravity is adjusted in cruise by moving fuel around, to give
efficient cruise performance] is contained in a software only upgrade to
standard 6.1. [...]

FMGS double failures 

After landing the aircraft's Central Maintenance System had logged a fault
in No 2 FMGEC. This was removed and sent to France for data extraction and
fault analysis. No fault was found within the hardware and a comparable
software fault could not be reproduced on the test bench.  Nevertheless, the
BITE data dump showed that at 1435 hours the No 2 FMGEC had detected a CLASS
1 HARD failure within itself and a simultaneous fault within FMGEC No 1. The
investigation was complicated by the involvement of several sub-contractors
in the manufacture of the FMGEC and its database.

[...]

Airbus Industrie were aware of the double FMGS failure mode that had first
emerged on the A320 series aircraft. On A320/330/340 aircraft, each FMGEC is
linked to its own set of peripherals and inertial reference system. Both
FMGECs achieve their own computations and exchange data through a cross talk
bus. One FMGEC is declared as master and the other as slave; the master
FMGEC is related to the engaged autopilot. Some data in the slave FMGEC is
synchronised to the master but all data inserted on any MCDU is transferred
to both FMGECs and to all peripherals.

According to Airbus Industrie, there are several ways in which the exchange
of data and/or a problem in one computer can affect the other computer.
Often the computers reset themselves after a few seconds but occasionally a
fault results in repetitive resets or attempts to resynchronise. The fifth
reset relatches the computer, which will not recover without a power
interrupt. Reset breakers for manual power interrupts are on the flight deck
overhead panel. Dual resets occur when both FMGECs encounter failures at the
same time.  They generally occur after a pilot entry that involves use of
the navigation database or to an event synchronised between both flight
management systems. Latched double failures usually occur if pilots
successively perform three inputs that cause a reset, or if an `impossible'
computation of predictions occurs.

Airbus Industrie have succeeded in radically reducing the frequency of
double FMGS failures on the A320 series aircraft; they are also addressing
the problem on the A330 and A340 series. [...]

[end quote]

I point out that so-called Byzantine failure modes and algorithms for
avoiding them in distributed systems were first identified and studied in
the 70s by my former SRI colleagues Lamport, Shostak and Pease under the
auspices of the SIFT project, and since then by many, many others. As for
other such topics in computer science, this was regarded as `theory' for a
few years. I could hazard a guess that many aerospace engineers still have
not heard about this area. The account above of the problems with the
A320/330/340 master/slave FMGECs may give RISKS readers reason to inform
themselves about the `theory' of how all this anomalous and possibly
dangerous behavior can be avoided in the first place. Many papers in the
January 1994 issue of the Proceedings of the IEEE speak about the current
state of the art.

Finally, the story.

On the ground in Tokyo before departure, one FCMC indicated numerous faults.
It is accepted procedure to depart with only one FCMC operative - they did
so, and followed the appropriate procedures for calculating fuel with only
one FCMC. Early in cruise, the map symbology on the commander's EFIS
(Electronic Flight Instrument System) disappeared and his MDCU
(Multifunction Control and Display Unit) ceased calculating.  They slaved
both off the copilot's DMC (Display Management Computer).  The EFIS is the
pretty screen in front of the pilot that tells himher which way is up, which
way is forward, and which way, as well as how fast (in three dimensions),
and where heshe is.  The MDCU displays flight plan info, and a bunch of
other things. About an hour later, they found that the commander's EFIS had
restored. Logical indications from the No.2 FCMC were also restored later by
`resetting the computer'.

Now come a few things which one should really think about hard.

Getting close to home (Heathrow), the copilot tuned in the Lambourne VOR (a
radio beacon) manually, to ensure that the EFIS displays were still
accurate. They were cleared to fly direct to the beacon, but a few miles
east, "the commander's EFIS map display symbology froze and lost all
computed data [..]. His MDCU displayed the message `PLEASE WAIT' together
with a page normally seen only when loading in data before flight. He was
unable to obtain any other display. At [roughly the same time], the
[copilot's] EFIS and MCDU exhibited identical behavior."

Notice that not all flight control info was lost from the EFIS - they could
still fly the airplane. They `dialed in' the ILS using a "back-up method",
and while doing so received an ECAM warning of low fuel state and
instructions to open crossfeeds (airplanes like this have many tanks and
fuel is pumped around between them). The warning reoccurred and readings
indicated they had some 2 tonnes (2000kgs) of fuel less than expected.  They
discussed traffic density with ATC, and eventually declared an emergency in
order to get priority for landing.

They had the autopilot automatically capture the ILS, which is when they hit
the sidelobe. `The glidepath bar moved rapidly down the ILS display before
moving rapidly up once again; the autopilot's attempt to follow the
glidepath resulting in unusually high pitch rates and so the autopilot was
disconnected.' The commander informed the tower they were having problems
with the glideslope and requested an SRA (Surveillance Radar Approach). In
an SRA, the controller talks the airplane down localiser and glideslope
continuously, by giving an uninterrupted stream of position information
relative to the glideslope/localiser pair. It's very impressive.

Aircraft are on `final approach' when they're lined up with the runway
centerline and heading down the glideslope to land. (This should not be
confused with when the flight attendant says `final approach' to the
passengers, which is usually when the aircraft is even before initial
approach phase.) The approach was for Runway 09 Right at LHR (the `09' means
that it's pointing roughly 90\deg to North). The crew were on the SRA, being
vectored (given magnetic headings to fly) to intercept the final approach
course. They were flying a heading of 180\deg and were commanded to change
to 130\deg.  When they turned the heading selector knob on the autopilot,
both commander's and copilot's heading `bugs' moved correctly (that's an
indication on the directional gyroscope of which heading you want the
autopilot to fly to and hold - I had a lower-tech version on my Piper
Archer), but the flight director bars went in opposite directions and the
airplane followed the false movement of the copilot's bar, and turned right
instead of left. At this stage, the copilot disconnected autopilot and
flight directors and flew the plane `manually' (see first paragraph for why
this is not quite an accurate expression for these aircraft).

They landed without further incident; after taxiing in and shutting down,
the fuel indications recovered; and thankfully everyone lived happily ever
after.

Peter Ladkin

---

Date: Wed 22 Mar 95 14:06:55-PST
From: John Rushby <RUSHBY@csl.sri.com>
Subject: Re: A340 incident at Heathrow (Ladkin, RISKS-16.96)

I'm not sure you need to invoke Byzantine failures to explain the problems
reported with the double FMGS failures in the Airbus A340 and its relatives,
though Byzantine-fault-tolerant architectures are simpler and more regular
than others -- and might therefore be less prone to bugs.

A Byzantine failure is usually interpreted as a hardware fault that cases
the errant device (e.g., a sensor) to provide conflicting information to the
systems that interrogate it.  These faults can be masked by suitable
Byzantine-fault-tolerant algorithms (invented, as Peter correctly points
out, by Pease, Shostak and Lamport during the SIFT project at SRI.
Incidentally, you can retrieve a picture of SIFT, and of Pease, Shostak, and
Lamport via WWW at URL http://www.csl.sri.com/ft-history.html ).

However, Byzantine hardware faults don't seem to be the problem with the
A340 FMGS--rather, it seems to have been a plain bug in the redundancy
management.  And from the description, it seems that the reason there are
bugs is that the design of the system is not amenable to comprehensive
analysis and thorough comprehension.  The great contribution of Lamport et
al. was the "state-machine" approach to fault-tolerant system design
(tutorial reference at bottom).  The advantage of this approach is that it
provides a relatively simple architecture that can provably tolerate ANY
KIND of fault, up to some number.  In contrast, the type of architecture
used in most aircraft systems is based on FMEA, where you explicitly try to
anticipate and counter each specific kind of fault.  This leads to
complexity, and thence to bugs, and also to the possibility of overlooked
fault modes (and, more likely, overlooked COMBINATIONS of faults).  The
disadvantage of the state-machine approach is that it requires a lot of
redundancy (3n+1 channels to withstand n simultaneous faults).  This is
overcome, to some extent, by the "hybrid" fault-models introduced by the
people at Allied Signal who developed the MAFT architecture.  (There's a
paper by them in the issue of the IEEE proceedings that Peter mentions).
MAFT is the only architecture for primary flight control developed by a
manufacturer of these things that uses the state-machine approach.  It was
proposed for the 7J7 and 767X, but Allied dropped out of the bidding after
Boeing cancelled these and then invited new proposals for the 777.

Systems above the PFC (primary flight control/computer) level usually seem
to use dual, or dual-dual redundancy rather than the quad-and-above found in
PFCs.  The state-machine approach may not be appropriate here, but I'd hope
that ideas from modern fault-tolerant design, and from formal
state-exploration and verification could add something.

As an aside, the mechanisms of fault tolerance, distributed coordination,
concurrency management, etc. employed in aircraft systems owe little to
those studied by academic researchers.  For example,

  Not far from there (CNRS-LAAS a research center concerned with
  fault-tolerance), Airbus Industries builds the Airbus
  A320s.  These are the first commercial aircraft controlled solely by a
  fault-tolerant, diverse computing system.   Strangely enough this
  development owes little to academia.  (IEEE Micro, April 1989, p.6)

Of course, there is little reason to suppose that academic researchers know
more about fault-tolerant architectures for avionics systems than those who
actually develop them, but it does mean that the architectures and
mechanisms used in aircraft systems cannot draw on the extensive analyses
and (in some cases mechanically checked) proofs that have been published and
subjected to peer review in computer science journals.

John

Introduction to the state-machine approach:

@article{Schneider:state,
	AUTHOR = {Fred B. Schneider},
	TITLE = {Implementing Fault-Tolerant Services Using the State
		Machine Approach: A Tutorial},
	JOURNAL = {ACM Computing Surveys},
	YEAR = 1990,
	VOLUME = 22,
	NUMBER = 4,
	PAGES = {299--319},
	MONTH = Dec
}

We've done lots of work applying formal methods to algorithms for
state-machine replication under hybrid fault models.
[You can get the redundancy down to about n >3a+2s+m where a, s, and m are
the numbers of arbitrary (Byzantine), symmetric (wrong but consistent),
and manifest (obvious, or crash) faults to be tolerated simultaneously.]

Examples, if you're interested:
  http://www.csl.sri.com/podc94.html
  http://www.csl.sri.com/tse93.html
  http://www.csl.sri.com/compass94.html
  http://www.csl.sri.com/cav93-hybrid.html
  http://www.csl.sri.com/ftcs93.html
  http://www.csl.sri.com/ftrtft92-jmr.html
  http://www.csl.sri.com/ftrtft92-ns.html
  overview:  http://www.csl.sri.com/tse95.html

See also NASA's overall program and their own work in this area:
  http://shemesh.larc.nasa.gov/fm-top.html

John Rushby                   Email: Rushby@csl.sri.com
Computer Science Laboratory   Tel: (415) 859-5456 (hit #0 to escape voice-mail)
SRI International             Fax: (415) 859-2844
333 Ravenswood Avenue         WWW: http://www.csl.sri.com/rushby/rushby.html
Menlo Park, CA 94025, USA     ftp: ftp.csl.sri.com/pub/{reports|pvs}

---

End of RISKS-FORUM Digest 16.96 

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991002122938/http://www.somewhere.com/)