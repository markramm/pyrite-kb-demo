---
id: old-software-versus-new-software
title: old software versus new software
type: writing
writing_type: rre-post
date: 1996-12-20
url: http://commons.somewhere.com:80/rre/1997/old.software.versus.new..html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - forwarded-content
  - libraries
  - privacy
  - rre
  - rre-post
  - telecommunications
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/old.software.versus.new..html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20001026033959/http://commons.somewhere.com/rre/) | **Most Recent Article: Wed, 25 Oct 2000** |

# old software versus new software

```
---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Fri, 20 Dec 1996 14:56:30 -0800 (PST)
From: risks@csl.sri.com
Subject: RISKS DIGEST 18.70

RISKS-LIST: Risks-Forum Digest  Friday 20 December 1996  Volume 18 : Issue 70

---

Date: Fri, 20 Dec 96 9:56:52 PST
From: "Peter G. Neumann" <neumann@csl.sri.com>
Subject: BART software crash and system delays

Bay Area Rapid Transit (BART) had another bad day.  At 7am, a ghost train
appeared at the San Francisco 24th Street station, requiring manual
operation through that station.  Independently, three trains had to be taken
out of service because of mechanical problems.  All of this caused a
15-minute delay systemwide.  Later, a computer crash caused delays up to 30
minutes systemwide, from 5:50pm to 9:45pm on 19 Dec 1996.

BART also had a serious power cable outage in the transbay tunnel on 12 Dec
1996 (not previously reported here by itself, because of its lesser
relevance to the computer systems -- although it certainly had a major
effect on the system as a whole).  That cable problem was traced to sloppy
maintenance after the cable was damaged way back when it was installed back
in the early 1970s.  BART now observes that an overall cable overhaul had
been considered prior to the 12 Dec outage as an urgent step in upgrading
the aging infrastructure.

---

Date: 20 Dec 1996 09:55:44 +0000
From: "Nick BROWN " <Nick.BROWN@DCT.coe.fr> (Tel (+33)388412674 )
Subject: Problems of "unforeseen" system aging

Reading some back issues of RISKS, I realised how many of the incidents and
problems reported are due to systems (embedded and otherwise) getting old.
The "system" (made up of the people who use it, as well as all the computer
"systems") has to be able to cope with the oldest and newest technology in
it, and all the breakdowns in all the (non-upgradable) component systems.
With the pace of change in technology (try buying a 1 megabyte SIMM), we are
going to find ourselves more and more unable to maintain the systems we
build.

Current examples are such things as: air-traffic-control computers being
kept going long after the manufacturer can officially no longer supply the
spares, by wizened (i.e., over-45) hardware engineers with soldering irons
and a bag of those big fat 20-watt resistors; car "computers" which tell you
the car's average speed over the last hour, for the first four years of the
car's life, and then flash "88 8888" at you unless you spend $1250 for a
replacement unit; a four-year-old PC for which you can't buy a new disk
drive (the BIOS can't handle anything bigger than 512 MB).

Future examples: anything with a smart card in it; the often-documented
problem of reading information stored on 30-year-"guaranteed"-lifetime
optical disks in 30 years when the disk might be readable, but no computer
system can connect to the drive; and of course the year 2000.

People are very good at adapting to change (once they get over the emotional
hurdle of accepting it's going to happen) and working with the limitations
of old and new; just look at any home with items as diverse as a TV and a
toilet.  Computer systems aren't at all good at it, and anything with
firmware is just disastrous.

Here's a little test for readers who work in systems specification.  Have
you ever seen a requirements, functional, or design specification for any
computer application system that specified not just the hoped-for start date
for production use of the system (you know, the one where you have to
subtract a year for political reasons, even though you know there's no way
it'll be ready in time), but also the END date, after which the system would
be taken out of use and replaced with something else?  For advanced
students: what would have been the effect on any given project of doing so?

Nick Brown, Strasbourg, France

  [The juxtaposition of this item with the BART
  item is of course purely coincidental(!).  PGN]

---

Date: Tue, 10 Dec 1996 11:37:30 +0100
From: Roland Giersig <roland.giersig@aut.alcatel.at>
Subject: Arrogance of Micro$loth Products - BEWARE!

This is about a "feature" in WinWord 6 that a colleague stumbled across. The
incident shows the full arrogance that MS products exhibit when dealing with
situations with ambiguous semantics.

The said colleagues job was to prepare monthly reports about estimated and
real work-power efforts regarding some projects work-packages. For the first
few months he wrote these reports using the WinWord installed on his
laptop. Recently he switched over to using the WinWord installed on a
central NT server using WinCenter to access it remotely from his Sun
workstation. As it is common practise with such recurring reports, he opened
the report from last month to change the figures and save it under a new
name.

Now the figures were listed in a table, and the sum of each column was
calculated via the "Table Formula Sum(above)" function. Before he started
changing the numbers, he accidentally pushed F9 ("Update Fields") while the
cursor happened to be in the sum field.

Can you imagine how big his surprise was when suddenly the column sum
CHANGED before his eyes? Remember, he didn't change anything! And WITHOUT
WARNING! And to add insult to injury, the sum was WRONG!

Avid MS "fans" surely know by now what was wrong: the LANGUAGE
settings of the two Windows versions differed! And thus the symbol for
the decimal point was `.' on the one machine and `,' on the other.

The arrogance? NO WARNING! And the sum function does not even just truncate
then numbers, no, it somehow interprets the comma or period as a list,
because summing "1,4" and "2,3" gives...  TADAH! "10"!!! (it used to give
"3,7" with the other language settings)

The RISK? I really wonder how many reports are out there with wrong numbers
because some poor dilbert-type employee typed it on his computer and her
boss printed it from another computer with different language
settings. Maybe even someone got degraded or fired "because s/he reported
the wrong numbers"!

Also, WinWord is the only editor I know where you open a file, close it
again and WinWord asks you if you want to save the changes!!

(Another example of built-in arrogance: I tried to import some ASCII-text
records into MS Access. Instead of asking about the format, Access silently
tried to interpret the text itself and finally reported "1746 errors
found"!)

So the final lesson learned is: 

          >>> MS documents ARE NOT PORTABLE! <<

(And another example of non-portabililty: MS Project stores the
workdays-per-week number as a PER-USER setting, not per-project!  Exchange a
Project with a colleague and BINGO! Everything gets re-scheduled.)

There are surely lots of other examples, maybe others would like to share
their "experiences" too.

BTW, I am sure that some of these "features" are or will get fixed. But I am
also sure that nobody will receive a bugfix or upgrade for free, as it is
common practise with other software companies. Instead you will be prompted
to "upgrade to Windows97 and WinOffice2000 for a real cheap $999.99 now and
your problems will be solved". Sweet arrogance!

My feelings are best reflected by this signature found on the Net:
 "Microsoft is not the ANSWER.
  Microsoft is the QUESTION,
  and the ANSWER is NO!"

Roland 

PS: Sorry if this sounds very emotional, but I have already wasted
enough precious time with things like these.

Roland.Giersig@aut.alcatel.at        (speaking only to, err, for myself)
ALCATEL Austria, Scheydgasse 41, A-1210 WIEN.    Phone: +43-1-27722-3755

---

Date: 15 Aug 1996 (LAST-MODIFIED)
From: RISKS-request@csl.sri.com
Subject: Abridged info on RISKS (comp.risks)

 The RISKS Forum is a MODERATED digest.  Its Usenet equivalent is comp.risks.
=> SUBSCRIPTIONS: PLEASE read RISKS as a newsgroup (comp.risks or equivalent) 
 if possible and convenient for you.  Or use Bitnet LISTSERV.  Alternatively,
 (via majordomo) DIRECT REQUESTS to <risks-request@csl.sri.com> with one-line, 
   SUBSCRIBE (or UNSUBSCRIBE) [with net address if different from FROM:] or
   INFO     [for unabridged version of RISKS information]
=> The INFO file (submissions, default disclaimers, archive sites, .mil/.uk
 subscribers, copyright policy, PRIVACY digests, etc.) is also obtainable from
 http://www.CSL.sri.com/risksinfo.html  ftp://www.CSL.sri.com/pub/risks.info
 The full info file will appear now and then in future issues.  *** All 
 contributors are assumed to have read the full info file for guidelines. ***
=> SUBMISSIONS: to risks@CSL.sri.com with meaningful SUBJECT: line.
=> ARCHIVES are available: ftp://ftp.sri.com/risks or
 ftp ftp.sri.com<CR>login anonymous<CR>[YourNetAddress]<CR>cd risks
 or http://catless.ncl.ac.uk/Risks/VL.IS.html      [i.e., VoLume, ISsue].
 The ftp.sri.com site risks directory also contains the most recent 
 PostScript copy of PGN's comprehensive historical summary of one liners:
   get illustrative.PS

---

End of RISKS-FORUM Digest 18.70 

---

Standard RISKS reuse disclaimer:

  Reused without explicit authorization under blanket
  permission granted for all Risks-Forum Digest materials.
  The author(s), the RISKS moderator, and the ACM have no
  connection with this reuse.
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20001026033959/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20001026033959/mailto:webmaster@somewhere.com). |