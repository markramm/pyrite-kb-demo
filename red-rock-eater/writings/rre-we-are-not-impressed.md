---
id: rre-we-are-not-impressed
title: "[RRE]we are not impressed"
type: writing
writing_type: rre-post
date: 1999-04-01
url: http://commons.somewhere.com:80/rre/1999/RRE.we.are.not.impressed.html
importance: 6
research_status: partial
tags:
  - cognitive-science
  - commerce
  - cryptography
  - environment
  - government-info
  - health
  - international
  - media
  - military
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1999/RRE.we.are.not.impressed.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009113626/http://www.somewhere.com/)

  

# [RRE]we are not impressed

```
[C'mon, guys, you can do better than that!  Security on the Internet is
so shoddy that we should have had a whole ecosystem of living, breathing,
self-perpetuating, utterly ineradicable worms going by now.  What's the
problem?  You virus authors can redeem yourselves by getting at least one
worm thoroughly entrenched in the NT boxes of the world, including the
military sites, by Y2K.  Maybe then we can finally have the revolution
that it is evidently going to take to get ourselves an operating system
whose most basic architecture is up to the standards of 1974.  Otherwise
we'll all start laughing at you.]

=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html
or send a message to requests@lists.gseis.ucla.edu with Subject: info rre

---

Date: Wed, 31 Mar 1999 21:49:20 -0800 (PST)
From: risks@csl.sri.com

RISKS-LIST: Risks-Forum Digest  Thursday 1 April 1999  Volume 20 : Issue 26

---

Date: Tue, 30 Mar 1999 08:01:17 PST
From: "Peter G. Neumann" <neumann@csl.sri.com>
Subject: Melissa and RISKS

With all the furor since last Friday over the Melissa virus-like Trojan
horsed e-mail propagation (see next items), deeper issues are somehow lost
in the shuffle.  The vulnerabilities exploited in the MS Word macro virus in
Microsoft Outlook and Outlook Express have been around for a long time and
are likely to be around for a long time.  Although some palliative fixes are
available, the fundamental problems remain.  (For example, filters deleting
e-mail with "Subject: Important Message from ..." are only partially useful,
in light of recent versions of Melissa with blank Subject lines.)  The basic
system infrastructure is incapable of adequately protecting itself against
all kinds of misuses, and this particular exploit is just another reminder
that many folks need to wake up.  The situation could have been much worse,
but unfortunately many folks who depend on systems that are inherently
inadequate do not get the proper messages when the situation is not a
terrible disaster.  On the other hand, even if we had terrible disasters, it
does not seem to be enough.  And this was presumably not even an early April
Fool's spoof -- just another example microcosmically of what could be done
macrocosmically.  Many of the constructive lessons that should have been
learned from the Internet Worm over 10 years ago are still unlearned.

  [The late-breaking news (31 Dec 1999) that Yugoslav crackers are
  performing denial-of-service attacks against the NATO Website should
  also come as no surprise.  Can it be that only RISKS readers realize
  how flaky our compunications <*> infrastructures are?]

    [* I spent last Saturday at the 70th birthday roast for my PhD thesis
    professor, Tony Oettinger, who long ago coined the combining term 
    "Compunications".  In that the string "pun" is contained therein, it
    seemed appropriate to mention it here.  PGN]

---

Date: Tue, 30 Mar 1999 16:51:23 -0800
From: Rob Slade <rslade@sprint.ca>
Subject: Melissa macro virus

A report prepared by Robert M. Slade

The following is an attempt to bring together the information about the
Melissa virus.  It is taken from the most reliable available sources.
Additional sites have been listed at the end of the article.  I have not
added a copyright line to this message in order to allow it to be used as
needed.  I will be posting the latest updated version of this article at
http://sun.soci.niu.edu/~rslade/melissa.txt and
http://victoria.tc.ca/techrev/melissa.txt.

The virus, generally referred to as W97M.Melissa.A (with some variations:
Symantec, in a rather strained effort to be cute, seems to be calling it
"Mailissa"), is a MS Word macro virus.  This means that, if you don't use
Word, you are safe.  Completely safe.  (Except for being dependent upon
other people who might slow their/your mail server down.  More on that
later.)  If you need to look at MS Word documents, there is a document
viewer available (free, as it happens) from Microsoft.  This viewer will not
execute macros, so it is safe from infection.

In the messages about Melissa, there have been many references to the
mythical and non-existent "Good Times" virus.  Note that simply reading the
text of a message still cannot infect you.  However, note also that many
mailers, in the name of convenience, are becoming more and more automated,
and much of this automation concerns running attached files for you.  As
Padgett Peterson, author of one of the best macro virus protection tools,
has stated, "For years we have been saying you could not get a virus just by
"opening E-Mail.  That bug is being fixed."

Melissa does not carry any specifically damaging payload.  If the message is
triggered there will be text added to the active document.  The mailout
function can cause a large number of messages to be generated very quickly,
and this has caused the shutdown of a number of corporate mail servers.

If you have Word set with macros disabled, then the virus will not active.
However, relying on this protection is a very dangerous proposition.
Previous macro viruses have also killed macro protection in Word, and this
one does as well.

The name "Melissa" comes from the class module that contains the virus.  The
name is also used in the registry flag set by the virus.

The virus is spread, of course, by infected Word documents.  What has made
it the "bug du jour" is that it spreads itself via e-mail.  We have known
about viruses being spread as attachments to e-mail for a long time, and have
been warning people not to execute attachments (or read Word documents sent
as attachments) if you don't know where they came from.  Happy99 is a good
example: it has spread very widely in the past month by sending itself out
as an e-mail attachment whenever it infects a system.

Melissa was originally posted to the alt.sex newsgroup.  At that time it was
LIST.DOC, and purported to be a list of passwords for sex sites.  I have
seen at least one message theorizing that Melissa is someone's ill-conceived
punishment for viewers of pornography.  This hypothesis is extremely
unlikely.  Sending a virus to a sex related newsgroup seems to be a reliable
way to ensure that a number of stupid people will read and/or execute your
program, and start your new virus off with a bang.  (No pun intended.)

If you get a message with a Melissa infected document, and do whatever you
need to do to "invoke" the attachment, and have Word on your system as the
default program for .doc files, Word starts up, reads in the document, and
the macro is ready to start.  If you have Word's "macro security" enabled
(which is not the default) it will tell you that there is a macro in the
document.  Few people understand the import of the warning, and there is no
distinction between legitimate macros and macro viruses.

Because of a technical different between normal macros and "VBA objects," if
you ask for a list of the macros in the document, Melissa will not show up.
It will be visible if you use the Visual Basic Editor, but only after you
have loaded the infected file.

Assuming that the macro starts executing, several things happen.

The virus first checks to see if Word 97 (Word 8) or Word 2000 (Word 9) is
running.  If so, it reduces the level of the security warnings on Word so
that you will receive no future warnings.  In Word97, the virus disables the
Tools/Macro menu commands, the Confirm Conversions option, the MS Word macro
virus protection, and the Save Normal Template prompt.  It "upconverts" to
Word 2000 quite nicely, and there disables the Tools/Macro/Security menu.

Specifically, under Word 97 it blocks access to the Tools|Macro menu item,
meaning you cannot check any macros.  It also turns off the warnings for
conversion, macro detection, and to save modifications to the NORMAL.DOT
file.  Under Word 2000 it blocks access to the menu item that allows you to
raise your security level, and sets your macro virus detection to the lowest
level, that is, none.  (Since the access to the macro security menu item is
blocked, I do not know how this feature can be reversed, other than
programmatically or by reinstallation.)

After this, the virus checks for the
HKEY_CURRENT_USER\Software\Microsoft\Office\Melissa?\ registry key
with a value of "... by Kwyjibo".  (The "kwyjibo" entry seems to be a
reference to the "Bart the Genius" episode of the "Simpsons"
television program where this word was used to win a Scrabble match.)

If this is the first time you have been infected (and this "first time"
business is slightly complicated), then the macro starts up Outlook, in the
background, and sends itself as an attachment to the "top" 50 names in
each of your address lists.  (Melissa will not use Outlook Express.)
Most people have only one (the default is "Contacts"), but if you have more
than one then Outlook will send more than 50 copies of the message.  Outlook
also sorts address lists such that mailing lists are at the top of the list,
so this can get a much wider dispersal than just fifty copies of the
message/virus.  There was also a mention on one message about MAPI and
Exchange servers, which may give access to a very large number of mailing
lists.  From other reports, though, people who use Exchange mail server are
being particularly hard hit.  Then again, people who use Exchange are
probably also standardized on Word and Outlook.

Some have suggested setting this registry key as a preventive measure, but
note that it only prevents the mailout.  It does not prevent infection.  If
you are infected, and the registry key is removed at a later date, then a
mailout will be triggered the next time an infected document is read.

Once the messages have been sent, the virus sets the Melissa flag in the
registry, and looks for it to check whether or not to send itself out on
subsequent infections.  If the flag does not persist, then there will be
subsequent mass mailings.  Because the key is set in HKEY_CURRENT_USER,
system administrators may have set permissions such that changes made are
not saved, and thus the key will not persist.  In addition, multiple users
on the same machine will likely each trigger a separate mailout, and the
probability of cross infection on a common machine is very high.

Since it is a macro virus, it will infect your NORMAL.DOT, and will infect
all documents thereafter.  The macro within NORMAL.DOT is "Document_Close()"
so that any document that is worked on will be infected when it is closed.
When a document is infected the macro inserted is "Document_Open()" so that
the macro runs when the document is opened.

Note that not using Outlook does not protect you from the virus, it only
means that the 50 copies will not be automatically sent out.  If you use
Word but not Outlook, you will still be infected, and may still send out
infected documents on your own.  The virus also will not invoke the mailout
on Mac systems, but definitely can be stored and resent from Macs.  At this
time I do not have reliable information about whether it can reproduce on
Macs (there is one report that it does), but the likelihood is that it can.

Vesselin Bontchev has noted that the virus never explicitly terminates the
Outlook program.  It is possible that multiple copies may be invoked, and
may create memory problems.  However, this has not been confirmed, and is
not probable given the "first time" flag that is set.

The message appears to come from the person just infected, of course, since
it really is sent from that machine.  This means that when you get an
"infected" message it will probably appear to come from someone you know and
deal with.  The subject line is "Important Message From: [name of sender]"
with the name taken from the registration settings in Word.  The test of the
body states "Here is that document you asked for ... don't show anyone else
;-)".  Thus, the message is easily identifiable: that subject line, the very
brief message, and an attached Word document (file with a .doc extension to
the filename).  If you receive a message of this form *DO NOT OPEN THE
DOCUMENT WITH WORD!* If you do not have alternate means or competent virus
assistance, the best recourse is to delete the message, and attachment, and
to send a message to the sender alerting them to the fact that they are,
very likely, infected.  Please note all the specifics in this paragraph, and
do not start a panic by sending warnings to everyone who sends you any
message with an attachment.

However, please also note that, as with any Word macro virus, the source
code travels with the infection, and it will be very easy to create
modifications to Melissa.  (The source code has already been posted to one
Web site.)  We will, no doubt very soon, start seeing many Melissa variants
with different subjects and messages.  There is already one similar Excel
macro virus, called "Papa."  The virus contains the text "Fred Cohen" and
"all.net," leading one rather ignorant reporter to assume that Fred was the
author.  Dr. Cohen was the first person to do formal research into viral
programs.

There is a message that is displayed approximately one time in sixty.  The
exact trigger is if the current system time minute field matches the current
system time day of the month field when the virus is run.  In that case, you
will "Twenty-two points, plus triple-word-score, plus fifty points for using
all my letters.  Game's over. I'm outta here." typed into your document.
(This is another reference to the "Simpsons" episode referred to earlier.)

One rather important point: the document passed is the active document, not
necessarily the original posted on alt.sex.  So, for example, if I am
infected, and prepare some confidential information for you in Word, and
send you an attachment with the Word document, containing sensitive
information that neither you nor I want made public (say, the fact that Bill
Gates is a jerk for having designed the technology this way), and you read
it in Word, and you have Outlook on your machine, then that document will be
mailed out to the top 50 people in your address book.

Rather ironically, a clue to the identity of the perpetrator may have come
from the identification number embedding scheme recently admitted by
Microsoft as having been included with Office and Windows 98.  
   [Traced to an AOL user, apparently...  PGN]

A number of fixes for mail servers and mail filtering systems have been
devised very quickly.  However, note that not all of these have fully tested
or debugged.  One version that I saw would trap most of the warning messages
about Melissa.

Note that any Word document can be infected, and that an infected user may
unintentionally send you an infected document.  All Word documents, and
indeed all Office files, should be checked for infection before you load
them.

Information and antiviral updates (some URLs are wrapped):

http://www.cert.org/advisories/CA-99-04-Melissa-Macro-Virus.html
http://www.ciac.org/ciac/bulletins/j-037.shtml
ftp://ftp.complex.is/pub/macrdef2.zip
http://www.complex.is/f-prot/f-prot.html
http://chkpt.zdnet.com/chkpt/hud0007500a/www.zdnet.com/zdnn/stories/
  news/0,4586,2233030,00.html
http://www.zdnet.com/zdnn/special/melissavirus.html
http://www.symantec.com/techsupp/mailissa.html 
http://www.antivirus.com/vinfo/security/sa032699.htm
http://www.avp.com/melissa/melissa.html
http://www.microsoft.com/security/bulletins/ms99-002.asp
http://www.sendmail.com/blockmelissa.html
ftp://ftp.rubyriver.com/pub/jhardin/antispam/procmail-security.html
http://www.innosoft.com/iii/pmdf/virus-word-emergency.html
http://www.sophos.com/downloads/ide/index.html#melissa 
http://www.avertlabs.com/public/datafiles/valerts/vinfo/melissa.asp
http://www.pcworld.com/cgi-bin/pcwtoday?ID302
http://www.internetnews.com/bus-news/article/0,1087,3_89011,00.html
http://cnn.com/TECH/computing/9903/29/melissa.copycat.idg/
http://www.pcworld.com/cgi-bin/pcwtoday?ID308

rslade@vcn.bc.ca  rslade@sprint.ca  robertslade@usa.net  p1@canada.com
http://victoria.tc.ca/techrev    or    http://sun.soci.niu.edu/~rslade

---

Date: Wed, 31 Mar 99 13:54:52  GMT
From: leveret@warren.demon.co.uk (Nick Leverton)
Subject: Melissa and monocultures

The current outbreak of the Microsoft Word "Melissa" virus/worm is a
graphical illustration of the RISKS of monoculture.  Agriculturalists long
ago discovered the problems of single strain crops, in that they provide an
ideal habitat for an adapted pest or disease which can wipe them out.

With W97M/Melissa, the global e-mail network of at least one major
international computer corporation with which I am familiar had to be
disabled for 24 hours on Mon/Tue 1999-03-29 to 1999-03-30 to prevent the
spread of Melissa-infected documents.  (Melissa, for those fortunate enough
not to have encountered it, is a Microsoft Word 97 macro virus, which also
acts as a worm by reading 50 entries from a Microsoft address book and
mailing itself out with subject "Important information from ...").

Ironically, and the point of this mail, sites within the corporation still
running the older Unix/X.400 environment or the niche Unix/SMTP environment
were unaffected, except that they were brought down too by the lack of
connectivity from corporate mail gateways.  A heterogeneous environment
poses much greater barriers to the spread of this or any virus.  Reliance on
a single product or family of products, from a similar supplier, is a RISK
that is familiar in the engineering and farming professions but needs to be
better known in the computing ones.

Nick Leverton

  [Lloyd Wood notes that Microsoft itself put a halt to all outgoing
  e-mail throughout the company on Friday to guard against propagation.]

---

Date: Tue, 30 Mar 1999 17:05:50 +0100 (IST)
From: Ronan Waide <waider@scope.ie>
Subject: Melissa and GUIDs

Of course, conspiracy folks can enjoy the following course of events:

1 Presence of GUID in Microsoft-made documents revealed.
2 Melissa worm wreaks havok on the net.
3 Alleged author of worm tracked with GUIDs.

Let's wait for

4 Microsoft praised for having GUIDs in documents.

waider@scope.ie / Small Planet Ltd. / +353-1-8303455 / +353-1-8300888 (Fax)

---

Date: Sun, 28 Mar 1999 12:03:11 -0700 (MST)
From: Bear Giles <bear@coyotesong.com>
Subject: Melissa + meme = future disaster

While reading the press coverage about the Melissa e-mail virus/work, it
occurred to me that a trivial change would make it far worse.

The problem was that Melissa advertised pornographic sites, so it was often
brought to the attention of responsible parties who could recognize it was a
virus and take appropriate measures.  If it were a human virus, it would be
something that sent people rushing to the doctor.

What if Melissa's message were something innocuous?  What if it was a meme
with a proven track record of being readily passed from person to person?

  Make $20,000 with only $5!

  Send your business card to a dying child seeking to get into the
  Guiness Book of World Records!

  Send this message to 100 friends and get a free trip to Disney World
  from Bill Gates and Disney!

When people feel good, how many rush to the doctor to verify it isn't due to
brain cancer?  Of those who do, how many are taken seriously?

The most obvious effect of this change is that far fewer people would bring
the message to the attention of their MIS department or ISP. Even hardened
security experts might let the message slide as just another scam or urban
legend.  Only the sheer volume of messages would indicate that something odd
was occurring.

A less obvious effect of this change is even worse.  Few people would
forward an ad for pornographic sites on their own, but the aforementioned
messages (and others) are forwarded.  With changes.  The current virus can
be easily caught at the mail server by checking the subject line... but what
if "helpful" individuals were personalizing it?  Ditto the non-viral
contents?

Even if it's technically possible to scan the contents of every mail
document for an embedded macro virus, is it ethical?  Such a filter would be
invasive... and yet offer no guarantee that a copycat virus wouldn't get
through.  The real problem, after all, isn't in the virus itself, it's in an
application for a single company defying all common sense and loading
macros from e-mail.  I think it's no coincidence that I haven't seen this
virus...  and I and my friends all run either Linux or MacOS.

Bear Giles <bgiles@coyotesong.com>

---

End of RISKS-FORUM Digest 20.26 

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009113626/http://www.somewhere.com/)