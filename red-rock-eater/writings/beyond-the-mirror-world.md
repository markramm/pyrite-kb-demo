---
id: beyond-the-mirror-world
title: "Beyond the Mirror World"
type: writing
writing_type: paper
url: "https://pages.gseis.ucla.edu/faculty/agre/mirror.html"
coauthors: []
key_concepts: []
importance: 5
research_status: stub
tags:
  - paper
  - auto-imported
---

## Source

Automatically imported from: https://pages.gseis.ucla.edu/faculty/agre/mirror.html

## Content

### Beyond the Mirror World: Privacy and the Representational Practices of Computing

#### Philip E. Agre Department of Information Studies University of California, Los Angeles Los Angeles, California 90095-1520 USA pagre@ucla.edu [http://polaris.gseis.ucla.edu/pagre/](https://web.archive.org/web/20190723151840/http://polaris.gseis.ucla.edu/pagre/) This is a chapter in Philip E. Agre and Marc Rotenberg, eds, [*Technology and Privacy: The New Landscape*](landscape.html), MIT Press, 1997. Please do note quote from this version, which changed slightly before publication. This version also omits several figures that can be found in the print version. 9000 words.

In January 1996, the California Air Resources Board (ARB) issued a Request
for Proposals (RFP 95-7) entitled Incorporation of Radio Transponders into
Vehicular On-Board Diagnostic Systems. The ARB observed that, starting
in 1996, new cars and light trucks in California will be equipped with an
on-board diagnostic (OBD) system that illuminates a dashboard indicator
when it detects a malfunction in the vehicle's emissions system. It
also observed that drivers may not actually get their malfunctioning
cars fixed until their next scheduled inspection check. With an eye
to enforcing compliance with emissions laws, therefore, the ARB proposed
to build a fleet of ten test cars, each equipped with a transponder that
is capable of transmitting the OBD error codes to roadside (or possibly
satellite-based) receivers. Specifically, in response to a query from
the receiver, the RFP specifies that the transmitter is able to supply the
following information:
> the full 17-digit vehicle identification number (VIN) of the vehicle   
> any fault codes reported by the OBD system   
> the location of the vehicle at the time of query   
> a status code

The receiver should be able to store the date and time of all queries to
passing cars, along with the information that the cars return, including
"vehicle location (to the zip code level, and city)". Although this RFP
only envisions the construction of test vehicles, the successful bidder is
asked to analyze the system's cost effectiveness "assuming that 1,000,000
vehicles equipped with the [transponder-equipped diagnostic system] are
added to the fleet beginning in the year 2000".

The ARB system is presumably intended to be used only for its stated
purpose, ensuring compliance with emissions regulations. The fact is,
though, that the system as specified could easily be used to track the
location of every car that is equipped with it, regardless of whether
it has any fault codes to report. The potential for abuse ought to
figure significantly in any weighing of risks and benefits from the
system, especially given that the newer cars on which the system would
first be installed are the least likely to experience emissions system
malfunctions. What is so striking about the RFP, though, is not that it
is unusual. To the contrary, the RFP takes for granted a whole vocabulary
of technical methods that has become familiar and widespread. The winning
bidder, for example, is instructed to "investigate the possibility of
coordinating this effort with other agencies or entities", so as to
"suggest the most effective and efficient infrastructure for statewide
electronic fleet monitoring". These other agencies include the California
Department of Transportation, which has been working on transponder-based
toll collection projects for several years, using a transponder
architecture that is expressly designed to be extensible to other
applications.

The ARB is not unaware of the privacy concerns that their plans may
raise. These concerns are described at length in a report on legal issues
(Di Genova and Macomber 1994) by the previous contractor on the emissions
monitoring project. They have also been reported in the press (Rogers
1996; Halpert 1995). Although the project may conceivably be derailed
by protests from affected industries, on a technical level the system
retains a sense of inevitability; it seems clearly the logical culmination
of a path of technical development. Although wireless capture of onboard
fault codes has been rendered practical only recently through decreasing
costs of microprocessor power and digital wireless communications, little
about the RFP is technically new or difficult; any competent computer
systems designer can imagine how it might be embodied in a working system.
Such a system, moreover, would be similar in its workings to hundreds of
other computer-based technologies for tracking human activities that have
arisen in recent years, or that are currently being developed. Together
these technologies constitute, in effect, an emerging infrastructure --
decentralized to be sure but pervasive nonetheless -- for the systematic
surveillance of numerous spheres of human life.

Ever since the rise of organizational computing in the 1950s, social
imagination has always associated computing with surveillance. The
reasons for this association are clear enough: computer systems analysis
and design promptly took up and generalized the methods of rational
administration that organizations had developed throughout the modern
era (Clement 1988). The technical concept of "algorithm" was assimilated
to the bureaucratic concept of "procedure", and the technical concept
of "data" was assimilated to the bureaucratic concept of "files". So long
as computers have been understood in this manner, as inherently suited
to social relationships of rationalized control, debate about privacy has
been structured as a series of tradeoffs, and by the assertion of abstract
rights (such as dignity, autonomy, association, or self-determination)
against specific encroachments (each accompanied by a compelling
justification). Lyon (1994), for example, accurately notes that the
same technologies that have raised concerns about a "surveillance society"
have historically made possible many benefits that most citizens would
prefer not to surrender. Society, prodded in part by the resistance and
agitation of concerned groups, may respond to such dilemmas by shaping
data-protection regulation, but the resulting regulatory process must
always contend with the putative benefits of particular surveillance
technologies.

The technical methods of computing have always defined the landscape
across which these controversies are conducted (Pool 1983, p. 251). Until
very recently, though, these technical methods have not themselves become
matters of dispute. Computers as cultural objects have, in effect, been
essentialized -- treated as a stable category with fixed relationships to
larger social practices. This ahistorical understanding of computers has
eroded somewhat in recent years as citizens have experienced the endless
turmoil of the personal computer industry first-hand. The emergence
of computer networking technologies such as the Internet, moreover, has
popularized an alternative, liberatory construction of computers that
focuses on their communications function (Feenberg 1995). Significant
changes in computer architecture do appear occasionally, such as
the emergence of RISC architectures in the early 1980s (Radin 1983).
Nonetheless, certain fundamental aspects of computer architecture have
remained stable. The vast majority of computer processors are still
serial, and virtually all of them employ the register-transfer model that
first arose in the 1940s. Calculations are still overwhelmingly digital,
and computer memory still consists of a hierarchy of media, each indexed
by a linear sequence of addresses. On the whole, computing has progressed
by augmenting and accelerating basic architectural choices, not by
replacing them. Although technical research projects have proceeded in
many directions, the innovations that have become widespread in actual
practice generally been built on top of existing methods, or they provide
generalizations or rational reconstructions of existing practice.

The architecture of a computer does not completely determine its use in
institutional contexts. Even so, computer systems design and practices
of rationalization have evolved together in a slow, continuous motion for
fifty years. The purpose of this chapter is to explore this evolution.
Although some valuable histories of system design practice as a whole
have been produced (Edwards 1996; Friedman 1989), my particular goal is to
gather some fragments toward a history of data. Computers raise privacy
issues when organizations use them to represent human beings and their
lives, and by analyzing the history of these representational practices I
hope to make the architecture and social practices around computing seem
less immutable. This history, as subsequent sections will make clear, is
not a matter of linear progress. The concept of data changes over time,
impelled both by the metaphors of technical language and by technical
practitioners' experiences in trying to get their systems to work.
Toward the end of the story, two things happen at once: a mainstream,
data-centered model of computing emerges alongside a model based on
public-key cryptography. I will argue that the various models of data,
despite their seeming differences, are coherently related to one another
and to the institutions of computing.

Although I will sketch these models of data, my main purpose is not
technical exposition. Instead, I wish to explore the "practical logic"
of computing work (Agre, forthcoming). What happens when a technical
community with a definite worldview, perhaps influenced by certain
metaphors, puts that worldview into practice? Any given metaphor will
necessarily consign certain aspects of reality to the practitioners'
peripheral vision. A metaphor may even misrepresent the very methods
that supposedly embody it. To the extent that practitioners apply their
methods in concrete situations, though, the marginalized features of
reality will reassert themselves -- most likely in the form of recurring
patterns of difficulty whose nature may not be clear at first. The
progress of technical work is, in this sense, largely reactive: the
technical community applies certain metaphors in organizing its work,
a certain pattern of difficulty emerges, and the existing methods are
modified or extended according to some understanding of the difficulties.
Only rarely will an entirely new metaphor arise, and then the old and new
metaphors are likely to coexist, whether as competitors or complements.
New methods arise when a new metaphor makes sense of large parts of
practitioners' experiences, but they are only adopted once they can be
fitted into the sprawling network of other methods by which the technical
community as a whole designs and builds complex systems. In this way,
computer work develops through the influence of its language, the mutual
constraints of its methods, and the recalcitrance of the world that lies
beyond both. Reconstructed historically, this development makes a certain
kind of sense, and this sense is the practical logic of the work.

### Representing Activity

The first methods for representing human activities on computers were
derived from the work-rationalization methods that industrial engineers
had been developing since the 1910s. Thus the phrase "information
processing": the idea was that computers automate a kind of factory work
whose raw material happens to be information rather than anything physical
or tangible.

Industrial engineers, starting with Taylor (1923) and Gilbreth (1921),
developed two broad categories of representations: process charts for
representing the flow of materials through a manufacturing process, and
time and motion study diagrams of particular jobs. Much has been written
about the sociology of early work rationalization (Braverman 1974; Guillen
1994; Montgomery 1987; Nelson 1980; Thompson 1989), but I am specifically
concerned with work rationalization as a representational practice. How,
and in what sense, do computers come to embody representations of human
activities?

Figure 1 presents an example of a process chart that follows the
progress of various parts, and the various operations performed on them,
in the assembly of a tin for storing tea. Note, first of all, that
the representational scheme consists of a small vocabulary of discrete
elements. These elements can be used both to represent an existing
form of activity and to prescribe a new one. In each case, the scheme
presupposes that activities can be broken down into discrete units. These
units need not be sequential (i.e., they might overlap), but they identify
discrete categories of action into which particular empirical streams of
action must be parsed.

Figure 2 presents Gilbreth's units for motion study, the "therbligs";
this particular diagram of the therbligs is from Shaw 1952. Once again,
the idea is that work activities can be decomposed into a fixed set of
categories (search, find, select, etc.). Figure 3 provides an example
of the therblig notation scheme in action; in this case, each action
is decomposed according to the respective roles of the worker's arms,
fingers, and palms, both left and right. The therblig system includes
units for representing rest and delay, and it includes a unit to represent
moments when the worker must stop to construct a plan. This latter unit
is distinctive. In Derrida's (1976 [1967]) terms, the "plan" therblig
is the supplement of the system: an extra term that closes up a gap in
the system while simultaneously embracing it as a whole. The whole idea
of motion study, after all, is to minimize or eliminate this extra term
by displacing the planning effort into the work of engineers. By making
this supplementary term an explicit part of his representational scheme,
Gilbreth acknowledges, if only directly, that reality always surpasses any
particular representation of it. Subsequent schemes in the same tradition
generally did not make room for explicit planning, but they did build upon
a vast body of practical experience in getting such schemes to work.

Couger's (1973) survey of the emergence of systems analysis methods
in computing makes explicit the connection between Gilbreth's use of
process charts and later computing practice. The initial concern was
the flow of forms in an organization. The rationalized organizational
use of paperwork was highly developed before the invention of the computer
(Yates 1989), and computing practice drew on an established tradition of
automating paper-based work. Figure 4, for example, a tabulating machine
process chart from the 1940s, represents the flow of Hollerith cards
through various machines. Each card corresponded to a particular record,
in this case records specifying orders and production levels for various
models of a company's products. As this diagram makes clear, techniques
used to map the flow of parts in manufacturing were carried over to the
flow of documents in the course of "manufacturing" other documents. The
focus was on the documents as physical artifacts, to be processed like any
others, and not on the meaning of the various representational elements
in the documents. The representational nature of the documents, in other
words, was secondary. The systems analyst's job was to represent the
forms, not the things that the forms represented. The transition from
paper forms to Hollerith cards to database entries was gradual and uneven,
and the concept of information served to abstract the common functionality
of these media without drawing any particular attention to the
representational nature of media themselves, or to the facts about the
world that these media conveyed. This accounts for a curious feature of
the information processing metaphor: information is treated as a tangible,
measurable substance, but only in a minimal sense does the information
seem to be about anything (Agre 1995a). Couger (1973, p. 196) concludes
his survey by pronouncing it "amazing" that systems analysts had made
little use of computers to construct the representations that they
employed in their work, even though their work consisted in the design
of computerized representations. But in retrospect the discrepancy makes
sense: the early systems analysts did not recognize much commonality
between the representations (process charts) that they manipulated
in their work and the representations (office documents) that were
manipulated by the people they studied.

### The Mirror World

The information processing metaphor proved misleading in important ways.
Having been motivated by the automation of existing work methods based
on paper forms, it was not particularly helpful to database designers,
whose task was to devise record-structures for new categories of digital
information. The original databases were inevitably modeled on the
tabular information that had long been stored on paper forms, with rows
that corresponded to particular things in the world and columns that
corresponded to particular attributes of those things.

This view of data was formalized by Chen (1976) in the entity-relationship
model of data. Although many databases had been designed in the two
decades before Chen's highly influential paper, the entity-relationship
model brought database design into focus as a body of practitioner
experience. Perhaps its greatest conceptual innovation was a clear
distinction between data records and the entities that they represent.
Though seemingly abstract, the point was not philosophical but
organizational; by starting the design process with an enumeration of
entities, the database designer is supposed to ensure that the resulting
design reflects actual business needs. Database designers, after all,
were generally trained as general-purpose system analysts rather than
in the particular industry whose substance the data was to represent,
and their attention was naturally focused more on databases as such
than on the categories that were implicated in particular applications
domains. Nor was the point at all obvious; even a contemporary manual
of data modeling (Reingruber and Gregory 1994), in trying to define the
concept of an entity, repeatedly blurs the distinction between records and
things. Having surveyed various definitions of "entity" in the literature,
Reingruber and Gregory (p. 64) extract the following themes:
> An entity is a `thing' or `concept' or `object'. . . . Or it may
> represent the fact that we need to capture information specific to only
> a subset of the instances of an entity. . . .
>
> An entity is not a single "thing", but rather a representation of
> like or similar things that share characteristics or properties. For
> example, King Lear and Hamlet are both plays, and have properties such
> as name, author, cast of characters, and lines of verse. The entity
> describing these might be PLAY, with King Lear and Hamlet as examples
> or instances or occurrences of PLAY. . . .
>
> Entities involve information. The "things" that entities represent are
> things about which the enterprise wants or needs to retain. . . .

These sentences shift repeatedly between treating entities as things in
the world and treating entities as representations of things in the world.
Their choice of example facilitates the confusion, given that the word "play"
refers to both the text and the performance, the representation and the
thing represented. Reflecting on the above points, they "refine our view
of entities" as follows:
> Entities are collections of attributes that satisfy a particular set of
> rules established for relational modeling. (ibid., p. 64)

This definition is perfectly ambiguous. Real things can, with some effort,
be viewed figuratively as collections of attributes, but entity-relationship
data records are precisely collections of data elements called attributes.
These authors may have been misled by the practice, common but usually
well defined in the literature, of using the word "entity" to refer both
to categories of things (cars, people, companies) and to instances of
those categories (my old 240Z, Jacques Martin, IBM). Be this as it may, the
conflation of representation and reality is a common and significant feature
of the whole computer science literature. (In artificial intelligence,
for example, formally specified activities such a chess and logical
theorem-proving serve the purpose that plays serve for Reingruber and
Gregory.)

The entity-relationship approach employed a graphical notation, a recent
and relatively streamlined version of which is found in figure 5. Each box
in this diagram stands for an entity and each link stands for a relationship,
with symbols on the links that indicate whether the relationship is one-to-one
(for example, cars and engines) or one-to-many (for example, cars and wheels),
and whether the relationship exists necessarily (every car has at least one
seat) or optionally (a car may have a roof but need not). This notation
scheme can express distinctions of a certain degree of ontological delicacy,
but only up to a point. During the same period, by contrast, AI research
in knowledge representation developed a complex multilevel analysis of
ontological and epistemological categories for the purpose of representing
structural relationships that are much more complex than have usually arisen
in business data (Brachman 1979; Borgida 1991). Within database research,
similar but less ambitious work on semantic and conceptual data modeling has
had little influence on mainstream practice. Instead, the mainstream focus
has been on the business significance of large databases of relatively simple
records that can be searched quickly.

During the 1980s, then, data became increasingly central to the practice of
computing. Even though the design of a database accounts for a minor portion
of the overall cost of designing a system, the structure of data has profound
consequences for the design of algorithms. Once created, data can be used for
a variety of purposes, including purposes that were not envisioned when the
database was originally designed. Database designers therefore increasingly
viewed their work as independent of program design, and they evolved canons
of good practice that responded to cases where database designs failed to
generalize to new applications. Amidst these imperatives, there arose a new
model of computing. Whereas information processing was primarily concerned
with the structure of processing, the newer model was primarily concerned with
the structure of data. And the purpose of data was to reflect the repertoire
of entities in which the business dealt.

The apotheosis of the emerging data-centered view of computing is a popular
book entitled Mirror Worlds, written by the prominent computer scientist David
Gelernter (1991). Mirror Worlds repays close reading. As the title makes
clear, the book's central metaphor is the computer as a mirror of the world;
Gelernter suggests that the progress of computing will inevitably produce a
single vast distributed computer system that contains a complete mirror image
of the whole of reality. Although the computer as mirror is at best a tacit
theme in the database literature, Gelernter makes it thoroughly explicit
and offers it as a way of extrapolating current directions in technical
development:
> You set up a software mirror wherever you like, then allow some complex
> real-world system to unfold before it. The software faithfully reflects
> whatever is going on out front. (p. 6)

The Mirror World, Gelernter suggests, will permit individuals to investigate
reality without leaving home, simply by "traveling" in the digital mirror:
> Capturing the structure and present status of an entire company, university,
> hospital, city or whatever in a single (obviously elliptical, high-level)
> sketch is a hard but solvable research problem. The picture changes
> subtly as you watch, mirroring changes in the world outside. But for most
> purposes, you don't merely sit and stare. You zoom in and poke around, like
> an explorer in a miniature sub. (p. 15)

Video cameras figure prominently in his vision, as befits the optical metaphor
of the mirror:
> Eavesdrop on decision making in progress. Among other things, you will
> discover video feeds down here. When you dive into City Hall, one part of
> the display on your screen might be a (little) TV picture. You can mouse
> over there and enlarge the thing, if you want to hear the mayor's press
> conference or the planning board meeting. (p. 17)

Gelernter is well aware of the privacy concerns that computers have raised,
and much of his book is concerned with the nature of public space in the era
of the Mirror World:
> The Mirror World isn't snoopware. Its goal is merely to convert the
> theoretically public into the actually public. What was always available
> in principle becomes available in fact. Organized, archived, spiffily
> presented, up to the minute and integrated into a whole. (p. 19)

As the last phrase suggests, one purpose of the Mirror World is to repair
social fragmentation by making it possible to grasp the world as a totality
through its computer representation. Gelernter refers to this form of
understanding as "topsight":
> If insight is the illumination to be achieved by penetrating inner depths,
> topsight is what comes from a far-overhead vantage point, from a bird's eye
> view that reveals the whole -- the big picture; how the parts fit together.
> (p. 52)
>
> It used to be generally conceded that whole-sightedness -- a due respect for
> what Madison calls "the permanent and aggregate interests of the community"
> -- was a good thing. Today, all sorts of angry factions are proudly
> dedicated to the methodical tearing-to-shreds of public life. Rapacious PAC
> lobbyists in Washington and multiculturalists at Stanford are quite agreed
> that a little E pluribus unum goes a long way. (p. 31)

Gelernter views Mirror Worlds (which are sometimes singular, sometimes plural)
as extensions of public spaces that can facilitate democratic decision making:
> . . . Mirror Worlds function in part as fire walls opposing the onslaught
> of chaos. But they aren't mere fire breaks. They are beer halls and grand
> piazzas, natural gathering places. (p. 6)
>
> Every Mirror World neighborhood is equipped with a public message board.
> Candidates can post statements. Toward election time, we can set up a
> special political playground, where they can hold forth at greater length.
> (p. 23)

In response to fears that computers are necessarily instruments of social
control through surveillance, Gelernter argues that the Mirror World will make
it possible for ordinary citizens to turn that same power of surveillance back
against the state:
> Mirror World is some huge institution's moving, true-to-life mirror image
> trapped inside a computer -- where you can see and grasp it whole. The
> thick, dense, busy sub-world that encompasses you is also, now, an object
> in your hands. A brand new equilibrium is born. (p. 3)
>
> [Mirror Worlds] scotch that great primal modern fear, to be entangled by
> the sucker-arms of the modern institutional state, and all those private
> mini-states within which . . . we hang embedded. They offer penetrating
> vision; they repair the shattered whole. (p. 184)

In this latter passage, Gelernter suggests that Mirror Worlds will offer
defenses against both the state and the "private mini-states", but he does
not develop this metaphor of private organizations as states or address the
politics of making private organizational information public.

In response to critiques of representation that associate it with emotional
drives for domination and control (e.g., Walkerdine 1988), Gelernter embraces
those drives and promises to democratize them:
> Don't mistake this topsight search for a mere intellectual drive. It's an
> emotional quest too. . . . our grandest accomplishments reflect the innate
> urge to dominate. . . . The pursuit of topsight is intellectually compelling
> because it is emotionally compelling. . . . what lends [Mirror Worlds] a
> uniquely potent potential is the submerged iceberg mass of their emotional
> appeal. . . . topsight to the millions. . . . (p. 184)

Gelernter is aware that security concerns will arise:
> Many Mirror Worlds will contain a good deal of confidential information.
> Professional thieves will certainly be attracted. (p. 197)

Moreover, despite his major emphasis on those parts of the world that
are normatively open to public view, such as public spaces and the state,
Gelernter also offers a model of selective access to the sensitive information
that these vast databases will surely contain:
> Granted, lots of new information-gathering devices have been installed.
> But the information they are gathering and feeding into the Mirror World
> is strictly public information -- or information to which this particular
> Mirror World's clientele is entitled. And the Mirror World will
> discriminate judiciously among visitors. The public at large, for example,
> is entitled to enter the City Hospital Mirror World, and to learn a good
> deal about what's going on. Furthermore, anyone is entitled to see his own
> medical records. But very few people have access to anyone else's, although
> they are all stored down here. Access to private information is closely
> controlled. (p. 19)

To implement this version of access control, Gelernter complicates his
metaphor of travel in a Mirror World landscape:
> The Chief Cameraman is a crucial figure in the Mirror World landscape.
> . . . he knows who you are. He knows exactly which televiewers belong
> to you; which are public; which are private, but you're allowed to see;
> and which you are not allowed to have anything to do with. (p. 196)

Gelernter, clearly, is a technological utopian who seeks to refute the
technological pessimism of the social theorists. He regards the Mirror World
and its political benefits as inevitable -- immanent in the technology as
it is already developing. Despite his contempt for interest-group activism
and the entangling tendencies of the modern state, he is not a libertarian.
To the contrary, he seeks a democracy of liberal individuals, and he thinks
of the Mirror World as a collective undertaking through which the conditions
of liberal democracy might be established:
> The real software revolution . . . will center . . . on software that steps
> over the crucial boundary between private and public. It will have to do
> with "public software works" with civil software-engineering, with Mirror
> Worlds. The software revolution hasn't begun yet; but it will soon.
> (pp. 7-8)

Despite his focus on the public sphere, to be sure, the traditional rhetoric
of organizational control (Beniger 1986) resurfaces whenever Gelernter's
standpoint shifts from that of the ordinary citizen to that of the
organizational leader:
> A parable: consider the modern, state-of-the-art fighter aircraft. It's
> so fantastically advanced that you can't fly it. It is aerodynamically
> unstable. . . . Modern organizations are in many cases close to the same
> level of attainment -- except that, when they're out of control, they don't
> crash in flames; they shamble on blindly forever. (p. 19)
>
> It isn't easy for a hospital administration with the best of intentions to
> make sure that bad or inappropriate or newly outmoded or wrongly sequenced
> or mutually inconsistent or maximally expensive or unnecessarily dangerous
> procedures are never scheduled. A battery of software agents planted in a
> Mirror World can watch for bad practices full-time. (p. 20)

This is a point of instability in Gelernter's argument. At some moments he
presents the Mirror World as a mirror of the public world, but then at other
moments he presents it as a mirror of the entire world. The Chief Cameraman
appears on moments when it is necessary to negotiate this difference.

Gelernter's conception of data differs greatly from the information processing
metaphor. The metaphor of information processing has not vanished, but it
has gone backstage. The computational mechanisms concerned with constructing,
maintaining, and using the Mirror World are still called processes, and
Gelernter uses a hydraulic metaphor to describe them:
> Oceans of information pour endlessly into the model (through a vast maze of
> software pipes and hoses): so much information that the model can mimic the
> reality's every move, moment-by-moment. (p. 3)
>
> A Mirror World is an ocean of information, fed by many data streams.
> . . . Data values are drawn in at the bottom and passed upward through a
> series of data-refineries, which attempt to convert them into increasingly
> general and comprehensive chunks of information. As low-level data flows
> in at the bottom, the big picture comes into focus on top. (p. 27)

Despite the change of metaphor, then, the technical methods that Gelernter
describes are not radically different from those of classical systems design.
The mirror metaphor and the information processing metaphor are more like two
sides of the same coin, logically independent perhaps but each connected to
the other within the discourse of computing as it has evolved historically.

### Representation and Professional Distance

These metaphors are constituents of a discourse; what, though, about the
practices? Gelernter intends to project the future development of computing
technology, and in one sense he is correct: the mirror metaphor provides
one way of expressing a central theme in recent technologists' visions of
computing. Research on virtual reality, for example, is predicated on the
idea that computerized gear attached to a user's body can create immersive
"worlds" that deserve to be called a substitute for reality (Benedikt 1991).
Likewise, a massive community within the computer research world is concerned
with simulating reality for a wide variety of purposes. The US military has
heavily funded such research in support of its ambitious attempt to blur the
distinction between real and simulated battlefields. One battle during the
Persian Gulf War, for example, was thoroughly instrumented and recorded so
that later training exercises could recreate it in fine detail and explore
different directions that it might have taken (Sterling 1993). This project
is continuous with the larger phenomenon that Edwards (1996) calls "cyborg
discourse", which treats human beings, social institutions, and the natural
world as components of one overarching "system". Even when extravagant
ideologies of this kind are missing, the mirror metaphor aptly expresses the
most basic procedure of traditional computer systems design: prepare a roster
of the entities that are present in some part of the world, determine which
relationships among those entities are significant for the tasks at hand, and
create data records whose structures and interconnections map those entities
and relationships one-for-one. Simply put, the computer profession is trying
to reproduce the whole world in the workings of machinery.

Gelernter's vision, then, is congruent with much of the overtly articulated
motivation for pervasive computerization in contemporary industrial society.
His optimism about this vision, though, is hard to evaluate. One approach
would be to accept the metaphor and dispute his sense of proportion: Mirror
Worlds, while increasing the capacity of citizens to conduct computer-mediated
surveillance against the powerful, might be held to increase the already
vastly greater capacity of the powerful to conduct surveillance of their own.
But this argument, which perhaps accurate, is not particularly compelling.

A more sophisticated analysis must begin with the mirror metaphor itself.
In fact this metaphor permits Gelernter, presumably without intending it, to
gloss over numerous features of the actual practice of computing, namely the
diverse forms of mediation between representations and reality (Agre 1995b;
Bowers 1992; Star 1989). Let us consider a few of these.

\* Ontology. A computer can only capture and calculate with what it can
represent. A Mirror World can feed video streams into citizens' living
rooms and store them in databases, but it will not be able to interpret
them in any significant way. The Mirror World's ability to summarize,
abstract, or evaluate the world will depend on the ontology embodied in
its representations.

\* Standards. To have any hope of representing the world in a compact
and useful way, a Mirror World will require that the same ontology, or a
manageably small set of ontologies, be used to represent human affairs the
world over. But this kind of ontological uniformity can only be achieved
through the uniform imposition of standardized categorizations and measurement
schemes (Bud-Frierman 1994).

\* Instrumentation. A mirror can be installed next to an activity without
having much effect on it. But if an activity is to be reflected in a computer
database, its participants must somehow be provided with equipment that can
capture the necessary data. This instrumentation will normally require that
the activity be reorganized in some way, for example by requiring employees
to enter certain data after each job. The introduction of new formal methods
can lead to subtle and pervasive reorganizations in the equilibrium of work
in a given site (Berg 1997).

\* Authentication. A Mirror World which claims to report the activities of
particular people and things must presuppose some material process to verify
their identity. The mirror metaphor postpones this requirement, displacing
the need for identification to the end user of the system who observes the
activities at a digitally mediated distance.

\* Interpretation. Gelernter predicts that Mirror Worlds will eliminate the
need for political interest groups by providing everyone with equal access
to an overall view of society. This assumes that the necessary syntheses
of raw data can be performed automatically. In reality, one major function
of an interest group is its interpretation and synthesis of information. The
work of a legislative analyst, for example, is nowhere near being automated,
although perhaps it can be displaced geographically from the legislature as
drafts of legislation become available on line.

\* Selection. If a Mirror World is easy to set up then presumably anybody
can set one up anywhere. But as the complexities of mirroring become more
evident, the question arises of which data are created in the first place,
and which are stored. Gelernter (1991, p. 27) acknowledges that data streams
generated by environmental sensors can easily create more data than could
possibly be stored. But he assumes that choices about filtering and storage
of the data can be made automatically while preserving the utility of the
system for users.

\* Bias. Citizens using a Mirror World to gain an overview of the real world
will depend on a great deal of software. But software can embody biases that
are not obvious to its users, or even to its authors (Bowers 1988; Friedman
and Nissenbaum 1994). Seemingly objective calculations are routinely deployed
for strategic purposes (March and Olsen 1989). The mirror metaphor promises
an undistorted image of the world, or at worst an anamorphic image if the
mirror is warped, but other types of bias are harder to conceptualize within
the framework that the metaphor provides.

\* Performance. Once Mirror World surveillance becomes pervasive, people
will design their activities with an eye to their consequences of surveillance
(Dourish 1993; Suchman 1992). The activities will become, in effect, staged
performances that project, to the greatest possible extent, the participants'
preferred construction of reality.

The mirror metaphor, then, minimizes our sense of representations as material
things. Computer representations differ from the reality of human activities
in many ways, and computers' ability to create and maintain representations
of human activities presupposes a great deal of prior work (Agre 1994).
The language and practices of database design do not reflect this work, for
the simple reason that it is someone else's job. Databases receive data, and
it is parsimonious to describe the various data elements in a straightforward
fashion as proxies that map a preexisting reality. A database designer might
be told that actions or statuses fall into certain discrete categories, for
example, without needing to know how that categorization is performed in real
life.

The space between representation and reality does sometimes become visible in
database designers' disciplinary texts. Simsion's outstanding data modeling
text, for example, points out that the designer must often choose whether
a given concept is to be understood as an entity or as a relationship, and
he warns against imagining that the answer can be read straight off of the
underlying reality:
> If we think of the real world as being naturally preclassified into entities
> and relationships, and our job as one of analysis and documentation, then we
> are in trouble. On the other hand, if we see ourselves as designers who can
> choose the most useful representation, then this classification into entities
> and relationships is a legitimate part of our task.
>
> Some in the academic world choose the first option: that there are entities
> and relationships "out there" that we need to document consistently. When
> reading the literature, watch out for this assumption -- it isn't always
> explicitly stated. (Simsion 1994, p. 93)

Simsion is referring here to the entity-relationship approach's distinction
between entities and records, as well as its insistence on giving priority to
entities as pre-given features of the business. Nonetheless, he regards the
designer's job as a choice among equally objective representation schemes:
> It is helpful to think of E-R modeling as "putting a grid on the world":
> we are trying to come up with a set of non-overlapping categories so that
> each fact in our world fits into one category only. Different modelers
> will choose differently shaped grids to achieve the same purpose. Current
> business terminology is invariably a powerful influence, but we still have
> room to select, clarify, and depart from this. (p. 80)

Simsion's text provides a valuable record of database designers' collective
experience. Having run up against a certain pattern of difficulty, it is
possible to warn future practitioners against the errors that caused it.
He warns, for example, that commonly used business terms often make poor
names for entities in a data model because these terms may have accumulated
a variety of context-dependent meanings that ought to be mapped onto several
distinct categories of data (p. 64). These warnings outline the contours of
the database designer's epistemological standpoint; they reflect the manner
in which problems become visible from that particular location in the
organizational and disciplinary division of labor.

This effect is most instructive in the case of the designer's choice of
primary keys for a database. The primary keys are those columns in a given
table (i.e., those attributes of a represented entity) that serve to identify
uniquely the entity instance represented by a separate row in the table.
Historically, the notion that these keys are plural derives from practices
such as identifying individual human beings in terms of their names and
dates-of-birth. Paper forms, for example, commonly ask for an individual's
date-of-birth in order to serve as a "tie-breaker" in cases when two people
have the same name. This practice is deeply entrenched in the profession,
not least because, in the normal course of business, queries to databases
tend to employ these "natural" keys. (The effect reinforces itself: the
use of date-of-birth as an identifier in existing databases requires it to
be collected, and then its availability facilitates its use as an identifier
in future databases.) Nonetheless, Simsion argues against the practice.
Some of his arguments are more aesthetic than practical: it is hardly good
engineering, he suggests on pp. 202 and 205, to rely on a probabilistic
assurance of having gotten the right record. A more clear-cut problem can
arise when the scope of a system is broadened post hoc, after the database
has been designed; a choice of keys for the narrower range of things might
not suffice for the broader range (p. 204). His strongest argument, though,
is that foreign keys -- that is, keys whose values are assigned by someone
besides the database designer -- can change. A person might change her name,
or her date-of-birth might be discovered to be in error. Changing existing
online records to reflect the new values will be hard enough, given that the
primary key may be used to identify the individual in numerous tables. But
it may be impossible to update records that have been archived on fixed media.
Simsion says on p. 206: "[the] foreign key maintenance problem is usually
the most effective method of convincing programmers and physical database
designers of the need for stable primary keys".

The point has significant consequences for privacy. The mirror metaphor,
as well as the conceptual and linguistic tendency to conflate records with
the entities they represent, makes it seem reasonable to employ a "natural"
identifier such as name and date-of-birth as the primary key. But, Simsion
suggests on p. 202, a cold look at the technical requirements for a primary
key provides a compelling case for the use of "surrogate keys" -- arbitrary
numbers used solely to signify an individual's existence and not its other
attributes. So long as representations and reality are conflated, it is
difficult to comprehend privacy in any terms other than control over access
to individually identified data records. Practitioners' experiences, though,
have led to a tacit and indirect awareness of the necessity of cleanly
distinguishing representation and reality. Principled application of data
modeling methods and surrogate keys, it must be said, is hardly the norm in
current industrial practice. Nonetheless, consistent use of surrogate keys to
identify data subjects affords other technical options for protecting privacy.

### New Privacy Strategies

At the conclusion of their 1996 meeting in Manchester, England, the European
Union Data Commisioners released a statement reporting their decision
to "work over the next year on Privacy Enhancing Technologies to promote
these techniques for reducing the extent to which personally identifiable
information is used in information systems, with a view to developing pilot
projects which can be examined at their next annual meeting and used as models
to promote the further adoption of these techniques in industry, commerce and
public administration".

The foregoing analyses help explain why the data commissioners' initiative
is possible in theory, and why it is exceedingly difficult in practice. Ever
since Sweden passed the first data-protection law in 1973, privacy policies
have followed a common model grounded in the Fair Information Practices
(Westin 1967; Rule 1974, 1980): presupposing the existence of computerized
data records that identify individuals, governments have sought to regulate
the conditions under which such records are created, used, and propagated
(Flaherty 1989; Bennett 1992).

The data commissioners' analysis of privacy-enhancing technologies (PETs)
relied upon a study by the data commissioners of Ontario and the Netherlands
on technologies of anonymity (Information and Privacy Commissioner and
Registratiekamer 1995; see also Burkert's chapter in this volume). This study
suggested the use of a system element called an "identity protector" to shield
individual identities from organizations holding data records about them.
The underlying technology for identity protection was developed in large
part by Chaum (1985, 1986, 1990, 1992; see also Chaum, Fiat, and Naor 1988).
Chaum observes that data records cannot cause privacy problems for individuals
unless they can be traced back to the individuals whose lives they represent.
So long as databases identify individuals by a universal identifier such as a
name or a government-issued identity number, records can easily be propagated
and merged, and thus employed for secondary purposes to the individual's
detriment. Chaum's alternative approach is to employ digital pseudonyms,
also called pseudoidentifiers. Individuals wishing to transact business with
an organization need not identify themselves. Instead they present proof that
they own a particular pseudonym, and then they use a cryptographic protocol to
present "credentials" (Chaum 1985) that warrant that some relevant predicate
holds (for example, being old enough to purchase alcoholic drinks) without
revealing the information upon which the credential is based (i.e., one's
precise age). The purpose of the identity protector is to manage and
authenticate these pseudonyms, which are then used as surrogate keys in
the relevant organizational databases. Figure 6 illustrates one possible
configuration of an identity-protecting architecture. In this case, the
identity protector is interposed between a system user and a variety of
"pseudo-domains", each of which employs a different pseudonym to identify
the user. By providing a different pseudonym to each organization, the user
can control which personal information moves across organizational boundaries
(Chaum 1990). Other configurations are possible, depending on where the
sensitive identification is stored, which parts of the system actually need
to know the user's identity, and what kind of auditability might be required.
For example, the Air Resources Board's scheme to detect drivers who fail to
repair their emissions systems, discussed at the outset, could employ a kind
of "identity escrow" that discloses the identity of a driver (or the car) only
when fault codes consistently show up over a certain period.

Despite their complexity, schemes based on digital pseudonyms offer certain
advantages beyond the protection of individual privacy. Because databases
indexed by pseudonyms no longer contain individually identifiable information,
they need not be secured as tightly. Information can also be more readily
transferred across organizational boundaries for purposes such as statistical
research. Authentication poses a problem for these schemes, however, and the
most appropriate method of authentication will depend on the particulars of
each application. Photographic or biometric identification of individuals
(Clarke 1994) would seem to defeat the whole purpose of an anonymous system.
Smart cards carry the risk of loss or theft. Users probably cannot be
expected to remember large numbers of distinct passwords. Technologies based
on biometric encryption, though, may be useful for pseudonymous authentication
in certain applications. In the biometric encryption system marketed by Mytec
Technologies of Toronto, individuals initiate a relationship with a given
organization by permitting a Mytec device to encode a known data string using
an optically transformed fingerprint image. On subsequent occasions, they
are able to initiate a transaction by placing a finger on a scanning device to
decrypt the encoded information. The organization, meanwhile, does not retain
an image of the individual's fingerprint or any other individually identifying
information.

Encouraging adoption of such technologies, unfortunately, requires more than
technical existence proofs. One significant issue is trust in the system
itself. After all, the system could also be used as a traditional biometric
authentication system by encoding a universal identifier; an organization that
simply claims to be using biometric encryption is therefore not necessarily
protecting anybody's privacy. The issue is already being tested in Ontario,
where a social activist group, the Guelph Coalition Against the Cuts (1996),
has begun a campaign against a provincial government plan to employ biometric
encryption in distributing social assistance payments. They suggest that
"a multi-billion-dollar corporation making money by treating the poor like
criminals" provides a suitable symbol of the conservative government's cuts
in social welfare programs. Fingerprinting and fingerscanning systems for
welfare recipients have, after all, been implemented in the United States;
the issue here is whether the Ontario system based on biometric encryption
deserves to be assimilated to the police-state metaphors that have long shaped
public understanding of universal identification. It is conceivable that any
misunderstandings could be repaired through a suitable public communication
campaign. One potential model might be the successful campaign that Pacific
Bell conducted in the spring of 1996 as a condition of its introduction of
Caller ID service to California. The issues around pseudoidentity, however,
are much more technical, and the technology itself is counterintuitive even to
computer professionals.

Indeed, the force of habit among designers is another significant obstacle
to the adoption of PETs. So long as the language of computer system design
tends to blur the difference between representations and reality, and treats
data records as mirror images of the world, the firewall that PETs provide
for individual identity will remain nearly unthinkable -- designers will
often simply assume that records pertaining to individuals can be traced back
to them. The problem does not lie in the practices of database design, which
may evolve toward the use of identifers that can equally easily be universal
or pseudonymous -- in that limited sense, the methods of computer system
design do not, as social theorists have often assumed, inherently lead to
the invasion of privacy. Instead, privacy invasion results from the way in
which the technical methods are customarily applied. The necessary change
in customs can be encouraged through model programs and exhortation from
policymakers. Ultimately, though, it will be necessary to revise the training
of system designers to reflect the emergence of new technical options.
Lessons will be needed in cryptography and protocols for the management of
pseudonyms, of course, but other necessary revisions are less obvious. The
examples provided in database texts, for example, almost invariably identify
human beings by their names, and they rarely provide any sense of the moral
issues that are at stake in the selection of primary keys.

Much experience will have to accumulate before PETs can be integrated into the
wide variety of institutions and concrete life situations to which they are
applicable in theory (cf. Bijker and Law 1992). Troubles arise immediately
when organizational relationships are not confined to digital media. Customer
service telephone numbers, for example, have typically required individuals
to identify themselves, and telephone interactions based on pseudonyms will
inevitably be clumsy. Customers who enjoy the record-keeping benefits of
periodic statements (from credit cards, banks, the phone company, and now
automatic toll-collection systems) will require some way of obtaining such
statements without disclosing their name and mailing address.

Perhaps the most significant accomplishment of PETs to date is the beginnings
in a shift of imagination. When records of personal information can always
be traced back to the individual whose life they represent, privacy interests
trade off against system functionality. The result, as the historical record
plainly shows, is that privacy interests almost invariably lose out in the
end. Data-protection regulation can contain the abuse of personal information
within this framework, but it cannot contain the proliferation of technologies
that create and use personal information for ever broader uses. Markets in
privacy can operate at the boundaries of the system, for example to express
customer choice about secondary uses of transaction-generated information,
but such markets require that customers be able to estimate the disutility of
secondary use despite the enormous credit-assignment problem. (The issue is
one of transparency: "How did they get my name?") PETs, however, promise to
provide data subjects with much more detailed control over the use of their
information, as well as greatly lowering the price of refusing to disclose it.
Whether that promise is fulfilled, however, depends on a great diversity of
factors.

### Conclusion

I hope to have suggested the utility of historical investigation of computing
as a representational practice. A brief chapter cannot survey the whole
field of computer science or even the whole subdiscipline of systems analysis;
numerous chapters in the complex history of data have been glossed over,
and relevant areas such as data communications and security have been left
out entirely. Nonetheless, some clear trends can be discerned. At stake is
the sense in which a technical field has a history: what it inherits from past
practice, how this inheritance is handed down, the collective thinking through
which the field evolves, and how all of this is shaped by the institutional
contexts within which the work occurs.

To answer these questions, one might suggest that privacy problems have arisen
through the application of industrial methods to nonindustrial spheres of
life, where normative relations of representation and control are different.
But that statement alone is too simple. Technical work is not indifferent
to the contexts in which it is applied; quite the contrary, it is continually
confronted by the practical problems that arise in pursuing instrumental goals
in particular concrete settings. Another part of the problem, then, is the
manner in which "problems" arise in the course of practitioners' work, and
how these problems are understood. Database designers, for example, have been
forced to clarify their methods on numerous occasions when existing databases
have been used for new and unforeseen purposes.

Yet these mechanisms of practical feedback were evidently not adequate
to stimulate the invention or ready adoption of methods that decouple data
records from human identity. The mathematicians who did invent such methods
in the 1980s were explicitly motivated by a desire to protect privacy, and
they have faced an uphill fight in getting their ideas adopted. Much of
this fight, of course, has been overtly political (see Phillips's chapter
in this book). Organizations with pecuniary interests in the secondary use
of personal information will presumably not be enthusiastic about the new
technologies. But on another level, I want to suggest, the fight concerns
basic understandings of representation and its place in human life.
Information is not an industrial material or a mirror of a pre-given reality.
It is, quite the contrary, something deeply bound up with the material
practices by which people organize their lives together. Computer systems
design will only escape its association with social control once it cultivates
an awareness of those material practices and the values they embody.

### Acknowledgments

One version of this paper was presented at the University of Toronto, where I
benefited from the comments of Andrew Clement. Another version was presented
at AT&T Labs, where Paul Resnick, Joel Reidenberg, and several others offered
helpful comments. Michael Chui and Roger Clarke kindly offered suggestions on
a draft.

### References

Agre, Philip E. 1994. Surveillance and capture: Two models of privacy.
*The Information Society* 10, no. 2: 101-127.

Agre, Philip E. 1995a. Institutional circuitry: Thinking about the forms and
uses of information. *Information Technology and Libraries* 14, no. 4:
225-230.

Agre, Philip E. 1995b. From high tech to human tech: Empowerment, measurement
and social studies of computing. *Computer Supported Cooperative Work*
3, no. 2: 167-195.

Agre, Philip E. Forthcoming. *Computation and Human Experience*.
Cambridge University Press.

Benedikt, Michael, ed. 1991. *Cyberspace: First Steps*. MIT Press.

Beniger, James R. 1986. *The Control Revolution: Technological and Economic
Origins of the Information Society*. Harvard University Press.

Bennett, Colin J. 1992. *Regulating Privacy: Data Protection and Public
Policy in Europe and the United States*. Cornell University Press.

Berg, Marc. 1997. *Rationalizing Medical Work: Decision-Support Techniques
and Medical Practices*. MIT Press.

Bijker, Wiebe E., and John Law, eds. 1992. *Shaping Technology / Building
Society: Studies in Sociotechnical Change*. MIT Press.

Borgida, Alexander. 1991. Knowledge representation, semantic modeling:
Similarities and differences. In *Entity-Relationship Approach: The Core of
Conceptual Modeling*, ed. H. Kangassalo. North-Holland.

Bowers, C. A. 1988. *The Cultural Dimensions of Educational Computing:
Understanding the Non-Neutrality of Technology*. Teachers College Press.

Bowers, John. 1992. The politics of formalism. In *Contexts of
Computer-Mediated Communication*, ed. M. Lea. Harvester Wheatsheaf.

Brachman, Ronald J. 1979. On the epistemological status of semantic
networks. In *Associative Networks: Representation and Use of Knowledge by
Computers*, ed. N. Findler. Academic Press.

Braverman, Harry. 1974. *Labor and Monopoly Capital: The Degradation of Work
in the Twentieth Century*. Monthly Review Press.

Bud-Frierman, Lisa. 1994. *Information Acumen: The Understanding and Use of
Knowledge in Modern Business*. Routledge.

Chaum, David. 1985. Security without identification: Transaction systems to
make Big Brother obsolete. *Communications of the ACM* 28, no. 10:
1030-1044.

Chaum, David. 19\_\_. Demonstrating that a public predicate can be satisfied
without revealing any information about how. In *Crypto '86*

Chaum, David. 19\_\_. Showing credentials without identification: Transferring
signatures between unconditionally unlinkable pseudonyms. In *Auscrypt
'90*

Chaum, David. 1992. Achieving electronic privacy. *Scientific American*
267, no. 2: 96-101.

Chaum, David Amos Fiat, and Moni Naor. 19\_\_. Untraceable electronic cash. In
*Crypto '88*

Chen, Peter Pin-Shan. 1976. The entity-relationship model: Toward a unified
view of data. *ACM Transactions on Database Systems* 1, no. 1: 9-37.

Clarke, Roger. 1994. Human identification in information systems: Management
challenges and public policy issues. *Information Technology and People*
7, no. 4: 6-37.

Clement, Andrew. 1988. Office automation and the technical control of office
workers. In *The Political Economy of Information*, ed. V. Mosco and
J. Wasco. University of Wisconsin Press.

Couger, J. Daniel. 1973. Evolution of business system development
techniques. *Computing Surveys* 5, no. 3: 167-198.

Derrida, Jacques. 1976. *Of Grammatology*. Johns Hopkins University
Press. Originally published in French in 1967.

Di Genova, Frank, and S. Kingsley Macomber. 1994. *Task Order Contract for
Emissions Inventory Projects: Final Report*. Report SR94-01-01, prepared
for California Air Resources Board by Sierra Research.

Dourish, Paul. 1993. Culture and control in a media space. In *Proceedings
of the Third European Conference on Computer-Supported Cooperative Work*,
ed. G. de Michelis et al. Kluwer.

Edwards, Paul N. 1996. *The Closed World: Computers and the Politics of
Discourse in Cold War America*. MIT Press.

Feenberg, Andrew 1995. *Alternative Modernity: The Technical Turn in
Philosophy and Social Theory*. University of California Press.

Flaherty, David H. 1989. *Protecting Privacy in Surveillance Societies:
The Federal Republic of Germany, Sweden, France, Canada, and the United
States*. University of North Carolina Press.

Friedman, Andrew L. 1989. *Computer Systems Development: History,
Organization and Implementation*. Wiley.

Friedman, Batya, and Helen Nissenbaum. 1994. *Bias in Computer Systems*.
Report CSLI-94-188, Center for the Study of Language and Information, Stanford
University.

Gelernter, David. 1991. *Mirror Worlds, or the Day Software Puts the Universe
in a Shoebox*. Oxford University Press.

Gilbreth, Frank B. 1921. *Motion Study: A Method for Increasing the
Efficiency of the Workman*. Van Nostrand.

Guelph Coalition Against the Cuts. 1996. Campaign against
fingerscanning. Message circulated on Internet, July 10.

Guillen, Mauro F. 1994. *Models of Management: Work, Authority, and
Organization in a Comparative Perspective*. University of Chicago Press.

Halpert, Julie Edelson. 1995. Driving smart: A new way to sniff out
automobiles that pollute. *New York Times*, October 22.

Information and Privacy Commissioner (Ontario) and Registratiekamer
(Netherlands). 1995. *Privacy-Enhancing Technologies: The Path to
Anonymity* (two volumes). Information and Privacy Commissioner (Toronto)
and Registratiekamer (Rijswijk).

Lyon, David. 1994. *The Electronic Eye: The Rise of Surveillance Society*.
University of Minnesota Press.

March, James G., and Johan P. Olsen. 1989. *Rediscovering Institutions:
The Organizational Basis of Politics*. Free Press.

Montgomery, David. 1987. *The Fall of the House of Labor: The Workplace,
the State, and American Labor Activism, 1865-1925*. Cambridge University
Press.

Nelson, Daniel. 1980. *Frederick W. Taylor and the Rise of Scientific
Management*. University of Wisconsin Press.

Pool, Ithiel de Sola. 1983. *Technologies of Freedom*. Harvard University
Press.

Radin, George. 1983. The 801 minicomputer. *IBM Journal of Research and
Development* 27, no. 3: 237-246.

Registratiekamer. See Information and Privacy Commissioner.

Reingruber, Michael C., and William W. Gregory. 1994. *The Data Modeling
Handbook: A Best-Practice Approach to Building Quality Data Models*.
Wiley.

Rogers, Paul. 1996. Your future car may be a spy: Clean-air proposal raises
privacy concerns. *San Jose Mercury News*, June 14.

Rule, James B. 1974. *Private Lives and Public Surveillance: Social Control
in the Computer Age*. Schocken.

Rule, James B., et al. 1980. *The Politics of Privacy: Planning for Personal
Data Systems as Powerful Technologies*. Elsevier.

Shaw, Anne G. 1952. *The Purpose and Practice of Motion Study*.
Harlequin.

Simsion, Graeme C. 1994. *Data Modeling Essentials: Analysis, Design, and
Innovation*. Van Nostrand Reinhold .

Star, Susan Leigh. 1989. Layered space, formal representations and
long-distance control: The politics of information. *Fundamenta
Scientiae* 10, no. 2: 125-155.

Sterling, Bruce. 1993. War is virtual hell. *Wired* 1, no. 1: \_\_\_-\_\_\_.

Suchman, Lucy. 1992. Technologies of accountability: Of lizards and
aeroplane. In *Technology in Working Order: Studies of Work, Interaction,
and Technology*, ed. G. Button. Routledge.

Taylor, Frederick Winslow. 1923. *The Principles of Scientific
Management*. Harper.

Thompson, Paul. 1989. *The Nature of Work: An Introduction to Debates on the
Labour Process*, second edition. Macmillan.

Walkerdine, Valerie. 1988. *The Mastery of Reason: Cognitive Development and
the Production of Rationality*. Routledge.

Westin, Alan F. 1967. *Privacy and Freedom*. Atheneum.

Yates, JoAnne. 1989. *Control through Communication: The Rise of System in
American Management*. Johns Hopkins University Press.