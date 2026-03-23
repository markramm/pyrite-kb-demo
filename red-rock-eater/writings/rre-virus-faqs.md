---
id: rre-virus-faqs
title: "[RRE]virus FAQs"
type: writing
writing_type: rre-post
date: 1999-03-31
url: http://commons.somewhere.com:80/rre/1999/RRE.virus.FAQs.html
importance: 6
research_status: partial
tags:
  - civil-liberties
  - commerce
  - cryptography
  - education
  - environment
  - international
  - law
  - media
  - military
  - privacy
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1999/RRE.virus.FAQs.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009104002/http://www.somewhere.com/)

  

# [RRE]virus FAQs

```
[In response to my message calling for a rain of worms upon NT, one
person noted that NT was modeled heavily on the prototypical 1970's
operating system, namely VMS, which I have to grant.  He also argued
that the main problem was with lousy applications, but I think that's
a half-truth.  The reason I get so upset about all of these security
breaches is that they make me feel old.  More than half my life ago,
I started programming in Univac 1100 series assembler.  I even wrote
an industrial-strength virtual memory system, interrupt handlers and
all, for an operating system that had no such thing.  This machine,
first a Univac 1108 and then an 1100/43, if I recall correctly, was
designed for batch operation.  Its interactive command line system was
a kludge designed to simulate Hollerith cards.  Its hard memory was
unimaginably vast at 256K words.  And it ran a time-sharing operating
system that routinely handled forty users.  The thing is, that OS's
security was rock-solid.  I hacked the daylights out of it, and it
never even occurred to me that I could cause anything approaching the
havoc that people are routinely warned about in radio headlines today.
I crashed it once, maybe, but in the usual way, by overflowing a table.
The closest I ever got to breaching security was my brilliant scheme
for circumventing the memory-use limitations that the computer center
imposed during the day -- 56K words, if I remember correctly.  When
I did this, of course, the system operators simply called me on the
phone and told me to knock it off.  This machine couldn't have had the
power of a Pentium.  When I first starting using it, it had magnetic
core memory and a frigging *rotating magnetic drum* for mass storage.
But still it was vastly more reliable than any machine to which I have
access today.  The great majority of computer users have never known
such a machine.  That level of security and reliability is science
fiction so far as they can tell.  They live in a world in which it is
normal for operating systems and applications programs to be designed
to run random bits of computer code that they pull down from the net,
and to do so with absolutely no security protections at all.  So far
as these normal people can tell, the earth was created with Word macro
viruses in it (stop and think about that -- viruses in *Word macros*
-- what ignominy!), and you'd never know from reading the paper that
it is possible for a program to check ahead of time whether it is about
to overflow a stack.  This is not just a technical issue; it's a social
justice issue.  It would be entirely feasible for us to have software
that works, but instead we have a whole generation of entrenched
software standards that seem as if designed to induce powerlessness,
dependency, and self-blame among non computer experts.  We should be
ashamed.  That's why I'm calling on the virus writers of the world to
wreck it all, so that we can throw it all away, back up a few decades,
and start over.  NT is better, I admit, but it's still a mess, and it
doesn't fix the applications.  Our standards are too low.  Consider:
When I was in school we spent much of our spare time comparing notes
on the fundamental shoddiness of Unix.  Simson Garfinkel and friends
gathered those notes into the very funny UNIX-HATERS book (qv).  Now,
however, Unix is the gold standard for operating systems, the basis
for comparison when evaluating something like NT.  That's how far
we've regressed.  Believe it or not, letting several programs from
different sources all run on your machine without trashing anything
sensitive or interfering with one another was a *solved problem* over
thirty years ago!  Am I just having a bad week?  I don't think so.
For more like this, see <http://w3.one.net/~sunlion/linuxriot.html>.]

=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html
or send a message to requests@lists.gseis.ucla.edu with Subject: info rre

---

Date: Fri, 2 Apr 1999 15:15:00 -0800 (PST)
From: risks@csl.sri.com

RISKS-LIST: Risks-Forum Digest  Friday 2 April 1999  Volume 20 : Issue 29

---

Date: Wed, 31 Mar 1999 16:58:47 -0500
From: Mich Kabay <mkabay@compuserve.com>
Subject: Origins of PC / Mac Virus Vulnerability

Letter to the Editors, ATLANTIC MONTHLY.

Dear Editors:

I enjoyed Robert Buderi's historical overview of the rise of computer
viruses (April Atlantic) -- a particularly timely contribution to
public knowledge given the explosive spread of the Melissa virus and
similar e-mail-enabled nuisances in late March 1999.

Unfortunately, technologically unsophisticated readers may have
concluded that computer viruses are inevitable outgrowths of the
nature of computers.  Now, any author must select what to include or
not, especially when writing within a word-count limitation.  As a
contribution to the discussion, not as a criticism, I did want to add
a couple of fundamental points that were not mentioned in the article
but that may help readers understand why we are suffering this
cyberplague.

1) Computer viruses in the wild exist almost exclusively on Microsoft
DOS, Microsoft Windows 3.x, 95, & 98 and Apple MacOS operating
systems. For all practical purposes, there are no viruses in UNIX,
MVS, VMS, MPE and other operating systems that run on workstations,
minicomputers and mainframe computers.  The root (no pun intended)
of our PC virus woes is design decisions made long ago.  Microsoft
engineers decided to dispense with a security kernel -- the part of
the operating system that determines exactly what kinds of operations
an ordinary user is permitted to perform.  The security kernel limits
certain other operations to supervisory users (often known as "root")
and yet others to the operating system itself.  In well-behaved
operating systems, changing a memory location (for example) is usually
a restricted operation.  Under Windows95, in contrast, every user
is in effect root and programs the user runs can do anything at all.
Without this vulnerability, viruses in the PC and Mac worlds would be
severely limited in their effects (the "payload").

When PC and Mac operating systems introduce a security kernel into
their operating systems, much of the viral payload would be defused.

2) Microsoft engineers decided to turn office software into a general
programming tool.  MS-Office programs include macros -- not an unusual
feature for word processors and spreadsheets in the last 20 years.
Unfortunately, they also decided to allow two functions that made
their software vulnerable to macro viruses: (a) automatic execution
at startup; and (b) access to system routines.  Without these features,
Word and Excel macro viruses would not be as powerful nor as virulent
in their replication as they are today.

When Microsoft changes the defaults on Word and Excel to prevent
automatic execution of macros, PC and Mac viruses will have greater
difficulty in replicating.

Public awareness of the design decisions underlying our vulnerability
may help sway software engineers towards improvements in our working
environment.

M. E. Kabay, PhD, CISSP, Director of Education, ICSA Inc. -- Vermont
255 Flood Road  Barre, VT 05641-4060 <http://www.icsa.net>  802-479-7937

---

End of RISKS-FORUM Digest 20.29 

---

[http://www.cert.org/tech_tips/Melissa_FAQ.html]

Frequently Asked Questions About the Melissa Virus

Last Updated: March 31, 1999

1.How many reports have we received? 

We have first-hand reports of more than 300 organizations affected, 
covering more than 100,000 individual hosts. 

2.Is the damage limited only to denial-of-service? 

No. Under some circumstances, confidential documents can be leaked 
without the user's knowledge. These circumstances include the use of a 
single template file by more than one user, and the transmission of an 
infected document to another user who has not previously been infected. 
Additionally, if you fail to clean up the virus correctly and completely 
(for example, by not cleaning the normal.dot file) you may expose 
confidential information at a later time. 

3.What about Papa, and other variants? 

We have received reports of other variants of Melissa, including one 
named Papa. At the present time, we have not received a significant 
number of reports of Papa outbreaks. If you practice antivirus 
precautions on a regular basis, you can protect yourself against Papa 
and other variants of Melissa. 

4.Are Macro viruses new? 

No. According to the Department of Energy's Computer Incident Advisory 
Capability (CIAC), macro viruses for Microsoft Word appeared as early as 
1995, with over 1000 variants for Word and other products by 1998. See 
http://www.ciac.org/ciac/bulletins/i-023.shtml for more information. 

5.Why was Melissa so serious? 

Melissa was different from other macro viruses because of the speed at 
which it spread. The first confirmed reports of Melissa were received on 
Friday, March 26, 1999. By Monday, March 29, it had reached more than 
100,000 computers. Some sites had to take their mail systems off-line. 
One site reported receiving 32,000 copies of mail messages containing 
Melissa on their systems within 45 minutes. 

6.Are Macro viruses limited to Microsoft Word? 

No. Macro viruses can affect other products, including other products 
from Microsoft such as Excel and Powerpoint. The Papa virus, for 
instance, is reported to be spread via Excel. 

7.Is Melissa a worm? 

Melissa requires user interaction to propagate, therefore we do not 
consider it a worm. However, Melissa can propagate quickly from one 
computer to another with minimal interaction required by the user. 

8.Does the Melissa virus affect MacOS? 

The Melissa virus can infect files stored on and shared with MacOS-based 
systems running Word 98. However, when the virus runs on MacOS systems, 
it is not able to send electronic mail, and its propagation will be 
slower on MacOS systems. 

9.Can I protect myself by marking the normal.dot file read-only? 

At best, marking the normal.dot file read only is a stop-gap protection. 
On Windows 98/95 systems and on MacOS, viruses can circumvent the 
read-only protection. Instead, we recommend setting Word to prompt the 
user before making any changes to the normal.dot file if you are 
concerned about changes to that file. 

10.How can I protect myself against variants of Melissa? 

Disable macros by default. Use caution when operating any product when 
macros are enabled. Keep your antivirus products up-to-date. Be leery of 
unsolicited documents or executable programs received in electronic 
mail. Beware of software that comes from untrusted sources. 

11.Who wrote Melissa? Why was Melissa written? What crimes has the 

author committed? What is the status of the investigation? 
The CERT Coordination Center is a technical organization. We concentrate 
on the technical aspects of computer security problems. We have no legal 
authority and we do not "catch the bad guys."

12.Can I be affected if I don't use Outlook? 

If it is installed, Outlook is used by the virus to send mail. 
Otherwise, Melissa behaves like a normal virus: you can infect others by 
carelessly sharing files. 

13.I use a mail package other than Outlook. Am I affected? 

The mailer you use to read mail doesn't matter. The virus will use 
Outlook, if Outlook is installed, to send copies of itself. How you 
receive it doesn't matter. 

14.How effective are systems that look at the subject of the mail 
message? 

Systems that rely solely on pattern matching to recognize the virus can 
be used as a stop gap measure to prevent the spread of a particular 
virus, but will fail as soon as the virus mutates so that it no longer 
matches the pattern. This can be very effective as a short-term fix, but 
will not provide long-term protection.

15.Is Melissa the most dangerous virus possible? 

Melissa was relatively non-destructive and easily detected. Variants 
could be significantly more destructive or stealthy. We strongly 
encourage you to be aware of the risks posed by viruses and other 
computer security concerns at all times. 

16.Are you aware of the connection between the Melissa virus and the 
television show The Simpsons? 

Yes.

17.What products are affected? 

Outlook 98 and Outlook 2000 for Windows platforms can be used to 
propagate the virus. Microsoft Word 97 and Word 2000 for Windows and 
Word 98 for Macintosh can be used by the virus to infect other 
documents. Earlier versions of Word, including Word 95, cannot be used 
to infect other documents, nor can Outlook Express on any platform be 
used to propagate the virus via email.

18.Why is it called Melissa? 

It was named Melissa by the antivirus software vendors. 

19.Do you have to open the email attachment to be infected? 

Yes. To be affected by Melissa and other, similar macro viruses, you 
must open the attachment and permit macros to run. You cannot be 
affected by Melissa or similar viruses merely by receiving the email.

20.If I receive the virus mailed to me by someone, should I notify them?

 
Yes. We encourage you to notify them. More information about dealing 
with incidents can be found in our Incident Reporting Guidelines at

http://www.cert.org/tech_tips/incident_reporting.html

21.I am a novice user and know little about computer language. I read 
your virus alert and tried to determine whether or not my Word macros 
were disabled. I use Office 97, professional version, and did not find a 
way to disable the macro function. However, under the menu options 
"Tools/Options/General" I found a checked box that says "Macro virus 
protection." Will this option provide adequate protection against the 
Melissa macro virus and other, similar viruses? 

If this option is checked, Word will give you a warning any time you 
open a document that has macros embedded in it. The warning will give 
you the opportunity to prevent any macros from running.

22.Are the Melissa macro virus and Happy99 the same thing? 

No. While Melissa is a macro virus, Happy99.exe is a Trojan horse 
program. For more information about Happy99.exe, please see Incident 
Note IN-99-02 Happy99.exe Trojan Horse at

http://www.cert.org/incident_notes/IN-99-02.html

---

This document is available from: 
http://www.cert.org/tech_tips/Melissa_FAQ.html. 

---

CERT/CC Contact Information

Email: cert@cert.org
Phone: +1 412-268-7090 (24-hour hotline)
Fax: +1 412-268-6989
Postal address:

CERT Coordination Center
Software Engineering Institute
Carnegie Mellon University
Pittsburgh PA 15213-3890
U.S.A.

CERT personnel answer the hotline 08:00-20:00 EST(GMT-5) / EDT(GMT-4) 
Monday through Friday; they are on call for emergencies during other 
hours, on U.S. holidays, and on weekends. 

Using encryption

We strongly urge you to encrypt sensitive information sent by email. Our 
public PGP key is available from http://www.cert.org/CERT_PGP.key. If 
you prefer to use DES, please call the CERT hotline for more 
information. 

Getting security information

CERT publications and other security information are available from our 
web site http://www.cert.org/. 

To be added to our mailing list for advisories and bulletins, send email 
to cert-advisory-request@cert.org and include SUBSCRIBE 
your-email-address in the subject of your message. 

Copyright 1999 Carnegie Mellon University.
Conditions for use, disclaimers, and sponsorship information can be 
found in http://www.cert.org/legal_stuff.html.- "CERT" and "CERT Coordination Center" are registered in the U.S. 
  Patent and Trademark Office 

  ---

  NO WARRANTY
  Any material furnished by Carnegie Mellon University and the Software 
  Engineering Institute is furnished on an "as is" basis. Carnegie Mellon 
  University makes no warranties of any kind, either expressed or implied 
  as to any matter including, but not limited to, warranty of fitness for 
  a particular purpose or merchantability, exclusivity or results obtained 
  from use of the material. Carnegie Mellon University does not make any 
  warranty of any kind with respect to freedom from patent, trademark, or 
  copyright infringement.
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009104002/http://www.somewhere.com/)