---
id: rre-quality-of-service
title: "[RRE]\"quality of service\""
type: writing
writing_type: rre-post
date: 1998-09-09
url: "http://commons.somewhere.com:80/rre/1998/RRE.quality.of.service.html"
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - rre-post
  - auto-imported
  - rre
---



## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1998/RRE.quality.of.service.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/20000115152614/http://www.somewhere.com/)

  

# [RRE]"quality of service"

```
[Dan Tebbutt of Australian Personal Computer magazine heard about
Andrew Odlyzko's work through RRE and interviewed him on the subject
of "quality of service" -- the idea that Internet architecture should
evolve to provide a hierarchy of service qualities at different
prices.  This idea seems on the surface to make economic sense, and
also given the diverse demands of different applications (for example,
e-mail versus real-time video).  But they also seem on the surface
to perturb our sense of the social values that go with the Internet.
And besides, information economics generally and the Internet in
particular have a way of being counterintuitive.  So it's not a simple
issue.  I've enclosed both Dan's finished story and the raw interview,
both by permission of the magazine (http://www.apcmag.com).  I'm not
competent to endorse Andrew's arguments one way or the other, but even
though they're more technical than most of the stuff that goes out to
RRE, they're a relatively lucid introduction to the issues, which tend
to be debated in a narrower community than they ought to be.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html
or send a message to requests@lists.gseis.ucla.edu with Subject: info rre

---

Profile November 98: Quality and equality

 Dan Tebbutt

 Conventional wisdom says the Internet needs different levels of
 service to expand.  AT&T's Andrew Odlyzko argues everyone should be
 treated better.

     The Internet is the ultimate classless society.  Big Brother, BHP
     and the boy next door are all treated equally in the heart of the
     Net, despite each having radically different demands and paying
     vastly disproportionate amounts for connectivity.  Internet
     routers simply don't distinguish between an online tax return,
     a million-dollar extranet supply line deal and an IRC flame war.
     It's all just packets.

     But experts suggest that the Net will need to become more
     discriminating before it can move to the next level.  If the
     global IP network is ever to become as mission-critical in
     society and commerce as the phone system, gurus contend, we'll
     need to implement quality of service (QoS) levels.  Essentially
     this means you get what you pay for: government and business
     could cough up more to guarantee their transactions arrive on
     time every time, while recreational surfers would tolerate a
     little delay in order to save money.

     Infrastructure providers agree QoS is desirable -- not least
     since it will allow them to charge enterprise customers more
     for value-added services.  Telephone companies, Internet service
     providers, networking vendors and Internet standards bodies
     are working feverishly to develop QoS engineering.  The telcos
     piously preach Asynchronous Transfer Mode (ATM) as the perfect
     approach to differentiated service.  Unconvinced, the Internet
     community is devising alternatives like Resource Reservation
     Protocol (RSVP) and Multi-Protocol Label Switching (MPLS), a
     standard for proprietary vendor technologies that allow faster
     switching to replace routing (see story).

     Against these commercial and technological imperatives, Andrew
     Odlyzko is something of a heretic.  A researcher with dominant
     US long-distance carrier AT&T, Odlyzko believes there is an
     alternative to differential service levels: give everyone better
     service.

     "After studies over the last year looking at what's going on over
     the Internet, I am not so sure that you need QoS," he told APC.
     "It might be economically optimal to provide high-quality service
     for everything.  My guess right now is that it might actually
     be best to strive for that goal as opposed to putting much more
     complexity into the network for quality of service measures."

     His work is based on intensive examination of traffic behaviour
     on large data networks around the world.  Analysing usage
     patterns on research networks, corporate leased lines, university
     campuses, telco infrastructure and Internet backbones led Odlyzko
     to conclude that, rather than QoS engineering, more bandwidth is
     the best way to improve Net performance.

     Odlyzko argues QoS engineering proposals like RSVP, ATM and MPLS
     would significantly increase Internet complexity without ensuring
     higher performance for Net users.  "Quality of service for the
     network does not guarantee anything about the quality of service
     that's perceived by the customer," he said.  "That's a very
     serious defect in the quality of service measures that are being
     worked on.

     "Quality of service covers a wide umbrella of different
     approaches.  Many are too complicated -- not all of them, but
     certainly RSVP is one that doesn't scale and involves out-of-
     context settings and end-to-end bandwidth reservations through
     the network.  Others . . . would force the Internet into a
     straitjacket.  Some people propose assigning different priorities
     to different packets depending on the application, but that of
     course would conflict with IPsec encryption, so you'd have to
     have a separate signalling system that could partially decrypt
     headers.  Everything adds more complexity and I think that's
     undesirable."

     ATM no salvation

     Despite his telco affiliation, Odlyzko remains unconvinced about
     the merits of ATM.  "I do not see it as a solution today and I
     doubt whether it is going to be a solution in the future," he
     said.  Empirical data suggests ATM does not address the real
     characteristics of Internet traffic.

     "The problem is that ATM was designed with a vision that the
     network would be doing something very similar to the traditional
     voice network in which you have lengthy conversations or flows.
     You also have reasonably well-defined bandwidth and latency
     guarantees.  That is true for voice communications.  That is true
     to some extent for the multimedia communications that have been
     expected to dominate at some point.  [But] that is definitely not
     what we see on the network today," he said.

     "My conjecture is that this is not what we're going to see in
     the future.  That's a very heterodox view, contrary to accepted
     wisdom, but I have documented that that is not what we see on
     data networks, especially when you look at the lightly congested
     private line networks.  These consist of very bursty traffic and
     we can see why that might be so, because most Internet traffic
     today is HTTP."

     ATM advocates tend to underestimate the importance of Web
     traffic, Odlyzko feels.  "Web browsing encompasses a variety of
     important applications, many of them mission-critical, such as
     when your customers might be ordering from you or your doctor
     might be looking up information relevant to your sickness. 
     It's all transacted through the HTTP protocol, and that leads
     to bursty traffic.  Usually the traffic consists of relatively
     few packets so you do not have a well-defined flow.  Sources are
     dispersed all over the world, the transactions are very brief,
     and you don't have a well-defined bandwidth requirement because
     basically what the end user cares about is getting the stuff to
     the browser right now.

     "That's not the world for which ATM was designed," he added.
     "You might say HTTP and the World Wide Web is just one of many
     things, and eventually we are going to have packet voice and
     multimedia applications on the Internet.  That is true -- but
     my guess is that by the time those things do migrate, there will
     be so much other packet traffic that this will be a very small
     fraction of the total.

     "What is likely to dominate is machine-to-machine communication
     where again what would matter is satisfying end-user desires."
     These mechanised transactions will be triggered by human demands,
     said Odlyzko.  "One example is in the medical arena: it's not
     practical right now for radiologists to do telemedicine because
     the bandwidth requirements are too high.  They want to transmit
     many huge, multi-megabyte files within a few minutes.  Current
     networks will not support it.  Future networks will, so the world
     where I envisage telemedicine working is one in which the surgeon
     who finds something on the operating table can consult with a
     specialist and transmit images.  The specialist might want to
     search for similar images.

     "So there will be a whole set of transactions with software
     agents running to different databases -- but all in response
     to urgent human need.  That will then lead to very bursty
     transmissions, not the ATM world of long-lived, well-defined
     flows.  That's why I don't see ATM as a solution."

     Change of heart

     Odlyzko was not always opposed to quality of service.  Only a
     year ago he published 'A modest proposal for preventing Internet
     congestion' (see http://www.research.att.com/~amo/doc/networks.html),
     a paper that offered a new approach for enabling QoS.  The
     document set out a method to deliver differentiated service via
     economics rather than technology.  Odlyzko argued the Net could
     be partitioned into a number of logical networks, each with
     varying transmission fees.  There would be no formal QoS
     guarantees, and all traffic would be treated equally within its
     logical subnet.  The theory, inspired by Paris Metro Pricing
     (PMP), was that most customers would prefer the cheapest network,
     so heavy loading would slow its performance.  Meanwhile, a
     minority of customers needing faster service would pay more
     to use lightly loaded segments.  If too many people upgraded,
     performance would lag; this decline in service would encourage
     some people to downgrade to save money, thus alleviating
     congestion in a classic self-regulating market.

     In keeping with his current ideas, the proposal celebrated
     Odlyzko's conviction that "simplicity was of the utmost
     importance".  "I felt PMP was the easiest way to provide people
     who are willing to pay more with higher quality service.  In that
     kind of environment you would be getting higher quality service
     on average."

     Indeed, PMP-style class differences already exist to some extent.
     Expensive private leased lines give well-heeled customers low
     utilisation and more responsive networks for a price.  Semi-
     public ATM and frame relay networks deliver good performance
     for slightly less, while the vast majority of Net users remain
     attached to cheap, low-bandwidth options like dial-up modem links
     and ISDN.

     "When I looked at what happens in private line environments I
     see that power users in general do pay more," explained Odlyzko.
     "What people care about is latency -- not just latency for a
     single packet, but the latency for a whole transmission such as a
     Web page.  That is worth something.  Various people will pay more
     for low utilisation because they really care about being able to
     transmit quickly.  In that sense there is a certain very rough
     equity whereby the power users do pay more because they utilise
     their networks at lower rates."

     Lower utilisation levels

     Therein lies the crux of Odlyzko's thesis: better network
     performance derives from lower utilisation levels, rather
     than complicated QoS technology.  It's a larger version of the
     dilemma many corporate network managers face in congested local
     area networks -- namely whether to throw cheap bandwidth at
     the problem or deploy more sophisticated technology to manage
     bandwidth better.  In ATM's heyday, bandwidth management seemed
     the logical answer.  But fast, low-cost Ethernet hardware made
     bulk bandwidth an easier alternative, so now desktop LAN users
     generally have the luxury of bandwidth far above their average
     needs.

     Can this over-engineering approach translate to the Internet?
     Odlyzko believes it can if there is sufficient network traffic
     aggregation and a competitive market for bandwidth.  The more
     traffic transfers to the Net, the more efficient it will become,
     he feels.  "If you are going to move corporate traffic from
     private line networks to the Internet, that would free up
     all those private lines to be used for Internet traffic.  You
     have huge potential increases in efficiency of utilisation of
     transmission links because you can aggregate the traffic, you can
     take advantage of statistical multiplexing, and you can gain from
     larger economies."

     Yet some experts fear Internet overload if too many enterprises
     dump leased lines to save on astronomical carrier charges.
     That's where competition has a hand to play, according to
     Odlyzko.  "If someone dumps a private line, the carrier can take
     that line and use it for Internet traffic.  Remember the lines
     used for voice traffic, private lines and the Internet are
     basically the same lines from the telephone company provider's
     point of view," he said.

     "If a corporation does not buy the line, the telco will sell
     it to other buyers such as Internet service providers.  They
     certainly have no incentive just to hold it empty.  Of course,
     there is now the question of whether you have a monopoly or a
     competitive environment.  If you have competition, the telco
     doesn't have any choice: if they don't provide Internet service,
     somebody else will."

     In any event, Odlyzko's research suggests companies won't dump
     existing networks.  "From all the evidence I have been able
     to gather, it is unlikely that private line networks are going
     to decrease.  In general, what seems to happen is that new
     applications migrate to new networks such as frame relay or the
     Internet.  Private line networks stay in place; people are very
     reluctant to abandon reliable communications because so much
     infrastructure ties into them," he added.

     "The main question for the future of the Internet is whether
     customers are willing to pay for high quality by having low
     utilisation rates, or whether many links will be congested,
     with QoS providing high quality for some select fraction of data
     transfers," Odlyzko wrote in a recent research paper on network
     economics.  The paper concludes that optimal traffic management
     is "unattainable, and we should seek the simplest scheme that
     works and provides necessary transmission quality . . . Network
     managers will have a hard time making everything interoperate
     satisfactorily even without worrying about QoS."

Date: Mon, 16 Nov 1998 09:52:48 +1000
From: Dan_Tebbutt@acp.com.au
Subject: Andrew Odlyzko interview

Hi Phil

Since it was your message that encouraged me to contact Andrew for a
wonderful discussion about the evolution of the Internet, I'd like to
offer the text of the interview (or my writeup) to send to RRE, if you
think it's useful.  He was fascinating to talk to.

The edited profile is at http://www.apcmag.com/profiles/ .... the
first item in the list (called "Quality and equality").  Feel free
to grab text and post to RRE, acknowledging that it's reprinted with
permission from AUSTRALIAN PERSONAL COMPUTER magazine
(http://www.apcmag.com).

or you may find the raw interview interesting.... it's below.

kind regards

dan

Andrew Odlyzko

AT&T Research

Interview via phone Wednesday 9 September 1998 by Dan Tebbutt

APC: What is wrong with existing QoS proposals for the Internet, such
as ATM, RSVP, MPLS and proprietary proposals such as tag-switching, IP
Navigator and Fast IP?

AO: A variety of things.  Many of them are too complicated -- not all
of them, but certainly RSVP is one that doesn't scale and involves
out-of-context settings and end-to-end bandwidth reservations through
the network.  Many others suffer from complexity or would force the
Internet into a straight-jacket.  Some people propose assigning
different priorities to different packets depending on the
application, but that of course would conflict with IPsec encryption
so you'd have to have a separate signalling system that could
partially decrypt headers.

Everything adds more complexity and I think that's undesirable.

APC: Is quality of service a desirable characteristic in the Internet?

AO: Quality of service covers a wide umbrella of different approaches.
As of a year ago, I did believe you needed to provide quality of
service, or more precisely differentiated services.  That's where the
Paris Metro Pricing proposal came from.

Now, after the studies I carried over the last year looking at what's
going on over the Internet, I am not so sure that you need it.  I am
now inclining more and more towards the view that it might be
economically optimal to provide high-quality service for everything.

It doesn't mean that you will solve all problems: one of the basic
problems that you will always have is latency.  If you are going from
Australia to the US and back, you are going around the world so the
round-trip time over fibre is something of the order of 200ms.  If
you're doing telephony, 200ms is getting to the range where it begins
to be noticeable.  It's a basic law of physics: you have to deal with
it unless you are going to provide some latency-hiding techniques.
But you can certainly come very close to this 200ms latency with
existing technologies if you have a very lightly loaded network.

My guess right now is that it might actually be best to strive for
that goal as opposed to putting much more complexity into the network
for quality of service measures.

APC: Do you see ATM as a partial or complete solution to quality of
service issues?

AO: No, I don't see that at all.  I do not see it as a solution today
and I doubt whether it is going to be a solution in the future.  That
does not mean that I do not see a place for ATM.  I think there is a
place for ATM today in the core of the network.

The problem is that ATM was designed with a vision that the network
would be doing something very similar to the traditional voice network
in which you have lengthy conversations or flows.  You also have
reasonably well-defined bandwidth and latency guarantees.  That is
true for voice communications.  That is true to some extent for
multimedia communications that have been expected to dominate at some
point.  [But] that is definitely <I>not<I> what we see on the network
today.

My conjecture is that this is not what we're going to see in the
future.  That's a very heterodox view, contrary to accepted wisdom,
but I have documented that that is not what we see on data networks,
especially when you look at the lightly congested private line
networks.  These consist of very bursty traffic and we can see why
that might be so, because most Internet traffic today is HTTP.

Web browsing encompasses a variety of important applications, many of
them mission-critical, such as when your customers might be ordering
from you or your doctor might be looking up information relevant to
your sickness.  It's all transacted through the HTTP protocol and that
leads to bursty traffic.  Usually the traffic consists of relatively
few packets so you do not have a well-defined flow.  Sources are
dispersed all over the world, the transactions are very brief and you
don't have a well-defined bandwidth requirement because basically what
the end user cares about is getting the stuff to the browser right
now.

That's not the world for which ATM was designed.  This is what we say
today.  You might say HTTP and the World Wide Web is just one of many
things and eventually we are going to have packet voice and multimedia
applications on the Internet.  That is true -- but my guess is that by
the time those things do migrate, there will be so much other packet
traffic that this will be a very small fraction of the total.

What is likely to dominate is going to be machine-to-machine
communication where again what would matter is satisfying end-user
desires.  It's going to be machine-to-machine communication, but
triggered by human demands.  One example is in the medical arena: it's
not practical right now for radiologists to do telemedicine because
bandwidth requirements are too high.  They want to transmit many huge
multi-megabyte files within a few minutes.  Current networks will not
support it.  Future networks will, so the world where I envisage
telemedicine working is one where the surgeon who finds something on
the operating table can consult from with a specialist and transmit
images.  The specialist might want to search for similar images.  So
there will be a whole set of transactions with software agents running
to different databases -- but all in response to urgent human need.
That will then lead to very bursty transmissions, not the ATM world of
long-lived, well-defined flows.  That's why I don't see ATM as a
solution.

APC: So you'd suggest ATM is being used now as a "fat dumb pipe", as
you've called it?

AO: ATM right now is being used in the cores of networks where you
have flows that are better defined.  If you are an Internet service
provider and you aggregate traffic at some point and transmit between
those points, then usually the aggregated traffic does correspond to a
reasonably well-defined flow.  Under those conditions, ATM does make
some sense, and there are certainly some advantages to doing switching
as opposed to routing -- there's much less overhead so you can do it
much faster.

Some people propose dispensing with ATM and just running packets over
fibre, while other people would dispense with using SONET.  There
certainly is a big overhead with ATM.  ...  But I'm not enough of a
hardware expert to stake my reputation on predicting what technology
will dominate in the network core.

APC: Do you ATM as significant technology for delivering quality over
the last mile in the customer access network?

AO: Again I'm sceptical.  I don't really see ATM as a solution for
quality of service problems.  ATM is fine if you have the bandwidth --
but if you do have bandwidth, why do you need ATM? [The question] is
what happens when demand exceeds the capacity of your link: in that
case somebody has to lose.  I don't see that all the extra mechanisms
and overhead of ATM will provide a better service than IP-based
solutions.

APC: Do you think quality of service and differentiated service-based
pricing is too hard for the Internet?

AO: Not necessarily.  I think it's undesirable, but it can be done:
that's what I was proposing with Paris Metro Pricing.  A year ago when
I put out that paper I was absolutely convinced you had to have
differentiated services and user-specific pricing over the Internet.
Now I'm not so sure.  We may have to do it.  In that case it is
possible to do it, although it would be hard to implement.

APC: You've looked at private lines.  As companies look to move
private wide area networks to VPNs across the Internet, how do we take
more traffic onto the Net without creating further burdens? How should
VPN traffic be charged?

AO: That all depends.  Given that I strongly believed in user-based
pricing and quality of service a year ago, I understand the attraction
of those approaches.  Certainly you might say it's economically
rational to have differentiated services.  Today you have on one hand
a large set of corporate customers who care about quality of service
and pay a lot for their private line networks and on the other hand
you have many users who are very price-sensitive and seem to be
willing to put up with low quality of service.  Therefore you'd say
let's have differentiated services on the Internet and allow corporate
users to use VPNs with higher quality and higher cost than residential
dialup users.  That is certainly one solution.

Some people say the Internet could not possibly carry voice traffic
because there is so much more of it than data traffic, or they might
say private line traffic would overwhelm the Internet.  That is only
true if you take a static view of the Internet.  Remember the Internet
is growing.  If you are going to move corporate traffic from private
line networks to VPNs on the Internet, that would free up all those
private lines to be used for Internet traffic.  That's why you have
huge potential increases in efficiency of utilisations of transmission
links because you can aggregate the traffic, you can take advantage of
statistical multiplexing and you can gain from larger economies.  So
in some sense I do not see moving corporate traffic up to VPNs as a
threat to the Internet.  In fact, I see that as a great promise for
improving transmission for everybody and producing lower costs and
better service for everybody.

APC: But aren't companies going to dump those private lines and shove
more onto the Internet because it's cheaper?

AO: But how to they dump the private lines? Remember the lines used
for voice traffic, private lines and the Internet are basically the
same lines from the telephone company provider's point of view.  You
have the basic facilities networks such as AT&T, MCI, WorldCom and
Sprint own.  This is what all these services ride on.  At a higher
level these lines are assigned either for voice or for packet traffic.
If someone dumps a private line, the carrier can take that line and
use it for Internet traffic.

APC: But is there any economic incentive for the telco? Current leased
lines are incredibly expensive, and customers pay Internet connect
charges as well.  Won't customers dump their costly private lines and
just keep the Internet connection?

AO: If a corporation does not buy the line, the telco will sell it to
other buyers such as Internet service providers.  They certainly have
no incentive just to hold it empty.  Of course, there is now the
question of whether you have a monopoly or a competitive environment.
If you have a monopoly, a single telco which owns everything, they
could keep the Internet traffic on private lines.  But if you have
competition, the telco doesn't have any choice: if they don't provide
Internet service, somebody else will.

On the other hand, I do not see the Internet as much of a threat to
the incumbent telcos.  From all the evidence I have been able to
gather, it is unlikely that private line networks are going to
decrease.  What's going to happen is the growth rate will slow down.

For example, frame relay services -- which are growing at rates
comparable to the Internet in the US -- was often predicted to take
traffic away from private line services.  But that hasn't really
happened: private lines are still growing.  There are instances of
corporations which have migrated their internal networks to frame
relay, but in general what seems to happen is that it's the new
applications that are migrated to new networks such as frame relay or
the Internet.  Private line networks stay in place: people are very
reluctant to abandon reliable communications because so much
infrastructure ties into them.

APC: Essentially corporate customers will consume more instead of
abandoning leased lines.

AO: I think so.  I do see a big growth opportunity for virtual private
networks over the public Internet, but I do not expect a big retreat
from private lines or frame relay.

APC: On a philosophical level, is it fair that more demanding users
should pay more -- and what should they get in return?

AO: Again my view has changed.  Last year I thought you had to have
differentiated services.  Paris Metro Pricing was my proposal because
I felt simplicity was of the utmost importance and I felt PMP was the
easiest way to provide people who are willing to pay more with higher
quality service.  In that kind of environment you would be getting
higher quality service on average.

When I looked at what happens in private line environments I see that
power users in general do pay more.  ...  What people care about is
latency -- not just latency for a single packet, but the latency for a
whole transmission such as a Web page.  That is worth something.
Various people will pay more for low utilisation because they really
care about being able to transmit quickly.  So in that sense there is
a certain very rough equity whereby the power users do pay more
because they utilise their networks at lower rates.

APC: So does the PMP proposal exist currently, in that private leased
lines and semi-public ATM and frame relay lines already achieve the
objectives of what you've called a "rough equity"?

AO: No.  What you see with private networks and frame relay or ATM is
not PMP because there you have a single quality of service -- a single
high quality of service.  It's not PMP.

APC: But the combination of the Internet, semi-public lines and
private lines does deliver different services at different price
points.

AO: That is beginning to approach it.  You already are beginning to
see something emerge along those lines in the Internet arena with
different carriers offering different grades of service.  MCI has
separate networks for business and residential customers.  Corporate
customers very often can go to the big national carriers and get a
link directly to the big backbones which are more lightly used so have
higher quality of service -- but they pay a high price.  Or they can
get a much lower price from regional ISPs that have higher utilisation
and a few extra routers along the way increasing latency.

It's not quite PMP because you don't have an easy transmission where
you can choose almost on a packet by packet basis where your
transmissions go.  In a way, my prediction was and still is [that] if
you're going to have differentiated services and user-sensitive
pricing then you are going to end up with Paris Metro Pricing.  Your
comment is very perceptive: we are starting to see PMP pricing.

APC: You could even go to the extent of using different ISPs for
different tasks to hack it together on a packet by packet basis...

AO: That introduces inefficiency.  It's much cheaper to buy one big
pipe to a single ISP than two separate pipes to two separate ISPs.

APC: Do you expect private lines will start declining at some stage?

AO: At some stage perhaps, but not necessarily in absolutely quantity.
I expect they will decline quite rapidly as a fraction of the total
network, but the number and bandwidth of private lines may not
decline.  There will always be special demands where people will want
extra security.  As the data network universe grows, that will be a
smaller piece of the pie but it will be as large as it is today or
even larger.

Look at electric power generators: almost everybody today relies on
centrally generated electricity via the power grid.  You also have
stand-by generators at important facilities, and there is much more
generating capacity than there was 100 years ago.

APC: Essentially your view is that QoS should be delivered by
economics rather than technology: different pricing levels should
encourage network buyers to assign priorities and decide what level of
service to pay for, instead of imposing a technology solution such as
RSVP on the network.

AO: Yes.  But that's only if you have to have differentiated quality
levels.  One of the things which has come through in my studies, and I
am making this much more explicit in my current paper, is that when
you look even at corporate networks, there is a wide variation in
quality of service on domestic US links and international links.

I'm putting in there an example of a trans-Pacific line from the US to
Australia which is very heavily congested.  Basically what seems to be
happening [is that], without announcing it to everybody, corporate IT
planners are tolerating low quality of service on expensive links
across the Pacific or the Atlantic.  That tells me a lot about
willingness to pay.  I certainly see price of transmission as a
critical variable.

If prices do not decline rapidly enough, you will need to have
differentiated services and indeed the very simplest way to provide
this is some sort of PMP.  Why is it simplest? That comes back to your
original question about what's wrong with current QoS efforts.  One of
the things I see wrong is that the measures proposed do not
incorporate the technology for quality of service with pricing.

If you are going to have differentiated service levels, you are going
to have to have a pricing scheme.  What I am saying is let's use just
pricing.  Let's cut away from all the extra effort and extra overhead
in trying to provide a service guarantee.  Let's just go with expected
levels of service.

APC: When do you see QoS technology as attractive? Larry Roberts
suggests criticism of complexity is just a marketing approach, and
more complex might be much better.

AO: I think that's the wrong point of view.  I think the less complex
it is the better.  My argument against complexity is that networks
should not be treated in isolation.  One of the mistake people make is
talking about the Internet as if it were a phone network where the
service is well understood.  Networks permeate much more deeply into
organisations.

People are hardly ever interested in networks because of the network;
they want to run applications.  Those applications are typically hard
to get right as it is.  There are so many other things to get wrong
without worrying about the complexity of the network and negotiating
with the network.  I completely disagree with Larry Roberts.

APC: How do we conceal the Internet's complexity without limiting its
flexibility? Last year I theorised that network unreliability and
complexity meant we were not ready for devices like network computers.

AO: There are so many areas of unreliability to worry about.  Quality
of service for the network does not guarantee anything about the
quality of service that's perceived by the customer.  That's a very
serious defect in the quality of service measures that are being
worked on.

It will be very hard to conceal the Internet's complexity but we
should strive to do it.  There are other problems causing difficulty
with the network computer aside from network complexity and lack of
bandwidth.  I find the NC idea in many ways attractive, but you need
to have reliable networks.  That's an absolute requirement and we
certainly don't have it.

How do we conceal the Internet's complexity? Well, one way to do it is
to provide high quality of service for everybody.  In particular, that
means relatively low utilisation -- throwing bandwidth at the problem.
Other things are more technical measures: IPv6 would help a lot, as
would more security inside the network.

The pretext of the Internet is providing flexibility at the edges, but
that forces too much of the decision-making onto the edges where it's
wastefully duplicated by network managers at thousands of
institutions.  Some functionality such as security should be provided
inside the network.

APC: That's going to be difficult given not only US restrictions but
also the Wassenaar Arrangement worldwide.

AO: To some extent, but you could provide low levels of security such
as 40-bit encryption universally around the world.  That would provide
enough real security, but it would discourage many attacks.
Authentication of packets could be done, so ISPs would refuse to
forward packets where the return address is forged.

APC: You are somewhat more conservative than others with your
estimates about voice versus data traffic.  Has Net growth plateaued
since what you call the "anomaly period" in 1995/96?

AO: Yes, if by plateauing you mean a 100 percent growth rate -- which
is unbelievable in most other contexts.  A 100 percent growth rate is
what Internet seemed to experience all through the 1980s and early
1990s.  There was a period of two years with anomalous growth [when]
some academic networks that were already pretty well wired [joined
up].  Now we seem to be back to this 100 percent growth rate.  Very
few technologies grow at that rate.

You might call me conservative, but in any other context I'd be called
a raving lunatic!

APC: You argue that data networks won't be as efficient as voice
because they have different characteristics.  Should we have a new
metric for efficiency on data networks?

AO: That's a point I am making more explicit in this new paper: the
distinction between economic efficiency and engineering efficiency.
Namely the low efficiency of data networks is a result not of anything
inherent in the technology but as a result of conscious human choice.

Some of the data that I collected showed that it is possible to run
packet networks at very high utilisation levels.  ...  The problem is
that when you do that the users experience frustration: you have World
Wide Wait.  I certainly have experienced that when trying to telnet
from Europe.  People choose low utilisation to get what they want.

APC: How do you strike the balance between efficiency and customer
performance?

AO: I am not sure there is any single measure.  What really matters is
customer utility, which is a very complicated thing.  ...  In general
people care about their big applications and to measure what utility
they get from these applications is hard.  To measure how much of
application's utility level comes from different network performance
levels is even harder.  It's hard to come up with any quantitative
measures.

APC: Do you see that there is a limit to over-engineering? How much
can bandwidth compensate?

AO: What may very well happen in an environment of falling prices --
it's a different story if prices rise -- is a continuum of decreasing
utilisation levels.

If you look at local area networks, utilisation levels appear to have
decreased dramatically over the last decade as a result of the
interaction of customer preferences and rapidly falling prices for
bandwidth.  There was some rationality to it: it's not that everybody
was given Gigabit Ethernet for their PC.  Network administrators work
out who needs what: most people are satisfied with Ethernet, power
users will get Fast Ethernet, special cases will get Gigabit Ethernet.
Prices do constrain what you get, but there is a fall in utilisation
levels.  This will continue at the edges of the network.

In the core of the network it's not clear.  It could be that
aggregating traffic -- even very bursty traffic -- may produce
relatively steady but low utilisation levels.

APC: Do you expect circuit and packet networks to start mingling and
merging? Do you expect ultimately we will have one network, or are the
characteristics just too different?

AO: I expect that we will have basically one network -- with the
proviso that legacy networks are likely to survive for quite a while.
Earlier we talked about private lines and why they will remain for a
long time, and similarly some legacy voice networks might stay around
for some time.

Already at the facilities network level there is no distinction
between voice and data networks.  At AT&T we have OC-48 links: some of
the traffic on them is packet and some is switched voice.

The reason I am confident voice will move towards packet networks is
that in a reasonable period of time (say 10 years or so) packet
networks will be so large that it would not be sensible to run a
separate voice network.  If somebody really cares about high-quality
voice services it would be easier to set aside special channels on the
packet networks for voice traffic, rather than having a separate
system of switches and transmission lines

APC: Finally, do you think end-users should be optimistic about
solutions to Internet complexity?

AO: The Internet has a lot to learn about interfaces from the switched
voice network.  At the moment the Internet is simply too complicated.

For example, the penetration of the Internet in the US is roughly half
of the households that have PCs.  That says something: the glass is
either half full or half empty.  On the half empty side, half the
households find PCs too expensive or too complicated.  Now on the half
full side, households that do have PCs -- how many of them have
Internet access from home? It turns out about half.  These are people
who have shelled out typically $US1,000 to $US2,000, so $US20 per
month (the going rate for Internet access in the US) should not be an
insurmountable financial burden.  Yet half of them don't do it.  So it
seems the Internet is not simple enough or attractive enough for them.

You have to work on the complexity of the PC or give them different
access devices like WebTV or other Internet appliances.  The
attraction of going after that market is great enough that the
industry will move in that direction and provide satisfactory
interfaces.

One of the great achievements of the switched voice network was that
they had a very simple interface that could be used on 700 million
lines around the world.  That's a key lesson for the Internet to
learn.  At the moment the Internet is learning the wrong lessons from
the phone system by trying to go for guaranteed quality of service.
That's not what we should be going after.

APC: Is there reason to expect the congestion situation will get
better in terms of the user experience?

AO: Yes.  Prices of transmission will drop substantially and
congestion will be less of a problem.

ENDS
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/20000115152614/http://www.somewhere.com/)
