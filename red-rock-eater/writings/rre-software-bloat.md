---
id: rre-software-bloat
title: "[RRE]software bloat"
type: writing
writing_type: rre-post
date: 1999-04-30
url: http://commons.somewhere.com:80/rre/1999/RRE.software.bloat.html
importance: 6
research_status: partial
tags:
  - civil-liberties
  - cognitive-science
  - cryptography
  - environment
  - internet-policy
  - labor
  - media
  - military
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1999/RRE.software.bloat.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009050252/http://www.somewhere.com/)

  

# [RRE]software bloat

```
[I've taken the liberty of reformatting these messages to 70 columns.
I've also deleted the author's e-mail address at his request.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html
or send a message to requests@lists.gseis.ucla.edu with Subject: info rre

---

Date: Fri, 30 April 1999
From: risks@csl.sri.com

RISKS-LIST: Risks-Forum Digest  Tuesday 4 May 1999  Volume 20 : Issue 35

   FORUM ON RISKS TO THE PUBLIC IN COMPUTERS AND RELATED SYSTEMS (comp.risks)
   ACM Committee on Computers and Public Policy, Peter G. Neumann, moderator

---

Date: Fri, 30 Apr 1999 16:22:48 +0000
From: [address deleted] (RA Downes)   
Subject: The Bloatware Debate

One of the chief hallmarks of early UNIX was how simple, compact
programs worked well together.  Brian W. Kernighan's definition of a
good program was a program so good and so consistent that it could be
used for an entirely different purpose and be expected to work well.
UNIX, they said, was a way of thinking more than an operating system.
And, with Brian's Software Tools series, it was surely so.

Microsoft Windows is also a way of thinking - or not thinking, to be
more exact.  In almost every possible sense it is the anathema of the
programming community, if that community still abides by and adheres
to the solid thinking delineated by Brian so many years ago.

MS Windows programming is considered too difficult to attempt head on.
Where we come from most major corporations, financial institutions and
the like promised a smooth transition from UNIX or DOS to Windows 3.1x
within a matter of weeks.  Management talking of course.  When they
found this would not work they decided to invest heavily in 16-bit
Visual Basic applications.  Operative word "heavily".  These bloatware
masters sunk almost any machine made.  Clearly this was not the answer
either.

People looked to Kahn.  Borland, with its Turbo C, saw the opening
and released Borland C, and shortly thereafter Scott Randell who a
year earlier had toured with MSC 7.0 (which admittedly never worked)
was out rocking again, this time with Visual C++.  The environment
was unbelievable; the executables were extremely bloated; but still
and all it was Microsoft talking, and still and all they were smaller
than the corresponding Borland images.  COBOL programmers everywhere
were suddenly encouraged to learn C++, develop code browsing skills,
learn about preprocessors, assembly language, CodeView and subsequent
debuggers, and the world entered into a tailspin.

What originally started as a rather feeble but lucky attempt to get
on the OO bandwagon, the MFC soon became something you'd like to see
Steve McQueen kill.  Patches and work-arounds and bugs and more bugs,
and bloat and more bloat.  The current splash screen module is a case
in point: Microsoft includes a 16-color bitmap which weighs in at
nearly 200KB for you.  This bitmap can be compressed with RLE encoding
to less than half that size.  The idea of banging a 100KB splash
bitmap in an application is still, however, sickening.  Yet Microsoft
gladly gives you the bitmap at 200KB, happy if you don't understand
what you are doing by using it.  Your application will be more
sluggish than their own bloatware, and people will be less inclined to
complain about what they themselves do.

Microsoft's RegClean, a popular product for fixing corruptions in the
MS Windows Registry is another case in point.  When this application
was originally introduced I downloaded it and wondered about its size.
It weighed in then at nearly a megabyte.  Similar applications out
there were 20KB and hardly more.  What was inside this monster?  I
opened it and looked inside.

Remember all those stories about how surgeons in the old days just
threw their rubber gloves inside the patient's stomach before sewing
them back up again?  Well here you had it.  There were humungoid
bitmaps never used.  There were dozens of icons never referenced.
There were tens of kilobytes of entries in the string table that had
no meaning for the application whatsoever.

I honed the app down and came to the conclusion that the actual
size of RegClean should be about 45KB.  That as compared to its
distribution size of nearly one megabyte.  Clearly bloat is not only a
question of adding features almost no one wants.  Bloat is a condition
of the mind, permeating software houses everywhere.

Clearly again the distribution of RegClean was highly irresponsible.
But remember, MS Windows is not just an operating system - it is a way
of thinking, or not thinking as you may have it.  And it has permeated
the entire industry today.  Our hats off to Microsoft.

In conclusion: there are few application domains even today that
require executables of over 100KB, and most ordinary tasks can be
adequately managed by executables in the 20KB range.  This is simply
a fact.

There are no excuses.  Either we think or we don't.  There is no in
between.

RA Downes  Radsoft Laboratories <http://www.radsoft.net>

---

End of RISKS-FORUM Digest 20.35

---

Date: Tue, 4 May 1999 09:06:59 -0700 (PDT)
From: risks@csl.sri.com

RISKS-LIST: Risks-Forum Digest  Tuesday 4 May 1999  Volume 20 : Issue 37

   FORUM ON RISKS TO THE PUBLIC IN COMPUTERS AND RELATED SYSTEMS (comp.risks)
   ACM Committee on Computers and Public Policy, Peter G. Neumann, moderator

---

Date: Sun, 02 May 1999 16:12:13 +0000
From: [address deleted] (RA Downes)
Subject: Re: Bloatware Debate (Downes, RISKS-20.35)

A certain "Johnny" has written to me from Microsoft because of
my posting in RISKS-20.35 about MS bloat.  The tone was a thinly
disguised threat.  In his opening, "Johnny" stated that the "bloat"
of MS RegClean was due no doubt to having static links.  Discussing
the sweeping ramifications of such a statement is unnecessary here.
The mind boggles, it is sufficient to state.  The MSVC runtime is a
mere 250,000 bytes and in fact is not statically linked anyway to MS
RegClean, AFAIK [as far as I know].  MS RegClean is an MFC app and
will by default use the dynamically linked MFC libraries.  And even
if its static code links were an overhead here they would add but a
small fraction of the total bloat, say 40KB at most.

For whatever reason, I decided to download the latest version of MS
RegClean from BHS again and pluck it apart.  This is what I found.
I have tried - and it has been difficult - to keep subjective comments
out of this report.

Current Status of RegClean Version 4.1a Build 7364.1

---

Image Size (Unzipped and ready to run): 837,632 bytes (818KB)

---

(Subjective comment removed.)

Import Tables

---

The import section in the PE header.  This gives an indication of just
how (in)effective the use of Bjarne's C++ has been.  In this case,
the verdict is: "pretty horrible".  A walloping 7,680 bytes are used
for the names of the relocatable Win32 imports.  These are the actual
names of the functions (supposedly) called.  MS RegClean does not
call most of these functions - they remain because an MFC template was
originally used, most likely borrowed from another application, and
it was never "cleaned".  This is corroborated by what is found among
the "Windows resources": over half a dozen standard menus, assorted
graphic images, print preview resources, etc. that have nothing to do
with the application at hand.

Resources

---

Please understand that resources not only bloat an executable with
their own size, but with additional reference data, in other words the
bloat factor of an unused or bad resource is always somewhat larger
than the size of the bloating resource itself.

Accelerators

---

Sixteen (16) unused accelerators from an MFC template were found:
Copy, New, Open, Print, Save, Paste, "Old Undo", "Old Cut", Help,
Context Help, "Old Copy", "Old Insert", Cut, Undo, Page Up, Page Down.
MS RegClean uses only one accelerator itself, not listed here.

Bitmaps

---

This was a particularly sorry lot.  The main bloat here was a splash
screen bitmap weighing in (no RLE compression of course) at over
150KB.  Further, Ctl32 static library bitmaps were found, meaning MS
RegClean is still linking with the old Ctl32v2 static library which
was obsolete five years ago and which automatically adds another 41KB
to the image size.

Cursors

---

Six (6) cursors were found, none of which have anything to do with
this application.

Dialogs

---

A very messy chapter indeed.  MS RegClean walks around with eighteen
(18) hidden dialogs, of which only one or at the most two are ever
used.  The others are just - you took the words out of my mouth -
junk.  The findings (read it and weep):

*) Eleven (11) empty dialogs with the caption "My Page" and the static
text "Todo", all identical, all empty, and of course all unused.  This
is a wonder in and of itself.
*) The main "wizard" dialog actually used by the application is left
with comment fields to help the programmers reference the right
controls in their code (subjective comment removed).
*) A "RegClean Options" dialog which AFAIK is never used.
*) A "New (Resource)" dialog, probably a part of the development
process, just stuffed in the stomach at sew-up time and left there for
posterity.
*) A "Printing in Progress" dialog.
*) A "Print Preview" control bar dialog.

Icons

---

MS RegClean has three icons, all with images of 48x48 in 256 colors
(of course).  The funniest thing here is that the authors of MS
RegClean have extracted the default desktop icon from shell32.dll,
which is available at runtime as a resident resource anyway and
at no image bloat overhead at all, and included it in toto in their
executable.

Menus

---

MS RegClean has eight (8) menus, at least half of these are simply
junk left around by the MFC template.  Another menu indicates that
the authors of RegClean have in fact worked from an internal Microsoft
Registry tool - rather bloated in itself it seems.

String Table(s)

---

Actually it need only be one string table, but Microsoft itself has
never learned this.  The findings here were atrocious.  And you must
remember that strings stored in a string table are stored in Unicode,
which means that their bloat automatically doubles.  Further, MS's way
of indexing strings in a string table means a 512 byte header block
must be created for every string grouping, and strings are grouped
according to the high 12 bits of their numerical identifiers (yes
they are 16-bit WORD identifiers).  Meaning indiscriminate or random
numbering of string table entries will make an otherwise innocent
application literally explode.

347 (three hundred forty seven, yep, your video driver is not playing
tricks on you) string table entries were found in MS RegClean,
including 16 identical string entries with the MS classic "Open this
document" as well as archaic MFC template toggle keys texts which are
not used here (or almost anywhere else today).  Most of these strings
have - of course - nothing to do with the application at hand.

Toolbars

---

Toolbars are a funny MS way of looking at glyph bitmaps for use in
toolbar controls.  MS RegClean has two - one which may be used by the
application, and one which was part of the original MFC template and
never removed.

Total Accountable Resource Bloat

---

The total accountable (i.e. what can be directly calculated at this
stage) resource bloat of MS RegClean 4.1a Build 7364.1 is over 360,000
bytes (350KB).

Total Accountable Code Bloat

---

Harder to estimate, but considering that most of the code is never
used, only part of an MFC template that the authors of MS RegClean
lack the wherewithal to remove, the original estimate of a total
necessary image size of 45KB for the entire application must still
stand.

In Conclusion

---

Bloat is not a technical issue, but verily a way of thinking, a
"state of mind".  Its cure is a simple refusal to accept, and a well
directed, resounding "clean up your act and clean up your code!"

PS. Send feedback on RegClean to regclean@microsoft.com

RA Downes, Radsoft Laboratories  http://www.radsoft.net

---

End of RISKS-FORUM Digest 20.37 

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009050252/http://www.somewhere.com/)