---
id: windows-security-bugs
title: Windows security bugs
type: writing
writing_type: rre-post
date: 1996-01-10
url: http://commons.somewhere.com:80/rre/1996/Windows.security.bugs.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - forwarded-content
  - rre
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1996/Windows.security.bugs.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991006085245/http://www.somewhere.com/)

  

# Windows security bugs

```
[This is a little out of context, but it provides pointers to further
information.  I take no stand on whether its criticisms are just.]

Date: Wed, 10 Jan 96 11:07:48 PST
From: RISKS List Owner <risko@csl.sri.com>
Subject: RISKS DIGEST 17.62

RISKS-LIST: Risks-Forum Digest  Weds 10 January 1996  Volume 17 : Issue 62

---

Date: Mon, 8 Jan 1996 19:16:50 -0800
From: Rich Graves <llurch@Networking.Stanford.EDU>
Subject: Microsoft continues to mislead public about Windows security bugs

Please do not dismiss this as mere "Microsoft Bashing." c2.org has
similar promotions running for Netscape, DigiCash, and Java. 

The following is a quote from Microsoft's "Knowledge Base" technical
support and marketing database, which is online in CompuServe and at: 

  http://www.microsoft.com/kb/peropsys/windows/q90271.htm

  Security of the Windows for Workgroups Password Cache
  _____________________________________________________

  The password list file is encrypted with an algorithm that meets the U.S.
  government Data Encryption Standard (DES). This encryption technology is
  the highest security allowed in software exported from the United States.
  The odds of breaking the encryption algorithm are less than those for
  random guesses of what the password might be.

  Even if your logon password is blank, Windows for Workgroups generates
  seemingly random data in your PWL file, so you cannot discover the
  passwords if you look at the PWL file using a file viewer. Currently, no
  user interface exists that allows you to unencrypt passwords in the PWL
  file, so password caching in Windows for Workgroups is as secure as the
  choice of the password used to encrypt your PWL file.

As Microsoft well knows, this is completely untrue. The rest of the world
has known that this is untrue since November 29th. Microsoft quietly
acknowledged on December 7th (after a day of much "Internet Strategy"
hype, and after the deadline for the morning papers) that the exact same
implementation was insecure in Windows 95, and claims to have released a
patch that fixes the problem (the efficacy of the Win95 patch does not
appear to have been verified by anyone outside Microsoft, however). 

Microsoft has not even admitted that this bug in both Windows 95 and
Windows for Workgroups affects Windows for Workgroups, apparently because
they have decided not to fix it. 

Information on the .PWL implementation bugs was first broached on the 
sci.crypt newsgroup in late November 1995, then discussed on the 
cypherpunks list and refined for Community ConneXion's "Hack Microsoft"
promotion, http://www.c2.org/hackmsoft/.

We have since been given a sample trojan horse that will very efficiently
exploit this bug in Windows for Workgroups. Distributed as a Word Basic
virus, MIME attachment, or downloadable archive (note that Exchange and
Internet Explorer unwisely execute downloaded binaries without even a virus
check, a problem that Sun's Java has long acknowledged and addressed), this
trojan horse could collect passwords and other sensitive information from
.PWL files and other sources and send them out via e-mail, possibly through
an untraceable chain of remailers or to a throwaway trial account on, for
example, America "Online."

We believe that it would be highly irresponsible to release the full version
of this hack, but we will soon release a crippled demonstration-only version
if Microsoft does not at the very least admit that this problem has always
affected Windows for Workgroups, correct their online documentation, publish
the specifications of the Win95 security patch for review by outside
security experts, and issue a public retraction.

See also:

  http://www.microsoft.com/kb/peropsys/windows/90210.htm
  http://www.microsoft.com/windows/pr/clarifications.htm
  http://www.c2.org/hackmsoft/

  http://www-leland.stanford.edu/~llurch/win95netbugs/faq.html

  {mirror of above} http://www.mari.su/guide/win95/
  {mirror of above} ftp://ftp.demon.co.uk/pub/mirrors/win95net/
  {more mirrors are under construction in Australia and elsewhere}

In other news, I assume everyone knows by now that NT's claimed C2 security
rating was granted *for use a standalone workstation only*. It has been
widely reported that its NetWare Services implementation does not ask for
passwords for nonexistent usernames, making a potential cracker's job that
much easier. The correct response, which is given by real NetWare servers
and other servers that are certified C2-secure on networks, is to silently
ask for a password in all cases.

I started getting copies of hackmsoft@c2.org mail on December 20th. It's
really depressing.

We've also seen problems with Microsoft Access 95's security. Basically,
there is none. Anyone can access the network-enabled Access as any user
without knowing the password. We don't think it would be responsible to
publicly release this hack, either, until Microsoft has had another chance
to patch the hole (they've known about it for some time).

These are far, far worse than the widely publicized bugs in Netscape's SSL
implementation, which have been fixed. Yet the only place I've seen them
mentioned is the lapdog Seattle Times, which only reports bug fixes in
glowing terms.

Is anybody listening?

- -rich
 owner-win95netbugs@lists.stanford.edu
 ftp://ftp.stanford.edu/pub/mailing-lists/win95netbugs/
 gopher://quixote.stanford.edu/1m/win95netbugs
 http://www-leland.stanford.edu/~llurch/win95netbugs/faq.html

---

End of RISKS-FORUM Digest 17.62 

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991006085245/http://www.somewhere.com/)