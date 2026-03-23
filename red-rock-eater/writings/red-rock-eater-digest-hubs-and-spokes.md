---
id: red-rock-eater-digest-hubs-and-spokes
title: Red Rock Eater Digest - Hubs and Spokes
type: writing
writing_type: rre-post
date: 2000-01-01
url: http://commons.somewhere.com/rre/2000/RRE.Hubs.and.Spokes.html
coauthors: []
importance: 6
research_status: partial
tags:
  - education
  - internet-culture
  - media
  - military
  - telecommunications
---




## Source

Automatically imported from: http://commons.somewhere.com/rre/2000/RRE.Hubs.and.Spokes.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](http://commons.somewhere.com/rre/) | **Most Recent Article: Tue, 15 Aug 2000** |

```
---

This message was forwarded through the Red Rock Eater News Service (RRE).
You are welcome to send the message along to others but please do not use
the "redirect" option.  For information about RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html

---

Date: Thu, 27 Apr 2000 10:19:43 -0700
From: Jessica Marantz <jmarantz@telegeography.com>

HUBS AND SPOKES:
A TELEGEOGRAPHY INTERNET READER

by TeleGeography, Inc.
Washington, DC: TeleGeography, 2000
ISBN 1-886142-23-8

http://www.telegeography.com/Publications/hs00.html

TABLE OF CONTENTS

Introduction

Global Internet Primer
	Architecture
	Finance
	Governance
	Demand
	Voice
	What Next?

International Internet Bandwidth
	Providers
	Connectivity
	Exchanges

International Internet Indicators
	Network Metrics

Reference

GLOBAL INTERNET PRIMER: FINANCE

Who pays for the Internet?  "The answer is either really long or
really short depending on what you're trying to say," says Scott
Bradner, a leading Internet expert at Harvard University.  The
Internet does not have a set economic model, so there's no standard
way network providers are remunerated for the resources they use.
End of story.

The longer answer is more complicated, precisely because the
Internet's provisioning model is not static.  Whereas a typical call
over the public switched telephone network (PSTN) involves two or
three different networks, a typical Internet transmission may involve
five or ten.  And the connectionless transmission technology on
which the Internet is based also means that the role of each of these
networks cannot easily be predicted in advance.  Smaller networks
typically pay larger networks for connectivity, but many larger
networks themselves exchange their traffic without charge under a
peering, sender-keeps-all basis (see Figure 1, "A Primer on Peering").
They seek to recoup their network costs primarily from their end users
and their downstream ISP customers -- not always from other networks,
as in the telephony world.  To understand why the Internet's schemes
for funding international networks are so different from the traffic-
based settlement arrangements over the PSTN, a brief digression on
technology is useful.

The Connectionless Network

Traditional phone networks, built for voice communications, switch
or assign a dedicated end-to-end circuit for every call.  That is
reliable, but oriented heavily toward a limited set of applications
whose bandwidth usage is fairly steady: every connection needs its
own circuit.  Minute-by-minute and circuit-by-circuit payment methods
consequently developed to compensate network providers.

The Internet is a radical departure from this pattern.  It is based on
packet switching: no dedicated connection is required, and a dedicated
route doesn't have to be set up between sender and receiver.  Instead,
all communication is converted to digital format, broken up into
chunks of data called packets or datagrams, given an address, and sent
out into the network -- packet by packet.  What's most significant
is that the path each packet takes may be radically different: all
they have in common is that they end up in the same place, ready
to be reassembled into a coherent message. That makes it hard to
bill Internet communications in the way that traditional phone
communications are billed.  But it is more efficient for moving
traffic around when that traffic may consist of a tiny message sent
one moment, a huge graphics file the next, and then nothing for a
few minutes -- what traffic engineers call "bursty traffic," because
it comes in sudden bursts.

Some have compared the process to mailing a book through a postal
service that accepts only postcards: each page must be sent
separately, and arrives individually; the receiver must reassemble the
pages back into the right order before reading.  When first proposed
in the 1960s by Paul Baran, in the U.S., and separately by Donald
Davies in the United Kingdom -- and later refined in the early 1970s
by pioneers like Robert Kahn and Vint Cerf -- it sounded like a
crazy idea.  But it worked.  (For an engaging history of the period,
see Peter Salus' book, Casting The Net.)  Since the early principles
of Transmission Control Protocol/Internet Protocol were published
by Kahn and Cerf in a paper entitled "A Protocol for Packet Network
Intercommunication" (IEEE Transactions on Communication, May 1974),
packet delivery has not changed much.  Along the way, routers --
computers acting as "smart" switches, as opposed to the automatic
forwarding of bridge switches -- still store and forward packets.
After forwarding, if the first router doesn't receive acknowledgment
that the packet has arrived safely at its destination, it resends
the packet.  The protocol self-adjusts to achieve the best possible
service; routers send packets as fast as they can with the lowest
error rate.  And in socialistic fashion, all packets are treated
equally, on a best-effort basis.

It wasn't very reliable, and still isn't.  If there's a lot of
congestion on a single route, packets are dropped -- not such a good
thing for time-sensitive traffic such as telephone calls.  But the
original designers cleverly built in robustness.  Because routers
are simply dedicated computers, they can make sophisticated decisions
about how to route traffic most efficiently.  And when the network
is congested or a link lost, they can find out about it and choose
another route -- so that if a backhoe digs up a cable, or a fishing
trawler cuts one in two, it is a problem, but not necessarily the
end of the line.  With network information and topology that is
well-distributed, properly configured, and actively maintained, the
Internet should be able to route around any central point of failure.

With the basic architecture and design principles already in place,
the U.S. National Science Foundation (NSF) began funding data
networking pioneers at 13 supercomputing centers across the U.S. in
1985.  A nationwide circuit for the traffic was commissioned.  The
academic institutions had to strike deals with local telecom providers
to lease local and regional circuits.  More and more institutions
sought to be connected to the NSFNET backbone, the network's main
transport infrastructure.

Things moved quickly.  As the network had grown, more and more uses
were found for it -- but as long as the National Science Foundation
ran the backbone, its Acceptable Use Policy (AUP) was the formal
framework for what kind of traffic could run over its facilities:
"NSFNET backbone services are provided to support open research and
education in and between U.S. research and instructional institutions,
plus research arms of for-profit firms when engaged in open
scholarly communications and research.  Use for other purposes is not
acceptable."  In 1991, three private IP networks -- General Atomics
(CERFnet, now owned by MCI WorldCom), UUnet (now owned by MCI
WorldCom), and Performance Systems International (PSInet) -- danced
around the AUP by creating the Commercial Internet eXchange (CIX,
www.cix.org), an open peering point for the exchange of network
traffic.

The idea stuck.  The Internet had proved its commercial viability;
by 1992, the U.S. government wanted out, and the NSFNET's backbone
transmission network was privatized -- and began to accept commercial
traffic, marking what may have been the beginnings of the Internet
as we now know it.  Then, in 1994, the NSF commissioned four network
access points (NAPs), essentially traffic exchange points similar in
function to CIX, located in southern New Jersey, outside Washington,
D.C., Chicago, and San Francisco.  All were run by different
telecom operators.  In a remarkably short period of time, the basic
ingredients of today's global Internet had emerged.

Of course, an application from outside the traditional Internet
community would dramatically shake things up.  The World Wide
Web, developed by Tim Berners-Lee and popularized around 1993, was
soon followed by the Mosaic browser, forerunner to Netscape.  The
exponential growth the Internet had seen until then -- users and
host counts generally doubled annually -- hit massive proportions
and backbone traffic surged.

What You Pay Depends On What You Do

Back to the economics.  Traffic, as we have seen, is routed over
the Internet on a virtual pathway without fixed routes or network
connections.  The physical networks which make up the Internet --
typically leased circuits from telephone companies -- do interconnect,
though.  And networks do exchange traffic.  The economics of how that
happens are key to understanding who pays for what on the Internet.

That said, the Internet industry has matured enough to make basic
distinctions between different categories of service providers or
ISPs.  Doing so provides, in part, the answer to how international
infrastructure providers, such as telcos, are and will be compensated.

The generic term "Internet service provider" (ISP) has become
meaningless.  It does not distinguish, for instance, between large
international ISPs (IISPs) with global infrastructure (such as MCI
WorldCom or PSINet), or local online providers that bundle content
with the access services they buy for their customers, such as EasyNet
in Europe (www.easynet.co.uk), AsahiNet in Japan (www.asahinet.or.jp),
or CAIS Internet (www.cais.net) in the U.S.  Nor does it take into
account whether the service provider's customers are individual users,
who tend to request content; content providers who pay to export
data; or other transporters of data.  These differences can weigh
heavily: unlike telecom finance, Internet cost recovery may involve
compensation both for transporting bits, and for the kind of bits
being carried -- content.

Better, then, to break down the industry into four classes: (1) firms
that specialize in Web site hosting, such as Exodus (www.exodus.net);
(2) downstream ISPs who buy most of their long-haul backbone transit;
(3) online service providers which bundle Internet access with a
focus on content and interface, like AOL and Japan's NiftyServe
(www.nifty.ne.jp); and (4) backbone ISPs.  The cost structure and
the money flow is determined by the category to which one belongs.
And because most players belong to different categories at different
points in their activities -- even most backbone ISPs tend to be
downstream from someone else -- those cost structures are complicated
affairs.  Taken together, though, the worldwide market for Internet
access is now big business: it was to have grown from $25 billion in
1997 to more than $100 billion in 2000, according to Zona Research
(www.zonaresearch.com).  Let's take a look at the components.

Content Hosting Providers

Web server "farms" emerged from the ISP industry itself, but are
now somewhat separate: companies have made Web hosting into a niche
business and are growing rapidly.  The important fact is that their
traffic flow is mostly uni-directional -- the antithesis to the
bilateral, unmetered peering arrangements of old.  Instead, the few
bits of data that trickle in when a user requests a Web page are
overwhelmed by the flood of outgoing audio, video, image, and text
objects.  As a result, backbone ISPs demand that hosting providers,
which typically do not maintain a national network, purchase
connectivity from a backbone or downstream ISP whose customers seek
the content.

This can lead to conflict.  Web hosting firms claim that backbone
ISPs are already compensated by their end customers, so that to seek
compensation from the content provider would mean a double payment.
The backbone ISP counters that it is forced to haul the content
provider's traffic on its own network to reach its customers -- and
it wouldn't need so much infrastructure if the server farm had its own
national network.  Backbone ISPs thus only agree to accept a server
farm's traffic at a price.

In August 1998, a peering dispute erupted between GTE Internetworking
and Exodus over this very issue, and both firms' customers came close
to losing direct connection to one another.  Since then, the issue
has continued to simmer.  Though access providers still have the upper
hand in negotiating peering agreements with content providers, the
situation has evolved considerably, and negotiations now typically
depend on the perceived value of the content to the access provider's
customers.

Downstream ISPs

A similar logic is used for downstream ISPs, who provide Internet
access to even smaller providers, corporate customers, and end users.
The price of Internet connectivity varies by location and amount
of data.  In late 1998, for example, a downstream ISP in Cambridge,
Massachusetts could lease a 45 Mbps circuit for $2,500 per month.  But
that paid only for the facilities required to meet the gateway of an
upstream backbone ISP.  The price to connect with the backbone, which
lets the downstream ISP's customers reach other destinations on the
Internet -- this arrangement is usually known as "transit," as opposed
to "peering" (see Figure 2, "Exchanging Traffic") -- can be as high as
$30,000 per month.

While the connection fee may seem a crippling cost for U.S.-based
ISPs, service providers outside the U.S. must also pay for the cost
of an international private line if they wish to connect directly with
the Internet at its core.  Such a connection does not come cheaply --
trans-Pacific circuits, for example, were in 1998 going for as much as
$60,000 to $80,000 a month for a 45 Mbps line.

However, most downstream ISPs and large corporate users that purchase
Internet connectivity do not pay based on their actual usage, bit by
bit, but based on a usage profile, broken down into different tiers.
It would be too expensive and the tools too awkward to meter and
charge every data flow.  Indeed, many Internet engineers believe the
cost of measuring and billing for exact usage could put a debilitating
premium on Internet service.  Lest the dilemma seem fanciful, consider
the U.S. long distance telephone business.  With coast-to-coast
U.S. rates of $0.07 a minute or less, up to 40 percent of the rate
for long distance telephony may reflect the costs of monitoring and
monthly billing.

So on the Internet, the backbone ISP's network measures the overall
traffic pattern by glancing at the router's bytes in and bytes out
and charging the downstream ISP accordingly.  This allows a customer
to lease a line with much more capacity than is ever used, pay a
sum closer to the actual usage, and be assured that should traffic
spike, the line can meet the demand for an additional fee.  The only
drawback with this approach is that it sets up an incentive for the
upstream ISP to overbook capacity, under the hopeful (and reasonable)
assumption that all customers do not generate peak loads at once.
At MindSpring Enterprises Inc. (www.mindspring.net, now part of
EarthLink), chief executive Charles Brewer said in 1999 that 30
percent of company costs derive from connectivity fees and 13 percent
from customer service expenses.  He expected a complete reversal
within five years, as bandwidth becomes a commodity and ISPs must
differentiate themselves more by the services they offer.

Online Service Providers

Online service providers like AOL earn revenues not by reselling
network transmission service, but by bundled Internet access
with proprietary content and specialized commerce, selling ads,
and providing users with the ease-of-use which comes from special
software interfaces and customer hot-lines.  They are typically
the customers of upstream access and backbone providers, which also
manage the network points of presence (PoPs) accessed by dial-up
retail users.  AOL, for example, has outsourced nearly all of its
network transmission needs to MCI WorldCom subsidiary UUNet, though
it maintains a multi-vendor strategy to ensure redundancy.  Even AT&T
relied at one time on BBN's network, since acquired by GTE, to connect
leased-line commercial users.

The online service provider is either paid a flat monthly rate by
customers for unlimited service, or charges additional fees after a
set usage is exceeded.  The real payoff is in the eyeballs and the
mouse-clicks -- selling specialty content and advertising space and
taking a share of e-commerce revenue.  Data networking represents
online service providers' highest cost, apparently around 50 percent
of revenue.  Significantly, however, marketing, customer support and
subscriber acquisition represent close to 35 percent of revenue.

Backbone ISPs

All networks are beholden to backbone ISPs -- be they content hosting
facilities, downstream ISPs, or online service providers -- either
to furnish Internet connectivity or to manage the actual network
infrastructure.  Nor are backbone ISPs an exclusive category.  While
most network providers are increasingly specializing in specific
segments of the market, there are only a very few network connectivity
providers that aren't downstream from others.  Internationally, the
same dynamic applies.  Local downstream ISPs in Asia, Europe and
elsewhere need the larger, upstream networks, often the incumbent
telecom provider, for Internet connectivity.  And big Internet sharks
outside the U.S. find themselves but tiny sardines when they arrive
on U.S. shores with their leased circuit dedicated to IP traffic.
They must strike an interconnection agreement with one or more of the
Internet backbone networks, just like a regional U.S. ISP.

Some off-shore backbone ISPs have begun to acquire their own national
U.S. networks to obtain free peering.  Most have not.  In 1999,
Japan's NTT tried to aggregate its traffic with the large U.S.-based
backbone ISP Verio, in which NTT had taken a ten percent stake,
and Qwest was keen to piggyback onto EUnet International's peering
agreements when the U.S. telecom upstart bought the pan-European ISP
in March 1998, forming what would become KPNQwest.  The emergence
of backbone ISPs to provide connectivity to the Internet -- indeed
to determine what actually constitutes Internet connectivity -- is a
relatively recent phenomenon.  Not surprisingly, there's controversy
surrounding their role in the Internet food chain.  When the Internet
first evolved, ISPs were closer in size and swapped traffic freely.
Early Net applications, like file transfer protocol, led to more or
less symmetrical traffic among ISPs. In contrast, the Web creates a
split between the end users, who import data, and content companies,
who are data exporters.

That's new.  In the early days, the ganglia of network interconnections
were so complex -- since everyone accepted any other network's traffic
-- that the only way Internet engineers could map the Internet's
topology and traffic flow was simply to draw a cloud.  Today, however,
the terrific infrastructural investment, and major traffic imbalances
due to the emergence of Web hosting firms, have meant that the
practice of settlement-free peering is waning.  The two noticeable
exceptions are that local ISPs peer with their siblings at local
exchange points, and that the very biggest backbone ISPs -- the
Tier Ones who can move traffic pretty much anywhere without buying
long-haul transit from someone else -- continue to peer among
themselves.  Peering, in other words, is for those who are your peers
-- or appear to be.

The point: scale matters.  Unless your network is very big and
very fast and upgraded continuously, you are always somebody else's
customer -- which is one reason why regulators, otherwise leery
of interfering with the Internet's dramatic growth, have pondered
stepping in to try and keep the backbone market competitive.  Whether
or not they do so depends on a still-brewing argument over whether
or not Internet backbones, currently treated as enhanced services,
should be reclassified as public telecommunications infrastructure.
If so, then companies operating Internet backbones would be common
carrier operators, and therefore required to provide fair and
non-discriminatory terms to ISPs seeking interconnection.  If not,
then as enhanced services providers they continue to be able to pick
and choose with whom they connect and on what terms.  Like many of
the hard questions about an increasingly pervasive Internet, the
regulatory status of backbone networks -- basic telecom facility or
enhanced ("private") data pipe -- remain unresolved.

---

Jessica Marantz
TeleGeography, Inc.
T: +1 202 467 0853
F: +1 202 467 0851
http://www.telegeography.com
```

|  |
| --- |
| **[ProcessTree Network](http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](mailto:webmaster@somewhere.com). |