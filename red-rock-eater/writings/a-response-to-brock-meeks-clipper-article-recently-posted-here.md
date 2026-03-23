---
id: a-response-to-brock-meeks-clipper-article-recently-posted-here
title: a response to Brock Meeks' Clipper article, recently posted here
type: writing
writing_type: rre-post
date: 1994-06-08
url: http://commons.somewhere.com:80/rre/1994/a.response.to.Brock.Meek.html
coauthors: []
key_concepts:
  - privacy
  - surveillance
importance: 6
research_status: partial
tags:
  - civil-liberties
  - cryptography
  - forwarded-content
  - government-info
  - privacy
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1994/a.response.to.Brock.Meek.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991008162627/http://www.somewhere.com/)

  

# a response to Brock Meeks' Clipper article, recently posted here

```
Date: Wed, 8 Jun 94 12:17:53 EDT
From: lethin@ai.mit.edu (Rich Lethin)
Subject: [pagre@weber.ucsd.edu: Re:  Clipper (strong language -- parental discretion advised)]

Phil,

I believe Brock Meeks's Cyberwire dispatch, "SNAFU Redeux" overstates the
flaws in Clipper.

Two mathematicians (S. Brent Morris and Mark Unkenholz) from the NSA were
here on 6/2/94 for an MIT Theory of Computing Seminar to give a technical
overview of the Escrow Encryption Standard.  At the end of their talk they
talked about what Blaze found (it had been reported that day in a NYT
article).

I'm not a "cryptographic expert" but I can try to relay my understanding of
what they said.

They explained how keys are used in the Clipper and Capstone chips.
Several keys are involved - the session key, the chips's internal key, a
family key, and a 16-bit checksum used to authenticate the Law Enforcement
Access Field (LEAF).

Blaze found that a 20-minute exhaustive search could generate a bogus LEAF
that the receiver would accept as valid.  I don't remember whether they
said that this bogus LEAF (used to do the authorized wiretapping) would not
be usable for wiretapping but even if so, it is not news that the ability
to wiretap can be defeated by using alternate cryptographic techniques.

The polemic surrounding Clipper has gotten out of hand.  At the
NSA/Morris/Unkenholz talk, we got only 15 minutes of technical content in
the 1.5 hour duration because several members in the audience couldn't
suppress their charged second-guessing of nearly everything the speaker
said.  The moderator (Silvio Micali) intervened twice to ask people to
stick to technical questions and to stop repeating questions.  Toward the
end, people interested in technical content were booing those questioners
and calling for them to shut up.  It was an embarrassment to MIT and the
department.

Meek's dispatch, while entertaining is of the same caliber and matches the
general tenor of much of the net's discussion about Clipper, in that it's
more agitprop than information.

While the Skipjack algorithm used for encryption is not public, the
information about what gets encoded and how, how long the keys are, and the
details of the escrow programming and manufacture is public and would be a
couple of paragraphs long.  Why not just include that information as a
matter of course in these articles?

(To try to avoid making the same mistake myself, for people looking for
that information, I recommend looking at the FTP server maintained by the
EFF (ftp.eff.org) in the directory /pub/EFF/Policy/Crypto/Clipper.
Morris/Unkenholz said that the NSA was preparing a short technical spec to
be released soon.)

The major technical flaw in Clipper is that the escrow scheme can be
subverted by a single agent at manufacturing time.  When the Chips are
manufactured, there's a "single-failure-point" where the two keys and the
chip's ID all live in the same spot.  The key generation algorithm is via
an "algorithmic black box" at the manufacturing site.  Thus, rather than
requiring the subversion of the two escrow agents for unauthorized
wiretapping, the manufacturer of the chips (Microtronics) and the designer
of the algorithmic black box (NSA) could do it by themselves.

Of course, the other technical problem in Clipper concerns the secrecy of
Skipjack (the encryption algorithm itself), which could have an algorithmic
back door built in.

Much better escrow algorithms do exist, which do not have any of these
flaws.  Silvio Micali here at MIT has a TR about such an algorithm, which
allows a user to use his own encryption algorithm, key choice, etc. and
still inform k escrow agents that can verify their portion of the key is
enough without knowing the whole key.  It might be the case that Clipper
was designed and chosen before such protocols were discovered/designed.
It's no revelation that "government or mil spec" often lags state of the
art; Clipper is probably just one more example.

There are some other really interesting issues wrt to Clipper.  The NSA
manufactures the chips to physically deter reverse engineering...  how?
The NSA expects that the chip eventually will be reverse-engineered, and
has patented the algorithm to retain control over it (the patent will be
issued when the algorithm gets disclosed).  Because the algorithm is going
to eventually be public, the NSA openly admits that it's not one of their
most secure systems: they don't want "bad guys" to use the algorithm on
their own, and mil-grade traffic can't be carried by Clipper.  It seems
like they expect that by the time the algorithm becomes public, they will
have, or be able to break it economically.  A discussion of the "sliding
window" of vulnerability would benefit potential Clipper users, informing
them of the cost of cracking their communications and making informed
tradeoffs versus the value of the data their transmitting.

Rich
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991008162627/http://www.somewhere.com/)