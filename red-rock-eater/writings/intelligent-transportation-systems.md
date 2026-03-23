---
id: intelligent-transportation-systems
title: Intelligent Transportation Systems
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1994/Intelligent.Transportati.html
coauthors: []
key_concepts: []
importance: 6
research_status: partial
tags:
  - activism
  - community-networking
  - cryptography
  - digital-rights
  - education
  - government-info
  - history
  - internet-culture
  - internet-policy
  - labor
  - libraries
  - political-organizing
  - privacy
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1994/Intelligent.Transportati.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991008013646/http://www.somewhere.com/)

  

# Intelligent Transportation Systems

```
[Background: Intelligent Transportation Systems (ITS) is the new name (in 
the United States) for a whole batch of technologies currently being developed
for automating highways with lots of computers and networks.  The idea is to
distribute traffic information, collect tolls, regulate commercial vehicles,
increase safety and efficiency, and eventually permit fully automated traffic.
ITS raises serious privacy issues because it might involve capturing and
storing computerized records of everyplace you drive.  This is a short paper
for a law journal arguing that the crucial privacy-related decisions will be
made fairly  soon in the creation of a system architecture and the setting of
technical standards for these systems.  Now is the time for privacy activists
to do something about it.  More information about this soon.  In the meantime,
you might send a fax to ITS America (an industry group) at (202) 484-3483
asking for detailed information about the ITS America Fifth Annual Meeting
next March in Washington.]

  Reasoning About the Future:
  The Technology and Institutions of Intelligent Transportation Systems

  Philip E. Agre
  Department of Communication
  University of California, San Diego
  La Jolla, California  92093-0503
  pagre@ucsd.edu
  (619) 534-6328, fax (619) 534-7315

  Submitted to the Santa Clara Computer and High Technology Law Journal.

  Copyright 1994 by the author.

  This is a draft.  Please do not circulate it or quote from it.

  Italics are marked with asterisks.  Titles are marked with underscores.
  Footnotes are indicated as follows: [Footnote: text text text.]

//1 Introduction

A debate about Intelligent Transportation Systems (ITS) is not simply a debate
about technology. [Footnote: These systems were referred to until recently as
Intelligent Vehicle-Highway Systems (IVHS).]  It is, rather, a debate about
the future interactions between technologies and institutions that our choices
today will set into motion.  Arguments about such things are difficult to make
with any reliability.  It is easy to lapse into an unsophisticated optimism
for which the unpredictability of future events encourages us to err on the
side of progress, or an unsophisticated pessimism for which the possibilities
for authoritarian misuse of information technology encourage us to regulate 
it out of existence.  To make prudent choices about ITS, we need concepts 
to help us think about interactions between institutions and technologies.
This is obviously a broad topic; this article will pay particular attention 
to the institutions of computer system design and technical standard-setting.
[Footnote: For a more extended discussion of these and related issues, 
see Philip E. Agre and Christine A. Harbs, Social Choice About Privacy:
Intelligent Vehicle-Highway Systems in the United States, Information
Technology and People 7(3), 1994, in press.]

The United States Department of Transportation and a non-profit industry 
group called ITS America are currently engaged in an elaborate process aimed
at the creation of an "architecture" for American ITS systems.  [Footnote: US
Department of Transportation and IVHS America, IVHS Architecture Development
Program Interim Status Report, April 1994.]  This is a delicate process,
driven by several considerations:

 (1) ITS systems are complex.  The phrase ITS actually covers a diverse 
group of technologies and services.  Although it would be desirable for these
technologies and services to be designed to common standards, various segments
of the industry acquire their own momentum independently of the others.

 (2) Most US roadways are controlled by state agencies, usually with the 
aid of Federal funding.  ITS system design is thus an occasion for a complex
negotiation of government and private roles in operating a significant portion
of the country's infrastructure.

 (3) Although as a marketing matter ITS systems need only be standardized 
on a continent-by-continent basis, US manufacturers may find themselves
competing with standards and systems currently being developed in Europe 
and Japan.  If American ITS systems were to develop piecemeal through market
selection among a welter of partially defined architectures, the time required
for a single "winning" architecture to emerge might create a opening for
better-coordinated foreign alternatives. [Footnote: Lawrence A. Berardinis,
Smart highways get the green light, Machine Design, 64(16), 1992, pages
66-70.]

 (4) The major industrial firms in the ITS America alliance may have a 
common interest in developing a coherent American architecture, but their
interests diverge in other ways.  Each firm has its own distinctive strengths
and styles, and the emerging architecture definition will set the terms of
competition among these firms within the American market.

Although plainly oversimplified, these points may indicate the complexity 
of the institutional context in which decisions about privacy in ITS systems
will be made.  The stakes for these institutions are high, given uncertainty
about market acceptance of the systems that will emerge from this process.
Past experience with ITS provides some precedent for concern.  A proposed
road-pricing scheme in Hong Kong based on on Automatic Vehicle Identification
(AVI) encountered considerable resistance from advisory boards and
professional associations based on privacy concerns and the interpretation 
of road use fees as unwelcome taxation.  [Footnote: Sandford F. Borins,
Electronic road pricing: An idea whose time may never come, Transportation
Research A 22A(1), 1988, pages 37-44.]  At the same time, even if ITS systems
do not become legally mandatory, they may be introduced in such a way that
they become a practical necessity for large parts of the population.  Such 
a circumstance might arise, for example, through the demands of insurance
coverage or because of the lengthening lines at now understaffed manual
toll-paying stations.  It is thus difficult to predict accurately, or even
conceptualize clearly, the locus of "consent" for participation in ITS.

Due to constraints of space, in this paper I shall reduce the considerable
complexities of privacy in ITS to a single technological issue, namely 
whether the computers in the system capture information about individual cars
or drivers in individualized form -- that is, in a form that is indexed by 
a unique identifier for either the car or driver, or by some other code that
can be readily employed to cross-index multiple databases, thus constructing 
a dossier about a given individual.  It is worth emphasizing that this is 
not simply a matter of data security.  Significant potential dangers from ITS
systems do not derive only from unauthorized access to personal information.
They also derive from institutional pressures to employ this information 
for secondary purposes such as marketing.  Government agencies are today
engaged in a great deal of marketing on behalf of the businesses in their
jurisdictions [Footnote: Philip Kotler, Donald H. Haider and Irving Rein,
Marketing Places: Attracting Investment, Industry, and Tourism to Cities,
States, and Nations, New York: Free Press, 1993.], and ITS information 
could facilitate a great expansion of such activities.  The proliferation 
of computer-mediated tracking systems for numerous categories of people
(immigrants, "deadbeat dads", and so forth) is also a matter of concern, 
and imperatives of law enforcement will surely wear down any institutional
protections for individualized ITS data.  Perhaps these secondary uses of ITS
data are actually part of the systems' intended functionality, in which case
that fact should be openly confirmed and debated.  But I shall assume, to the
contrary, that ITS is intended solely to facilitate safety and efficiency in
highway traffic.

//2 Computer system design

Let us first consider the institutions of computer system design.  On a
technical level, it seems easy enough to pose the question of whether ITS
should capture individualized information.  Yet within the traditions of
system design, this question can only be posed in a limited and prejudicial
way.  In other work [Footnote: Philip E. Agre, Surveillance and capture: 
Two models of privacy, The Information Society 10(2), 1994, pages 101-127.], 
I have characterized these traditions in terms of the "capture model".  
When a system is meant to support human activities, traditional design 
methods begin by fashioning an ontology -- a formal system of categories 
and relationships to describe the people and things that populate that
particular domain of activity.  The next step is to embody this ontology 
in a representational scheme, on the assumption that technical means will 
be provided to "capture" the relevant aspects of the unfolding activity.

The logic underlying this procedure is simple enough: a computer can only
compute with what it can represent, and it can only represent what it can
capture.  The real-time capture of individualized information -- that is,
information indexed by a unique identifier for each individual -- is thus a
wholly natural application of standard design practices.  The space of design
alternatives is defined in terms of restrictions upon the ontology.  For
example, one might eliminate identifiers for people but retain them for cars,
or eliminate identifiers for cars but retain them for individual "smart cards"
that might potentially be purchased anonymously.  Each limitation placed upon
the ontology reduces the potential functionality of the system.  Designers
will typically experience the resulting constraints as artificial, and they
will not normally burden themselves with those constraints voluntarily.

It is not an exaggeration to say, then, that privacy invasion is an inherent
tendency of the conventional practices of computer system design.  Alternative
technical methods do exist, particularly schemes like "digital cash" that
employ cryptographic methods to authenticate transactions without necessarily
identifying the parties to one another.  [Footnote: Eamonn Sullivan, Firm 
has technology you can bank on: With "digital cash", transactions made over
public networks remain secure and private, PC Week 11(34), 1994, pages 83-85.]
If ITS is to avoid capturing large amounts of individualized data, though, 
the necessary social decision-making process will be swimming upstream against
the conventional practices and the tremendous inertia that they have developed
within the institutions of computing.

//3 Technical standards

Design practices are not the only source of inertia in technical choices 
about privacy.  The typical complex technological system combines elements
from a number of vendors, each of which must also function as part of 
numerous other systems as well.  (Some exceptions to this rule are found 
among military systems, which are often designed with more custom and fewer
off-the-shelf parts than commercial systems.)  This means that standards 
must be defined for the interfaces among these components.  The prototype 
of such standards might be pipe threads: pipes and elbows made by different
manufacturers can be fastened together if they conform to a common standard.
Standards can arise through a number of mechanisms.  One source of standards
is the state: telecommunications standards, for example, have historically
been negotiated by governments concerned with the interoperability of national
systems.  Standards can also arise through negotiations among alliances 
of commercial firms, conducted either through professional associations 
or (especially in recent times) privately.  [Footnote: William J. Drake,
Europe in the new global standardization environment, in Charles Steinfield,
Laurence Caby, and Johannes Bauer, eds, Telecommunications in Europe: Changing
Policies, Services and Technologies, Newbury Park, CA: Sage, 1992.]  ITS
standard-setting in the United States combines elements of all three of these
mechanisms, particularly if the DOT/ITS America architecture development
project is included.

But standards frequently persist through mechanisms far distant from the
institutions that defined them.  Regardless of the origins of pipe-thread
standards, for example, a manufacturer seeking to market a new line of pipes
will be well-advised to conform to the existing standard for pipe threads.
Unless the new pipes are aimed at an entirely new market, they will often need
to interconnect with existing pipes.  Manufacturers of computer keyboards,
likewise, have a powerful interest in conforming to the basic QWERTY 
layout.  Even though demonstrably superior layouts exist, at no point is 
it simultaneously in the interest of enough people to convert to any other
standard.  [Footnote: Paul A. David, Clio and the economics of QWERTY,
American Economic Review 72(2), 1985, pages 332-337.]

The entrenchment of technical standards in the marketplace has profound
consequences for ITS systems.  Some of these have already been alluded 
to at the outset.  Once a large number of systems has been deployed that
operate according to certain standards, that very fact will most likely 
create a powerful economic interest in the perpetuation of those standards,
even among companies whose products have not even been designed.  Among 
the most fundamental of standards for the interoperability of ITS products 
will be the scheme employed to define users' interactions with the systems.
If this scheme requires the routine capture of individualized data, then that
convention will most likely become entrenched in the market.  Conversely, if 
a scheme based on anonymous transactions becomes established then that scheme
will most likely become entrenched instead.

Which of these scenarios emerges will depend on some combination of government
policy, private alliance-building, market demand, and pure chance.  It is
entirely possible, for example, that a set of ITS standards with no privacy
protection beyond simple data security will emerge haphazardly through
incremental extension of existing systems originally meant for state agencies
charged with regulating commercial truck traffic.  On the other hand, it is
equally possible that a different set of standards might grow haphazardly
around any of a number of AVI schemes based on radio-frequency "transponders"
which broadcast their own internal identifier, not that of a person or car.
Or else the architecture development activities being conducted by DOT and ITS
America may function as intended by delivering a set of standards organized
around consciously chosen principles.

//4 Culture and participation

Though brief and incomplete, this analysis of technical institutions permits
us to frame more carefully the crucial question: what are the conditions of
informed social choice about privacy issues in ITS?

Some of these conditions are cultural.  Social responses to the privacy 
issues raised by new technologies will presumably be conditioned by historical
experiences and the symbolic encodings of historical memory.  The single most
important cultural understanding of privacy issues, at least in the United
States, is derived from historical experiences (mostly in Europe) of the
secret police.  These experiences are most frequently voiced through visual
metaphors (as in the term "surveillance"), and most especially through the
allegorical vocabulary of Orwell's 1984 ("Big Brother is Watching You").
While these cultural forms encode genuine historical experiences of state
oppression, they nonetheless fail to articulate adequately a variety of 
other threats to privacy.  They are only obliquely relevant to most projected
implementations of ITS, for example, in which participation is nominally
supposed to be voluntary.

"Big Brother" metaphors for technological privacy issues are accurate in one
unfortunate way: in both Big Brother's world and our own, most people have
little understanding of the technical and institutional machinery through
which routine surveillance is implemented in daily life.  [Footnote: Privacy
Rights Clearinghouse, First Annual Report of the Privacy Rights Clearinghouse,
Center for Public Interest Law, University of San Diego, 1993, pages 11-13 ff;
H. Jeff Smith, Managing Privacy: Information Technology and Corporate America,
Chapel Hill: University of North Carolina Press, 1994, pages 146-150 ff.]  
It is a matter of "they know everything about us", without any very definite
reference for the "they" or the "everything".  This abstract understanding 
is unfortunate because it encourages a passive fatalism about the control of
technology, as well as a diffuse and corrosive distrust of the institutions of
society.

One possible condition of informed social choice about ITS, then, is the
"visibility" of the machinery of data-collection.  This includes a variety 
of disclosure requirements, but it might also include requirements that
organizations employing personal data collaborate in the publication of "maps"
of the circulation of this dat among various uses.  Such visibility might help
rectify a broad category of routine market failures by permitting individuals
to make fully informed choices about the contracts they enter into -- most
particularly those adherence contracts which incorporate implicit or otherwise
obscure terms concerning secondary uses of personal information.  It might
also provide the grounding in personal experience that permits people to 
make informed choices about political matters, including the choice to commit
oneself to activism on particular issues.

Despite this cautiously optimistic conclusion, though, the obstacles to
genuine public participation in the most consequential decisions about ITS 
are considerable.  I have suggested above that these crucial decisions are
located primarily in the establishment of technical standards for the capture
and exchange of transactional information.  These are, unfortunately, among
the earliest and most conceptually obscure decisions to be made about ITS.
Moreover, they are likely to be made as part of a much larger and heavily
interconnected network of decisions, now being negotiated among a large number
of institutional parties.  Once technical standards have become entrenched 
in the market, it is unlikely that they will be changed through legislative,
administrative, or judicial action, or through consumer boycotts and the 
like.  The collective impact of individuals' refusals of privacy-invasive ITS
functionalities may have some effect, but such a scenario presupposes that
sufficiently many individuals understand the issues and that other legal and
economic pressures permit them the option of refusal as a practical matter.
In any event, the economic forces for standardization make it unlikely 
that individuals, or even sizeable organized groups, would have an adequate
bargaining position to force architectural modifications to large-scale
systems that are already in place.

//5 Conclusion

The outlook sketched here is largely pessimistic.  Lacking effective public
participation in the ITS design process, it is likely that the controversy
will move into the realm of symbolic manipulation.  Data security will no
doubt be emphasized in place of privacy, the practicality of anonymous use 
of ITS will no doubt be exaggerated, and vague and dystopian "Big Brother"
scenarios will continue to fill the newspapers.  Nonetheless, a clear role 
is emerging for a new form of public activism, in which citizens versed in
technical matters serve as mediators between technical decision-making and 
the broader public.  Volunteer activists associated with a public-interest
organization called Computer Professionals for Social Responsibility, for
example, have been active in shaping the privacy-related aspects of the
state-mandated AVI standards in California.  [Footnote: Personal communication
from Chris Hibbert and Lee Tien of CPSR.]  The Internet now brings detailed
information on such issues a rapidly expanding audience, and similar forms of
electronic communications may facilitate more informal and participatory forms
of interchange among government, industry, activists, and the broader public
than is possible through direct mail and talk radio.
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991008013646/http://www.somewhere.com/)