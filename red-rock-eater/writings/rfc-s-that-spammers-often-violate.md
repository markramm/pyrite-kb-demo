---
id: rfc-s-that-spammers-often-violate
title: RFC's that spammers often violate
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1997/RFC.s.that.spammers.ofte.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - forwarded-content
  - internet-policy
  - libraries
  - rre
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/RFC.s.that.spammers.ofte.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991005060745/http://www.somewhere.com/)

  

# RFC's that spammers often violate

```
[Dean's message provides additional grounds for complaint against spammers
who try to hide by providing bogus domain name information.  Also, for the
detailed Internet standards for mail etc, see http://www.imc.org/rfcs.html
See especially Extended SMTP (ESMTP), at http://www.imc.org/rfc1869 .]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date:         Sat, 15 Nov 1997 00:52:15 -0500
Reply-To:     Dean Robb <pceasy@NORFOLK.INFI.NET>
Sender:       Spam Prevention Discussion List <SPAM-L@PEACH.EASE.LSOFT.COM>
From:         Dean Robb <pceasy@NORFOLK.INFI.NET>
Subject:      RFC:  Proposal to InterNIC; other info

After spending the day buried in research, I've found a possible tool in
the anti-spam war.  First, in researching the applicable RFCs (available at
the InterNIC FTP, browser-readable) I discovered the following RFCs that
have applicability in getting spammers dealt with.  They're technicalities,
but hey...Capone went up on a tax rap.

RFC 2050, sec 4, #4 provides for the audit of a domain administrator's
registration information and the invalidation of his IPs for false/invalid
information.

RFC 1032 requires domain registration information to be complete, correct
and current.

RFC 920 requires a responsible INDIVIDUAL to be named as the technical/zone
contact in the domain registration info.

RFC 1173 (esp. sec. 2 and 4) and RFC 1174 spell out the responsibilities of
a domain host and network managers.

Now...why do we care?  Simple.  When we do a whois, and the domain
information is missing (like the guy who's contact address was "x") or
bogus (Reg Dom, domreg@PEC.net)...they have violated these RFCs.
Technically, they can't have an IP address.  RFC 1173/1174 state clearly
that it is the responsibility of the network managers hosting domains to
ensure that they follow the guidelines set down by the RFCs.  Therefore, if
the WhoIS info is bogus, the domain is illegitimate, and it is the ISPs
responsibility to fix the issue.

This can be useful for those ISPs that won't shut down a website because
the spam was sent via another network...here we have an argument as to why
the website should be shut down.  Chances are, the registration is invalid.

Additionally, many ISPs will do the initial registration for their clients,
and then the spammers can go in and edit the info to remove the
incriminating information.  If this is the case, then we have another tool
to bash the ISP with.

One other thing:  One of these RFCs requires the valid postmaster@domain
account.  For those spammers that we've discovered route that address to
dev/null, we can once again use that as an argument to shut them down.
Sorry...after reading all those RFCs and the InterNIC stuff...my brain is
semi-mush.

Now...on InterNIC.

As I noted in another post, their Registration Agreement says in no
uncertain terms that the information provided must be correct and stay
correct.  Now, InterNIC is not going to have the resources to back-check
all the domains for validity.  However, I intend to propose to them on
Monday that they verify those domains that we complain about (we being
anyone) having invalid information.  This provides the identification
mechanism...all they have to do is check the correctness of our information
and then nuke the domain.  I will argue to them that it would accrue the
following benefits:

1.  Cut down on net abuse.  If we take away a spammer's anonymity,
he/she/it might think twice.

2.  Help InterNIC fulfill it's contractual obligations to provide
registration services and WhoIS information.  What good is a searchable
registry if the information is bogus?

3.  Improve InterNIC's reputation by showing that they're trying to take
good care of the registry.

4.  Increase their profits.  If the registration is invalid, there's no
provision for a refund.  The spammer would have to pay again.

5.  Help the overall health of the 'Net.  One of the reasons for the
contact information in the registry is to provide a way to get hold of a
domain in case of a problem.  If the contact info is non-existant or bogus,
you can't very well get hold of them, can you?

Peripherally, it'll help the spam fight, too.  At the very least the
information would have to be correct...making it easier for us to get at them.

Comments?  Remarks?

Dean Robb
PC-Easy
On-site computer services
(757) 495-EASY [3279]
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991005060745/http://www.somewhere.com/)