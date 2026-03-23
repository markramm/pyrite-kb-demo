---
id: red-rock-eater-digest-institutional-analysis-for-design
title: Red Rock Eater Digest - Institutional Analysis for Design
type: writing
writing_type: rre-post
date: 2001-12-27
url: http://commons.somewhere.com/rre/2001/RRE.Institutional.Analys.html
coauthors: []
importance: 6
research_status: partial
tags:
  - history
  - media
  - military
  - social-computing
---




## Source

Automatically imported from: http://commons.somewhere.com/rre/2001/RRE.Institutional.Analys.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](http://commons.somewhere.com/rre/) | **Most Recent Article: Mon, 11 Feb 2002** |

```
---

This message was forwarded through the Red Rock Eater News Service (RRE).
You are welcome to send the message along to others but please do not use
the "redirect" option.  For information about RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html

---

  Institutional Analysis for Design

  Phil Agre
  http://dlis.gseis.ucla.edu/pagre/

  This is a draft.  Please do not quote from it.

  Version of 27 December 2001.
  7300 words.

//1 Introduction

I want to talk about two different methods of analyzing a problem for
purposes of design: the device-centered method and the institutional
method.  The device-centered method talks about users -- and thus
may present itself as being "user-centered" -- but it talks about
users using concepts drawn from the attributes of the device, or
from the design space of possible devices.  The institutional method,
by contrast, talks about users in social terms.  The device-centered
method is by far the most common in the computer world today, but its
limitations increasingly argue in favor of the institutional method.

Having been trained as a computer person, I expect that my argument
will seem foreign to many designers.  So before launching in, I want
to explain briefly where this exotic concern with sociology is coming
from.  Back in the old days when computers were large objects locked
in air-conditioned rooms, designers had enough problems getting
the computers to work at all.  Later their job became fitting the
computers into an organization's existing work practices, and later
still they became concerned with the convenience of the isolated
user (see Andrew L. Friedman, Computer Systems Development: History,
Organization and Implementation, Wiley, 1989).  At each step, the
computer has moved further out of the closet and become more entwined
with the lives of the people who use it.  And those people live
their lives in the social world.  We can look at the social nature
of computing from at least three perspectives:

(1) Design is a social process, with a variety of players and
issues, and the design process is becoming more complicated as more
considerations are brought to bear on designers' choices.

(2) Computer use is a social process, and the process of computer
use is becoming more complicated as security problems proliferate
and users form themselves into advanced communities.

(3) Computers mediate social relationships, and Web-based tools are
capturing and supporting those relationships in more detailed ways.

In these ways and more, system designers are already sociologists;
it is just a question of becoming better sociologists by drawing
the social content of computers and their design and use into the
open.  Several research movements have arisen to serve this need,
such as social informatics, participatory design, computer supported
cooperative work, and economic and legal analysis.  To speak of
"institutional analysis" is partly to reconstruct these diverse
approaches on top of a common theoretical framework.  Institutional
analysis of computing has already been under way for a quarter-
century, so I am not claiming to have invented it.  Instead, I
am trying to draw in a broader range of concepts from the various
literatures on institutions in order to provide the field with a
broader range of intellectual resources.

Here, then, is the problem that I would like to use to illustrate
the difference between institutional and device-centered analysis.
To begin with, imagine a world of ubiquitous computing.  Individuals
carry around their own portable and wearable devices, all of which are
wirelessly networked to one another and to the general public network.
Places such as cafes, offices, cars, and night clubs are equipped with
their own devices, all of them also networked to one another and to
the public network.  Individuals' devices are capable of interacting
with any other device in the world, including devices that become
relevant through their physical proximity.  The general idea is that
the individuals' devices are extensions of themselves, and support the
full range of activities and involvements that the individual engages
in.  Using these devices, individuals will become both more embedded
in their local surroundings -- through the connections that the
devices establish (either spontaneously or by command) with devices
in the immediate environment -- and less embedded in those surroundings
-- through the connections that the same devices establish (likewise)
with an unbounded range of devices elsewhere in the network.

We want to design devices for this world, but we understand from the
start that these devices will not stand alone.  Rather, the devices
will all be built atop a common architecture.  This architecture
starts with basic networking protocols like the 802.11 family,
the Ethernet, and the Internet, all layered in a hopefully rational
way.  The guts of the architecture, though, lies in higher layers
-- the middleware that provides generic services like file service,
transaction processing, encryption, document management, digital
libraries, and cross-media communication channels.  It is easy
-- far too easy -- to design this middleware architecture in a way
that excludes a priori whole categories of potential applications.
As a result, the design process will be doomed from the start unless
it can characterize the design space.

//2 The device-centered approach

Unfortunately, the design space is extremely hard to characterize
because it is so large.  And this is where the distinction between
the institutional and device-centered approaches becomes important.
Let us first consider the matter from a device-centered perspective.
Starting from the attributes of the devices -- and from attributes
of the user that follow from them -- we can start naming issues and
drawing distinctions:

(1) If an individual is alone in a place, then the place can adapt
itself to the individual -- displaying certain information on its
devices, setting itself to engage in certain kinds of interaction,
loading a user's preferences for the behavior of various features,
cueing certain content, directing sensors to measure some aspects
of the environment and not others, adjusting lights and environmental
controls, and even configuring motorized furniture and architectural
elements such as partitions.  If several individuals occupy the same
place, however, whether stably or in a shifting population, then the
place somehow needs to configure itself to the needs of the whole
population, and it will matter whether everyone is present for the
same purpose or different purposes, whether they need to allocate
access to devices, whether the space needs to be subdivided in one
sense or another, and so on.

(2) The network knows who you are, or at least it has an identifier
that tracks you from one place to the next, even if it cannot connect
that identifier to other identifiers in other databases.  In fact,
it's not the network that tracks you but various entities that you
relate with through the network.  At any given moment, you maintain
relationships to all of those entities, and in principle many of
them are capable of influencing the behavior of devices on you and
around you, whether through their initiative or yours or someone or
something else's.  But interaction in this world need not be competely
personalized.  Complete personalization is only one corner of the
design space.  The ways in which different devices interact with
you might depend on many different kinds of information: attributes
that you have (e.g., groups that you are a member of), statistical
inferences (e.g., gathered through the history of interaction with
other individuals about whom the entities in question might have
partial information), individuals' policies and situated choices about
what actions to take and what information to reveal (e.g., making some
documents public as on the Web), and so on.

(3) Privacy will be a concern, including the privacy of the various
people in a space vis-a-vis one another.  At one extreme, all of their
personal devices will be open to one another, forming a single pooled
data space.  At another extreme, the goal will be to create completely
disjoint activity-spaces in both a physical and an electronic sense
for each individual.  In the middle ground, rules and commands will
be needed to govern the movement of information between the different
users' personal data spaces.  Privacy will also be a concern between
the individual and whoever is in charge of the space.  For example,
in a market environment the interactions between people and place
might be governed by the protocols of a type of transaction, so that
no information needs to be transferred except what's defined within
those rules.  In a work environment, rules will need to be established
for the kinds of access that an employer might have to the states of
the employees' devices, which presumably record fine details of their
work activities.

(4) The spaces in question might support a simulation, for example
in an entertainment or training context.  Computational objects will
need to be created somewhere on the network, according to ancient
custom, to represent the objects in the simulated world.  Then the
devices' interfaces will all be configured to simulate the setting
being simulated, and computational resources will be brought online
to generate the needed animation, compute and display consequences
of simulated actions, and so on.  Simulation spaces can be more or
less encompassing, from the decorations of a theme bar to the total
immersion of a military training exercise.

(5) Interfaces in this world might be organized according to various
metaphors, by analogy to the famous (if inconsistent and half-baked)
desktop metaphor in personal computing.  One metaphor might be the
"backpack" in which individuals carry around the virtual documents
and devices that they use in various environments.  We can easily
imagine someone sitting down in a cafe and spreading their paperwork
on the table, whether for their own use or to share with someone
else, such as a customer.  The objects in the backpack would interact
with whatever devices they find in the vicinity, converting formats
where necessary or providing the user with options about which nearby
devices should be recruited for which purposes.  The backpack metaphor
suggests an obvious set of operations: adding things to the backpack,
cleaning it up, securing it against theft, having it searched by the
security people, and so on, some of which will make sense for a given
application and some of which will not.  (On the foundations of the
backpack metaphor, see the "Placeless Documents" project at Xerox.
On documents generally see David M. Levy, Scrolling Forward: Making
Sense of Documents in the Digital Age, Arcade, 2001.)

(6) Labor must be divided between personal devices and devices
that are embedded in places.  Many issues arise: what devices people
are willing and able to carry (e.g., weight, hands-free, headsets,
batteries, etc), cost (e.g., people might pay to get temporary access
to an expensive device in a copy shop or cafe), sensor practicalities
(e.g., it's hard for a room microphone to tell who's talking), natural
divisions of computational effort (e.g., subprocesses that require
intensive real-time data exchange should ideally be close together
in latency space), security (e.g., you don't want to put the only
copy of a valuable document in a device that is easily stolen by a
pickpocket), privacy (e.g., you want computations involving personally
sensitive information to happen on devices that you own or at least
trust), and so on.

(7) The activities that the devices will support will have a physical
form that can be supported in various ways.  Users might be stationary
or moving around, seated or standing, spreading work materials around
them, driving or being driven, sharing a space with others (e.g.,
family home, airplane cabin, theater, cubicles), focusing individual
or group attention on a physical object (e.g., eating dinner, drawing
a diagram, repairing an engine), or representing themselves to others
(e.g., giving a performance, updating an article, controlling what
aspects of an ongoing activity others can be aware of).  The physical
and digital environment might support these activities in many ways,
including the kinds of dynamic adaptation that I mentioned above.

//3 The institutional approach

That, then, is the beginnings of a device-centered list of dimensions
of the design space.  Ideally one would use these issues to interview
people who know about various application domains, gather scenarios
from them, compare and contrast various scenarios to generate further
issues, and iterate until the list becomes unmanageable.  I am not
saying that this type of device-centered analysis is wrong.  It is
one level of analysis.  But I do think that it is a mistake to work
exclusively on the device-centered level, and I also think that it
is a mistake to develop the device-centered analysis too far before
analyzing the problems on other, more abstract levels.  Design should
start by analyzing situations in the ways that they are meaningful to
the people involved, and those meanings start with the institutional
context within which the situation is organized.

Institutions -- medicine, education, markets, law, politics, family,
religion, traffic, diplomacy, open-source software development, and so
on -- thoroughly define the social situations that take place within
them: they define social roles for the participants (representative
and constituent, buyer and seller, doctor and patient, parent and
child, driver and passenger), they define physical and abstract
objects in terms of the roles they play in the activity (bank account,
boundary marker, case record, court verdict, agreements and contracts,
rights and responsibilities), and they define terrains upon which
people strategize their activities (career paths, social networks,
market opportunities, public identities).  Institutions can organize
activities in very different ways, and without a theory of them it
is easy to overgeneralize from particular cases.  That is why design
requires institutional analysis: by considering the differences and
analogies among institutions, it is possible to map the extent of
the design space, as well as the anatomy and physiology of particular
institutionally organized situations within which the designed devices
might be used.

Although it has not been systematized into a textbook of design, a
great deal of experience has accumulated with institutional analysis
anyway, enough to suggest some guidelines.  Most of these guidelines
are heuristic, meaning that they suggest what you should look for
and what you are likely to find, and analytical, meaning that they
suggest what types of concepts are likely to be useful and what types
of conceptual confusion are likely to arise unless you are careful.
The analytical suggestions, in other words, are not meant as strong
empirical generalizations but as warnings to ensure that the analyst
is choosing concepts in a conscious way.  Here are some of the
guidelines:

(1) The activity you are designing new devices to support already
occurs on some scale with existing media.  If you try to design
a completely new activity from scratch then you will probably fail,
because it is not going to fit into a web of existing practices
that is more complicated than you are ever likely to know.  So take
the trouble to understand the current practices before you go around
reinventing them.

(2) The activity in question is a unified phenomenon that happens
to employ a wide range of media, including face-to-face interaction
and paper, as well as old and new digital media.  If you have defined
the activity in terms of a particular medium then you have probably
defined it wrong.

(3) The people who use your device are unlikely to invent a new
institutional order; more likely they will translate the practices of
an existing institutional order into the terms of the new technology.
Activities do obviously change to some degree when they are performed
through the mediation of a new technology (e.g., electronic mail vs.
face-to-face), but they must still fit with the same complex of social
roles, the same ontology and strategic terrain, the same incentives,
and so on.  Attempts to give people new media might succeed; attempts
to give people new goals probably won't.  If you want to change the
world, give new media to people with positive goals.

(4) Most types of human interaction are intrinsically difficult at
some level, and technology doesn't change that.  A new technology
might transform people's interactional troubles in some way, or
it might provide them with resources to renegotiate their troubles.
But if the people using the technology have problems, that is not
necessarily a problem with the technology.  Perhaps the technology
works best when it gets out of the way and lets people get on with
their problems.

(5) Relationships are analytically prior to technologies.  So, for
example, it is a mistake to speak in terms of "online communities".
There are communities, whatever that means, and communities almost
always transact their business in several media, some of which might
be "online".  Media have a limited ability to shape the activities
that go on within them; it is relationships, which are organized
by institutions, that do most of the shaping.  A good symbol of
this might be an acting exercise that Peter Brook describes in "The
Empty Space".  He has two actors turn to backs from one another and
refrain from making any noise, and then he instructs them to establish
communication with one another.  Because they cannot see or hear one
another, they flail around for a while until they start to pick up
and synthesize enough subliminal cues (shadows on the wall, vibrations
in the floor, who knows), whereupon they become able to communicate
and interact quite fluently.  This is the situation with electronic
media as well: no matter how structured or unstructured they might be,
or how rich or impoverished, in the end they are just channels that do
not understand the great majority of the multi-layered communication
that takes place through them.  This is also what Paul Dourish is
talking about in his book "Where the Action Is".

(6) Relationships are organized by institutions, and as remarked above
we need to distinguish among the diverse cases without overgeneralizing 
(or, for that matter, undergeneralizing).  So, for example, if we were
to confine our analysis to hobbyist groups then we would probably fail
to analyze the more competitive aspects of activity that are prominent
in work or market settings -- aspects that are found in the hobbyist
groups, too, if we know where to look.  As a general rule, analytical
categories that are useful in particular institutions also "pick out"
real phenomena in other institutions as well.  Contrarily, categories
that seem useful only in the analysis of particular institutions are
probably not framed in a general enough way.  Institutional analysis
is valuable largely because of the cross-pollination that takes place
between analyses in different institutional domains; phenomena that
are noticed in one institution can be systematically carried over to
suggest lines of observation and analysis in others.

(7) In analyzing or prescribing people's relations to one another, we
mustn't presuppose that everyone has total privacy or that nobody has
any privacy at all.  We need to be open to the diverse ways in which
personhood might be negotiated in each domain, for example in terms of
concepts of personal boundaries.  A given institution might be found
to provide individuals with ways of admitting particular others into
wider or narrower circles of their lives.  An institution might also
be found to conceptualize these relations of nearness and farness in
different ways, and the prevailing conceptualizations may or may not
describe the actual practices.  Whatever the case, new media tend to
disrupt these issues of interpersonal distance more drastically than
any other aspect of people's lives together, and so it is particularly
important to understand the existing practices and their stakes.

(8) For design purposes it is tempting to build conceptual castles
that supposedly describe the fixed structures of people's lives.  The
reality, however, is that people construct social reality cooperatively 
in real time by animating and inhabiting a repertoire of forms that
their shared culture makes reflexively available as resources.  The
word "reflexively" here means that everyone knows that everyone else
knows what actions and states of affairs are possible.  In a meeting,
for example, everybody knows that the rules of order provide for an
agenda and for motions to move along to the next topic.  That makes
it easy to offer such a motion, since the offerer need only distinguish
their action of offering a motion from other possible meeting-motions.
What is more, the very fact that a meeting is happening is itself
something that the participants sustain cooperatively from moment
to moment, for example by the way they visibly detach from the
meeting if they have to deal with a distraction, or else apologize
if their detachment proves not visible enough.  The range of means
by which people display these sorts of social "moves" to one another
is alarmingly unbounded, and it would be good for the designer to
understand some of them.  The designer should not assume that the
social world gets made automatically or through the kinds of simple,
discrete, overt signals that are normally reified as command sets
on computers.  The point is important because not every category
that we use in our institutional analysis will reappear as the name
of a datastructure in our technical design; such conflations between
analysis and specification is central to the device-centered approach,
and it is calamitous.

(9) People's interests, knowledge, backgrounds, goals, and situational
understandings overlap.  People are neither wholly coincident with one
another nor wholly separate from one another.  People are different,
but they are not totally different, and indeed the act of defining a
difference already presupposes a shared background of meanings against
which any sort of definition could take place.  Overlap is a crucial
resource for negotiating relationships -- conversations commonly take
the form of establishing commonalities and using these as a point of
departure for exploring differences -- and they are also fundamental
to the life of many institutions -- no individual can possibly know
or do everything, so knowledge and skill is subdivided into overlapping
regions that cover the whole territory while still allowing people to
inform and evaluate one another, provide competent third parties for
disputes, shake up assumptions, and so on.

(10) The institutions that organize activities do not wholly constrain
them.  One common metaphor likens institutions to the rules of a
game, which define the ontology of the game while leaving players free
to choose their strategies for playing it.  That metaphor makes the
dividing line between fixed rules and variable strategies seem clearer
than it usually is, and it also suggests an intrinsic fairness that
real institutions usually lack, but it is certainly an improvement
on theories that portray society as a prison that totally specifies
its powerless inmates' actions.  Analyses of particular institutional
settings should take seriously the very hard problem of what "freedom"
means, and who has it, and to what extents, and under what conditions.

//4 The personal sphere

Those are some guidelines for an institutional analysis of a design
problem.  They obviously don't substitute for an analysis of an actual
case, but at least they will fend off some mistakes.  Applying these
guidelines to the case at hand -- characterizing the design space
of networked personal and site-specific devices -- will not be easy,
simply because we are asking an extremely abstract question.  We are
characterizing a large design space that encompasses activities in
dozens of institutions, and not designing a particular system for a
particular setting, and so we will need to proceed on an appropriately
abstract level.

Let us begin with the person.  Whereas "individual" is meant as a
neutral term for a human being, the "person" is an individual as
defined by a society and its institutions.  The "self" is a person's
own subjective experience and understanding of himself or herself,
and a "persona" comprises the representations of himself or herself
that a person projects to a given segment of the world.  Let us say
that every person carries around a "sphere" of social involvements.
This includes (roughly speaking) the person's property, social
relationships, the media channels they monitor, and (as communication
scholars say) the "messages" that they are exposed to through
various routes.  The phrase "personal sphere" sets up a contrast with
"private sphere", which has historically meant the family home, and
"public sphere", which means the realm of public culture and debate.

In defining such a term, I am obviously headed toward design:
ubiquitous computing makes it much easier to carry your personal
sphere with you.  You can carry virtual documents and devices in the
sort of "knapsack" that I mentioned above, you can maintain mutual
awareness and communications with everyone you know, you can use
portable media devices to keep your personal media environment running
wherever you go, and you are obviously bombarded with messages most
of the whole time.  Your personal sphere, however, is analytically
distinct from the aspects of it that happen to be supported by
a particular technology.  No technology that we design will ever
mediate the entirety of most of a person's relationships, whether with
friends, family members, coworkers, or celebrities.  The "extended
individual" of person-plus-sphere already exists -- by means, for
example, of a magazine, Walkman, paper letter, or cell phone -- prior
to anything that we might design, and is more complex than we as
designers will ever know about.  We are merely amplifying something
that is already going on.

Defining the individual's own sphere is easy enough; what is harder
is analyzing what happens in the relationships and interactions among
people.  Those spheres are somehow brought together.  This is a topic
that is very hard to think about without institutional ideas.  Let us
draw on two concepts, one institutional and one not.  I've mentioned
both before.  Barry Wellman talks about the "networked individualism"
that new communication technologies bring about.  We have always
had social networks, but new technologies allow us to be in much
more continual touch with everyone in our networks.  We become
like air traffic controllers who keep track of all of the planes
in their airspace.  The point is not that we are literally aware of
the whereabouts and current activities of everybody that we know, only
that we have been pushed much further in that direction.

Even though networked individualism is a compelling idea, however,
I am always uncomfortable with theoretical constructs that declare
qualitatively new conditions to have arisen just because technology
has helped us do more of the things we already did before.  As a
result, I prefer to think of networked individualism as a permanent
condition, one that already held during the Stone Age and that has
become more intense in fits and starts throughout history.  On this
conception, networked individualism is independent of particular
technologies; the concept encourages us to go looking for the diverse
means by which people maintain an ongoing awareness of one another --
visits, parties, rumors, letters, phone calls, Web pages, and so on,
all of them embedded in the society's larger workings in various ways.

One weakness of the concept of networked individualism is that the
concept of a social network does not distinguish between different
kinds of relationships.  Your doctor is part of your social network,
but you probably have a different kind of relationship to your doctor
than you have to your parents, your UPS driver, or the people you went
to school with.  So let us complicate the concept of a social network
somewhat; let us label every link in the social network -- that is,
every relationship between individuals -- with the institution that
organizes it.  Some relationships are organized by the medical system,
others by the political system, and so on.  To really make the concept
work for design, we need to add in artificial individuals such as
corporations that present a more or less unified persona to each of
their customers, but we can omit that detail for purposes of suggesting
how the analysis might work.

The idea, now, is that every person maintains some degree of continual
awareness of everyone to whom they are related by various kinds of
institutional connection.  And indeed the term "person" is appropriate
because we now have the makings of a nontrivial of the architecture
of the person.  Every institution defines its relationships in great
detail, including coincident and conflicting interests, language and
things to talk about, genres and other conventions of interaction,
and much else.  This leads us to the second useful idea, Bill Dutton's
analysis of "access" across a wide range of relationships.  He uses
the term more broadly than I will, starting from the familiar notion
of access to information and extending it to "access" to a person.
Access always has conditions, is always negotiated, and is always
organized by laws, norms, and customs.  When we put the two ideas
together, networked individualism plus a general idea of access, we
get a complicated but conceptually appealing picture of the social
world.  Every relationship is organized by the rules that go with its
institution, and that includes the structures and practices by which
people get access to one another.  Personal spheres come together in
the ways that institutions organize, whether through mutual secrecy,
negotiated merger, or the emergence of relatively stable collective
spheres for dyads, groups, or publics.

//5 Citizenship in civil society

How do we bring this down to earth?  Past a certain point there is
no substitute for the analysis of particular cases.  All a conceptual
framework provides is some assurance that the right questions
will get asked.  So consider the institutions of public debate --
the "public sphere" in contrast to the personal spheres that enter
into it.  Scholars argue that a healthy polity requires a developed
civil society, and (in an article entitled "The Practical Republic:
Social Skills and the Progress of Citizenship") I have offered a
theory of what that means: practices whereby citizens can become
publicly associated with issues and form themselves into a matrix
of relationships among issue-advocates.  This matrix has several
dimensions.  Thus, for example, an advocate for liberalized policies
on immigrants in California will develop relationships with advocates
for similar policies in other states (geographic dimension), with
advocates for liberalized policies on immigration at the federal
and local levels (vertical dimension), with advocates for immigrants'
rights in other institutional spheres besides legislative politics,
such as the university and the courts (institutional dimension), and
with advocates for other forms of policy liberalization and other
forms of minority rights (ideological dimension).

Issues, furthermore, are living things, and for every position on
every issue it has to be someone's job to track their development
by noticing, absorbing, remembering, synthesizing, and interpreting
all of the facts that are relevant to that issue.  That means
keeping track of events in the news whose significance might be
disputed, identifying patterns among those events, arguing their
own position, hearing about the arguments being offered by proponents
of different positions, articulating responses to them, and so on.
This is information work, and an conscientious issue-advocate will
soon develop a network of various types of players.  Each of the
relationships in that network will be organized by an institution,
depending on the individuals' roles; for example, issue-advocates'
relationships to legislative staffers differ from their relationships
to reporters, experts, newspaper editors, or program officers
at foundations.  Issue-advocates have cooperative and competitive
relationships among themselves as well, for example in negotiating
common positions when bills come before the legislature.  They invest
in deepening those relationships because they expect to need them in
the future; trust is often required, and they understand that they
might fall on opposite sides as often as on the same side.

The practices of issue-advocacy, in short, are highly developed,
and they are basically analogous on all levels of governance from
the global to the local.  From a design standpoint, the question is
how those practices might be supported and their conditions further
democratized.  Of course, some people feel no strong sympathy with
people who engage in issue-advocacy as a profession, especially the
ones who advocate positions that they disagree with.  But it is widely
agreed that civil society is stronger when the means of issue-advocacy
are widely distributed, and that is a goal to which design can aspire.
The idea is not to invent new institutions of issue-advocacy, which is
much more a social project than a technical one, as to democratize the
institutions that exist.

Observe that the problem has two levels: tools and skills.  We can
provide tools to people who already have the skills; unfortunately,
the skills remain a secret.  In fact, the process of identifying
oneself with an issue and becoming inserting into the ongoing matrix
of relationships among issue-advocates is crucial: until they find
themselves part of such a functioning network with its personalized
trust relationships and flows of information, it is entirely
natural for citizens to experience themselves as powerless outsiders.
So there is a barrier to overcome: not just providing the tools
but providing an opening that makes the role of full-fledged citizen
imaginable.  This is one area where school is more important than
technology; pedagogies that try to teach democracy by convening groups
for deliberation actually do democracy a disservice, in my view,
because communal deliberation is an advanced skill, one whose purpose
and workings can only be understood by citizens who have inserted
themselves into the matrix of civil society.  Much better to start
with the skills of issue-advocacy, one of which is sitting down
with other issue-advocates to hold a very structured discussion about
potential common ground over an emerging issue.  Some of the other
skills of advocacy, such as writing opinion columns or speaking in
public, are also more about school than technology.  Technology makes
some of them easier to teach -- many students find it motivating to
send their columns to distant readers, and watching yourself on video
makes it much easier to learn public speaking.  But simple tools go
a long way in that kind of teaching, and the hardest design problems
pertain to curriculum and lesson plans rather than to the technology
as such.

Let us assume that things decompose so neatly, then, and that the
skills can be taught in a controlled environment in school without
specialized technology.  (This is one of the advantages of approaching
the design problem on the assumption that you are amplifying existing
practices rather than inventing new ones, which would require you
to diffuse the technology and the skills at the same time.)  Teaching
the skills of issue-advocacy is probably not enough to bring a robust
civil society into existence, and technology probably has a role to
play in enabling people to get into the game despite everything else
they have going on in their lives.  To explore how, we need merely
walk through the various relationships that the institutions of civil
society define.  To start with, civil society requires that people
become publicly identified with issues.  The obvious approach is to
let everyone build a Web site about their issue, and that is surely
part of it.  It is still too hard for ordinary people to build their
own Web sites, and there is reason to believe that ISP's -- wanting
to minimize traffic and simplify their lives -- are happy that way.
But even if we solve that problem, a Web page is only one part of
a larger system.  Putting something on the Web only makes it "public"
in a narrow sense.  What matters is whether the individual becomes
associated with their issue in the minds of relevant parties in the
process: the other issue-advocates, editors and other gatekeepers,
citizens with particular interests in the issue, and so on, and for
that purpose it is necessary to equip citizens with the capacity to
make noise.  Internet campaigns are good for this purpose; they may
not reach "the public", but they reach the citizens who are already
integrated into the matrix of civil society.  Much experience has
accumulated with this process, and institutional analysis for design
should be continuous with a larger culture of best-practices transfer.
(On the importance of best-practices transfer for civic life, see
Carmen Sirianni and Lewis Friedland, Civic Innovation in America:
Community Empowerment, Public Policy, and the Movement for Civic
Renewal, University of California Press, 2001.)  The Internet also
lowers the barriers for ordinary citizens to become issue-advocates by
providing online access to research sources and the buzz of backchannel
information-sharing and discussion that lies at the foundation of
networked individualism among advocates, and best-practices study in
this context would also facilitate both social learning and technical
design.

But because my focus here is on mobility and physical environments,
however, let us consider the aspects of day-to-day political work
that happen away from the desktop computer terminal.  The accelerating
time-frames of political work, particularly when relevant bills
are moving in a legislature, do often require real-time engagement
among issue-advocates who are working the same side, and it would be
very helpful if an issue-advocate could stay involved in the action
while riding on the commuter train or waiting in the doctor's office.
One dimension of the advocate's personal sphere is a sophisticated
media environment, and it is easy to imagine tools based on heuristic
content analysis and digital libraries that monitor, organize, and
present the media from the point of view of a given issue.  Several
specialized news services already exist to serve this purpose, and new
tools could clear the ground for more.

The issue-advocate is an excellent example of networked individualism,
and new tools for supporting a continual immersion in the matrix of
civil society would be helpful as well.  Cell phones are part of the
story, but it would be extremely useful to have general-purpose tools
for managing a portfolio of relationships, including functionalities
like a call log, surveillance of the public statements of the relevant
players, and ready access to the documents that are related to current
projects with a given individual.  If the fine structure of these
relationships can be analyzed in detail, then it should become easy
(for example) for an issue-advocate to receive an item of information
from a network contact and make it available on their own Web site
with a few simple commands.  The idea is to break the process of
managing the constellation of real-time details into simple units,
starting with the air traffic controller metaphor but moving it out
of the control tower and onto the street.

Clearly, then, the issue-advocate -- whether professional or ordinary
citizen -- needs a complex informational window on the world.  This
window can be provided by a conventional portable computer, but other
forms are easy to imagine.  In a world of cheap display screens, for
example, it should be easy enough for public and private spaces of
many kinds to be equipped with large screens as a matter of course,
so that anybody who happens to be in the vicinity can grab one of them
wirelessly to give their personal sphere more room.  This would be the
electronic version of spreading out one's papers to work, except that
the papers can now include embedded video feeds and the like.  The
transition among various physical forms of the personal sphere, for
example spreading out from handheld device to different combinations
of public display screens and back, is an interesting interface design
problem, and the needs of an issue-advocate with a highly organized
personal sphere should make an excellent case study for it.

Even though it prepares its ground years in advance, issue-advocacy
is ultimately focused on the legislature, and few institutions require
electronic modernizing more urgently.  For legislatures throughout the
industrial world, the central question is whether legislators should
be able to vote from their home districts or whether they should still
be required to appear in person on the floor.  It is easy to see both
sides of the argument: legislators have a responsibility to immerse
themselves in the lives and views of the constituents, and they also
have a responsibility to deliberate together in the depth that only
face-to-face interaction currently affords.  It is interesting to
contrast the case of the legislators to that of the finance people in
New York.  They too serve as mediators between particular situations
in the field -- their investments -- and their negotiations with one
another.  Each side exerts its force, extensive travel is unavoidable,
and the real question is where they will make their home -- or as
traveling professional have long said, their "base".  In the case
of finance, argues Saskia Sassen, the answer is increasingly that
their make their base in New York or London.  The reason is clear
enough: their investments are too interchangeable and too spread out
geographically for any other base to make much sense.  Legislators,
however, are stuck with constituents in a particular geographic area,
and the unhappy result is that the forces from home and the capital
are equally strong.  Forcing them to appear on the floor to cast their
votes forces them to be in town, and recent reforms in the US Congress
that limit most votes to mid-week are the best simple compromise.

The bigger picture, though, is that the legislature on every level
of government is the focal point of an institutional circuitry that
reaches through layers of issue-advocates, journalists, and others
down to the level of ordinary citizens.  That circuitry works badly,
and the technological needs of issue-advocates provide a point of
departure for imagining how it might be remade.  The infrastructure
of politics has been revolutionized in the last quarter-century
through the membership-mobilization methods of the best-capitalized
interest groups, and what's needed is a common platform that allows
those sorts of infrastructures (by which we really mean organizational
arrangements as well as infrastructures in any narrow sense) to be
built more easily by anyone, much as the Internet provides a common
platform for the low-overhead construction of distributed applications
of diverse sorts.  The point is not simply that legislators should
be connected directed to their constituency as a whole, useful as that
might be for newsletters and constituent services.  The point, rather,
is that the matrix of issue-advocates who mediate between legislators
and citizens should have a clear line of sight to the action on the
floor and strong support for their real-time activities of analysis
and negotiation.  The more widely accessible that infrastructure is
to ordinary citizens, the better.

//6 Conclusion

This analysis of the informational life of the issue-advocate, however
brief, provides some hint of the complexity of institutional analysis
for design in a world of ubiquitous computing.  The starting-point
is the institution: the way that civil society, for example, organizes
a person's embedding in the larger social world, the informational
architecture of that embedding, and then the physical forms that
the architecture of that particular form of personhood might take in
an untethered technological environment.  Serious design, of course,
could only begin once several such institutional case-studies were
worked through in detail, and not just in the sketchy armchair manner
of this essay but in an empirical and participatory manner, iterating
with focus groups and mockups to bring some more reality to bear on
our all-too-self-confident technological imagination.  At that point,
once institutional analysis has taken hold, computer science as it
is already constituted is reasonably comfortable with the process
of abstraction and systematization that converts a series of domain
analyses to proposals about middleware that could support them all.
At that point it becomes appropriate to engage in the kinds of device-
centered analysis that I sketched and postponed above.

Ultimately, the role of institutional analysis in design should become
relatively comfortable.  System design is accustomed to reckoning
with the structures of social life, and it is accustomed to providing
tools that unconstrain the choices and strategies of a user community.
The relation between institutional analysis and technical design
cannot become entirely comfortable, however.  Social structure and
the formal structures of computing are different sorts of thing.  And
technical work is itself embedded in institutions and itself subject
to the same sorts of forces and limits as the institutions that good
designers should commit themselves to studying.  Design collides with
reality ever more complicatedly in the new world of socially embedded
computing, but at least we can hope to approach those complications
more consciously than before, and more responsibly.

end
```