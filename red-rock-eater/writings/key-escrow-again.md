---
id: key-escrow-again
title: key escrow again
type: writing
writing_type: rre-post
date: 2000-05-24
url: http://commons.somewhere.com:80/rre/1996/key.escrow.again.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - ai
  - cognitive-science
  - forwarded-content
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1996/key.escrow.again.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20000526162330/http://commons.somewhere.com/rre/) | **Most Recent Article: Wed, 24 May 2000** |

# key escrow again

```
[John Gilmore's analysis of the latest US gov't key escrow proposals,
plus a postscript.]

From:	IN%"gnu@toad.com"  "John Gilmore" 22-MAY-1996 07:22:01.12

I just read over the Clipper-III paper.  Here's the main scoop.  The
Government is trying to force key escrow on the world by incorporating
it into key certification systems.

They are playing on public ignorance of key certification, and are
trying in some cases to deliberately mislead people into thinking that
key certification and key escrow are the same thing.

Key certification is a way for a third party to declare that a
particular public key "belongs to" a particular identity.  E.g. that
key 85197FB5 really belongs to John Gilmore.  In PGP, people who know
you can "sign" your key to make this declaration.  Then, anyone who
trusts those people will know that your key is really yours.  When
they encrypt mail with public key 85197FB5, they can believe that
only John Gilmore can read it.

Key certification NEVER involves giving anyone a copy of your
private key.  Your private key is, and always should be, private to
yourself and nobody else.

Key escrow is a way for governments to get access to your private key
and read your private communications whenever they don't like what you
are doing or saying.  Or for any other reason.  So far, the only
government that is really pushing for this is the US government.
Their published policies for when they will access your key are
disturbingly non-specific.  I believe this is to cover for access by
the spy agencies such as NSA, which the public would not sanction if
it knew their current policies.

Even if the published policy for accessing your escrowed keys required
that a judge issue a warrant based on probable cause to believe a
crime has been committed -- which it doesn't -- that provides no
protection from a government that feels free to make any harmless act
into a crime.  As in the Soviet Union, lofty principles can be written
into the legal documents, but somehow citizens end up without
enforceable rights anyway.  I don't want to see my country go this
route, though it's obviously 80% of the way there already.

Because large-scale key certification systems will to some degree
involve centralization, they provide pressure points where the
government can try to force people to do bad things.  (One thing that
has kept the Internet free is that there was no central place to sue,
arrest, threaten, or otherwise terrorize into submission.)  In this
case, the bad thing they'll try to force is that the central
certification authorities will refuse to certify your key as yours,
even though they know it's yours, unless you first give the government
a copy of your private key.

Foreign relations are important to this policy, since if a significant
number of countries don't adopt this model then it won't work.  (Those
countries will build good crypto and export it, and it will leak out
around the world because of the worldwide demand for real privacy.)
The US is working hard in the OECD, the European Community, and in
one-on-one discussions with other governments, to convince them all to
impose key escrow on their citizens.

That's the scenario laid out by the Clipper-III paper.  It's a pretty
good strategy on their part.  Our job is to make it come out some
other way.

	John Gilmore

PS:  The whole paper is at http://www.eff.org/pub/Privacy/Key_escrow/
Clipper_III/960520_nist_clipper3_paper.draft.

Date: Thu, 23 May 1996 11:31:18 -0700
From: John Gilmore <gnu@toad.com>
To: Phil Agre <pagre@weber.ucsd.edu>, gnu@toad.com
Subject: Re: clipper iii 

[...]

One thing you should add is that digital signatures require key
certification.  A lot more people recognize the term "digital
signature" than "key certification".

The government is trying to hold digital signatures hostage in this
game.  Their paper says that escrow will only be required of "keys
used for confidentiality purposes and not keys used for signing
purposes", but my first take is that there is no practical difference.
An un-escrowed key certification hierarchy for digital signatures can
also be used for confidentiality.

	John
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20000526162330/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20000526162330/mailto:webmaster@somewhere.com). |