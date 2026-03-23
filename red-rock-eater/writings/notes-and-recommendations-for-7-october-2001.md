---
id: notes-and-recommendations-for-7-october-2001
title: "Notes and Recommendations for 7 October 2001"
type: writing
writing_type: paper
date: 2001-10-07
url: "https://pages.gseis.ucla.edu/faculty/agre/notes/01-10-07.html"
coauthors: []
key_concepts: []
importance: 5
research_status: stub
tags:
  - paper
  - auto-imported
---

## Source

Automatically imported from: https://pages.gseis.ucla.edu/faculty/agre/notes/01-10-07.html

## Content

```
As part of my program of not letting terrorists run my life, I have
written some notes on wireless design, transparency, the post-Napster
universe, and the concept of an institution.  I hope they're useful.

**

Blow up your cell phone.

In the United States, much has been said about the dot-com meltdown.
In Europe, however, the salient meltdown is in wireless.  Government
regulators auctioned off spectrum for broadband wireless services,
and a combination of clever auction design and speculative mania drove
prices to insane levels.  Now large parts of the European wireless
industry is imploding.  The Japanese industry is doing better; at
least they, unlike the Europeans, have some proven applications for
their current-generation wireless services.  But the assumption that
people will dive into broadband wireless just because it's there is
not proving true.  Time and again, industry seems surprised by how
long it takes to establish critical mass for a new standard in the
market.  The Internet was misleading in this regard; its sudden growth
resulted partly from pent-up demand during the period of "acceptable
use" policies.  The point, in any case, is that the wireless industry
is driving off a cliff.

At the most basic level, the cell phone industry has lost the simplest
driver of innovation: reducing the size of the handset.  Cell phones
are now so small that, barring sharp turns in human evolution, they'd
be useless any smaller.  They can be made cheaper, of course, and
from different materials, but we are rapidly heading to a world where
cell phones as such are no more exciting an industry than calculators.
So where should cell phone design head next?  Part of the problem is
simply industry habit: except in Japan, whose experience does not seem
to generalize, cell phones have been used almost exclusively for two
applications, voice communications and text messaging, and the latter
application isn't even widely used in the United States.  The market
has been unified by a few standards and a lot of price competition.

The future will be different.  I'd like to see the whole concept of
a "cell phone" blow up.  A "cell phone" as we know it now is a bundle
of functionalities: microphone, speaker, buttons, display, internal
software, and various elements of the communications protocol between
the handset and the base station, among others.  Location-finding
functionality is on the way.  One direction of future development
already seems clear: instead of wiring the communications protocols
into the hardware, generalizing both the software and the protocols
with "software-defined radio" that can be changed dynamically.  But
another direction has had less attention: unbundling the functionality
of the cell phone and then embedding various subsets and supersets
of that functionality into a world of other devices.  Taken together,
these approaches -- software definition and unbundling-and-embedding
-- can lead to a vast new design space.

Here are some possibilities.  In Japan, I am told, radio stations give
out radios that consist of nothing but a credit-card-sized piece of
plastic with embedded electronics and a headphone jack.  The radio is
tuned permanently to the station that gave it out, so it doesn't need
a dial or display, and it's only meant to be used with the headphones,
so it doesn't need a speaker.  The same thing could be done with cell
phones.  Imagine a small object with a headphone jack and a single
button on it.  When you push the button, it "dials" a pre-programmed
number, such as a service that provides movie times.  If interaction
is needed then the button could be used, or else speech recognition.
If you add a microphone to the device then parents could buy it,
program it with their own number, and give it to their children.  It
would be like a specialized calling card, except that it would include
much of the functionality of the phone as well.

Unbundled cell phone functionality can also be embedded in personal
technologies.  If we imagine that we will all become cyborgs, carrying
around a mess of suitably streamlined gear, all of whose components
talk to one another, then the "cell phone" will surely need to talk
to personal sensors, databases, display screens, and so on.  These
personal technologies could communicate with other services over
the network.  This sort of thing has been explored by the wearable
commputing people.  What has been less explored is the main good
purpose for such services: maintaining awareness of the many people
and institutions with which we have ongoing relations: the kids at day
care, the public personae of our professional acquaintances, the ball
scores, the bus we hope to board, the discussion groups we monitor,
and so on.  (Traditional HCI research has drawn some lessons about
maintaining real-time awareness of work collaborators that presumably
carry over to wearable services.)

Another assumption of the industry has been that cell phones are for
mobility.  But from an unbundling-and-embedding perspective this need
not be true.  Imagine a historical battlefield.  At each point where
something important happened, the rangers have installed a green post
with a button and a speaker, and maybe a video display or other more
imaginative kinds of interactive devices.  The green post now has a
cell phone embedded in it, or certain functionalities of a cell phone.
The rangers use it to manage the interpretive "content" at a distance,
for example updating it when new scholarship becomes available or else
extending it with special features for significant historical dates,
material in other languages, and so on.  The posts could also include
public-address capabilities ("the park closes in half an hour") or
emergency call functions, etc.  In this case, the "phone" sits still,
being tied to a significant place, even as the people move around.
The posts could also interact with "augmented reality" gear that is
carried by the park visitors, for example by projecting diagrams or
animation onto the landscape.

The "cell phone" functionality could also be embedded in objects.
Warehouses already have a world of tracking technologies, such as
RFID tags embedded in the boxes, for keeping track of where particular
items are stored. (This is a serious problem for warehouse people, and
large objects get lost in warehouses all the time.)  With time, the
object tracking devices could converge with the unbundled-and-embedded
cell phone.  It would then be possible to pose much more general
queries to the objects, for example embedding sensors in the contents
of the boxes to assure their environmental conditions, run periodic
tests on stored electronics, etc.  Of course, when an object "phones
home" across an institutional boundary, for example between a consumer
who owns a washing machine and the manufacturer that sold it, the
relationship across that boundary becomes more complicated.  It will
be necessary to design the relationship along with the technology.

It is evident, I hope, that the design space of the the unbundled-and-
embedded cell phone is quite large.  It should be possible to look at
a particular application area and brainstorm a spectrum of possible
applications, each requiring different subsets or supersets of cell
phone functionalities.  That very diversity will pose a significant
challenge to the cell phone industry.  Look at the experience so far
with WAP.  WAP may well succeed -- its poor showing so far may simply
be another manifestation of industry's tendency to underestimate how
long it will take to establish a new standard in the market.  But WAP
itself and the WAP coalition display every warning sign.  Not enough
attention was paid to interface design, and the wireless industry did
not understand how to build the alliances needed to make the various
WAP applications really work as businesses.  They had lots of demos,
lots of start-ups, but little serious market acceptance.

What was needed, and missing, is a robust feedback loop between
applications experience and the basic design of the standards.
Useability problems became critical late in the day, rather than being
at the core of the design process.  Unlike the traditional cell phone
applications of voice and text messaging, a platform like WAP succeeds
only if it achieves economies of scale twice over: first in each of
a large number of applications domains, so as to make each of the
applications viable, and then in the applications taken as a whole, to
make WAP services viable in general, for example generating demand for
WAP-enabled handsets.

The unbundle-and-embed design paradigm makes the situation both easier
and harder.  On the one hand, if it really is possible to disassemble
the existing cell phone architecture and embed some of the components
into other systems, then that can only help the existing architecture
redouble its current economies of scale.  On the other hand, if that
unbundling-and-embedding strategy becomes economically central to the
industry, then it will surely place signficant pressures on the future
development of the architecture: the same problem as WAP, only worse.

As the trend toward embedded services unfolds, the design process
will have to change.  History suggests why.  The initial telephones
were fixed in place, either fastened to phone booths or tethered by
wires.  For many years one could speak of a person as "waiting by the
telephone" because the telephone was a place.  Cell phones changed
that, as phones become attached to people.  But the functionality
of the phone remained much the same, and the designer didn't need to
know much about the phone user's way of life.  As cell phones acquire
more features, more knowledge about users becomes necessary, and as
cell phone functionalities are unbundled and embedded, the resulting
services will become intertwined with the patterns of their users'
lives.  This, it seems to me, is the main line of development in the
history of communications services: a progressive intertwining between
communications services and the lives of the people who use them.

It follows that the design process of the future will require a
more sophisticated understanding of the user community.  This starts
with anthropological fieldwork, and it includes participatory design
processes, mock-ups and prototypes, and systematic mapping-out of
the whole universe of potential applications niches.  A good place
to start, as I've mentioned in the context of wearable devices,
is with relationships.  Think of the unbundled-and-disembedded
cell phone functionalities not as devices for making phone calls,
but as infrastructures for maintaining relationships.  What is the
informational architecture of a user's ongoing relationship with a
family member, a school, a doctor, a video game company, and so on,
and what could those architectures become?  What issues, privacy for
example, are at stake in the design and ongoing renegotiation of that
architecture?  How can the design process be part-and-parcel of the
large-scale cultural process by which people reimagine their lives and
choose once again the relationships that make them up?

**

What changes and what stays the same.

A reporter called once to ask my opinion about a controversy that was
taking place near Los Angeles.  A company, it seemed, had set up a
Web site where high school students could post rumors.  Rumors were
posted, consequences had followed, and things had apparently gotten
bad by the time the school administrators heard about it.  Students
were posting anonymous libels, some of them severe, and students who
were preparing for football games would post messages effectively
challenging the students from the opposing teams to gang fights.
Students were allegedly near suicide.  The question was, what is
new in this?  Well, I answered, all of the elements you describe
are ancient.  High school students have always spread rumors about
one another, including evil ones that cause people to feel as though
their lives had ended.  Students from neighboring towns have always
challenged one another to fights.  The Internet, it seemed to me, had
not introduced anything qualitatively new.  Instead, it had amplified
existing forces and made them more visible to the outside world.
The reporter was unhappy with this analysis.  The reporter's job was
to produce news, and I was effectively asserting that nothing in this
situation was new.  We went back and forth a few times, but in the end
I wasn't able to help.

It strikes me that the conventions of news reporting introduce a bias
into our understanding of new technologies and their place in society.
And it's not just news reporting: scholars who want to get tenure are
asked whether they have discovered something, and the easiest way to
discover something in the social world is to declare that something is
new: for example, that we have entered an "information age", a concept
that has been renamed many times.  (James Beniger's book, "The Control
Revolution", includes a huge table of these names, and it's already
fifteen years old.  Nowadays the table would probably extend to book
length all by itself.)  If you can't declare a vast world-historical
discontinuity then you have to go to the trouble of analyzing the
same old world more deeply than others have, and that's a lot of work.

The hardest work, it seems to me, is analyzing just how the existing
forces of society are transposed in a world of pervasive information
and communication technologies.  Just to say that the existing forces
have been "amplified" is a huge improvement over the discontinuity
theory, since the language of amplification makes clear that the
force behind any changes in the world comes from the institutions that
organize people's lives -- including the ways that people take hold
of new technologies.  But still it's limited.  "Amplification" is a
metaphor.  It's vivid to say that the world's knobs are being turned
up to 11, but every metaphor has its limits.  What are the limits of
the amplification metaphor?

To start with, amplification draws a sharp distinction between
the "signal" -- whatever it is that's getting amplified -- and the
"amplitude" -- the factor by which the signal is getting multiplied.
The idea is that you can change the amplitude of a signal without
changing any other aspect of it.  But as every audiophile knows,
that's not quite true, especially when you turn the volume up.
Amplifiers clip, and then they fail altogether.  Just as importantly,
increasing amplitude eventually calls other factors into play.
Your mother tells you to turn the music down, the people upstairs
crank up their own amplifiers to compete, you get a reputation as
a noisy neighbor, and so on.  That sort of thing certainly happened
with the high school rumor site, which called into play all manner
of administrators, psychologists, parents, newspaper reporters,
college professors who got called on the phone for comments, and so
on.  The key point remains: what fuels the phenomena and determines
their shape is not the new technology as such but the existing
array of social forces.  But then sometimes, as old accommodations
break down, the forces reconfigure themselves in a way that the
metaphor can't explain.

I want to focus, though, on the one element of the story that did seem
to me largely new: the Web's ability to make the existing dynamics of
high school rumor mills visible to other parties.  This is a common
pattern with the Web.  Because traditional rumor-mongering happens
mostly in private conversation among trusted friends, is invisible to
the outside world.  When the rumor mill moves onto the Web, however,
a new layer of functionality gets inserted between the social dynamics
and the individuals who participate in them.  The new functionality
amplifies the spread of rumors by allowing people to spread rumors
outside their private groups, but it also bursts the confines of those
groups, both by providing mechanisms to spread a rumor outside the
confines of a private group and by giving everyone, even teachers and
parents, access to the same mechanisms.  Of course, the Internet also
amplifies rumor-mongering in other ways, for example in rumors that
are spread by private e-mails, or within closed mailing lists that
more closely replicate the private conversations among trusted friends
than does the open rumor-posting board.  But those mechanisms require
greater technical overhead (e.g., authenticating users), and they
are not capable of spreading rumors nearly as fast as the more public
boards.

So while the Internet amplifies many things, it only makes some of
them more transparent, and it's interesting to study the conditions
under which the Internet promotes transparency.  For some futurists,
technology as such promotes open information, their prototype being
music-sharing with Napster.  The intuition is roughly that computer
networks are proliferating so rapidly that it's impossible to keep
all the information under control, and that society will consequently
become perfectly transparent.  In my view, the innately transparent
Internet belongs on the same shelf as the flat earth and the black
helicopters.  The very idea flouts basic facts about computing.  IBM,
for example, makes its money by keeping corporate data under control.
Computer networks may proliferate wildly, but it does not follow that
data proliferates wildly.  To the contrary, a computer network is a
platform on which many architectures can be built.  The way you design
a computer architecture is that you talk, and then you convert your
talk into code.  If you talk in a thoughtful way about controlling
data, then architectures that control data are what you get.  So
transparency is by no means an automatic consequence of computer
networks.  Computer networks do sometimes promote transparency, but
the conditions under which they do so are complicated.

As a broad generalization, Internet-based activities are more likely
to be transparent if their participants are more numerous and less
powerful.  A large company, for example, can wire its intranet to its
personnel database, thereby restricting access to its own employees.
IBM, for example, recently held a real-time chat session with many
thousands of its employees, just to see what would happen.  Members of
a small group can simply send mail to the other members individually.
But if IBM employees wanted to set up a just-for-employees discussion
board outside the control of the company, they would have to check
members against the company phone book by hand, and they would have
no way to exclude impostors.  In the case of the high school rumor
board, all of these modes were going on simultaneously: communications
within the school's own computing systems, which they presumably
authenticated with some kind of login mechanism; private e-mails
among small groups of friends; and a public rumor board that anybody
could look at.  Because the public board was trying to do the
hardest job, it was least able to authenticate people.  That's what
made it powerful, in both positive and negative senses, and that's
also what made it transparent.  In the online context, the original
rumor-spreading dynamic split into several parts, but only one of
those parts became visible to parents, principals, and reporters.

(Note that these dynamics don't change much with the addition of a
standard user-identification mechanism such as Passport.  The dynamics
depend not on the identities of individuals but on their attributes,
such as whether they work for IBM or attend a certain school, or
whether they can authenticate themselves privately and informally
to one another.  It's true that Passport might require postings to
have names on them, but nothing says that the names have to be real.)

In the long run, then, the Internet takes something important about
society and leaves it just the same: it's easier for the few and the
powerful to organize themselves out of public view than for the many
and powerless.  Whether the Internet really changes things depends
on how you set your measuring instruments, and on what you measure.
At the end of the day, words like "amplification" are just heuristic
tools.  They call things to your attention and help prevent you
from making stupid mistakes.  But eventually you have to get down to
analysis of the specifics.  History is made on the ground, and the
mosh pit of social forces that contend in any given setting is just
as complicated as it ever was.

**

Competing with the past.

Napster made everyone feel cool.  It was fun, wasn't it?  The fact
is, though, that stealing musicians' work isn't cool.  It doesn't
matter that you're also stealing from the nasty record companies.
It's still wrong.  I recognize that the intellectual property laws
that the record companies pushed through Congress are unreasonable.
But "trading" music instead of paying for it is unreasonable too. 
And I know that trading music with your friends is a fair use.  But
some random person who rips their CD's onto a Napster server isn't
your friend.  Fair use is important, and the infamous laws trample
on it.  But in defending fair use, we shouldn't also get trapped into
defending theft.  Napster was a false alarm, and I'm glad it's gone.

Still, the problem remains: the record industry is a snakepit and the
radio industry is worse.  So what to do?  The long-term solution, if
one exists, involves new institutions that connect musicians and fans
without the dysfunctions of the institutions that we have now.  Let's
admit that we need such institutions, and that we have no idea what
they would be like.  In sending URL's to my list over the last year,
I have tried to suggest bits and pieces of the solution.

On one hand, you have the old-traditional methods by which bands build
audiences: touring, mailing lists, opening for established bands, and
doing their own distribution.  The Internet helps with all of these
things, and that is good.  Maybe the bands who are looking to record
companies to make them into stars overnight just need to learn how to
build a career.

On the other hand, you have new developments that extend the reach of
existing institutions: global media conglomerates that can use the Web
to cross-promote their music acts with their TV shows and films etc,
Web-casting that allows independent DJ's to build global audiences,
magazine sites that archive their critics' reviews, customer reviews
on Amazon, and so on.  Maybe we should just wait for these mechanisms
to take hold.

Or maybe not.  The truth is, we don't have a clue.  To figure out
what an alternative system might be like, we need to return to basics.
Some of the basics, as we know, seem promising.  Cheap production
technology means that more bands can have their own studios.  They
can produce their own CD's, and if they distribute free samples of
their music on the Internet.  A centralized site where bands can sell
their self-produced CD's would be good too, and it seems to me that a
company could prosper by marketing a bundle of online tools to bands
pursuing DIY careers.  (MP3.com does not count.)  Still, enormous
problems remain in the area of publicity.  The mass media persuaded
us that you could form an instant relationship with millions of
people through the grace of an appropriate gatekeeper, and it eroded
that part of our imagination in which audiences are built one person
at a time.  One irony of the Internet is that, despite its ubiquity,
it reconnects us with this one-to-one kind of organizing.  That,
in a deep sense, is the real business that record companies are
in: building a kind of social organization, an infrastructure in the
broad sense of that overused word, that connects fans to bands -- and
not just to the bands' music but to their tours, images, merchandise,
other fans, and so on.  Radio networks are an infrastructure, too, in
this broad social sense: not just equipment, but relationships.

Before we can understand how to use the Internet in replacing those
existing infrastructures, however, we need to understand them better.
How is it that they really function now?  What exactly is it that
we are trying to replace?  To that end, I want to focus on a single
issue that I cannot recall being discussed elsewhere: the sense in
which musicians, like the producers of any information product, are
competing with the past.  Information products have the distinctive
property that you can use them without using them up, and so much of
the information that has ever been stored in a permanent medium is
still out there.  (I realize that no medium is permanent, and that
lots of good people are dealing with the impermanence of old media.
But allow me to idealize that issue away for the moment.)  To be
heard, then, a musician must compete for listeners' attention not only
with other musicians who are currently playing, but with the whole
history of recorded music.  Novelists, scientists, and many others are
in the same position.

Who has it worst?  The problem is probably worst for musicians, in
that music retains its value better than most kinds of information.
Software goes bad because the hardware it runs on becomes obsolete,
and because the other software packages with which it becomes
compatible.  Still, Microsoft is very aware that its new products
compete with its old products, and Microsoft's survival increasingly
depends on its ability to compel people to switch from reasonably
functional existing products to excessively functional new ones.  The
Y2K debacle also reminded us of the unexpected longevity of business
software, especially custom applications.  The costs of switching
to new business software are so great that even very sophisticated
new enterprise systems often fail to compete with old COBOL programs.
Scientific works have a very short lifetime, and the institutions
of science are extremely effective at ensuring the obsolescence
of their products.  Scientific works are not very substitutable: if
you study worm genetics then a paper on butterfly migration doesn't
help you.  This is one reason why the prices of scientific works are
so inelastic, and why scientific journals are therefore so expensive.
Books about current politics (as opposed to political philosophy)
are notoriously short-lived, and used bookstore owners refuse to
buy them.  Works of fiction ought to compete with the past much more
than they do.  Because they are hard to judge by browsing, however,
they are extremely dependent on publicity campaigns whose details are
soon forgotten.  If readers could somehow be magically connected to
the single work of fiction among all works of fiction ever published
that they should most be reading right now, then new fiction would
probably cease to be economically viable.

That leaves music as the form of information that competes most with
the past.  The amount of recorded music in circulation has increased
almost infinitely in the past thirty years, and even though 99% of
it is deservedly forgotten, the remaining 1% is still more music than
anyone could listen to.  Whole industries make money from old music,
and many (if not most) radio stations and dance clubs define their
formats in terms of decades or genres gone by.  Many pieces of music
produce revenue (whether captured by their copyright owners or by
someone else) for decades on end.  Large quantities of music are
forgotten and then rediscovered, for example by enthusiast labels like
Yazoo or Rhino that are operated more for love than for profit.  But
in dollar terms, what makes those long-lived songs most valuable is
their familiarity: they have become standards, and they occupy a niche
in the heads of a certain segment of the population, some of whom find
them welcome when they come around again.  They are known quantities.

It follows that musicians face serious obstacles in making a living
from newly issued music.  They can make music that is stylistically
derivative, but it can only compete with the old, familiar music if
audiences care about things besides the music, such as identifying
with the musician as a celebrity.  In the old days a musician could
become established by playing new renditions of standards, but that
stops working as music moves away from melody toward unique "sounds"
produced in the studio.  Even listeners who are strongly interested
in novelty have large piles of old CD's that they listen to, and music
that departs from established formulas is generally an acquired taste.
That is why record companies must expend such huge sums of money
"breaking" new artists.  The money they invest promoting a new act,
however, turns into concepts in people's heads, and those concepts are
durable.  In a sense, the real "property" that is owned by a record
company is not so much the copyrights (or other kinds of contractual
control) over the songs, but the reservoir of familiarity with those
songs -- their "brand identity" -- that lives in the minds of the
audience.  It's that mental stuff that the industry makes its money
from over the long haul, and a wise record company will manage that
resource using whatever strategies best maintain its discounted
presented value.  The sheer amount of song-familiarity in circulation
at any given time, however, is limited: people can only listen to so
much music, and only so much revenue can be extracted from them as
they do so.  Familiarity with standards is capital, and there's no
room in the market for new capital until the old capital decays.  Of
course, the power of record companies to preserve the value of their
capital is not infinite.  Fashions change.  People did eventually
tire to some degree of rock and roll.  But the recalcitrance of music-
capital is considerable.

Most people will find this analysis distasteful.  But it seems to me
that many bands have little clue about the real nature of the record
business.  They resemble the shop-floor employee who has no clue about
the value added by the entrepreneurial effort of the capitalist.  Of
course, one can certainly question whether the market in each case is
structured to allocate rewards fairly between between the line worker
and the entrepreneur, and there can be no doubt that the notorious
terms of record companies' form contracts reflect a dysfunction in the
economics of the record industry.  Even so, alternative institutions
will not arise to replace the record industry until the entrepreneurial,
capital-creating work of record companies is comprehended and rethought.
That is what bands do when they build their own audiences: touring
in bad clubs, building mailing lists, and all of the other mechanisms
that I mentioned at the outset.  If a band is working basically as a
hobby then the economics are not very important: they can tour in bad
clubs while it's still fun, or maybe they can build a small audience
that keeps them minimally fed.  But if they want careers, then they
have to move their business operation to another level.

And that, presumably, is where the Internet comes in.  It's too
bad that, amid all the stories that have been written about Napster,
so few stories have been written about bands that have succeeded
in building careers through a combination of old and new means.
Why aren't business professors writing best practice studies for the
small businesses known as bands?  I know -- don't tell me.  They are
writing best-practice studies about the kinds of businesses that offer
lucrative consulting gigs to business professors.  Still, I do have
to wonder if 10% of the effort that goes into defending Napster could
go instead into something more constructive.

**

Three ways of looking at institutions.

Information plays many roles in our lives, and so radical improvements
in information technology are certain to changes our lives in more
ways that we can easily think about.  One useful tool for thinking
about those changes is the concept of an institution.  Institutions
provoke ambivalence, and reasonably so.  Institutions such as the
electoral system, the medical system, the university, the market,
the church, the theater, and commercial air travel all enable people
to do things that they want to do, but at the same time they also
constrain people in many ways.  That is the ambivalence: institutions
both enable and constrain, and they enable *by* constraining.

Institutions are not inherently good or bad, although particular
institutions can be either.  When we think of institutions, normally
we think of static, oppressive structures that run our lives from
afar.  But that's not right.  Institutions are more like grammars
of social life: rules that we are socialized into, and that we enact
every day without realizing half the complexity of what we are doing.
Institutions are distributed, in that they happen through the loosely
coordinated actions of numerous people, and they are dispersed, in
that they persist through numerous mechanisms of language, habit,
expectation, law, incentive, and design.  The distributed and
dispersed nature of institutions is counterintuitive.  To help make
it more intuitive, I want to present three ways of thinking about
institutions: as inscription, as a framework for careers, and as a
reservoir of skill.  None of these perspectives on institutions is
sufficient on its own, and many other perspectives would be required
to present a full picture.  But perhaps some of the usefulness of the
concept will become clear.

1. The institution as inscribed discourse

Let us consider an analogy among three things: software, law, and
architecture (i.e., the built environment).  All three arise in the
same way: you start with some vernacular language, you formalize that
language by processing it to recover its underlying structure, and
then you embody the resulting formalism in a combination of artefacts
and ideas that regulate people's lives.  In software this process
is called systems analysis, which really does start with informal
language about what the system is supposed to do; it then cleans up
the ambiguities, inconsistencies, and redundancies of that language
until the result can be converted into code.  In law the process
happens in several ways, such as the writing of legislation or the
rational reconstruction of popular intuitions in the form of common
law.  In architecture, the "program" of a building's functions is
drawn largely from the users' own language for naming and describing
the activities that will take place in the building.  A building
might have an entrance, a coatroom, offices for secretaries leading to
offices for executives, public areas and back offices, and so on, each
mapping a function from the program onto an architectural category.
(See Thomas A. Markus, Buildings and Power: Freedom and Control in
the Origin of Modern Building Types, Routledge, 1993.)  In each case,
the product is not simply the artefact (running code, printed law,
built structure) but the combination of the artefact and the language.
The artefact doesn't operate without the language, and the language
is grounded and stabilized to an extent in the recalcitrance of the
artefact.

The language that gets inscribed into software, law, and architecture
is not at all arbitrary.  In the case of law and architecture, the
language invariably reflects some human institution.  In law it is
often an informal institution that has stabilized in social practice
and is now being codified in law.  In architecture it is the language
with which an institution's participants name the institution's roles,
relationships, and activities.  In a hospital, for example, patients
go in some places, doctors in others, nurses in others, administrators
in others, visitors in others, and so on.  The social structure maps
onto the building, and individuals cannot "use" the building unless
they have mastered their respective social roles and thus, literally,
know their place.  Software has greater latitude: some software is
written about galaxies or fantasy worlds that are institutions only
in an extended sense.  Most software, however, inscribes paradigmatic
cases of institutions: running a business, publishing a book, keeping
track of money, flying aircraft in accordance with rules, and so on.

It is well-known by now that software can be viewed as a kind of law.
But it's important to generalize the point.  Institutions operate on
several levels, and one reason why they are so stable historically
is precisely that they are inscribed simultaneously in software,
law, architecture, language, bodily habits, conversational patterns,
and much else.  This is partly what it means for institutions to
be dispersed: the same structures are inscribed in several media at
once, each of which tends to reinforce the others.  When software
is written, each of the other levels (law, architecture, etc) pushes
the institutions of software-writing to write code that is aligned
with themselves.  When law is written, interest groups push to encode
their established practices into the legislation that governs them.
Not that institutions lack controversy; to the contrary, the operating
rules of an institution are well-understood as frozen accommodations
among contending interests.  (See Jack Knight, Institutions and Social
Conflict, Cambridge University Press, 1992.)  These accommodations are
always being tested at the margins, and any social disruption -- from
technology to culture to the relative prices of economic inputs --
can reopen old issues to negotiation once again.  Whenever a building
is built, likewise, different visions will always contend to shape
it.  The possibilities for shaping are always limited by institutional
constraints on other levels, but some room for shaping does always
exist.  Buildings can be made more or less flexible, thus settling
controversies or else leaving them open to some degree.  Likewise with
software and law.

2. The institution as a framework for careers

We are familiar with the concept of a career from a few institutions,
especially business.  But politicians also have careers, as do
ministers and soldiers.  In each case, we understand a career as
a sequence of jobs.  The term tends to imply that the arc of one's
career is upward, that something is accomplished and accumulated
along the way, and yet that the path from each job to the next is
largely routinized, for example in a ladder of promotions.  Athletes
are something of an exception: when we speak of an athletic career,
we usually don't imply that the athlete has moved from one position
to another, only that the player has racked up so many points,
broken certain records, been awarded certain honors, and so on.
If the player goes on to be a coach or announcer, we speak of that
as something they did after their career was over.  In this latter
sense athletes' careers are like everyone else's: if someone changes
professions several times, we don't usually talk about a career, or
we say that the person had several careers.

That is the usual notion of a career, and it cuts across a number of
institutions in an irregular way.  But I want us to define the concept
of career more generally.  Every institution, as I have said, defines
(among other things) a set of roles and relationships.  Everyone who
is involved in the institution is assigned to one or more of those
roles, and is entered into a standardized map of relationships.  In
that sense, everyone has a career in every institution that affects
them in any way.  The fans in the sports stadium have careers, for
example as they move from the bleachers to the boxes.  Nearly everyone
has a financial career, and starting in the 1970s those careers became
much more complex as ordinary individuals moved their money out of
banks and into money market accounts and then mutual funds and other
complex investments.  (See Joseph Nocera, A Piece of the Action: How
the Middle Class Joined the Money Class, Simon and Schuster, 1994.)
People invest great effort in their financial careers, strategizing
both to maximize their college and retirement savings and to build
their credit record.  Churches also define careers for their members,
for example in the rituals that mark life transitions.  Drivers have
careers that involve roles in many institutions: law, insurance, the
auto industry, and so on.  In some cases the term "career" sounds odd
because the institution does not inspire the sense of striving that
the term implies in the domain of paid work.  Sports fans may politick
for Super Bowl tickets, but for the most part they are not climbing
up the hierarchy of fanhood.  That's fine.  A career is a trajectory
through an institution, whether it is important or trivial, deliberate
or accidental, strategized or improvised, formalized or casual.

People's careers in different institutions interact.  This is clear
when we consider the role of social networks.  Networking is a central
mechanism of career-building in most institutions.  It's not entirely
who you know, and "knowing" someone can be a complex thing, but the
fashioning of networks is part of advancement in many institutional
careers, information-gathering in many more, and institution-changing
now and again in all of them.  And networks built in one context are
often useful in others.  Small business people such as carpenters and
accountants have a great incentive to go to church, aside from the
spiritual incentives, because church is a place to build the trusting
relationships that lead to jobs.  People enter politics partly to
build networks that will be useful in business, and they attend
universities partly to build networks that will be useful in their
professions.  When communication and transportation are poorly
developed, the networks created within different institutions will
overlap heavily, simply because it is hard to maintain networks
far from home.  Thus, lodges such as the Elks were once important
institutions for no reason other than maintaining social networks,
and in some areas they are still a backbone (for better or worse) of
local social orders.  Networking is more complex now that technology
and globalization have made far-flung networks increasingly possible
and necessary in many institutions, and the much-discussed decline
of social capital may reflect a decreased tendency for the social
networks created within different institutions to overlap with one
another.

The role-trajectory and social-network understandings of careers are
closely related.  People often gain access to new institutional roles
because of the social networks they have built, and they often take
advantages of their new roles to build new networks.  Careers have
other aspects as well, but this brief discussion of roles and networks
may indicate something of the complexity of institutional careers.

3. The institution as a reservoir of skill

One of the oldest conceptions of the institution is as a reservoir
of skill.  Thorstein Veblen wanted the world to be run by engineers,
and he saw the progress of industry as the accumulation of technical
knowledge in the engineering profession.  Knowledge for Veblen was
not the property of the individual engineer or company, but of the
engineering profession as a whole.  When engineers work on concrete
technical problems, they accumulate knowledge; when they work
together, they pool their knowledge; when they change jobs, they take
their knowledge with them; and they advance in their careers largely
by contributing new knowledge to the commons.  Veblen was writing in
the context of a vast movement of profession-building that started in
the railroads in the mid-19th century and then spread to hundreds of
other areas of society in the Progressive era.  Whereas the railroad
associations were largely spontaneous -- and could be, given the ease
of transportation on the rails and communication on the telegraph --
the engineering associations were controlled much more by employers,
a fact that David Noble has documented in detail but that Veblen wasn't
much interested in, given his agenda of taking social control away
from the financiers and giving it to the people who, in his mind, did
the real work.

Later in the 20th century, organizational theorists elaborated on
(without always acknowledging) Veblen's insight.  They observed that
the crucial type of knowledge is not technical knowledge in a narrow
sense, but business knowledge -- that is, how to use the technologies
in a business context.  A crucial discovery in the chemical industry,
for example, later came to be called economies of scope: manufacturing
modular building blocks from which numerous products could be
assembled, and developing all of the markets for those products so
as to ensure that the fixed costs of producing the building blocks
are fully recovered.  (For more on this topic, see the introduction
to Alfred D. Chandler, Jr., Franco Amatori, and Takashi Hikino,
eds, Big Business and the Wealth of Nations (Cambridge University
Press, 1997).)  Partly because Veblen's contribution was not fully
remembered, the people who told this later story tended to locate
the phenomena of collective memory in the individual firm (the
organization) and not in the industry (the institution).  They were
professors of business management, and their job was to tell managers
how to make their particular businesses succeed.  The circulation of
knowledge through job-changing was not central to their story, which
lost some of its analytical power as a result.

Another version of the story, from quite a different direction, is
found in Stephen Toulmin's two-volume opus "Human Understanding: The
Collective Use and Evolution of Concepts" (Princeton University Press,
1972).  Toulmin is a philosopher of science, a topic that Western
philosophy considers important because it promises to explain how
objective knowledge is possible, and he observes that science happens
in communities.  Scientists are socialized into their communities,
which instill in them all manner of intuitive and practical
knowledge, and shape and regulate their practices in numerous ways.
The knowledge that science produces is collective property, at
least in some crucial sense, and this discovery is good news, given 
how difficult it has proven to justify knowledge on the basis of
individual experience.

A later version is the concept of community of practice, which began
with work by Jean Lave and Etienne Wenger at a Xerox PARC spinoff,
the Institute for Research on Learning, in the 1980s.  Etienne later
wrote a book called Communities of Practice (Cambridge University
Press, 1998).  A community of practice is a group of people with
its own culture, which uses its rituals to pool knowledge among
its members.  New members are acculturated by participating at
the edges of the activity, for example through apprenticeship, and
then by moving to successively more central roles in the community.
The community of practice framework does not provide hard-and-fast
generalizations about the workings of the communities, but rather
a set of concepts that have proven useful in analyzing the workings
of many particular cases.  In a series of papers and a recent book,
The Social Life of Information (Harvard Business School Press, 2000),
John Seely Brown and Paul Duguid have developed the community of
practice framework in making suggestions about the future of several
institutions, such as politics and the university.  The key in each
case is to amplify (and certainly not to destroy) the conditions that
make communities of practice possible.  A university, for example,
should be viewed (at least from one perspective) as a mechanism for
introducing an individual into the community of practice in which they
will spend their career.

Even though the concept of the institution as a reservoir of skill
has developed mainly in the context of occupational communities, the
concept also applies to all of the communities that are created by any
institution.  This is a deep point: every institution defines a set
of social roles, and all of the occupants of those roles constitute a
community.  Now, it will be objected that the term "community" should
be reserved for special cases: groups of people that share an identity
and autonomous communications forums.  Some people feel strongly
about this: by watering down the word, they argue, we water down the
reality.  My own view is that we ought to analyze all of the diverse
mechanisms by which institutional communities pool their skills.  Some
of these mechanisms resemble the communitarian ideal, as for example
in well-developed professional associations.  Others, however, are
more spontaneous, organized more by shared ideology and culture than
by formal organizations.  Formal assocations, moreover, increasingly
fail to encompass the full range of informal skill-pooling mechanisms
that become possible as technology allows individual community members
to maintain ongoing relationships.  The term "community" in its more
traditional, honorific sense is an analytical straitjacket.  That term
has certainly been connected with positive values, such as autonomy,
that should often be encouraged.  But those values should receive
precise and specific names of their own, rather than riding on the
hopelessly overburdened term "community".

In any event, the consequences of viewing every institution as a
reservoir of skill are profound.  Every modern society consists of
hundreds of institutions, each of which generates several reservoirs
of skill among its participants.  Once these reservoirs of skill
have become analytically "visible", it becomes possible to study
the conditions under which they arise, and the conditions under which
they are reproduced or transformed.  Many societies, for example,
are said to lack functioning institutions.  The solution to that
problem depends on one's understanding of the nature of institutions.
If institutions could be made functional simply by passing laws or
chartering associations, then the problem would be easy.  In practice,
though, the hardest part of building an institution is to spread the
institution's knowledge throughout the relevant part of the populace.
The institution of banking, for example, exists only when the skills
of banking are widespread.  Those skills include the mechanics of
opening an account, but they also include the personal financial
strategies that make banks worthwhile.  The institutions of private
property, likewise, do not function correctly unless the society's
members know how to use them.  Otherwise one has simply created the
legal rationalization for state actions to take people's property away
from them, for example when someone else manages to create a legal
title or when the property is used as collateral for an ill-advised
loan.

4. The institution as all of the above

Those, then, are three ways of looking at institutions.  Institutions
provide a framework for individual and collective action, and people
run their lives within them.  Institutions allow people to pursue
strategies, share knowledge, form relationships, and much else.
Institutions provide people with discourses that organize their
conceptions of themselves and others, and for the most part people
follow the well-trodden paths that have been mapped by others before
them.  Those paths are precisely the institution's reservoir of
skill.  In this way, the concept of an institution promises to resolve
the ancient tension between determinism and free will: institutions
provide extensive enablements and constraints for people's dealings
with one another; they instill many layers of self-conception, skill,
and habit; and people experience all of that stuff as the landscape
upon which they pursue their life strategies, most of which are drawn
from the collective repertoires of their institutions.  People are
partially aware of the institutions that organize their lives, and
they also partially embody those institutions in a prereflective way.

The three aspects of institutions that I have sketched provide some
sense of institutions' distributed, dispersed nature.  Institutional
discourses are dispersed across the programs, laws, and buildings
into which they are inscribed, and then they are distributed among the
many individuals who learn to use them.  Institutions operate largely
in a distributed fashion through the incentives that motivate their
participants to pursue careers within them, and the unfolding career
strategies they adopt.  These strategies pervade the activities that
an institution organizes, and few activities can be well-understood
except by taking their participants' career strategies into account.
Each institution's reservoir of skills, likewise, is distributed
throughout the population that participates in it, and is also
dispersed throughout the various mechanisms (observation, textbooks,
maxims, career strategies, war stories, rules of thumb, and so on)
that spread those skills around.

That said, it is worth noting that the each aspect of institutions
has its own emphases.  The concept of inscription emphasizes the
categorical structure of institutions: the way they distinguish among
roles, define relationships and activities, and so on.  The concept
of career emphasizes strategy and networks, and pays little attention
to the day-to-day activities that an institution organizes.  And
the concept of collective skill is more akin to the anthropologist's
organic vision of culture than to the hard-edged formalism of the
other two concepts.  It follows that each concept helps deepen the
others.  The formal structure that is inscribed in software, laws,
and architecture provides a stable framework for the activities of
knowledge-sharing and the strategies of careers.  Knowledge-sharing
is driven largely by incentives to build careers.  Careers are built
using methods derived from observing the successes of others.  And so
on.

Of course, these are all rough generalizations.  Nothing is definite
until we bring the concepts to a particular case study and determine
which ones apply and how.  The advertisement I offer for the concept
of institution is not that it dictates any generalizable laws of
social order; such laws do not exist.  Rather, the concept of an
institution provides an elaborate conceptual framework that has proven
useful in analyzing diverse situations.  Using the same framework to
analyze many situations is particularly important, because the shared
concepts allow us to compare and contrast different cases.  Phenomena
that may be notorious in one situation may be obscure or forgotten
in other situations, and we can use the shared conceptual framework
to build analogies between them.  Each situation thereby becomes a
means of defamiliarizing the others.  This is the essence of social
analysis: each of us takes a set of analytical concepts out into
a particular situation, sees what phenomena the concepts draw our
attention to in that particular setting, sees what else we have been
led to notice in that setting as a result, coins a new concept to
name the previously unnamed thing we have seen, and contributes that
concept to the shared supply of concepts that others can bring to
their own situations.

The measure of social analysis, then, is not the strength of the
generalizations we can draw, but the depth with which we are able
to see what is going on in particular situations.  Every one of us
is likely to notice some things more than others, for example because
of our social background, but by putting names on things and telling
stories that make the names memorable, we make it possible for other
people to analyze the world more completely.  These analytical skills
are always important, but they are especially important now that the
world is changing in deep and uncanny ways.  We should be impatient
with simple generalizations about an "information age" that can be
characterized with a few slogans.  The reality is not simple, and
it's never going to be simple.  We will never sum it up, and we should
never try.  What we can do, though, is help equip one another to see
ever more clearly the institutional settings that we know and care
about, so that we can talk sense on the day when the people around
us finally see the changes happening, become alarmed, and ask us what
to do.

end
```