---
id: list-bombing
title: list bombing
type: writing
writing_type: rre-post
date: 1996-08-30
url: http://commons.somewhere.com:80/rre/1996/list.bombing.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - forwarded-content
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1996/list.bombing.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009222042/http://www.somewhere.com/)

  

# list bombing

```
[You may recall my messages about list bombing a while back.  This is
the nasty practice of forging messages that cause a disfavored individual
to be subscribed to many mailing lists.  Well, Netcom recently had a
huge attack.  I've been too hard on Netcom over other issues in the past;
this time they have my full sympathies, not least because all of us need
to get better list-handling software to avoid this problem in the future.
This issue of Risks includes a victim's perspective and a note from the
developer of Majordomo.  It also includes an amusing message on a separate
topic -- supermarket checkout systems -- and the Risks subscription
information.  The Risks Digest is still the best thing on the Internet.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Fri, 30 Aug 1996 09:30:22 -0700 (PDT)
From: risks@csl.sri.com
Subject: RISKS DIGEST 18.39

RISKS-LIST: Risks-Forum Digest  Friday 30 August 1996  Volume 18 : Issue 39

---

Date: Fri, 30 Aug 1996 11:04:48 -0400
From: dmethvin@cmp.com (Methvin Dave)
Subject: Re: Denial of service ... Netcom listservers (Markowitz, RISKS-18.38)

Let me provide a victim's perspective on Netcom's mail list troubles. I was
one of about two dozen people who were falsely subscribed to over 1000
mailing lists in the early hours of 10 Aug 1996 by someone calling
himself "johnny xchaotic". On 12 Aug, the mail bomber posted a manifesto
in news.admin.net-abuse; you can find a copy of it at
http://www.winmag.com/people/dmethvin/mailbomb.htm.

The good news as far as RISKS goes was that there were hundreds of mailing
lists that did the right thing and rejected the subscription request. Some
mail list software detected the inconsistency between the From address and
the rest of the header. Others realized that the sheer number of
simultaneous subscriptions reeked of spam. Others sent a confirmation
request that had to be returned to start the subscription; I deleted them
and the subscription never got started. Ahh, the beauty of well-behaved
software.

Netcom's mailing list software (and many others as well) fell into the other
category. It was suckered by the forged From in the header, wasn't at all
troubled that the attacker was asking to be signed up to every list at
Netcom, and didn't send any confirmation request before adding me to the
list.

By the time I logged on later that Saturday (about 10 hours after the attack
started), I had over 1600 mail messages. Since I was going on a long
business trip that week, followed by a vacation the next week, I knew I
wouldn't have time to deal with the problem immediately. I decided to have
my incoming Internet mail turned off at our corporate gateway, so that
messages to dmethvin@cmp.com would be bounced back to the sender. In
attempts to contact them, I found out that many of the other victims are
also bouncing mail, some because their mailboxes are full.

In the case of Netcom's mailing list, I suspect that since our bounced
messages went back to their mailing list address, the software just turned
them back around and sent them to the mailing list distribution again,
including all the people who couldn't accept mail. And guess what?  The
messages bounced again and again and again. There was nothing malicious that
I or any of the other victims needed to do to cause this loop, but if it
gets Netcom to straighten out their mailing list software then it's a good
thing.

Dave Methvin, Executive Editor, Windows Magazine  dmethvin@cmp.com

   [I guess that Dave can never have a WinDoze.  PGN]

---

Date: Mon, 26 Aug 1996 20:48:32 -0600
From: Brent Chapman <Brent@GreatCircle.COM>
Subject: Re: Denial of service ... Netcom listservers (Markowitz, RISKS-18.38)

I don't know anything about this incident or about Netcom's installation of
Majordomo (the mailing list management software in question), but speaking
as the original author of the software, let me quote the original design
paper ("Majordomo: How I Manage 17 Mailing Lists Without Answering
'-request' Mail", USENIX LISA 6 conference, 1992):

	... the goal is not absolute security, but to avoid people
	making a nuisance of themselves by abusing the Majordomo server.

By today's standards, Majordomo's "security" measures are incredibly weak;
they weren't particularly strong even 5 years ago, when the software was
written. Most lists are configured so that users can subscribe or
unsubscribe themselves, which is determined simply by checking that the
"From:" line in the header matches the address they're trying to
subscribe/unsubscribe, and thus trivially subject to forgery. Furthermore,
those operations that are "protected" are accessed through reusable
passwords sent in clear-text through e-mail, and thus trivially subject to
interception and reuse.

The next release of Majordomo (which will be version 1.94) will include a
simple challenge/response "confirm" mode for lists, where a supposed
subscriber will be sent pseudo-random confirmation string that they must
turn around and send back to the server before their subscription is
finalized.  This should significantly cut down on the spam subscriptions.
Version 1.94 is in alpha test now, and due for release sometime in the next
few months; send e-mail to majordomo-announce-request@greatcircle.com if
you'd like to be added to the list for notification when it's released, or
to majordomo-workers-request@greatcircle.com if you're interested in helping
with the development and alpha/beta test)

Clearly, I should have worked harder to keep folks from making a nuisance
of themselves with the original version of Majordomo.  Some days, I think
that releasing the damn thing was the biggest mistake I ever made...  :-)
And I now have a lot of sympathy for folks like Eric Allman (author of
Sendmail), whose creations have taken on a life of their own on the net...

Brent Chapman         | Great Circle Associates    | 1057 West Dana Street
Brent@GreatCircle.COM | http://www.greatcircle.com | Mountain View, CA 94041

  [RISKS is greatly indebted to Brent and majordomo.  They have greatly
  simplified my life, and will do even more in 1.94.  The challenge-response
  will also get rid of the jerks whose FROM: addresses are flagrantly
  unanswerable; on 28 Aug alone, I had to manually remove four would-be new
  subscribers whose given addresses bounced on the acknowledgement, and I
  had one more just before putting this issue out!  PGN]

---

Date: 28 Aug 1996 15:39:33 +0000
From: "Nick BROWN" <Nick.BROWN@DCT.coe.fr> (Tel (+33)88412674)
Subject: When the muzak goes quiet: risks of exception strategies

A few months ago, my wife was shopping in the supermarket when large lines
started to form at the checkout counters.  It turned out that (of course)
the whole payment system was down.

In this French store, the procedure to be followed in this case is very
simple: you wait.  I suppose the reasoning goes that even if all the
articles had price stickers, and all the checkout people had calculators
and/or very good mental arithmetic skills, there'd still be no point in
adding everything up by hand since the majority of people would have nothing
to pay with apart from their debit cards.

Anyway, after about half an hour, the lines got moving again, and my wife
made what turned out to be the right call: rather than dump her trolley and
hope that store employees would put all the frozen stuff back in the
freezers before bacteria decided to wake up and multiply for the next
customer, she made it through the line and was able to pick the children up
from school only a couple of minutes late.

I assumed this was pretty much all a store could do in this kind of case,
until I was in a Safeway supermarket in Britain last month [I think Safeway
UK is completely independent of Safeway US - NB].  While waiting in line at
the checkout, I was idly reading one of those stand-up signs that says
something like "to serve you better, this counter is closed", which was
waiting to be deployed on some unsuspecting victim.  When I turned it over,
however, I found another message, indicating that this supermarket chain, at
least, is prepared for when technological Armageddon strikes.  Here
(approximately) is what it said:

  "Owing to a technical problem, we are unable to process purchased items
  electronically.  Therefore, your bill will be calculated by multiplying
  the number of items in your basket by an average item price.  Thank you
  for your understanding."

Now, I presume this must be legal, because I said jokingly to the clerk "I
bet you hope that never happens" and he said "It happened when I was on duty
a few months ago".  Apparently the average item price (I wonder if this is
the average price of each stocked item, or a weighted average of what people
purchase) is around 94 pence, say US$ 1.42.  When the big moment comes, you
get the choice: pay the average price, or drop everything and leave the
store.

So, next time you're in Britain and the lights go low in the supermarket,
the message is clear.  Empty your trolley of canned vegetables and head for
the electrical goods and alcoholic beverages section.

The RISKS are numerous: huge financial losses for the store as savvy
comp.risks subscribers empty the shelves of foie gras and champagne;
confrontations between customers and clerks over the bill; and the store
(inadvertently) ripping you off if you just have to buy a pint of milk and
a small loaf of bread, right now.

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

End of RISKS-FORUM Digest 18.39 

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009222042/http://www.somewhere.com/)