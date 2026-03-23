---
id: spam-tools-phone-fraud
title: spam tools, phone fraud
type: writing
writing_type: rre-post
date: 1997-07-18
url: http://commons.somewhere.com:80/rre/1997/spam.tools.phone.fraud.html
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

Automatically imported from: http://commons.somewhere.com:80/rre/1997/spam.tools.phone.fraud.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991013231254/http://www.somewhere.com/)

  

# spam tools, phone fraud

```
[Simson's message follows up on the message about anti-spam tools that
I forwarded the other day; it includes further pointers on the subject.
I've also included a message about (what the author speculates is) an
809 area code fraud.  My main reason for including the latter message
is that I have seen several assertions, including one in a rumors-on-
the-Internet column in a well-known magazine about the world of the
Internet that shall remain nameless, that warnings about Caribbean
telephone fraud are hoaxes.  These assertions never, in my experience,
come with remotely the level of documentation as the warnings themselves.
This is a common pattern, I've noticed.  You may recall that the widely
repeated claims that wildly exaggerated rumors about the Lexis-Nexis
P-TRAK service had been widely posted on Usenet were never documented
or verified.  When I first made this observation, I was directed to a
great abundance of supposed evidence, almost all of which consisted of
entirely factual messages taken from news reports, or else the original
message, which contained only very minor errors.  And although my
sanity and honesty have been pointedly questioned on several occasions,
I never seen any better evidence, or indeed any further attempts to
document these serious claims.  On a related topic, several subscribers
pointed out the San Jose Mercury-News' utterly mysterious apology
for its series about the connection between various CIA assets and the
crack epidemic, which was publicized on this list among many others. 
The only reason that I haven't burdened you with abundant additional
material on this topic is that I'm really tired.  Perhaps by August
we'll finally manage to complete the switchover to Paul Duguid's guest
editorship, to which I am really looking forward.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Fri, 18 Jul 1997 16:44:45 -0700 (PDT)
From: risks@csl.sri.com

RISKS-LIST: Risks-Forum Digest  Friday 18 July 1997  Volume 19 : Issue 25

---

Date: Thu, 17 Jul 1997 16:43:26 -0400
From: "Simson L. Garfinkel" <simsong@vineyard.net>
Subject: Anti-spam redux

More time had elapsed between when I did my anti-spam DNS work and when the
article appeared in RISKS.  During that time, Vineyard.NET decided to
abandon our DNS-blocking SMPT server. The reason was that two key Internet
sites---AT&T's WorldNet and Dow Jones ---quiet simply refused to set up
valid reverse DNS for the mail servers.

We have since explored other blocking technology. We are continuing to block
mail that does not have a valid From: addresses. We now also allow our users
to have their own individual list of domains to block. We are doing this
with a modified SMAP, part of the Trusted Information Systems Firewall
Toolkit. You can download the modified SMAP from
ftp://vineyard.net/simson/smap.c. You can download the rest of the Firewall
Toolkit from ftp://ftp.tis.com/.

If you are running sendmail, I strongly suggest that you run the Firewall
Toolkit's SMAP wrapper. You can find instructions on how to install it in my
book Practical UNIX and Internet Security, published by O'Reilly &
Associates.

I am also told that there is a very nice list of domains to block maintained
by J.D. Falk, kept at: ftp://ftp.cybernothing.org/pub/abuse/

There is now also a mailing list of anti-spamming tools. You can find info
about it at http://www.abuse.net/spamtools.html

---

Date: Sun, 13 Jul 1997 14:08:08 -0400
From: Greg Corteville <cortevi5@egr.msu.edu>
Subject: The truth about Usenet's Psychic Spammers!

By now I'm sure we've all seen some of the garbage from the notorious
"psychic spammers" on just about every Usenet group.  I decided to do a
little investigating.  I wrote down a few of the 800 numbers listed in the
ads and went to a campus telephone that cannot be billed.  It has no long
distance service.  After dialing the number, callers are treated to a very
brief and very fake "recorded reading".  You are then urged to call a
different number for your "personal" reading.  The number they want you to
call has an 809 area code!

For those of you unaware of the 809 area code problem, I'll explain.  To
make an international phone call, you usually need to dial 011 first.  This
makes it quite obvious that it is an international phone call and will
likely be expensive.  However, several foreign countries have been assigned
"North American" area codes recently.  Among them, area code 809 for the
Caribbean.  Since these people are not bound by US law, they do not need to
disclose the full cost of making the phone call.  Callers are usually
charged exorbitant amounts of money, similar to a 900 number.  Some people
have been charged as much as $25 per minute!  These people are scam artists
and are using the Internet as their latest method of attack.

For more information on the area code 809 problem, take a look at these
websites:

http://www.fraud.org/809alert.htm
http://www.oag.state.tx.us/WEBSITE/NEWS/LEGALMAT/9701cpd.htm
http://www.ece.orst.edu/~alper/Info/scam.html

---

Date: 1 Apr 1997 (LAST-MODIFIED)
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
   [volume-summary issues are in risks-*.00]
   [back volumes have their own subdirectories, e.g., "cd 18" for volume 18]
 or http://catless.ncl.ac.uk/Risks/VL.IS.html      [i.e., VoLume, ISsue].
 The ftp.sri.com site risks directory also contains the most recent 
 PostScript copy of PGN's comprehensive historical summary of one liners:
   get illustrative.PS

---

End of RISKS-FORUM Digest 19.25 

---

Standard Risks disclaimer:

  Reused without explicit authorization under blanket 
  permission granted for all Risks-Forum Digest materials.  
  The author(s), the RISKS moderator, and the ACM have no 
  connection with this reuse.
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991013231254/http://www.somewhere.com/)
