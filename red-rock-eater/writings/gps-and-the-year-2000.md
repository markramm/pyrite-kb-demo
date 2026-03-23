---
id: gps-and-the-year-2000
title: GPS and the year 2000
type: writing
writing_type: rre-post
date: 2000-01-01
url: http://commons.somewhere.com:80/rre/1997/GPS.and.the.year.2.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - commerce
  - education
  - forwarded-content
  - government-info
  - international
  - libraries
  - media
  - military
  - rre
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/GPS.and.the.year.2.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991023045510/http://www.somewhere.com/)

  

# GPS and the year 2000

```
[I have taken the liberty of reformatting this message to 74 columns.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Mon, 31 Mar 1997 11:51:15 -0800 (PST)
From: risks@csl.sri.com
Subject: RISKS DIGEST 18.96

RISKS-LIST: Risks-Forum Digest  Monday 31 March 1997  Volume 18 : Issue 96

---

Date: Thu, 27 Mar 1997 11:10:33 -0700
From: "Jack K. Horner 120775" <jkh@lanl.gov>
Subject: Re: Risks Associated with the Year 2000 Problem

  [This is message sent to Rick Light <rxl@LANL.GOV> in response
  to a forwarding of a comment on the appended message from the 
  U.S. House Science Committee, particularly relating to those Y2K
  problems resulting from the omission of the "19" in the calendar
  year.  It is reproduced with the permission of the author.  PGN]

The problem is potentially much messier than just the occurrences of the
literal value "19" in date types.  ANYTHING in software that merely acts
as if the first two digits of the date are "19" will have insidious
effects.

About a year ago, I worked on an analysis of the Global Positioning System
(GPS) ground station code to try to characterize the Y2K problem.  We
found no less than ten types of manifestations of the problem in a survey
of a randomly selected sample of 10% of the code. The occurrence of the
literal value "19" was only one of these ten types.  Other types included
type overflow problems at various dates throughout 1999, Y2K arithmetic
that implicitly assumed no dates later than 31 Dec 99 were possible,
and implicit module-interface date-type conversions. These problems are
potentially infinite in their variety, and not all can be detected with
tools.  Furthermore, in GPS it is not possible to construct good test
cases to see what will happen at the millennium start, because the future
(time-) states of the system depend on physical values (orbital elements,
pole wander, Jovian gravitational force) that can be determined with
sufficient accuracy only from the actual operation of the system within
about three months of the time of interest.  Approximately 1% of the total
GPS code is affected by this class of problems, or affected it.

The GPS user-equipment code is in even deeper trouble because of the Y2K
problem, and the breakage will occur well before Jan 1, 2000.  Date, in
the GPS signal standard, uses exactly thirteen bits (these bits represent
a time-unit offset from a conventional epoch date).  This allocation is
burned into proms on all existing GPS user equipment.  On about August
20, 1999, the actual date value will overflow this 13-bit type, and
the equipment will fail to produce correct time or position information.
Best estimate is that there are ~10^6 pieces of user equipment that will
be immediately affected. Everybody who depends indirectly on those pieces
of equipment (meaning all the rest of us) will also be affected. The GPS
standards committee is desperately trying to figure out what to do with
the problem.

Various well-calibrated software estimation models (SLAM, REVIC, PRICE-S)
predict that fixing the Y2K problem in systems of about 500,000 lines of
code or larger will take more time than is available between now and the
year 2000, regardless of how many programmers are thrown at the job.  Most
of the US's military command-and-control systems contain more than 500,000
lines of code.

GPS is now the primary means of distributing time standards throughout
the US, and throughout much of the world.  (The accuracy of the atomic
clocks on board the GPS satellites is second only to those maintained by
the primary standards clocks in Washington.)  Thousands of large financial
computers ultimately take their time calibration from GPS, every day.
Interest on overnight multi-billion-dollar short-term electronic-funds
transactions is computed at millisecond granularity, derived from the GPS
standard.

Place your bets.

Jack Horner, CIC-8

>>Notice From:
>>United States House of Representatives
>>Committee on Science
>>F. James Sensenbrenner, Jr., Chairman
>>George E. Brown, Jr., California, Ranking Democrat
>
>>CONSUMER RISKS ASSOCIATED WITH YEAR 2000 PROBLEM CITED
>>
>>Washington, DC -- Rep. Constance A. Morella, chair of the Committee on
>>Science's Subcommittee on Technology, along with several of her
>>colleagues sent a letter today to the Clinton Administration requesting
>>information on the Year 2000 problem.
>>
>>"We initially thought the problem affected just computer software and
>>programs, but we are now learning that the magnitude and scope of the
>>Year 2000 challenge seems to be growing beyond just computers," Morella
>>stated.  "If consumer products which contain microchips are affected, we
>>need to know whether agencies are addressing this fact and whether the
>>American public is being adequately informed."
>>
>>The Year 2000 problem involves embedded microchips which are present in
>>many every day conveniences such as microwaves and elevators.  Most of
>>these products have internal timers which are programmed with the "19"
>>prefix.  When the year 2000 is ushered in, computers which are
>>programmed with the "19" prefix will interpret  the year to be 1900 -
>>not year 2000.  Some experts are predicting that if corrective actions
>>are not taken by the year 2000, businesses and possibly some sectors of
>>the government could face operational and fiscal disasters.
>>
>>"The Year 2000 problem poses a daunting challenge to consumers,
>>businesses, and government alike," said Representative Bart Gordon,
>>ranking Democrat on the Subcommittee who also signed the letter.  "I
>>look forward to working with Chairwoman Morella to increase the public's
>>awareness of the potentially catastrophic consequences if the Year 2000
>>problem is not addressed."
>>
>>The letter was drafted after a hearing last week in which several
>>witnesses reiterated their concerns about potential serious safety
>>consequences associated with the Year 2000 problem.  One study discussed
>>predicted that more than one-half of all organizations world-wide will
>>not fully complete the Year 2000 effort.
>>
>>"If the long-term forecast for the Year 2000 problem is dismal, there
>>must be a realization of failure, and new strategies must emerge from
>>this realization,"  Morella said.  She also said the response to the
>>inquiry would assist her Subcommittee with identifying Year 2000
>>situations which may affect the health and safety consequences of
>>consumers.
>>
>>In addition to Morella and Gordon, the letter was also signed by
>>Representative Stephen Horn, chair of the Government Reform and
>>Oversight Committee's Subcommittee on Government Management,
>>Information, and Technology and Representative Carolyn Maloney, ranking
>>Member on the Subcommittee on Government Management, Information and
>>Technology.

---

End of RISKS-FORUM Digest 18.96 

---

Standard Risks reuse disclaimer:

  Reused without explicit authorization under blanket
  permission granted for all Risks-Forum Digest materials.
  The author(s), the RISKS moderator, and the ACM have no
  connection with this reuse.
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991023045510/http://www.somewhere.com/)