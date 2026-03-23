---
id: notes-and-recommendations-for-21-december-2000
title: "Notes and Recommendations for 21 December 2000"
type: writing
writing_type: paper
date: 2000-12-19
url: "https://pages.gseis.ucla.edu/faculty/agre/notes/00-12-21.html"
coauthors: []
key_concepts: []
importance: 5
research_status: stub
tags:
  - paper
  - auto-imported
---

## Source

Automatically imported from: https://pages.gseis.ucla.edu/faculty/agre/notes/00-12-21.html

## Content

```
Some notes about spam, content-filtered e-mail, the breakdown of the
mind/body divide in computing, the art of public design, the hazards
of organizational learning, the amplification model, industrial design,
computer security, and cheap pens, plus assorted notes and (!) URL's.

**

The draft about architecture and context-aware computing that I sent
out a couple weeks ago is now in shape to be circulated.  It's at:

  http://dlis.gseis.ucla.edu/people/pagre/hci.html

If you think it might be useful then please pass it along to HCI
people, wired architects, wireless applications people, and anyone
else who might be interested.  If anyone has comments that might
affect it, there should be time before it goes to the printer.

**

Thou shalt not appear to spam.

Here is an unwritten rule of the Internet -- at least I've never seen
it written.  I know a guy who makes his living running a newsletter.
It's a paper newsletter -- he doesn't know a lot about the Internet.
Since it's his living, he advertises.  And since the topic of the
newsletter is specialized, he essentially has to locate his possible
subscribers one by one.  So when he is out surfing the Web, whenever
he comes across the Web page of someone who seems like they might be
interested in his newsletter, he sends them his standard advertisement
for it.  When he does this, some of the people complain.  They accuse
him of spamming them.  He feels hurt.  He knows all about spam, and he
doesn't feel as though he has spammed anyone.  To his mind, every ad
he sends is perfectly individualized.

It gets worse.  The same guy publishes a directory of people who
work in his specialized field.  He gets people's addresses from the
attendee contact lists at conferences and things like that.  Yet
some people accuse him of violating their privacy, and tell him that
he should ask their permission.  He feels hurt.  He knows all about
privacy, and doesn't feel as though he has invaded anyone.  To his
mind, the information he is publishing couldn't be any more public.

So who is right?  Are we dealing with paranoia?  No, I think we have
simply encountered an unwritten rule: not just "thou shalt not spam",
but "thou shalt not *appear* to spam".  If I get a boilerplate ad
in my mailbox, even if my address appears in the "To:" field, I can't
tell whether I have been spammed or not.  The more boilerplate the
message looks, the more I feel entitled to assume that the message is
spam.  And it's not even hard for a spammer to automatically generate
a little greeting like "Dear Phil" from their spam-list of people's
names and addresses.  So my rule is: the message isn't individualized
unless it reflects some specific knowledge of who I am.  Strangers who
send me commercial stuff are obliged to individualize their messages
in this way because, I claim, they have an affirmative responsibility
to show that their message isn't spam.

What about the directory?  The problem with a directory, especially
one that is available in electronic format, is that it can be used
to spam.  Even if this guy, in his heart of hearts, isn't planning
to spam, we have no way of knowing (a) that his intentions are pure,
(b) that he won't change his mind, and (c) that he will prevent his
directory from falling into the hands of those who shouldn't have it.
He should ask permission to include public information in his list
precisely because creating the list also creates the appearance of
contributing to spam.  "But isn't the information public?"  The fact
that you were in Central Park on Thursday is public, since anybody
who saw you in Central Park is allowed to know that you were there.
But it doesn't follow that they are allowed to compile a list of
everyone who was in the park on that day.  The quantitative difference
matters.

So that's the rule: no appearance of spam.  It's like the "appearance
of conflict of interest" norm in politics.  You know, like the outcome
of the election being certified by the campaign chair of one of the
candidates.

**

It has begun: the era of content-filtered e-mail.  I have had three
RRE messages bounced back to me by automatic content filters that had
been installed by the subscriber's organization.  For two of them, the
problem was that a URL included a word that allegedly also occurs in
virus code.  Really: the mail filter claims to detect a virus from one
word.  I would tell you what the word was, but I don't want my message
bounced back.

Here is the bouncemail from the other content-filtered message:

  Date: Tue, 19 Dec 2000 09:32:25 -0800
  From: System Attendant 
  To: "'Phil Agre'" 
  Subject: ScanMail Message: To Sender, sensitive content found
    and action taken.

  Trend SMEX Content Filter has detected sensitive content.

  Place = Red Rock Eater News Service; ; 
  Sender = Phil Agre
  Subject = [RRE]Supreme Court decision
  Delivery Time = December 19, 2000 (Tuesday) 09:32:23
  Policy = Anti-Spam
  Action on this mail = Quarantine message

  Warning message from administrator:
  Content filter has detected a sensitive e-mail.

The postmaster didn't respond to my request for an explanation, but
the message clearly says that my message was "quarantined" because it
contains "sensitive content".  This "sensitive" message happened to
be Mark Levine's analysis of the Supreme Court's Bush vs. Gore ruling.
I suppose the ruling itself could be considered obscene, but that's no
excuse.  This automatically generated bounce message also says "Policy
= Anti-Spam", but I don't know what ground it could have for regarding
my message as spam.  I happen to know the RRE subscriber at this site,
and he hasn't reported me as a spammer.

Aside from the obnoxiousness of content-filtering a person's incoming
mail, this sort of dumb filter is also a nuisance for the maintainers
of large mailing lists.  Similar problems arise from features that
automatically inform the message sender that the receiver has read
the message, and from dumb vacation programs and other half-witted
mail software.  Moreover, most of these messages don't provide me with
enough information to determine which user's mail is bouncing, and the
users themselves are rarely in a position to understand the problem.
I have 5000 people on my mailing list, so an automatic "smart" mail
program that is even a little bit stupid can be a continuing nuisance.
I suspect there's more where this came from.

**

I want to remark on a pattern in the history of computing: things that
start out artificially separate start to intertwine under the pressure
of real practice.  I have remarked on all of these cases separately,
but not the pattern.

My book about AI, "Computation and Human Experience", includes several
examples.  One of them is the distinction in AI between "planning"
and "execution".  The AI theory of action is that you make a plan and
then you execute it.  The planning-execution distinction is obviously
related to the distinction between mind and body in philosophy, and
also to the distinction between line and staff functions in industry.
In each case, practice has at least dented the walls, if not battered
them down.  It is hard to make plans in the real world because so
much is uncertain: you don't know where everything is, you don't
know precisely what the consequences of your actions will be, and you
certainly don't know what everyone else is going to do.  A substantial
degree of improvisation is intrinsic to life in a complicated world.

AI has been driven by this fact in three directions.  One direction
maintains the planning-execution distinction and confines itself to
highly controlled environments where the space of possible situations
that might arise is reasonably bounded.  If you only have a billion
possible situations to deal with, then you can get impressive results
with brute force and counterintuitive randomization techniques.  Some
real problems do fit this model, for the simple reason that industrial
environments have always been highly controlled for other reasons.

Another direction has been to jumble up planning and execution in what
are called "reactive planning" systems.  I don't find these approaches
terribly interesting philosophically, but I should note that some of
them are now being used in real applications.

The third direction has been to knock down the barrier between planning
and execution, and to make models of improvised activity.  This is the
approach that we took in our massive volume on "Computational Theories
of Interaction and Agency", and that we took in the design projects
in my book.  It also seems to me like the most important of the three
directions, because it is the approach that makes sense in the real
world of people's lives.  But it hasn't been the mainstream approach,
perhaps because of the inertia of the industrial way of thinking.
I think they'll come around, and Robert Johnston in Australia wrote
a fine dissertation explaining why.

The same pattern also happens with "cyberspace".  Longtimers on this
list have heard me rant endlessly about the reasons why cyberspace
is not a good way to think about the Internet.  Cyberspace is a whole
separate world, free from the constraints of ordinary, industrial-age
corporeal reality.  "Virtual reality" expresses the same basic idea.
In practice, however, this separation between the real world and
the digital world, between the atoms and the bits, hasn't been useful
and in most cases has been misleading and destructive.  Digital and
physical can be combined in many ways, and a complete separation
between them -- as for example in virtual reality -- is only one small
corner of a design space.  Augmented reality and ubiquitous computing
intertwine the electronics with the physical world, predicating the
functionality of the electronics on the patterns and meanings of the
embodied activities that people customarily undertake in the world.

Likewise, virtual communities -- virtual in the sense of all-virtual,
not-at-all face-to-face -- are only one corner of a huge design space.
Most communities use several media, not just the Internet, and most
communities use the Internet in several ways, not just in the confines
of a "virtual community" type of online discussion environment.  The
"virtual" side of the community is intertwined with the other sides.

Another example is found in the history of fashions in selling things
to consumers on the Web.  During the South Sea Bubble of 1998 and
1999, the received wisdom was that all-virtual companies, being wise
in the ways of the revolutionary new technology that was sweeping the
mightiest empires out of its path, would stomp on all of the pathetic
old "bricks and mortar" businesses.  Well, of course, that hasn't
happened.  The great majority of those magnificent new companies with
astronomical price-to-revenue ratios are tanking.  Despite my past
denunciations of Amazon.com's business plan I think that the current
Amazon-is-toast hype is overblown.  But Amazon.com is clearly the
exception.  The big fashion now, as you surely know, is "bricks and
clicks", or as they say on the radio, "bricks *and* clicks", as if
this were a startling new insight.

Of course, the new fashion is probably simplistic as well.  The point
is that the "bricks" side and the "clicks" side, once pitted against
one another as metaphysical opposites, are intertwining.  We've hardly
seen the beginning of their coevolution, and different sectors are
going to discover different complicated ways to fold electronics into
their ways of doing business.  And if we wake up from the opium-cloud
of hype for one minute we can realize that this intertwining of the
digital and the physical is nothing new.  Wal-Mart, after all, is a
seriously wired company.  From the start its business plan has been
predicted on real-time inventory tracking that avoids the need for a
layer of warehouses between factory and store.

So that's the pattern.  In each case you have two sides, one abstract
and one concrete, and in each case the two sides are compelled by the
pressures of practical reality to start intertwining.  In each case
there do exist special situations in which one can pretend that the
two sides are really different, but that's just one corner of the big
design space.  The origins of this abstract/concrete divide are clear
enough; they're as old as Western civilization, and no doubt other
civilizations as well.  One clear lineage dates back to Greek ideas
about mathematics as a separate, quasi-spirital realm, and to Plato's
closely related notion of a parallel realm of ideals accessible to
thought.  My point isn't exactly that all such divides are misguided.
I take no position here, for example, on the Christian distinction
between the spiritual realm and the world.  My point, rather, is
that Western culture, and especially the technological culture that
descends from the Greek veneration of math, habitually tries to split
the physical world from the world of mathematical and computational
abstractions, and that split is usually wrong.  And not just wrong
but destructive -- it causes people to think narrowly, design badly,
and invest unwisely.  It also causes people to disparage their bodies
and disrespect the physical world.  The news is that we live in the
physical world.  Always have, always will.  We have to start caring
about it.

**

Recommended: The article about redesigning the business card in the
January 2001 issue of Wired.  Those business card scenarios, such
as Marcus Gosling's outstanding pocket scanner/incinerator, finally
convinced me of the great commonplace of 2000, that industrial design 
is where the most interesting work in art is being done now.  Why is
that?  A designerly way to think about it is that designed objects,
because they imply a mass market, can be used in strange ways to imply
collective needs and desires that fine arts are not good at.  My way
of thinking about it, which is roughly the obverse idea in different
language, is that fine art is trapped in an institutional context --
the gallery, the critics, standing and looking at the art work -- that
is removed from people's lives.  Designed objects call up the complex
meanings that objects can take on when they are deeply embedded in the
routines of daily life.  I'm not much of an artist, and I have little
feeling for the "meaning" side of design.  I'm more concerned with the
"practical" side, in a broad sense -- how an object fits into patterns
of activity and community, and how it could fit differently.  Lots of
bad design is concerned solely with one side or the other.  But good
design, when it happens, is a revelation in terms of both meaning and
practice.  This can be true even when the design is really a study and
not intended to be manufacturable.  (I'm unclear, for example, how the
pocket incinerator keeps from frying the circuitry.  But never mind.)
All of the business card studies can be seen at <http://www.ideo.com/>.

**

Let me tell you a brief, heartwarming story about the Web.  You will
recall the draft paper about cell phones and architecture that I sent
out a few days ago.  Well, that paper claimed that theaters are sealed
against disruptions from the outside world.  In response, one reader
directed my attention to a movie theater in New York that is famous
for its subway noise.  She couldn't remember what it was called, but
she could remember roughly what intersection it was on.  The Angelika?
I asked her.  Yes, I think that's it, she said.  I was pleased enough
to know this small fact that I wanted to include a footnote about it
in my paper.  But how to be certain that it was really the Angelika
theater that suffers from noise from passing subways?  I could start
asking my friends in New York, but why start bothering people?  And
what if they didn't know?  I had a vague sense that the Angelika was
famous for its subway noise, but I could have been wrong.  At length I
had a brilliantly obvious idea.  I typed "angelika subway" into Google
and here was the second item that came up:

  Angelika Film Center - New York City

  ... not to mention regularly supplemented by the rumblings of
  the subway).  Nevertheless, the Angelika still gets its share of
  exclusive bookings, and the special ... 

  newyork.citysearch.com/E/V/NYCNY/0002/76/12/cs1.html - 29k - Cached

Okey-doke.

**

The art of public design.

I used to be a technical person -- I have a PhD in computer science
and all that -- but I stopped building things a long time ago.  I
still know a lot of my friends from my computer science days, but
others have fallen a way.  In one of my last conversations with him,
one of these friends from a previous reality informed me I was wasting
my life.  This is the sort of thing that computer people say to one
another.  He meant it ruefully, of course, but he also meant it as
a simple statement of fact.  The world for him is divided into two
basic activities: building things and idle talk.  Technology drives
history, and everything else is a waste.  Having moved myself out of
the "building things" category, he concluded quite logically that I
had decided to waste my life.

Nowadays my old friend is working in a famous media lab designing
inconsequential gadgets.  And me?  Am I wasting my life?  I don't
think so.  In fact I think he's wasting his.  He fritters his days
away on gadget-focused projects without an interesting vision of
how these gadgets might fit into people's lives.  The fallacy in his
reasoning is a narrow understanding of what it means to build things
-- or where things come from, their social construction.  Thomas Disch
wrote a book about science fiction whose title captures the point:
"The Dreams Our Stuff Is Made Of".  It's not a great book, but it's
a great title.  It points to an important fact: things congeal from
clouds of language -- from ideas about people and their lives.  Those
ideas are part of the design process just as much as the modularity
of the Java code.  If your ideas are bad then your systems will be
bad.  If your ideas are shallow then your systems will be shallow.
If your ideas are oblivious to the context of system use then your
systems won't be useable in context.  And that's what I do: I make
ideas that might congeal into systems.  It's public design, and it's
a good use of time.

What are the tenets of good public design?  I don't know that anybody
has written them down before.  Here is a first stab:

(1) Start with institutions: forces and structures in the social world
as it exists.  Your envisioned technology will change the world by
letting people do more of what they already want to do, in other words
by amplifying one or more of the existing forces.  So explain which
forces you have in mind, and what it would be like to amplify them.
Shop around for institutional ideas that are useful for this purpose.

(2) Show how the technology you envision intertwines with other things.
Free yourself from the assumption that technology is a separate sphere
unto itself.  Technology can't be your whole story; if it's 5% of your
story then you have the proportions right.  This will bother people
who need technology to be the bottom line.  Set those people straight.

(3) Don't try to read your story about the future off of the workings
of the technology.  Decentralized networks, for example, do not create
decentralized societies.  The opposite is more nearly the case: people
create technology according to an image they have in their heads.  If
people have crummy images in their heads, help them get better ones.

(4) Don't try to characterize the world system, or the current epoch
of history, or the five factors that define How We Live Now.  That's
a valid thing to do, but it's not public design.  Instead, gather
fragments of theory that seem to provide leverage in articulating
the dynamics of real cases, without the slightest attempt to put them
together into a grand architecture.

(5) Join the debate.  The goal of public design is not to get the
right answer in your head, or in some journal that 200 people might
ever read.  The goal is to change reality.  So get out there and
publicize the ideas.  Write magazine articles.  Start a big mailing
list.  Return reporters' phone calls.  Write in accessible language.
You're trying to have a material impact on the world by changing the
culture.  Not the mass culture, perhaps, but the culture of the wired
people who shape technological agendas in research and industry.

(6) Learn about standards dynamics.  It will only become real in
people's lives if it becomes a standard, and standards come about
in strange ways.  Get in the habit of thinking "we need a standard
for that" and then imagining what the missing standard might be like,
both technically and politically.  Is it a standard that requires
a critical mass of adoptees before anyone will find it worth the
trouble of adopting?  If so then you'll have to design the social
process by which that critical mass will come about.

(7) Put information technology in the context of intellectual history.
Computers are nothing but ideas made into machinery, and so you can't
understand where the computers are coming from unless you know about
the history of ideas.  Yesterday's ideas run our lives until we become
aware of them.

(8) Transcend the fight between the enthusiasts and the skeptics,
between the people who predict radical discontinuities and the people
who say that there's nothing new in the world.  They're both wrong.

(9) Liberate yourself from this historical myth: that technology
is at war with institutions, that technology drives history, that
institutions hold this technologically driven future back, that
institutions should therefore be destroyed, and that technology
is the best instrument for doing so.  This myth grips libertarians
and Marxists equally, and every element of it is a dangerous half-
truth.  Your public design work will be bad until you get past it.

(10) Let go of wanting someone to implement your ideas exactly as
you've envisioned them unless you plan to raise the money yourself.
Recognize that public design -- like any gadget demo -- is part of
a process of public discussion.  Your ideas go into the mix, and
the people who build new machines will grab bits and pieces of ideas
from different sources.

To illustrate what I mean by public design, let me use the example of
my paper about the nature of intellectual life and its consequences
for digital libraries.  I have a formula for writing these papers.
I go shopping for ideas that feel like levers.  These turn out largely
to be ideas about institutions.  Then I ask myself, what would happen
if we used information technology to amplify particular features of
these institutions?

In the case of the paper on intellectual life, I asked (among other
things) what would happen if we took the institutions of peer review
and generalized them to apply to everyone -- how it would work and
what kinds of technical and social innovations it would take.  I don't
claim to know the answer to this question.  I just think it's a great
question.

And it's a question that leads directly to fantasies about gear.
One could imagine building peer-review systems for contexts other
than academia, for example the people who maintain a certain kind
of equipment.  Questions immediately arise: what if those people
don't want to write papers?  Well, then maybe they make informal
videos, or maybe someone interviews them remotely, or maybe they
give a presentation remotely to their peers, which then gets captured.
In fact experiments like this have been done at Xerox and elsewhere.
But their design has a long way to go.  I want to help by explaining
more fully what these sorts of systems might accomplish, and what
their social prerequisites are.  I want to stir up imagination about
the matter, for example by describing the phenomena in ways that
people can understand from their own experience.  This is the cloud
of language from which things congeal.

The problem with gadgets is that they congeal from very small clouds
that are disconnected from broader and more useful ways of talking
about people and their lives.  The stories that their inventors
tell about them are usually impoverished.  They usually don't have
interesting things to say about people and their lives.  They tend to
make very flat, very broad generalizations about people.  By telling
better stories about people -- stories that are grounded in serious
ideas -- I hope to encourage the gadgeteers to iterate their designs.
Design works best when it gets robust feedback.  Critics provide one
kind of feedback, but public design is more positive.  Criticism by
definition is reactive, but positive design can articulate entirely
new areas of life that design might address.

**

The downsides of learning in a changing world.

Would-be revolutionaries routinely find that the world doesn't want
to change, and this pisses them off.  The dumb ones spin conspiracy
theories to explain the problem, and the smart ones spin institutional
theories.  Once you start spinning institutional theories, it becomes
a wonder that the world can change at all, so many are the dynamics
that try to keep the world just the way that it is.  One of these
dynamics might go by the name "hazards of induction".  Induction is
a kind of learning, and in some sense it's a property of all learning.
Induction is what happens when you notice a pattern in your experience
and develop a habit of action accordingly.  The pattern you notice can
be anything: you might notice that store-bought apples are tasteless,
that men want to solve problems while women want to talk about them,
that members of a certain ethnic group are angry or poor, that all new
initiatives get stifled by politics, that people misunderstand your
ideas in a certain way, or whatever.

The important thing about induction is that you don't know what the
pattern depends on.  "That's just the way it is", you say, and even
if you don't say it you still tend to assume that the pattern is
permanently and universally true.  The assumption is dangerous, of
course, because the world can change.  But if you don't know what
the pattern depends on, then you have no idea what changes to look
out for.  So when the world does change, you can get hurt.  What's
worse, if you assume that the pattern is permanently true, then you
might play your part in making it into a self-fulfilling prophecy.

The examples that I chose illustrate some of the stakes.  Many people
have noticed patterns, such as flavorless apples in supermarkets, that
result from market failures.  Different market institutions might lead
to better apples (and tomatoes, corn, etc), and if more people were
aware of the possibility then those alternative institutions might be
more feasible.  Many of the patterns are ethnic stereotypes that have
a basis in very narrow and unfortunate kinds of truth: not in the real
essence of the people, but in the conditions they've been forced into,
and in patterned interactions with members of one's own group.  Some
of the patterns result from transient configurations of technology and
industry structure.  Think of AT&T, which is dying a slow, ugly death
because so many patterns that held true in the voice-telephone world
no longer hold.  The habits of thought, action, design, organization,
and everything else that got ingrained during the Golden Age of the
telephone are still there, still driving the culture of the company.
Some of the patterns are just mysterious: are the differences between
men's and women's conversational styles real, or are they stereotypes,
or do they result from cultural socialization, or do we selectively
notice things about one another that only seem like patterns, or what?

Every noticed pattern, and every acquired habit, is learning.  It is
partly learning-by-doing, and it is partly learning-by-acculturation.
It's really the culture that learns such things, and that reproduces
them as well.  Now, learning is generally regarded as a good thing.
In fact it is the number one political issue that Americans enumerate
in polls.  The technologies and institutions of learning are central
topics of public discourse.  Companies go to great lengths to become
"learning organizations", and to capture and leverage as much learning
as possible from their dealings with products and clients.  Learning
is a kind of capital and an important kind: learning-by-doing exhibits 
positive returns to scale, meaning that the companies that get the
chance to learn by doing thereby obtain a competitive advantage that
provide them with more opportunities to learn by doing, thus setting
up a positive feedback loop.  Business historians make clear that
the real impact of new technologies is not felt until organizations
learn how to use them.  And past some point it's trial-and-error: you
try things until you inductively see what works, and then you do that.
A company's plant and equipment might be worth almost nothing, but its
inductive, practical organizational learning might be worth billions.

But it's complicated.  If the world changes then a vast background of
unarticulated assumptions can go bad, and those billions of dollars'
worth of learning can suddenly and insidiously depreciate.  The net
value of AT&T's learning may even be negative.  The regional phone
companies are still doing fine, but that's because the world hasn't
changed for them.  They're still monopolies, and their core competence
-- namely lobbying -- is still as valuable to them as it ever was.
But the long-distance companies' learning has gone south, and a whole
world of thought-patterns, a whole sense of scale and pace, and a whole
world of architectural assumptions and biases have all gone with it.
Everything is suddenly wrong: make-or-buy decisions, engineering values,
understandings of who the customers and competition are, you name it.
And it's not just the dinosaurs at AT&T.  A whole generation learned
how to do business during the Internet stock bubble; they were gods
for about five minutes, and now they're going back to get their MBA's.

How can we organize knowledge and learning to avoid this obsolescence?
It's a world of long-term profound change out there, and we don't want
learning to become less valuable.  The problem, obviously, is that
not enough assumptions are being articulated.  We need a culture of
articulating the background of reasons, assumptions, and premises
behind our thoughts and actions.  It's impossible to articulate this
background completely, and nobody is more delusional than the systems
rationalists who think they can.  But for the same reason it's always
possible to articulate more fully the reasons for the inductive patterns
one sees.  We need more vocabulary for these reasons, and we especially
need more vocabulary about the interactions between institutions and
technology.  This articulating of deeper reasons is a purpose of liberal
education, and it's also the reason why we should teach generalized
process and design skills in engineering.  We need conceptual frameworks
and analytical disciplines.  We need ideas.  And that's what we have
here: a business case for ideas.

Here is another way to think about it.  Institutions exist largely
to solve information problems.  If we had infinite communication and
computation capabilities then we could coordination our activities
from moment to moment through gigantically complicated negotiations.
But our communication and computation capabilities are finite, so
we have conventions and rules and belief systems that partition life
into manageable enough pieces that we can all focus on what we're good
at.  With radical improvements in information technology, it stands
to reason that institutions will change.  But institutional change is
very hard to understand.  Institutions define us.  We are socialized
into their practices.  We take them for granted.  Institutions provide
us with our identities and  our ways of understanding ourselves and
the world.  They define a landscape of opportunities and dangers on
every scale from interactional to global.  And upon that landscape
there evolves a vast web of strategies that people bet their lives on. 

This is particularly true in the first world, in countries like my
own, where institutions work relatively well and infrastructures
are maintained to support them.  Institutions and infrastructures
shape our lives while remaining largely out of sight.  We inductively
learn that the world works in a certain way, but we don't understand
how much complicated effort goes into producing and reproducing the
institutions and infrastructures that *enable* the world to work
that way.  The result might be called first-world myopia.  People
in the first world live in a dream.  We think that we determine our
own fates, that we are free and autonomous individuals, when in fact
we live in bubbles whose preconditions would scare us if we knew
just how numerous they are.  If there's a rock in the road, we just
assume that it's someone's job to pick it up.  The supermarket will
have food in it.  Airplanes fly.  You can get parts for your car.

Contrast this first-world myopia to the situation in a country like
Brazil where the institutions don't work as well.  The Brazilians'
whole consciousness is completely different.  They have an elaborate
cultural sense that daily life is a matter of improvisation.  Things
are getting better in Brazil, especially in Sao Paulo, which except
for the dreadful city government might as well be New York.  But they
still feel culturally that they know how to keep things moving even
when the institutions and infrastructures break down.  In a sense it's
a more conscious way of life.  First-world myopia means that you can
forget, or never even know, about the elaborate institutional systems
that make it possible to live in a bubble.  Then when an institution
does fail, for example if you are a victim of identity theft and the
credit reporting agencies and cops aren't interested in helping you,
then you are clueless, stranded, completely on your own.  It's not
something that first-world culture understands.

This is not a problem in Brazil.  Everyone in Brazail is painfully
aware of the vast institutional background that makes their lives
possible, precisely because that background keeps breaking.  And it's
not just individuals who possess this knowledge but the culture as
a whole.  The culture as a whole knows what to do when things break.
This knowledge flows freely through social networks, and people
maintain social networks precisely to stay alive when the institutions
break.  Who, then, is better prepared for the institutional upheavals
of the wired world?  The Brazilians, of course.  They know what it's
like to have the institutional ground shift under their feet.  Banking
revolutionized?  Universities upended?  Government imploded?  Industry
structure turned inside-out by fluctuating global commodity prices?
No problem.  Brazilians know what to do about that.  It's a great
country.

First-world myopia, by contrast, can be downright dangerous.  Think of
all those "experts" who flew to Russia in 1989 to advise the Russians
about how to create a market democracy.  Those people were dangerous
fools.  They had no idea what life was like in a society without
functioning institutions.  They really believed all this drivel about
the free market meaning an absence of government.  Here on Planet
Earth, markets require a vast network of institutions both public and
private, including a functioning legal system, autonomous professions,
and a culture that knows what a contract is.  In Russia, by contrast,
you had a culture that was so accustomed to dysfunctional institutions
that children grew up learning that survival required the skills of a
criminal.

It's not that the Russians aren't decent people.  Most of them are.
It's that the institutions of the Soviet era were so illegitimate that
decent people had no moral responsibility to pay the slightest heed to
their rules, and so dysfunctional that people couldn't have followed
the rules if they tried.  It's hard to build new institutions because
you can't just buy them or make them in a factory.  Institutions don't
just exist on paper; they also exist in people's minds and in a stock
of skills that people have come to rely upon in living their lives.
Banking, for example, is only about 20% a matter of things that happen
within the organizational confines of banks.  A society only has an
institution of banking if borrowers, lenders, regulators, and other
relevant parties -- i.e., everyone -- *believes* in banks, knows how
to use banks, and thinks they can get something by cooperating with
banks.  In a society with functioning institutions, everyone inductively
embodies many layers of these beliefs, skills, and strategies.  And
the institution persists largely because most people have forgotten,
or never realized, or can't imagine, that it could be any different.

That is the paradox for a world of radically changing information
technology.  There do exist alternative worlds in which information
technology is radically better than the technology we have now, and
in which our institutions are radically better too.  But it doesn't
follow that a path exists from here to there.  Our legacy institutions
set the ground rules for our lives, including the processes by which
we might move to new institutions.  The first step, it seems to me,
is to defamiliarize the institutions we have now, and to become more
like the Brazilians -- not in the sense that we embrace dysfunctional
institutions, but in the sense that we become conscious of the whole
institutional background that makes our lives possible.

**

The amplification model explained.

I often find myself caught in the middle of a recurring conversation:

  A: New technology will bring radical, total, discontinuous change.

  B: Oh come on, there's nothing here that's fundamentally new.

That's the whole conversation.  It pretty much ends right there, since
there's noplace for it to go.  Underneath any chronic intellectual
conflict you're likely to find basic commonality.  In this case, each
side agrees on something fundamental: that change is all-or-nothing.
Language, I must admit, abets this habit of thought by organizing
itself around binary contrasts that reduce to digital terms the analog
complexity of the real world.  But language doesn't condemn us to such
superficial thinking permanently, and long traditions of advanced use
of language provide us with better ways of talking about these things.

To get beyond the impasse between "discontinuous change" and "nothing
new", we need the amplification model.  The amplification model works
like this: use structural analysis to describe society as it already
is, pick a force that's already found to be at work, and ask whether
and how information technology will be used to amplify it.  If you
think that technology drives the world then you don't care about these
existing forces.  But if you think that *people* drive the world then
you will be curious about how people think, what they are already good
at doing, what their interests are, what strategies they know, what
opportunities they see, and so on.  If information technology helps
people to do more of what they already want to do, then they will be
sure to use it.  And that's how information technology changes the
world: it turns up some of the knobs that are already there.  As the
technology gets more powerful, the knobs get turned up higher.  After
a while, the existing balance of forces will be thrown so completely
out of whack that the existing structures of society will change,
whether gracefully or catastrophically.  Structures that are currently
marginal might become dominant as the currently dominant structures
shrink, or the whole shmear might blow up, to be replaced by something
completely different.  We don't know, and we won't know until we learn
how take the existing world more seriously and put the technology in
its place.

Here is an example.  People who study the role of the Internet in the
political process are often chagrined to learn that the people who use
the Internet to engage in politics are the same people who had already
been heavily involved in politics.  This result is often taken to be
(a) surprising, and (b) confirmation of the "nothing new" alternative
that refutes the prevailing "discontinuous change" hypothesis.  But
if you think about it for one second, you'll see that this "surprising"
result is completely obvious.  *Of course* it's the political junkies
who are drilling into esoteric political information on the Internet.
Why would someone who had been apathetic about politics suddenly become 
fascinated by political information, just because that information is
on the Internet?  In this case the "discontinuous change" hypothesis
is driven by the civic myth that democracy is healthy when everyone
consumes huge amounts of political information, so that the Internet-
strengthens-democracy thesis requires normal people to spend hours
drilling into political Web sites.  The civic myth is too simple,
and the civic myth's predictions for the Internet are *way* too simple.
The Internet is changing politics in many ways, but each of these ways
involves amplifying a mechanism that was already there.

The amplification model builds on a lengthy if little-known tradition
of institutional analysis of computing.  Its consequences are many.
That the people who do politics on the Internet are the same ones who
already do politics should be the *starting* point for analysis, not
its endpoint.  The amplification model is a contingency model: it says
that the Internet's "impact" in a given institutional context depends
heavily on facts that lie outside the Internet.  In other words, you
can't understand this "impact" until you know how the world already
works.  Once you see this, you will stop asking, for example, whether
the Internet centralizes or decentralize the world.  The prevailing
dogma is that the decentralized Internet also decentralizes the
world.  This is ridiculous.  There are forces in both directions,
toward centralization and away from it, and both forces are amplified.
You have to analyze the clash of forces in every case.  This kind
of answer doesn't fit in a soundbite, but it's the truth.  Or, more
accurately, it's a truer question.

**

I read the other day that the Los Angeles public schools have students
who speak 140 different languages.  Isn't that terrible?  Think about
it: there are 7000 languages in the world, and we only have 2% of them!
Is this America or what?  Surely we can get that number up to 5% if we
work at it.

**

Reading the newspaper about the latest computer security or privacy
outrage, one tends to miss the fundamentals of the problem: the poor
architectural design that is endemic in the computers that most real
people use.  Microsoft's practice of putting fully general executable
code in every nook and cranny of their products is an example, but
so is the absence of firewalls in most operating systems, which still
live in the Jurassic Park before work patterns started to revolve
around the Internet.  The problem is hard because we're stuck with an
installed base that works the wrong way.  What I can't recall anyone
writing about is the shape of the wrenching transformation that will
be required to set things right.  The "wrenching transformation" -- a
phrase from Al Gore's book -- is, of course, an analogy to the problem
of environmental pollution.  I don't want to be a polluter, but I
live in Los Angeles and so I can't avoid driving a car.  We have
an infrastructure here that tends to consume itself with pollution.
The problem can be solved with new auto engines and other technical
changes, so we probably don't have to raze the city and start over.
But given the infrastructure that keeps auto engines running, moving
to new engine technologies is a wrenching transformation in itself, as
the ignominious failure of electric cars thus far helps to illustrate.

It's the same with operating systems.  Where is the path from point A,
with its endless privacy and security crises, to point B, with decent
engineering taken for granted?  We don't even know what point B would
be like -- we don't have any widely accepted trust models for sharing
code in distributed computing, for example.  The problem is not wildly
different from the problem faced by old timesharing systems, but it is
different nonetheless.  Old timesharing systems could not be attacked
remotely by millions of people.  I applaud the efforts of people like
Richard Smith who go around poking holes in the systems we have now.
The next step, it seems to me, is spelling out the change agenda for
the transformation to the systems we should have instead.

**

People have been sending me pens.  Lemme tell you, you have not lived
until you have written with a Stabilo 's move elastic writer.  It's
impossible to describe, but on this Web page it's the one that looks
like a concave basketball:

  http://www.stabilo.com/stabilo.com/english/html/products/writing/write0.htm

Aside from being really weird-looking, it is the slipperiest pen ever
made.  It produces so little friction against the page that I still
can't write neatly with it.  Just get one.  I'm told that the 's move
powerball is also a trippy experience, but I haven't tried it yet.

The same reader (in Norway) sent me a Pilot Hi-Tecpoint V-2000 Extra
Fine (0.5mm) liquid-ink needle-point pen.  It's a bigger, more robust
version of the much-sought Pilot Hi-Tec-C.  Like the Hi-Tec-C it's
for people who write with a light touch.  The line is a little thin
for my taste, but probably not for precision freaks.  It has the best
rubber grip I've ever seen.

You know what's a darn good pen?  The "Colors" liquid-ink rolling ball
pens that they sell at Kinko's photocopy shops.  They're ugly as heck
with the Kinko's logo on them, but they're similar in philosophy to
the Reynolds Ink Ball, the Rotring Xonox Rollerball F, and the Micro
TANK-Pen.

A reader in Japan sent me a bunch of pens, including two copies of
that ultimate expression of contemporary Japanese culture, the Hello
Kitty gel pen.  They're not what you'd expect.  They're about seven
inches long, quite heavy, clear plastic, slightly textured grip, with
half-inch statues of Hello Kitty on the cap.  One of them actually has
a problem delivering ink consistently, but the other one works great.
You could never take these things to work.  Even the ink is not what
you'd expect, a kind of metallic off-greyish-blue that looks stranger
on the page than it does in the pen.  They each have decals with lots
of cool Japanese script that I can't read, plus (on one of them) the
English text "FOR SALE IN JAPAN ONLY".  Yeah.

**

An RRE reader writes:

  Here's an interesting experiment in line with odd visuals off
  computer monitors: stand some distance away from the front of
  your monitor (10-15 feet) and bite into something crunchy, like
  a pretzel or potato chips: your monitor's "display" will behave
  oddly.

Try at your own risk.

**

In response to my encomium to the LA Times' distribution system, a
couple of readers mentioned the (much smaller, but in its own way more
impressive) lunch delivery system in Mumbai (aka Bombay).  One said:

  Feh!  Bah!  Smell my socks!  You should check out the lunch-box
  distribution system in Bombay/Mumbai: from 175,000 housewives to
  their husbands/sons, routed by 5000 underpaid toilers.

  http://www.forbes.com/global/1998/0810/0109078a.html

  This system is shrinking tho, as more women work and with more fast
  food joints opening.

  http://www.csupomona.edu/~gurey/urp475/dabbawallah.htm

  The coding system used for the routing of the boxes thru the
  "switching" system was quite intricate and cryptic; doesn't seem to
  be anything online about it.  Pity.

There you go.

**

A certain small dilemma recurs at least once a day in running this
list: someone sends me a useful URL that I already have.  Should I:
(a) say "I've already got it, thanks"; (b) say "great thanks", as
if I hadn't seen it before; (c) say just plain "thanks"; (d) ignore
it; or (e) what?  If I pick (a) then it sounds like a rebuke and
the people tend to apologize for no reason.  But (b) feels dishonest,
because I don't feel the small spark of joy that I normally feel when
someone sends me a useful URL that I haven't seen before.  I don't
want to be lying to people.  I end up doing (c) a lot, but it doesn't
feel right either, since I do want to acknowledge when someone sends
me a useful URL.  I couldn't do (d) if I wanted to.  It's not a huge
issue, obviously.  In fact it's a microscopic issue.  But part of
the point of this list is to explore the properties of the medium,
and noticing this microscopic issue is part of that ongoing project.

**

Some URL's.

election

GOP's Depth Outdid Gore's Team in Florida
http://www.nytimes.com/2000/12/22/politics/22FLOR.html?pagewanted=all

Supreme Court Ruling: Right or Wrong?
http://www.latimes.com/print/asection/20001221/t000121670.html

The Five Worst Republican Outrages
http://www.villagevoice.com/issues/0051/barrett.shtml

civil liberties

ACLU challenge to library filtering law
http://www.aclu.org/news/2000/n121800a.html

INS Must Stop Using Secret Evidence
http://www.latimes.com/print/editorials/20001221/t000121539.html

Wireless Telematics Systems: Driver Distraction and Location Privacy Issues
http://www.thelenreid.com/articles/article/art77_idx.htm

Slippery Road Ahead for Wireless Location Apps
http://www.computerworld.com/cwi/story/0,1199,NAV65-663_STO51710,00.html?s

insurance company experiment (now ended) with GPS tracking of cars
http://www1.progressive.com/media_relations/Autograph.htm

Children's Internet Protection Act
http://www.epic.org/free_speech/censorware/cipa.pdf

new US medical privacy rules
http://www.hhs.gov/news/press/2000pres/20001220.html

intellectual property

Enter the "Stupid Patent Tricks" Contest
http://slashdot.org/features/00/10/08/0419212.shtml

Stealth Plan Puts Copy Protection into Every Hard Drive
http://www.theregister.co.uk/content/2/15620.html

Content Protection System Architecture
http://www.dvdcca.org/4centity/data/tech/cpsa/cpsa081.pdf

everything else

Itoya Etona staplers
http://www.itoya.com/stapler.html

Junk Science, Corporate Ideology, and Genetically Modified Food
http://monkeyfist.com/articles/731/plain/

Glaser Family Foundation
http://www.progressproject.org/foundation.html

Legal Information for Internet Professionals
http://www.gigalaw.com/

Here's to the Decline of an Evil Giant
http://www.latimes.com/print/techtimes/20001221/t000121752.html

arguments supporting Microsoft appeal
http://www.stern.nyu.edu/networks/2000-09abs.html

The Public Voice in Emerging Market Economies, Dubai, January 2001
http://www.thepublicvoice.org/events/dubai01/

end
```