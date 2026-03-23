---
id: http-cookie-privacy-risk
title: HTTP cookie privacy risk
type: writing
writing_type: rre-post
date: 1996-06-10
url: http://commons.somewhere.com:80/rre/1996/HTTP.cookie.privacy.risk.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - community-networking
  - cryptography
  - privacy
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1996/HTTP.cookie.privacy.risk.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009071641/http://www.somewhere.com/)

  

# HTTP cookie privacy risk

```
[We badly need a coherent general way of thinking about what it means
for other people's code to be running on our personal computers, and
for programs on our personal computers to be talking with programs
on other people's computers, including people we don't know or trust.
In a sense this is the coming-home-to-roost of a confusion inherent
in the concept of a personal computer.  The people who invented the
personal computer said to themselves, "hey, it's personal, so we don't
need a full-blown operating system with real security".  So first we
had viruses, until finally we systematized the kludges by which we
fend off the viruses.  Then we connected our personal computers to
the Internet, and I don't think we've seen a tenth of the heck that's
going to break loose from that.  The root problem here is that a
"personal computer", despite its misleading name, is fully as social
a creature as the old time-sharing systems ever were.  And yet their
design embodies no coherent model of how to negotiate those social
relationships.  The damage could be considerable.  Part of the damage
may come from misguided panics to one extreme or the others.  Cookies,
for example, are often treated as alien creatures invading our web
browsers.  And they could easily become that.  But they could just
as easily become a technology of privacy protection: so long as the
cookie doesn't identify you, there's a limit to how much damage it
can do.  Unfortunately, if your computer has its own unique Internet
address then that's sort of like a phone number, so that the whole
Internet comes with a built-in Caller ID that you can't easily turn
off.  We need to understand these things soon, before bad solutions,
knowingly or not, turn into market standards.  End of editorial.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Mon, 10 Jun 1996 18:16:05 -0700 (PDT)
From: risks@csl.sri.com
Subject: RISKS DIGEST 18.19

RISKS-LIST: Risks-Forum Digest  Monday 10 June 1996  Volume 18 : Issue 19

---

Date: 8 Jun 1996 01:38:13 GMT
From: hgoldste@bbs.mpcs.com (Howard Goldstein)
Subject: HTTP cookie privacy risk

I recently installed Netscape 3.0b4, a beta version, to try out the new
(compared to 1.1N) features and see how well FreeBSD runs foreign binaries.

One of the new features, a security feature strangely categorized as a
'network' feature, queries the user before allowing "cookies" to be set.
Out of curiousity I set it so as to find out how often this feature was
invoked.  Cookies (discussed in earlier RISKS volumes, I seem to recall)
[YES: RISKS-14.36, 17.89.  PGN] are documented at
http://www.netscape.com/newsref/std/cookie_spec.html .

I was surprised to find that every night for the last two weeks after
enabling this I've been handed a "cookie" by a site I never knowingly
visited, at http://ad.doubleclick.net .

Upon visiting this site I discovered they engage in attempts to collect
various data about web users including their o/s.  Why they feel it
necessary to 'ping' me each night to set a cookie I do not know, but it
seems they are also collecting data about browser usage.  Such a statistic
regarding times online while in a browser would seem valuable from a
marketing standpoint.

While cookies may be useful when voluntary and insofar as they may be
helpful to the user (as I feel the cookie I'm handed that avoids an access
validator for a particular newspaper's site).  Cookies from marketing
companies benefit me not.

Categorize this as a risk to users of older netscapes lacking the
conditional-cookie setting?  Or to advertisers who will find their targets
are hidden behind "mini" HTTP firewalls that hide the users from cookies
along with advertisement filter such as the one being tested by a North
Carolina startup?

Howard Goldstein   <hg@n2wx.ampr.org>

  [And you'd probably be surprised to know how many people are affected.
  But you know there has to be a gotcha with free web sites and free
  browsers, and lots of folks are selling lists.  Always look a gift
  Trojan horse in the mouth (and everywhere else too).  PGN

---

End of RISKS-FORUM Digest 18.19 

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009071641/http://www.somewhere.com/)