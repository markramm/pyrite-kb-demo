---
id: technology-and-privacy-in-intelligent-transportation-systems
title: Technology and Privacy in Intelligent Transportation Systems
type: writing
writing_type: rre-post
date: 1994-04-02
url: http://commons.somewhere.com:80/rre/1995/Technology.and.Privacy.i.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - commerce
  - community-networking
  - cryptography
  - education
  - forwarded-content
  - government-info
  - international
  - internet-policy
  - labor
  - law
  - privacy
  - surveillance
  - technology-policy
  - telecommunications
---



## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1995/Technology.and.Privacy.i.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009124951/http://www.somewhere.com/)

  

# Technology and Privacy in Intelligent Transportation Systems

```
  Technology and Privacy in Intelligent Transportation Systems

  Phil Agre
  Department of Communication
  University of California, San Diego
  La Jolla, CA 92093-0503

  pagre@ucsd.edu

  Conference on Computers, Freedom, and Privacy
  San Francisco, March 1995

Intelligent Transportation Systems (ITS) are being developed in most of the
industrialized countries.  Promoters of such systems envision information
technology being applied to transportation systems in a variety of ways,
primarily on public highways.  Applications extend from wireless provision of
traffic information to drivers to automatic toll-collection to law enforcement
to totally automated vehicles.  In the United States, the development of 
ITS is being managed by a complex network of government and private entities.  
At the center of this network is a close collaboration between the Department
of Transportation (DOT) and an industry association known as ITS America.  
The DOT and ITS America themselves have little power to dictate directions 
for the market in ITS equipment and services, but they play an important role
in coordinating negotiations over the system architectures that will ensure
compatibility of different vendors' offerings while attending to a variety of
non-technical concerns such as liability and regulatory compliance.

Among these non-technical concerns is privacy.  ITS may entail the collection
of large amounts of information on the travels of particular people, for
example through the automatic collection of tolls through road-side radio
beacons that interact with transponders attached to individual cars.  This
information obviously invites a wide range of secondary uses, from law
enforcement to targeted marketing to political repression.  The rules
governing the collection, dissemination, and protection of this information
have not yet been settled, although the decision-making process is already
fairly far along.

If ITS lives up to the expectations of its developers then it will have
implications for virtually everybody.  Yet public awareness of ITS is very 
low, and awareness of the privacy issues in ITS is low even in the community
of privacy advocates.  In these notes I would simply like to sketch some of
the basic issues.

Individually identifiable information.  It is widely supposed that ITS will
necessarily involve the collection of records that contain identifiers for
particular people (or their cars), and that the central privacy issue concerns
the disposition of these records.  But these premises are questionable.
Technologies such as digital cash should make it possible to use virtually all
ITS functionalities anonymously without taking additional laborious steps such
as visiting storefronts to pay for things in cash.  ITS is a good application
for digital cash because it is unlikely that ITS will lend itself to the kinds
of money-laundering that most concern the law enforcement community.

Security.  The security of ITS information against external attack or insider
leakage is clearly an important element of ITS privacy.  Since ITS may require
transmitting personal information wirelessly, interception or spoofing of 
this information is a clear danger; cryptography may therefore be one element
of the necessary security technologies.  But it is important to keep in mind 
that security is only one small part of privacy; cryptographic protection of
individual drivers' identities would alleviate some of the need for security
by decreasing the sensitivity of the data being transmitted while also greatly
increasing the degree of privacy protection inherent in the system.

Standards.  Much emphasis in privacy regulation focuses upon the regulation 
of data once it has already been collected, either because the collection of
this data is assumed to be inevitable or because no attention has been paid 
to privacy until data collection has been institutionalized.  One way that
data collection can become nearly irreversible is through the establishment
and entrenchment of technical standards.  Now that insecure protocols for
cellular telephone communications have become entrenched in the market, 
for example, it may be difficult to establish secure standards because 
many parties have made investments in equipment conforming to the insecure
standards.  Likewise, technical standards and basic architectural decisions
for Intelligent Transportation Systems that do not inherently protect privacy
will be nearly impossible to change later on.  Again, the crucial issue is the
collection of individually identifiable information.

Secondary use.  The privacy principles currently being distributed in draft
form by ITS America envision broad secondary use of ITS information about
individuals for marketing purposes, specifying only that marketers must notify
drivers of these secondary uses and provide them with an opportunity to opt
out.  (These principles, which are currently open for public comment, can 
be found on WWW at http://weber.ucsd.edu/~pagre/its-privacy.html ) The idea 
is that marketers might pitch offers to consumers based in part on where they
drive, or even upon where their cars are now located.  Yet opt-out systems
have worked poorly in other areas, and plausible technologies have been
proposed to provide these advanced targeting capabilities without providing
marketers with individual identifiers.  For example, drivers wishing to obtain
targeted advertising pitches could instruct their cars to activate digital
"agents" that contain a profile of their attributes and preferences, along
their current locations or anticipated locations ("who has a cheap family
restaurant coming up on this road?"); computers belonging to marketing
organizations would be able to respond to these queries with advertising
pitches that could be delivered back to drivers' onboard systems, with
cryptography being used to conceal their identities throughout the process.

Law enforcement.  Although unclear on the point, these principles also
envision few restrictions on law enforcement use of ITS information,
specifying that states must authorize any law enforcement uses of the data 
and that drivers should not be "ambushed" on account of information revealed
through ITS.  The practical meanings of these restrictions are not clear.
Society may decide that it wishes to provide law enforcement with generalized
abilities to track citizens' movements, but this would clearly be a grave
decision -- one that should be discussed well in advance rather than 
building the technical capabilities into ITS systems with virtually no public
discussion.

Commercial applications.  The ITS applications that are most advanced, 
and that have incorporated the fewest privacy protections, are those for
commercial vehicles.  Many long-haul commercial trucking companies, for
example, now routinely monitor their trucks using wireless technologies and
Global Positioning Satellites (GPS).  These systems make delivery schedules
more predictable and relieve drivers of some arbitrary work rules, while 
at the same time greatly increasing the level of surveillance to which
the drivers are subjected.  One danger is that the infrastructure already
developed for these commercial applications will be for consumer applications
as well.  Of more concern to most citizens, though, are experiments being
undertaken by some rental car companies to place GPS tracking systems in 
their cars.  Although these systems are primarily pitched in terms of their
driver-information and -security functions, they clearly also allow these
companies to track their property and potentially to regulate where it is
taken, information which may have secondary uses not necessarily foreseen by
renters.

Choice.  Proponents of ITS in the United States argue that use of the systems
will be voluntary.  Other countries, though, for example Singapore, have
proposed making ITS use mandatory, particularly to implement "road pricing"
systems that require pervasive toll collection.  But even when ITS systems 
are not mandatory de jure, they can still be mandatory in practice when
alternatives are impractical, for example when numerous roads are converted 
to toll roads or when cash payment is cumbersome.  Although no specific
proposals have been made to my knowledge, automobile insurance companies 
have an interest in requiring their policy-holders to employ ITS tracking
technologies in order to verify driving patterns.  As the available
information became more detailed, insurance companies would be able to adjust
their rates to increasingly specific aspects of a car's use, such as which
neighborhoods it is frequently parked in.  While some drivers may welcome 
the savings they can obtain by sticking to the right side of the tracks, the
price of refusal to comply with automatic surveillance is likely to be high.

Participation.  Public hearings on the DOT/ITS America architecture
development program have been held around the country.  Yet these hearings
were virtually unknown outside the ITS industry and the relevant government
agencies.  Although important decisions about ITS architecture are now 
being made, few fundamental, irreversible commitments have been made public
comment can still improve these decisions.  Interested parties may obtain 
a summary of the DOT/ITS America national architecture plan from Mr. George
Beronio; Federal Highway Administration; HTV-10 Room 3400; US Department 
of Transportation; 400 7th St SW; Washington DC 20590.  ITS America may 
be reached at 400 Virginia Avenue SW, Suite 800; Washington DC 20024-2730.

Strategies.  What is the best strategy for privacy advocates and others who
are concerned at the directions that ITS technologies might take?  If the
analysis above is correct, legislation and other forms of external regulation
will probably be a relatively low priority.  Instead, attention should focus
upon monitoring the standards-setting process for the benefit of a broad
audience, particularly the technically informed community on the Internet, and
pressing for broad application of inherent privacy protection through digital
cash and related cryptographic technologies.  Most of the parties involved in
ITS development stand to lose more through potential public resistance to ITS
technologies than they stand to gain through secondary uses of individually
identifiable ITS information.  As a result, these parties may be receptive 
to proposals that ITS embrace the privacy-protection technologies of the next
century rather than the outdated privacy-invading technologies of this one.

References.

Philip E. Agre and Christine A. Harbs, Social choice about technology:
Intelligent vehicle-highway systems in the United States, Information
Technology and People 7(4), 1994, pages 63-90.

Sheri Alpert, Privacy on intelligent highway: Finding the right of way, Santa
Clara Computer and High Technology Law Journal 11(1), in press.

Lawrence A. Berardinis, Smart highways get the green light, Machine Design,
64(16), 1992, pages 66-70.

Sandford F. Borins, Electronic road pricing: An idea whose time may never
come, Transportation Research A 22A(1), 1988, pages 37-44.

David Chaum, Achieving electronic privacy, Scientific American 267(2), 1992,
pages 96-101.

Sheldon W. Halpern, The traffic in souls: Privacy interests and the
intelligent vehicle-highway systems, Santa Clara Computer and High Technology
Law Journal 11(1), in press.

Mark Hepworth and Ken Ducatel, Transport in the Information Age: Wheels and
Wires, London: Belhaven Press, 1992.

Ronald K. Jurgen, Smart cars and highways go global, IEEE Spectrum 28(5),
1991, pages 26-36.

Peter Marks, For a few lucky motorists, guidance by satellite, New York
Times, 2 April 1994, pages 1, 16.

Don Phillips, Big Brother in the back seat?: The advent of the "intelligent
highway" spurs a debate over privacy, Washington Post, 23 February 1995,
page D10.

Richard Simon, Camera gains more exposure as a device for traffic control,
Los Angeles Times, 20 February 1995, pages B1 and B3.

US Department of Transportation, Nontechnical Constraints and Barriers to
Implementation of Intelligent Vehicle-Highway Systems: A Report to Congress,
June 1994.

Matthew L. Wald, Two technologies join to assist lost drivers, New York Times,
30 March 1994, page A13.

Charles P. Wallace, Singapore in high-tech tangle to fight automobile
gridlock, Los Angeles Times, 3 February 1995, page A5.
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009124951/http://www.somewhere.com/)