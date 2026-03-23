---
id: financial-cryptography-97-anguilla
title: Financial Cryptography '97 - Anguilla
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1997/Financial.Cryptography.9.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - administrative
  - auto-imported
  - civil-liberties
  - commerce
  - cryptography
  - democracy
  - education
  - forwarded-content
  - government-info
  - international
  - labor
  - law
  - libraries
  - military
  - privacy
  - rre
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/Financial.Cryptography.9.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991022234122/http://www.somewhere.com/)

  

# Financial Cryptography '97 - Anguilla

```
[Here is a report on the Financial Cryptography conference.  You'll observe
that it comes from a definite point of view that may not always correspond
to my own, but I think it's useful as a technical summary.  It's forwarded
with permission; it differs slightly from other drafts you may have seen
on the net (e.g., on cyperpunks) because of minor editing I've done at the
author's request.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Tue, 4 Mar 1997 20:39:21 -0000
From: "Duncan Goldie-Scot" <dgs@live.co.uk>

[...]

Financial Cryptography '97 - Anguilla
by Alex van Someren

The first Financial Cryptography conference, held in late February 1997 in
the Caribbean tax haven of Anguilla, proved to be a worthwhile forum for
serious work in the field of electronic money; this despite the dubious
honour of being rated the top 'deductible junket' in the January '97 issue
of Wired magazine.

The five-day programme of presentations on electronic commerce, e-money and
state-of-the-art cryptography was eclectic but concentrated on genuine
technical issues and was pleasingly free from the ravings of the extremist
privacy lobbyists so ubiquitous on the Internet.

The first day of proceedings concentrated on anonymity and unlinkability in
electronic transactions.  Of particular interest was the Janus system
developed by researchers at Bell Labs (Lucent Technologies, Murray Hill'
NJ, USA) for proxying Internet services including Web browsing.  Janus
automates the process of completing application forms for subscription
services at web sites, removing the need to invent new username/password
pairs for each service while at the same time preserving the anonymity of
the user.  Besides the anonymity issue, Janus has the potential to remove
several repetitive typing burdens on regular Internet users.

David Kravitz (BTEC/CertCo, New York, NY, USA) presented a proposal in
which e-cash anonymity could be controlled by the user.  For example,
he introduced the notion of 'distress cash'.  A user might have two pin
numbers, one of which guarantees anonymity while the other, if coerced by
a robber to reveal the pin code, would revoke anonymity and allow e-cash
tracing.

Unlinkable transactions

Also notable was work by a team including staff of AT&T Labs (Murray Hill'
NJ, USA) and the US Navy Research Laboratory (Washington, DC, USA) on
unlinkable serial transactions.  They proposed a system to allow membership
groups to be established in which members could prove the validity of their
membership without disclosing details of their identity or previous
transactions - such systems have considerable potential application in
electronic voting systems, for example, or for preventing Encyclopaedia
Britannica building a record of the pages you have visited.

On day two Simon Lelieveldt (Dutch National Bank, Amsterdam, NL) gave a
valuable insider's view on the recent Bank for International Settlements
report on the security of electronic money.  One interesting conclusion by
the BIS was the acceptance that it is possible to achieve better security
in electronic money systems than is offered by non-electronic systems in
present use.  He offered no general guidelines on preferred technical
solutions and stressed that the bank could only evaluate detailed
implementation plans and the likely consequences of  any particular scheme.

David Birch (Hyperion Consulting, UK) gave a rousing dissertation on the
global denationalisation of money and presented some compelling statistics
underlining the trend towards the disappearance of specie and the emergence
of self-issued 'loyalty' currencies from supermarkets and other major
retailers.  He also drew attention to the catalytic social potentials of
global electronic networks for the development of wholly new markets for
(and of) services and the need for real deployment of viable micropayment
systems in support of these markets.  In particular he stressed the
important role that smart cards will play and invited developers to study
Microsoft's specifications for smart card readers linked to PCs.

Fault induction attacks

One of the big encryption news stories last year was about fault induced
attacks.  Bellcore published a paper claiming that submitting smart cards
to microwaves and studying the mistakes the card made would make it
possible to reverse engineer the cards.  At the time it received some
exaggerated press comment, largely as a result of the original Bellcore
claims.

David Maher (AT&T, Mountain View, CA, USA) downplayed the threat of such
attacks, with particular reference to Mondex.  He also revealed that the
roll-out version of Mondex uses public key digital signatures.  Ultimately
it is the multi-layered security procedures which provide the protection:
David Maher was less willing to defend the 'security through obscurity'
whereby the Mondex protocols have not been published for public scrutiny.
Day three began with renowned cryptographer Ronald Rivest (MIT, Boston, MA'
USA and the R in RSA) giving a keynote speech setting out some perspectives
on financial cryptography and clearly demonstrating that his skill in pure
mathematics is matched only by his expertise in the applying the same.
Later, in his entertaining rump session, he proposed lottery tickets as a
form of cash and proved that there is a place in cryptography for humour as
well as mathematics.

Several speakers had applied themselves to the development of flexible
micropayment systems and the possible trade-offs afforded to their
deployment by using statistical sampling techniques in defence from the
dangers of double-spending - most transactions are offline but there is
sampling based on the assumed risk attached to each transaction.  In
particular, Yacov Yacobi (Microsoft, Redmond, USA) described an interesting
approach to reducing the need for online processing of e-cash transactions'
a widely-perceived obstacle to their successful deployment because of its
costs.

Law based approaches to security

Attention on day four focused on legal issues and the potential abuses of
e-money for money laundering.  A paper by Markus Jacobsson (UCSD, La Jolla'
CA, USA) and Moti Yung (BTEC/CertCo, New York, NY, USA) described a
technique making ingenious use of diversity and multi-party distribution to
increase the level of trust in e-money systems.

Their approach would require the co-operation of several banks or
regulators to originate and revoke anonymity in an electronic cash system'
a method more likely to be acceptable to civil liberties supporters than
many of its predecessors.

Edward Radlo (Fenwick & West, Palo Alto, CA, USA) delivered the latest
update of his on-going study of legal issues in cryptography from a U.S.
perspective - the airing of American feelings about Export Control
legislation and the First Amendment was largely limited to this session.
He believes that the FBI is now the main advocate of both strong export and
domestic controls.

Peter Swire (Ohio State University, Ohio, USA) suggested a contract model
for preserving consumer privacy, especially in the area of bank databases.
Michael Froomkin (University Miami School of Law, FL, USA) took the
argument a stage further by developing a model in which a large number of
certification authorities (CAs) provide graded certificates which are
trustworthy either to the extent of the procedural checks that the CA
carries out before granting a certificate or relies on customer trust of
known CAs.  He believes that CAs should be forced to accept limited
liability to pre-agreed levels.

Author Peter Wayner delivered an interesting perspective on the money
laundering business in his evening session.  He described a number of
ingenious schemes which have been used, many based on the false pricing of
otherwise conventional contracts. This was followed by a rump session of
short informal presentations.

Onion routing

In one, the US NRL team revisited their fascinating proposal  first
presented at the Workshop on Information Hiding in May 1996 (Cambridge'
UK), for a multi-layered 'Onion routing' technique for networks which is
highly resistant to traffic analysis.  This involves layerings of
encryption that resist eavesdropping and traffic analysis.  The scheme
would rely on having a large number of 'onion routers' on the Internet
(www.itd.nrl.navy.mil/ITD/5540/projects/onion-routing).

In another, consultant Adam Shostack (Boston, MA, USA) invoked Clausewitz
in his argument that cryptography is the ultimate post-modernist munition'
shared by anarchists and nations alike.

Gold Certification Authority

The final day included a plea from Paul Lampru (VeriFone, Atlanta, GA, USA)
for a 'Gold Certification Authority' standard to facilitate the public
deployment of e-money in support of healthcare and social security systems
- substantial civil liberties concerns were raised by the audience as a
result.

Theodore Goldstein (Sun/Javasoft, Mountain View, CA, USA) described the
security model underlying the Java electronic commerce framework (JCEF)
which would allow different financial services to work together.  The full
specification for JECF is at http://java.sun.com/commerce.  Sun's
open-minded attitude towards peer review of their software source code won
him a heartfelt and spontaneous round of applause.

Barbara Fox (Microsoft, Redmond, WA, USA) described a 'Grand Unified
Meta-Protocol (GUMP)' to reduce reinvention in the design of protocols for
e-commerce systems; she blamed working with physics graduates for an
acronym surely worthy of, if not deserved by, Microsoft.

David Kravitz (CertCo, NY, USA) presented a scheme for providing partial
anonymity for customers by shielding customer names from merchants.

Conclusions

Overall the conference was well attended, although representatives of banks
were notably absent, and its content was wide-ranging and highly topical.

Although the choice of location does not perhaps present the most
appropriate optics, Financial Cryptography is a conference which deserves
to succeed and which has got off to an auspicious start - the organisers
and programme committee are entitled to feel that they have made a real
contribution to the advancement of electronic commerce as we enter its
all-important deployment phase.

Alex van Someren is a founder and Managing Director of nCipher Corporation
Ltd., a start-up company delivering solutions for electronic commerce
systems. nCipher is based in Cambridge, UK and is affiliated with Newbridge
Networks Corporation.  http://www.ncipher.com - mailto:sales@ncipher.com

Endpiece

One of the many interesting side discussions at Financial Cryptography '97
worked through some of the potential of a global Internet stock exchange.

The starting point is that the existing markets are inefficient on a number
of levels.  They tend to be parochial - US investors invest in the US; UK
investors invest in the UK.  In any case, regulatory hurdles make it
difficult for people to invest directly in cross-border IPOs. The markets
are also too expensive - investors pay out exorbitant fees to mutual funds
and brokers for what is generally agreed to be an indifferent service.  The
markets are lop-sided in their information flows - professional analysts
are either briefed by company finance directors or, at least, have better
access to professional sources of information.  Finally, they are
ineffective at raising money for entrepreneurs.  An Internet stock exchange
could eventually help correct (partially at least) these problems providing
a low cost mechanism for Internet based IPOs and subsequent trading.  There
would have to be some specified level of due diligence and, to protect the
small investor, a requirement that investors prove they have the competence
and resources to make risky investments.  All investors would have equal
access to the company news pages with simultaneous news alerts being
emailed to interested investors as they are released.  Whichever investors
backed such a global exchange would have a strong economic incentive to
protect its reputation - outside the clutches of the SEC, state regulators
and, in the UK, the myriad of SROs. This model imagines an exchange with
its own clearing and settlement house which would hold electronic share
certificates and client accounts.  Ian Grigg of software house Systemics
(iang@systemics.com) suggested an interesting alternative.  Why not have
independent issuing houses whose reputations and thus business prospects
would stand or fall on their track record?  They would issue clients with
digital stock certificates which could, when the markets became
sufficiently liquid, be traded on any of a number of competing Internet
based stock exchanges.  As it is assumed that these exchanges would be
automated price/time order matching systems, there would be no role for
brokers.  However, there would be a role for independent market makers to
quote a bid/ask spread on illiquid stocks and also for the usual gamut of
would-be gurus peddling their charts and analyses of prospects.  It quickly
becomes apparent that we don't really need all these expensively paid
brokers with their marble halls and $1m bonuses or any of the mutual funds
with their thousands of door-stepping salesmen.  If an investor wants to
track the market, he can download a routine to build the appropriate index
(or unitised indices for the small investor).  As Simon Fedida
(windjammer@cableinet.co.uk) pointed out last month, there are already
companies offering quantitative analysis routines for the private investor.

Does this all sound a far-fetched flight of fancy?  We'll find out more
next month with reports on the progress of plans for Internet stock
exchanges in the US.

Duncan Goldie-Scot
dgs@live.co.uk

<snip>

Duncan

---

Duncan Goldie-Scot
Editor
Financial Times Virtual Finance Report
172 Tachbrook Street
London SW1V 2NE
Tel: +44 171 834 2460
Fax: +44 171 976 6592
Email: dgs@live.co.uk
Web: http://www.live.co.uk/Ftvfr.htm

---

Type Bits/KeyID    Date       User ID
pub  1024/4E138C75 1997/03/04 Duncan Goldie-Scot <dgs@live.co.uk>

-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: 2.6.3ia

mQCNAzMcLSYAAAEEAOXC2HiHJSu/IUwSnnapkaK0QihE826dVUCH7UpyQKQTFQMa
FdZ60/3+cXq1zz+kQ3TaYSwiBAVjMeuIgSa62H66ih4j/mGbBk2+z4ZETj3bfXpC
Gk1gDJCfLwvV7LmOhyLSVucG5iMJe5Acv5+psE12p2P15/R3EX/bsa9OE4x1AAUR
tCNEdW5jYW4gR29sZGllLVNjb3QgPGRnc0BsaXZlLmNvLnVrPokAlQMFEDMcLSZ/
27GvThOMdQEBL2wEANDrT1rAMyIdpHiBem8VFtiBb08YbLyuODYYhVsI/7p81fpI
hpbNz8WK7ZzzKBhoRflVL+F5rvmcZNnI1WrQSvKxAezvTINTpaZSct+62LgOMJvc
uzJ614S0l3J+zeum/3AwfPuZN3rK7mHnt2k8Vgs6xalNPezoEBrsxTdpnb4H
=RFsu
-----END PGP PUBLIC KEY BLOCK-----

--- end forwarded text
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991022234122/http://www.somewhere.com/)