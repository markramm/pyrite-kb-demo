---
id: writing-and-representation
title: "Writing and Representation"
type: writing
writing_type: paper
date: 1988-05-17
url: "https://pages.gseis.ucla.edu/faculty/agre/ni.html"
coauthors: []
key_concepts: []
importance: 5
research_status: stub
tags:
  - paper
  - auto-imported
---

## Source

Automatically imported from: https://pages.gseis.ucla.edu/faculty/agre/ni.html

## Content

### Writing and Representation

#### Philip E. Agre Department of Information Studies University of California, Los Angeles Los Angeles, California 90095-1520 USA pagre@ucla.edu [http://polaris.gseis.ucla.edu/pagre/](https://web.archive.org/web/20200210084530/http://polaris.gseis.ucla.edu/pagre/) This is a chapter in Michael Mateas and Phoebe Sengers, eds, *Narrative Intelligence*, Amsterdam: John Benjamins, 2003. Please do not quote from this version, which probably differs in small ways from the version that appears in print. 8300 words.

[Author's note: This is a heavily abridged and revised version of a paper
that I circulated informally in 1989. I have not tried to bring it up
to date. Some parts of the argument are developed further in (Agre 1997).
Another subsequent work that treats these issues is (Hutchins 1995).]

**Introduction** 

The notion of representation obviously labors under a long philosophical
history (Judovitz 1988, Rorty 1979, Silvers 1989), not to mention the history
of art (Hagen 1986, Wallis 1984), literature (Auerbach 1953, Brodsky 1987,
Krieger 1987), and historiography (Hartog 1988, White 1973). These days,
though, it also labors under an appreciable technical history, handed down
through a practice of building computer systems that construct, maintain,
and manipulate "representations" (Brachman and Levesque 1985, Haugeland
1981). And the philosophical and computational issues interact. I often find
that philosophy helps to interpret the difficulties that arise in my technical
practice. And I want to believe that technical practice can help philosophy.
In writing the stories that follow, I have explored some places where
technical questions align with philosophical answers. I don't yet know how to
convert these answers back into technical practice.

I disagree with two widespread ideas about representation, namely "semantics"
and "world models". The main tradition of semantics holds -- presupposes
-- that a representation has a "meaning" or a "content" independent of the
identity, location, attitudes, or activities of any particular agent (but
cf. Barwise and Perry 1983). This meaning or content is often understood as
a systematic, objective relationship between the representation itself and
states of affairs obtaining in the world. A world model is a component of a
physically realized computational system, an object whose internal structure
stands in a systematic, objective, analogical relationship to states of
affairs presumed to obtain in the world. Some computational process maintains
the model as the world changes; reasoning about the world involves inspecting
and manipulating the model. I will argue that both semantics and world models
overlook central features of representations and their use.

On the positive side, I offer two suggestions about how people use
symbolic representations. The first is that *people interpret symbolic
representations in making sense of particular situations*. Interpretation
is a situated activity.

(Whatever the form of the representation, whether written or spoken or
displayed on a video monitor, I shall speak of its configuration of symbols
as a "text". The "representation" is the actual material object: the sheet of
paper, the speech signal, or the video image.)

My second suggestion is that *what a given text is talking about is a fresh
problem in every next setting* (Amerine and Bilmes 1988, Zimmerman 1970).
The work of relating a text to a concrete setting -- looking around, poking
into things, trying out alternative interpretations, watching someone else,
getting help -- will generally be both "mental" and "physical", though it is
best not to distinguish. Relating a text to a concrete setting takes work
because the text might be relevant to the situation in a great variety of
ways. The text has a great deal of "play", so that much of one's interpretive
effort must wait until the time comes. This is the opposite of extracting
a "meaning" from a text as soon as it arrives. The point is not that
interpretation is wholly unconstrained by the text; rather, interpretation
is constrained jointly by the text and by the circumstances in which it is
interpreted. The only way to explain the point is through examples.

(1) I'm trying to find a friend's house in a heavily wooded mountainous rural
area. I had received directions to the house by e-mail and printed them out
so I could carry them in the car. I knew the main road, but I knew nothing
about the residential streets leaving it. The last two paragraphs read:

> About a mile up from the intersection, look on the left for Elk Tree
> Road -- it's a dirt road with a little bus stop at the end. Follow
> Elk Tree *past* the first left (Elk Tree WAY) to the mailboxes and
> take the middle of the three-way fork on the right, Upper Elk Tree
> ROAD.
>
> My place is the first one on the left, #27. Park on the left
> shoulder near my red Honda, and come down the steps and up the
> stairs to my front deck. (If you went to the main door, you'd get
> my landlords, not me.)

I had the sense to check my odometer at the intersection so I'd know when
"about a mile up" was coming. Even so I somehow missed Elk Tree Road the
first time. The bus stop is obvious enough if you know where to look for
it, but it's a little way up the dirt road and obscured by foliage. The
most difficult part, though, concerned the "three-way fork on the right".
When I got to the mailboxes (dozens of them, in fact) I had to find some way
to interpret the scenery as "the three-way fork on the right". Unfortunately,
I could only count two roads on the right. After much backing up and looking
around, I decided that a large driveway roughly straight ahead was the third
road. Setting off along the "middle" road, I looked for the first place
on the left. The road snaked down a hillside with many houses on the right.
Finally I came to a house on the left. I couldn't find any street numbers
(no surprise out here) but there was definitely a red Honda parked outside.
I parked, got out, looked for the place that "come down the steps and up the
stairs to my front deck" was talking about. I found such a place but it led
me to the side door of a cluttered garage. A great deal of searching and
asking around followed. Even though something was clearly wrong, that red
Honda made me reticent to abandon any of my previous interpretations.

To make a long story short, the middle branch of the three-way fork
immediately branched into Lower Elk Tree Road steeply down to the left and
Upper Elk Tree Road steeply up on the right. A large hand-painted sign for
Upper Elk Tree Road clearly marks the split, but I was already looking for the
first place on the left. Writing this now, I realize that it makes perfect
sense for *Lower* Elk Tree Road to branch steeply down and *Upper*
Elk Tree Road to branch steeply up, but at the time I didn't give the right
branch any thought at all since I simply did not see the branch *as*
a branch. If you're standing there looking at the branch *as* a branch
then it's hard to imagine how it looked to me, but it never occurred to me
that I had another choice of roads to make. The sign must have occupied a
reasonable portion of my visual field, but I was already looking for a house,
not a sign, and to the left, not the right. In short, I saw what I assumed
the instructions were telling me to see. Told about a "three-way fork
to the right" and unable immediately to see such a thing in that place, I
*worked*, successfully, to see it. Told about "the first [place] on
the left", I unquestioningly saw what the instructions implicitly told me was
there, namely the road on which my friend's house was located.

(2) A friend recently taught me to fold origami paper cranes. In walking
me through the various steps, she often had to explain by some combination
of words, pointing, and demonstrations where and how to fold next. The
intermediate forms don't look much like cranes, and the paper keeps taking on
unexpected new identities as you fold it, even after you've gotten reasonably
proficient. These forms can be hard to talk about because they're importantly
asymmetrical in nonobvious ways. Even demonstrations are only of limited use
if you can't see the asymmetries for yourself.

In the course of her explanations my friend said things like "put your finger
in the pocket", "fold it back to make a boat", and "make the legs skinnier".
Making each of these metaphors refer to parts and aspects of the folded paper
always took considerable effort, even though it was always wholly evident in
retrospect. Much of my friend's job was to get me to look at my partly-folded
origami crane in the right way, so that certain parts and aspects would stand
out as units for me. She was teaching me the skill of seeing my paper
*as* having a pocket, a boat, or legs. Although I got better at this
skill, it never stopped taking work. The work only became more routine.

(3) The final example comes from my experience teaching people to program
computers. If you're comfortable in front of a computer terminal, it's
easy to teach the wrong things. You've got all kinds of theory, but theory
doesn't help someone who hasn't yet gotten the idea of being "in" the editor.
So I sit the student at the keyboard and tell them very concretely what to
look at and what to type. As they get comfortable, my instructions grow more
abstract. For example, I might say "Type open paren then ...", only to see
them type the letters "o p e n" and "p a r e n". In that case I have to point
out where the parenthesis keys are. Later, though, I can say things like,
"Let's define a function called ...". When they're learning to read code,
I have to point out that there are conventions about indentation that result
in common types of code having characteristic shapes. And I don't explain
abstraction hierarchies until I explain that two hunks of code that look alike
are often good candidates for a common abstraction.

As these examples illustrate, my prototype of representation is natural
language, whether as spoken utterances, written texts, or mental thoughts.
In each case, figuring out what in the situation the text was talking about
took work: creative improvisation, reference to artifacts, and interactions
with others. The work consisted in relating natural language to concrete
situations: identifying the things the words were mentioning, seeing materials
under metaphorical descriptions, and heuristically associating visual patterns
with verbalized technical abstractions. And the work required to make sense
of "take the middle of the three-way fork" or "put your finger in the pocket"
or "define a function" might differ greatly in different settings or under
different conditions.

I want to concentrate on representations written on paper. The image of
standing in a kitchen or on a street with a written text in your hand is a
good reminder that relating texts to circumstances requires work and that
this work requires understanding in some measure what you're doing. You have
to understand what you're doing since the text certainly doesn't (cf. Searle
1981). Obviously representations often influence your actions, but you
don't understand what you're doing in virtue of owning them. This point is
supposed to apply equally to all forms of representation, not just writing.
The idea that understanding does not reside in representations is difficult
and consequential. The paper's later stories will explore this idea in the
context of "internal language".

Five fairly independent notes follow.

*The homunculus and the orbiculus* is an assault on the notion of a world
model, placing it in a philosophical tradition of trying to explain the human
ability to act competently in the world by pretending that the relationship
between person and world is reproduced inside the person's head. This sort of
explanation is seductive because it plays to the principal strength of current
computational technology: building abstractions inside of computers that are
almost entirely cut off from the outside world. But it doesn't work well in
practice.

*Writing as bad and good metaphor for representation* contrasts two ways
in which written texts might be regarded as prototypes of representation.
The first, "bad" way focuses (however tacitly) on certain physical properties
of written texts. This bad understanding of writing is central to the main
tradition of computing. The second, "good", way concentrates on more abstract
aspects of written texts: both the text and your surroundings are outside of
you, and so it takes work to see the world as being what the text is talking
about.

*A story about photocopier supplies* also concerns written instructions.
A secretary is justifiably annoyed because somebody has put laser-printer dry
toner in the photocopier. What happened and why? At issue is the selective
use people must make of the representational materials that surround them.
I defend the culprit, arguing that the phrase "dry toner" on a bottle is
not "ambiguous" in a way that anybody could be expected to notice, even if
evidence serving to identify and resolve the ambiguity is readily available.
One would like photocopier users to be "careful", but it's hard to formulate
the demand in an actionable way, given that such a problem could hide behind
any of the vast number of unarticulated assumptions that form the background
of any such activity.

*A story about some instructions at a performance in an art gallery* is
another story about instructions, this time a single sentence that one person
hollered to a group of others. These instructions did not function well
because the recipients could not see, or even imagine, what in the setting
the instructions could be talking about.

*A story about my routines for reading the Sunday Globe* is a story about
an instruction I issued to myself in the course of reading the newspaper one
Sunday morning. The pattern of activity in which the instruction participated
had long since become routine. Nonetheless, the way in which the instruction
went wrong reveals that it was something like an natural language imperative
and not, for example, a computer program. In this case, a change in the
environment led me to make a different sense of an ambiguous phrase than I
used to.

The stories are not supposed to prove any general propositions. Instead,
they invite you to be aware of similar phenomena in your own experience
of everyday representation-use. Computational investigations and awareness
of everyday life can influence one another. Parallel pursuit of these two
kinds of inquiry will, I believe, lead to deeper understandings of why our
life is the way it is and why machines can take certain forms and not others.

**The homunculus and the orbiculus** 

In the old days, philosophers accused one another of believing in
someone called a *homunculus* -- from Latin, roughly "little person".
For example, one philosopher's account of perception might involve the
mental construction of an entity that "resembled" the thing-perceived.
Another philosopher would object that this entity did nothing to explain
perception since it required a mental person, the homunculus, to look at
it. Computational ideas appeal to these philosophers because they can imagine
"discharging" the homunculus by, for example, decomposing it into a hierarchy
of ever-dumber subsystems (Dennett 1978: 124).

But the argument about homunculi distracts from a deeper issue. If the
homunculus repeats in miniature certain acts of its host, where does it
conduct these acts? The little person lives in a little world -- the host's
surroundings reconstructed in his or her head. This little world deserves a
Latin word of its own. Let us call it the *orbiculus*. One way to say
"world" is *orbis terrarum*, roughly "earthly sphere". But *orbis*,
I am told, extends metaphorically in the same ways as "world" in English: one
might speak of the world of a peasant or a movie director, meaning roughly
their existential world, "the world they live in" (more literally, their
sphere). So the orbiculus is your world copied into your head.

AI is full of orbiculi. A "world model" is precisely an orbiculus; it's a
model of the world inside your head. Or consider the slogan of vision as
"inverse optics": visual processing takes a retinal image and reconstructs
the world that produced it (Hurlbert and Poggio 1988). You'll also find an
orbiculus almost anywhere you see an AI person talk about "reasoning about
X". This X might be solid objects, time-extended processes, problem-solving
situations, communicative interactions, or any of a hundred other things.
"Reasoning about" X suggests a purely internal cognitive process, as opposed
to more active phrases like "using" or "participating in" X. AI research
on "reasoning about X" requires representations of X. These representations
need to encode all the salient details of X so that computational processes
can efficiently recover and manipulate them. In practice, the algorithms
performing these abstract manipulations tend to require a choice between
restrictive assumptions and computational intractability (see Brachman and
Levesque 1984, Hopcroft and Krafft 1987).

If you prefer the phrase "using X" over "reasoning about X", an AI person
will ask you, "But we can reason about things that aren't right in front of
us, can't we?" AI's version of mentalism offers seductive answers to many
questions, and this is one of them. According to mentalism, reasoning about a
derailleur proceeds in the same way regardless of whether the derailleur is in
front of you or across town. Regardless of where the derailleur is located,
you reason about it by building and consulting an orbicular derailleur-model.
If having the derailleur present helps you, it is only by helping you build
your model.

This is, of course, contrary to common experience. As we all know, the
first several times you try to reason about a derailleur (1) it has to be
sitting right in front of you and (2) you have to be able to look around it,
poke at it, and take it apart (Chapman and Agre 1986). I've disassembled
and reassembled several derailleurs. Yet without a derailleur in front of
me, or at least a good diagram, I cannot explain how a derailleur changes
gears, or even list the parts involved. Experts can, but not an amateur like
me. Why aren't several disassemblies and reassemblies of derailleurs enough
to build a mental model of them?

Maybe the computational complexity of reasoning with realistic world models
is trying to tell us something. Maybe what you learn when you gain experience
with a derailleur or a city or a recipe is more specific. Perhaps it is more
biased to the specific things you've had to remember in the course of the
activity. Perhaps it is more closely tied to your goals at particular moments
of the activity. Perhaps it is more organized around the experience of the
individual situations that arise in the course of the activity. These are
difficult ideas. The question is complicated and messy and poorly worked out.
But that's to be expected. Expecting it to be easy is a sign of addiction to
the easy answers of the orbiculi.

**Writing as bad and good metaphor for representation** 

Within the technologically informed human sciences, cognition is almost
universally understood to involve the mental manipulation of assemblages
of symbols called representations. These representations represent the
individual's world -- they are the orbiculus. The vast majority of this
research assumes symbolic representations to have certain properties.
They are:

> object-like (neither events nor processes),
>
> passive (not possessing any sort of agency themselves),
>
> static (not apt to undergo any reconfiguration, decay, or effacement,
> except through an outside process or a destructive act of some agent),
>
> structured (composed of discrete, indivisible elements whose
> arrangement is significant in some fashion),
>
> visible (can be inspected without thereby being modified), and
>
> portable (capable of being transported to anyone or anything that
> might use them without thereby being altered or degraded).

Although the cognitivist understands symbolic representations as abstract
mental entities, all of these properties are shared by written texts (Latour
1986). Words like "structured", "inspected", "modified", "transported",
and "altered" are metaphors that liken abstractions inside of computers
to physical materials such as paper. Observe also that most of these
properties are deficient or absent for spoken utterances, which evaporate as
quickly as they are issued (Derrida 1976: 20) and are only decomposed into
discrete elements through complex effort. Thus we can speak of a writing
metaphor for representation.

This conception of representation-as-writing is topical for several reasons.
The connectionist movement has lent urgency to the seeming conflict between
symbolic manipulation and the relatively simple, uniform, statically and
locally connected, highly parallel hardware of the human brain (Fodor
and Pylyshyn 1988, Hutchins 1986, Rumelhart et al 1986). Anthropologists
such as Goody (1986), Ong (1982), Harris (1980, 1987), and Latour (1986)
have challenged views of cognition that make universal principles out of
psychological and social phenomena found only in literate cultures.

This section has three purposes. First I argue that symbolic representation
in artificial intelligence is, historically, modeled on written texts, as
opposed to (say) photographs or spoken utterances. Then I describe how
writing is a bad metaphor for symbolic representation. These arguments
implicate prevalent technical methods. Finally I describe how writing is
a *good* metaphor for symbolic representation. These arguments suggest
new technical directions.

Representation as writing

Roy Harris (1987), among others, has argued that ideas about representation
in philosophy and linguistics have been biased by writing. He observes that
these fields have emphasized those aspects of human utterances that appear
in a conventional written representation. One might read in a textbook a
sentence such as,

> Suppose that John says to Mary, "Please close the window".

and this sentence will be taken to specify some hypothetical event. We do not
normally wonder, and only rarely are we told, about several aspects of John's
action:

* his tone of voice,* his articulation of the various phonemes,* the shape of his intonation,* the timing of the various elements within the utterance,* the timing of his utterance relative to other actions and events,* whether he and Mary have a history of interactions over this window,* his position relative to Mary and the window,* his posture,* his gestures,* his facial expression,* the direction of his gaze,* whether and when he has caught Mary's gaze.

(For the horrors of trying to make written notations of these things, see
Atkinson and Heritage (1984) or Levinson (1983) for an introduction to
Jefferson's notation system used in conversation analysis.)

Given that these aspects of speech regularly affect the import of utterances,
a written sentence must be considered a poor representation of a spoken
utterance. But most philosophical and linguistic analyses have proceeded on
the basis of this idealized representation, a tradition that AI has carried
on. The point is not that these fields talk about writing; only that they
concentrate on the aspects of representation that writing normally captures.
As a result, theories will naturally tend to lean on distinctions that writing
captures, and not on the many distinctions it doesn't.

Among the many routes by which the writing metaphor entered AI practice,
one moment stands out: Newell and Simon's (1963, 1972) invention of symbolic
programming. Most of Newell and Simon's domains, especially in their earlier
work, have been domains like cryptarithmetic in which the "world" consists of
a sheet of scratch paper. Newell's production system models do not contain
separate mechanisms for the scratch paper and for the agent's "short-term
memory". Newell and Simon invented symbolic programming in order to implement
the sorts of structures and operations that their models specified. List
structures, like scratch paper, and like the symbolic structures of all
subsequent AI programming languages, have many properties of writing and few
properties of speech. People invented writing because there's nothing in
their heads that's anything like paper.

Writing in the head

AI research is often caught in a pattern whereby mechanisms that seem
extremely "expressive", "powerful", and "general" refuse to scale up. Let's
return to the properties that AI has ascribed to symbolic representations
-- object-like, passive, static, structured, visible, and portable -- and
consider how they lead to difficulties of scaling and implementation.

Symbolic programming languages endow their datastructures with all six
properties of writing. They implement these properties using pointers that
metaphorically make objects visible to processes. Pointers connect the
components of structures. One transports a structure by "passing" a pointer
to it. Structures only change when processes change them. Pointers do
not obey any locality beyond that of their own connectivity. Thus they are
eminently reconfigurable.

Pointers cause two sorts of difficulties. First, they require their
implementation medium to be infinitely reconfigurable (Chapman 1991: 35-41).
They fight both against the locality of physical space and against the
inertia of physical machinery and its interconnections. On serial machines
we observe this difficulty in the complexities of dynamic storage management.
On parallel machines we observe it in the complexities of shared-memory
management. Pointers also cause algorithmic complexity. Just as you can
write symbols on paper in any order, a pointer can point at anything. As a
result, algorithms for the manipulation of symbolic pointer-structures often
suffer from the combinatorial arbitrariness of the objects they reason with.

If writing is a good metaphor for symbolic representation, then, it is not
because we have things in our heads that are object-like, passive, static,
structured, visible, and portable. These properties of writing don't help us
to understand human use of symbolic representation *in general* because
they are the properties of written texts that are *specific to written
texts*. Far from picking out the essence of symbolic representation, they
dwell on the physical activity of using a written text: inscribing, gathering,
comparing, storing, and destroying. The invention of writing was important
precisely because it permitted these useful forms of activity.

Writing as representation

How, then, can writing serve as a model of symbolic representation? Imagine
that you're using a recipe -- that is, a recipe on paper -- to help you cook
dinner. Or perhaps you're using some directions -- again, on paper -- to
help you get to a party. The paper has a paradoxical position. Even though
it's a physical object with a definite size, mass, and location, it plays its
role -- at least qua representation -- entirely through your interpretation.
And even though it seems to offer opinions about the particulars of the
situation, it only does so because you figure out what in your surroundings
it's talking about.

The paper in your hand is both part of the material situation and doubly
removed from it. It underdetermines the sense you make of it because it
is separate from you -- after all, someone else in the same situation would
probably do something different. And it underdetermines what in the situation
it picks out because you are separate from your surroundings -- after all,
it would probably be useful in other situations as well. A similar argument
then applies, not just to notes written on paper, but to all symbolic
representations: their meaning must be completed in the act of use (Ingarden
1973). The world does not come innately parcelled out into the categories we
find mentioned in written texts. Instead, people use representations to help
them make sense of particular situations. What a given text is talking about
is a fresh problem in every next setting.

(For those who care about such things, this is what Jacques Derrida means
by the word "writing". For introductions to Derrida's philosophy see Culler
(1982) and Norris (1982). I have also been influenced by Garfinkel's (1984
[1967]) ethnomethodological ideas about the indexicality of representation
use. For an introduction see Heritage (1984).)

This idea has many consequences for computation. The relationship between
internal processes and internal symbolic representations is qualitatively the
same as the relationship between a person and a sheet of paper. The idea of
cognition as a process operating on symbolic representations is therefore of
less help than we had hoped. We can put symbolic representations inside our
robots, but the hard problems remain.

What other forms might a theory of symbolic representation take? Vygotsky
(1978 [1934]; for an introduction see Wertsch 1985) suggests that cognitive
skills involving mental representation arise from the everyday use of physical
representations, many of which are embedded in patterned social relationships.
These skills are diverse because the everyday forms of representation use are
diverse: speaking and hearing give rise to internal speech, making and looking
at pictures give rise to visualization, and so forth. And the "internal" and
"external" uses of representations tend to blur together in practice. But the
internal processes differ from the external processes because the insides of
our heads aren't like the outsides. Instead, they are shaped by the kind of
machinery we have in our heads. For example, internalized speech is far more
consequential than internalized writing because our brains are better suited
for reproducing speech than writing. If this is true, then many properties
of speech that philosophy and linguistics have marginalized, such as tone of
voice and intonation (and their pragmatic import in particular contexts of
use), will have to be readmitted to our theoretical center stage.

**A story about photocopier supplies** 

Back when I worked at counter jobs, I discovered that people are oblivious to
signs. You could put a big red sign with stars and arrows

> THE MACHINE WILL BE BACK UP AT MIDNIGHT

anywhere you liked and people would still walk up to the counter and ask "when
will the machine be back up?".

Here is an example of this effect.

> Date: Tue, 17 May 1988 17:05 EDT   
> From: J...   
> To: All-AI   
> Subject: Xerox copiers and Lazer Printers
>
> Due to someone's IGNORANCE, CARELESSNESS, or LACK OF PATIENCE,
> SOMEONE PUT DRY IMAGER FOR THE LAZER MACHINE INTO THE XEROX MACHINE
> on the 8th floor. These supplies, although both dry imager, ARE
> NOT INTERCHANGEABLE!!! It says on the box it comes in (and on the
> bottle itself) which machine it is for.
>
> We were warned by the Xerox people before that if this happened
> again, they may discontinue servicing our machines -- not to
> mention the cost of having it corrected (or maybe having to get a
> replacement).
>
> If there is a problem with the xerox or lazer machine on the 7th
> floor and you do not know how to correct it or have a question,
> see D.... She is in charge of the overall care of those machines
> as I am the machines on the 8th floor (I can be located at ...).
>
> Because of one person's lack of resourcefulness (he/she could of
> went down to the 7th floor or seen me or D), we are all suffering!
> If it is after hours and you are not sure what to do, it is better
> to do nothing than ruin a machine.
>
> --J

In the old days, when the photocopier needed dry toner, one looked around, saw
the bottle marked "dry toner", opened the machine, found the reservoir marked
"dry toner", and put the contents of the bottle into the reservoir. Sometimes
someone would put the toner someplace else, or they'd put something else into
the toner reservoir, but these things didn't happen often.

By the late 1980s, however, many rooms with photocopiers in them also had
laser printers in them. (Laser printers did not yet have disposable print
cartridges with their own toner supplies.) And in the copier/printer room on
the 8th floor of the MIT AI Lab, the two types of dry toner were incompatible.
So what happened when the copier ran out of dry toner? Exactly the same thing
as before. Except that the bottle marked "dry toner" one happens to come
across first might or might not be the correct dry toner.

Does this happen because people are too lazy to check whether it's laser or
copier toner? After all, as J points out, "It says on the box it comes in
(and on the bottle itself) which machine it is for". Do the people just go
irresponsibly ahead putting laser toner in the copier figuring it's probably
OK? Do they proceed despite a conscious uncertainty?

Although we must appreciate J's situation, I think all these hypotheses are
unnecessary. Put yourself in the place of someone to whom the photocopier
is asking for dry toner, and suppose that you had not yet known that the
copier and printer employed two incompatible types of dry toner that could
be confused for one another. You made dozens of separate moves in answering
the copier's call to be resupplied with toner, and any of those moves could
be mistaken in dozens of different ways. The actual problem, namely that
the bottle marked "dry toner" was not actually the correct substance, is
pretty obscure, as if somebody parked a car nearly identical to yours a couple
spaces down. In the case of the wrong car, some discrepancy would probably
force itself upon your attention before you got too far. Yes, evidence of the
mistake was readily available, but were you really supposed to list all the
things you might be doing wrong and go looking for evidence to rule out each
one? That would be impossible.

The problem, in short, is only obvious in retrospect. Having been warned
that toner comes in two types, one should probably start to check. But nobody
is born with that knowledge. Someone could become perfectly proficient at
replacing toner in copiers and still run afoul of this difficulty, simply
because types of toner had never become an issue for them. The arrival of
the laser printer would invalidate one of the innumerable implicit background
assumptions of their toner-changing routine, but it is hard to articulate the
general policy that could have informed them of this. Read the fine print on
every label every time? But the world is full of representations; how do you
decide when to stop reading them all and start doing something? The phrase
"dry toner", to us, having been informed of the problem, is ambiguous: it
could mean "laser dry toner" or "copier dry toner". But that ambiguity is
only consciously and morally an ambiguity for *us*, the well-informed.
And for all we know, "dry toner" could also be ambiguous in an unlimited
variety of other ways.

In the end, all we can do is stop moralizing and fix the problem. Make the
toner bottles so different that it's physically impossible to install the
wrong stuff. Train everyone. Or lock up the toner.

**A story about some instructions at a performance in an art gallery**

One day I went to the MIT Media Lab to see a performance. The performance
took place in a windowless room that's about thirty feet square with a high
ceiling. When we arrived the doors hadn't yet opened, so the audience milled
about outside. Finally the time came and the ticket-seller wandered into the
lobby and yelled something like, "OK the doors are open". Then as people were
drifting toward the door she moved into the middle of the crowd and yelled a
complicated set of instructions that went something like this:

> You can sit on the chairs or you can go to the back wall and look
> through the windows or you can go up on the balcony, but don't lean
> against the side wall.

None of us could see the inside of the performance space as she was saying
all this, so we had no way of knowing what she meant by windows, side wall,
back wall, balcony, etc. This room has no windows or balconies, and so
the yeller must have been referring to structures that were built specially
for the performance. One could feel the crowd being uncomfortable, many of
them turning to their neighbors in an attempt to get clarification. I found
myself trying to visualize the scene, but I had no idea how to place even the
"side wall", much less the balcony and the windows. Both the impossibility
of visualizing the scene and the effort spent trying to visualize it seemed
to make the instructions unusually hard to remember, as if they were nonsense
syllables, and several people could be heard repeating parts of them over to
themselves or to their neighbors.

I found this amusing, and adopting a gently ironic imitation of the register
and diction of the yeller I said something like, "you can stand between the
monsters but don't sit on the toadstools". Not many people got the joke, I'm
afraid, and especially not the yeller. I found this interesting in itself.
The yeller was obviously familiar with the room, and she presumably had no
problem visualizing what she was talking about. She evinced no awareness that
others might be having a problem.

Once inside, there was an audible rush to attach the words to parts of the
room, which was dark and full of peculiar wooden structures. The "side wall"
is immediately there on your right, verifiable by the readily visible chairs
along it, and the "balcony" could be found along the back wall with a little
scanning. The "windows" weren't at all obvious; they were windows in the wall
supporting the balcony, behind which one could stand. I suggested we go for
the balcony; although no stairs were immediately visible it was obvious where
they should be and others were already headed that way ahead of us.

In this story, the peculiar relationship between the instructions and the
physical setting disrupted an aspect of language understanding that normally
goes unremarked. The situation resembles the mnemonist's method of loci: if
someone tells a story that happens in a familiar space -- or a space for which
you have a cultural model, such as a story set in a generic Western kitchen
-- the objects and actions in the story get "placed" in a way that can be
either quasi-visual or kinaesthetic or both. If you can't put the elements
of the story in their places then you won't be able to hang onto them, just
as we had trouble hanging onto the balcony and windows in the ticket-seller's
instructions.

This story connects to a larger theme about language. I want to believe that
an utterance has no meaning outside the particular concrete setting where
it's used. But then how can we can talk about things that are distant or
hypothetical? Consider the examples that linguists ask you to evaluate out
of context, like those sentences where you're supposed to indicate whether the
pronoun can refer to (a) John or (b) Bill. Often I've found an interpretation
not-OK until I work out a hypothetical context that makes it OK.

I suspect that such exercises get consistent results only because of
cultural conventions about the default contexts. The willingness to evaluate
decontextualized sentences *at all* is culturally specific. The
cognitive anthropologist A. R. Luria (1976), for example, found his informants
refusing to answer syllogistic reasoning tests until they knew the particulars
of each sentence -- the equivalents of the John and Bill who remain so
comfortable as ciphers in my own culture. These people haven't learned the
language game of decontextualized grammar and syllogism quizzes, and don't
care to.

Heath (1983) describes how this capacity for decontextualization arises.
She found that middle-class parents use rituals like bedtime-story-reading
to introduce children to decontextualized letters, words, and forms of
speech. Children who don't get this training have a harder time relating
to decontextualized school exercises. Decontextualization is a complex and
culturally specific skill laid on top of the more natural ability to relate
language to familiar contexts. This has led to two quite different phenomena
-- one of them more fundamental and universal than the other -- being run
together and confused, with the later, more articulated phenomenon (the
ability to perform certain tricks with decontextualized representations)
getting all the credit.

**A story about my routines for reading the Sunday Globe** 

This is a story about the indeterminacy of plans. The plan was something I
said to myself as part of a settled routine. And I have a theory about the
role of plans in settled routines. A routine might start out being mediated
by an imperative utterance, such as a command you subarticulate to yourself.
As the routine settles down, I hypothesize, it will still exhibit all the
underdetermination, ambiguity, and indexicality of the original utterance,
long after you've lost all awareness of any English being involved. Just
because the activity has gotten "compiled" -- as computer people would say --
doesn't mean that the connection between the plan and the concrete situation
of using it becomes any less problematic. Why? Perhaps you never stop saying
the plan-text to yourself; perhaps as you routinize your actions you routinize
your interpretive process as well.

Here, then, is the story. The Boston Globe recently began an expanded arts
section in their Sunday edition. Called "Arts Etc", it gathers all the Sunday
movie, arts, book reviews, arts schedules and advertising, and high-brow
cultural commentary. This section doesn't have clearly delineated departments
except for the final few pages, which are marked off for book reviews. The
book review department, in fact, is wholly unchanged from the pre-Arts-Etc
Sunday Globe. The first of the book review pages has its own banner and
distinctive format, and all of the longer book reviews begin on that page
and continue inside, where there are also shorter reviews and lists of best
sellers and so forth.

Now, when reading the newspaper I will often come across the continuation of
an article that looks interesting even though I hadn't noticed it when I was
reading the page on which it began. So I'll have to back up to the earlier
page to read the beginning of the article.

Last Sunday, then, I was reading a book review in the Globe. In particular,
I was in the interior of the book review section, having followed an article
from the book review section's first page (which, let us say, was page C15),
when I came upon a headline about an author I was interested in reading about.
Focusing on this headline, I found that it was a continuation. Whereupon,
oddly, I turned to page C1 -- i.e., the front page of the whole arts section
-- and not to page C15 -- i.e., the first page of the book review section.
I *knew* that all the book reviews began on C15, not C1, but I turned to
C1 anyway. When I got C1 in front of me, it was not at all what I expected;
momentarily confused, I figured out that I should turn to C15 instead.

Saying "C1" and "C15" is of course misleading. I don't think I knew that it
was section "C" or page 15. My mistake, I think, turned on my never having
reflected on the odd relationship between the two pages: the book review
section was a clear "part" of the arts section, but the arts section didn't
have any other clear "parts". Both page C1 and page C15 were the "front"
of something -- the arts section and the book review section, respectively.
I had long been familiar with the Sunday Globe book review section's format,
and its design and layout did little to make it look like a part of the
superordinate arts section.

Here's what I think happened. When I went to turn to the beginning of the
review I wanted to read, I turned to "the front", perhaps even "the front of
the section". I'm not sure what I mean by double-quoting those two English
phrases, but I want to mean something fairly literal. That is, I think I made
my mistake because I was saying a phrase to myself in English, the phrase was
ambiguous, and I interpreted it wrongly.

I've been reading newspapers for at least fifteen years and Boston Sunday
Globe book reviews for almost ten years. Stumbling upon the continuation of
an article and wanting to find its beginning is a routine I've been through
many hundreds of times. And at least a couple dozen of these episodes must
have occurred during my reading of the Sunday Globe's book reviews.

Why did I know to turn to the "front" of the section? Not all articles in
the rest of the paper start at fronts of sections. I think at some point I
noticed, and articulated to myself, that the book reviews start at the front
of the book review section. So this was not the first time I've said "go
to the front of the section" to myself in my head in such a situation. This
internal uttering-to-myself and the actions I typically take in consequence of
it must certainly have worn deep grooves in my brain by now. You might think
that it was so thoroughly "compiled" that it no longer resembled English.
Yet still it was capable of this very language-like underspecification of the
situation. I still had to figure out what the English phrase was referring
to in this specific concrete situation, and even though this figuring occurred
perfectly automatically, smoothly, and routinely, it was still problematic.
I could still get it wrong.

So "the front of the section" was ambiguous in this situation. But all of
this still doesn't explain why, on the particular moment in question, it led
me to turn to C1 rather than C15. Before the Globe reformatted and publicized
its "Arts Etc", I had never given any particular thought to the idea of the
Sunday Globe having an "arts section". In fact I clearly recall the first
Sunday of the new section: the front page of the paper -- i.e., A1 -- had an
ad for it, and despite the silly name I decided to give it a fair try. In
fact it contained a useful article about Soviet dissident films, a topic that
interested me. The matter of "the Globe's new arts section" -- in exactly
those words -- had thus been on my mind. I don't want to conclude that
the arts-section interpretation was "stronger" than the book-review-section
interpretation, but whatever is operating as we constantly use background
information to "fill in the details" of utterances when determining their
relevance to particular concrete situations was operating here as well.

**What I'm trying to figure out** 

Implicit in these stories are some ideas about representation and action.

> 1) Writing model of representation. By "writing", I mean that the
> representation is something apart from you. It is a resource in
> situated action (Suchman 1987). You have to make sense of it in each
> next situation. There are no complete, systematic, guaranteed rules
> for this making-sense. And when you *do* manage to figure out what
> in some situation a representation is talking about, there is no way
> to finish listing what about the situation enabled you to do this.
>
> 2) Dependency model of routine evolution. All forms of activity
> are snapshots in the evolution of routines. The routines themselves
> are intertwined with the patterns of society and with the layout
> of particular places. The model says: when you think a new thought
> in some situation, you connect it back to its premises (Stallman and
> Sussman 1977). When you believe those same premises again in some
> future situation, you automatically call up the conclusion.

I'm trying to relate these two ideas. I think most concrete activity requires
you to interpret representations, that is, "making sense of a representation
in each next situation by figuring out what in the situation it is talking
about". So, for example, "turn left" will indicate different actions in
different situations.

This sounds like a lot of work. If it were really a fresh challenge to make
sense of "turn left" or "open the bottom drawer" on every moment, how would we
ever do anything? But I don't think it's that bad. What you have in practice
is a patchwork of routinized methods. In some past situation someone said
"take the next left", and you took certain specific concrete actions: you
looked around, you searched for particular shapes and colors, and maybe you
walked around and looked some more. You had your own reasons for doing all
these things, and all of your actions and their reasons got connected, so now
they're ready and waiting to happen again in new situations. In subsequent
situations some of the reasons might not have applied, so instead you took
other actions, and these themselves led to new connections.

Perhaps after enough of this you develop a sufficient repertoire of routines
to apply "turn left" to almost all of the left-turn situations you encounter
in the average day. You've developed habits of interpretation. So whenever
you tell yourself -- or someone else tells you -- "turn left", you'll be able
to do it right away, "automatically", without any hesitation or difficult
figuring-out.

These routines, like all routines, will evolve (Agre 1985a, 1985b). Very
often the evolution of a routine involving a representation will permit
you to undertake the activity without the representation being present in
physical form. For example, using a recipe ten times might let you make
the dish without the recipe. One precondition for this effect seems to be
that you understand the reasons for the recipe's instructions, but this turns
out to be a complicated idea. In any event, there's a sense in which the
representation never goes away. Even when you're routinely deciding to turn
left or add salt, you're still -- in some sense I wish I understood -- saying
the utterance "turn left" or "salt to taste" to yourself, and you're still
interpreting it just like any other natural-language utterance that you need
to relate to a concrete situation.

**Acknowledgements** 

Conversations with Marty Hiller and Jeff Shrager helped me think about what
people do with instructions and directions. David Chapman and Beth Preston
carefully read a draft of this paper. Michael Mateas helped with the final
revisions.

Patricia Morison helped with Latin etymology.

The "Upper Elk Tree Road" directions in the introduction and the computer
message in "A story about photocopier supplies" are reproduced with the
permission of their authors. I have altered them slightly to suppress
identities and remove some comments on other matters.

**References** 

Agre, Philip E. (1985a). The structures of everyday life. Working Paper 267,
MIT Artificial Intelligence Laboratory.

Agre, Philip E. (1985b). Routines. AI Memo 828, MIT Artificial Intelligence
Laboratory.

Agre, Philip E. (1997). *Computation and Human Experience*. Cambridge:
Cambridge University Press.

Amerine, R. & J. Bilmes (1988). Following instructions. *Human Studies*,
11, 327-339.

Atkinson, J. Maxwell & John Heritage (Eds.) (1984). *Structures of Social
Action: Studies in Conversation Analysis*. Cambridge: Cambridge University
Press.

Auerbach, Erich (1953). *Mimesis: The Representation of Reality in Western
Literature*. Translated by W. R. Trask. Princeton: Princeton University
Press.

Barwise, Jon & John Perry (1983). *Situations and Attitudes*. Cambridge:
MIT Press.

Brachman, Ronald J. & Hector J. Levesque (1984). The tractability of
subsumption in frame-based description languages. *Proceedings of the
National Conference on Artificial Intelligence, Austin, TX*, pages
34-37.

Brachman, Ronald J. & Hector J. Levesque (Eds.) (1985). *Readings in
Knowledge Representation*. Los Altos, CA: Morgan Kaufmann.

Brodsky, Claudia J. (1987). *The Imposition of Form: Studies in Narrative
Representation and Knowledge*. Princeton: Princeton University Press.

Chapman, David (1991). *Vision, Instruction, and Action*. Cambridge: MIT
Press.

Chapman, David & Philip E. Agre (1986). Abstract reasoning as emergent from
concrete activity. In M. P. Georgeff & A. L. Lansky (Eds.), *Reasoning about
Actions and Plans*. Los Altos, CA: Morgan Kaufmann.

Culler, Jonathan (1982). *On Deconstruction: Theory and Criticism after
Structuralism*. Ithaca: Cornell University Press.

Dennett, Daniel (1978). *Brainstorms: Philosophical Essays on Mind and
Psychology*. Montgomery, VT: Bradford.

Derrida, Jacques (1976). *Of Grammatology*. Translated by G. C. Spivak.
Baltimore: Johns Hopkins University Press.

Fodor, Jerry & Zenon Pylyshyn (1988). Connectionism and cognitive
architecture: A critical analysis. *Cognition*, 28, 3-72.

Garfinkel, Harold (1984). *Studies in Ethnomethodology*. Oxford: Polity
Press. Originally published in 1967.

Goody, Jack (1986). *The Logic of Writing and the Organization of
Society*. Cambridge: Cambridge University Press.

Hagen, Margaret (1986). *Varieties of Realism: Geometries of
Representational Art*. Cambridge: Cambridge University Press.

Harris, Roy (1980). *The Language-Makers*. Ithaca: Cornell University
Press.

Harris, Roy (1987). *The Language Machine*. Ithaca: Cornell University
Press.

Hartog, Francois (1988). *The Mirror of Herodotus: The Representation of
the Other in the Writing of History*. Translated by J. Lloyd, Berkeley:
University of California Press.

Haugeland, John (1981). *Mind Design: Philosophy, Psychology, Artificial
Intelligence*. Cambridge: MIT Press, 1981.

Heath, Shirley Brice (1983). *Ways with Words: Language, Life, and Work in
Communities and Classrooms*. Cambridge: Cambridge University Press.

Heritage, John (1984). *Garfinkel and Ethnomethodology*. Cambridge:
Polity Press.

Hopcroft, John E. & Dean B. Krafft (1987). The challenge of robotics for
computer science, in Jacob T. Schwartz & Chee-Keng Yap, eds, *Algorithmic
and Geometric Aspects of Robotics*, Volume 1. Hillsdale, NJ: Erlbaum.

Hurlbert, Anya & Tomaso Poggio (1988). Making machines (and artificial
intelligence) see. *Daedalus*, 117, 213-239.

Hutchins, Edwin (1986). Mediation and automatization. *Quarterly Newsletter
of the Laboratory of Comparative Human Cognition*, 8, 47-58.

Hutchins, Edwin (1995). *Cognition in the Wild*. Cambridge: MIT Press.

Ingarden, Roman (1973). *The Cognition of the Literary Work of Art*.
Translated by R. A. Crowley & K. R. Olson. Evanston: Northwestern University
Press.

Judovitz, Dalia (1988). *Subjectivity and Representation in Descartes: The
Origins of Modernity*. Cambridge University Press.

Krieger, Murray (Ed.) (1987). *The Aims of Representation: Subject, Text,
History*. New York: Columbia University Press.

Latour, Bruno (1986). Visualisation and cognition: Thinking with eyes and
hands. *Knowledge and Society*, 6, 1-40.

Levinson, Stephen C. (1983). *Pragmatics*. Cambridge: Cambridge
University Press.

Luria, A. R. (1976). *Cognitive Development: Its Cultural and Social
Foundations*. Translated by M. Lopez-Morillas & L. Solotaroff, edited by
M. Cole, Cambridge: Harvard University Press.

Newell, Allen & Herbert A. Simon (1963). GPS, a program that simulates human
thought. In E. A. Feigenbaum & J. Feldman (Eds.), *Computers and
Thought*. New York: McGraw-Hill.

Newell, Allen & Herbert Simon (1972). *Human Problem Solving*. Englewood
Cliffs, NJ: Prentice-Hall.

Norris, Christopher (1982). *Deconstruction: Theory and Practice*.
London: Methuen.

Ong, Walter J. (1982). *Orality and Literacy: The Technologizing of the
Word*. London: Methuen.

Rorty, Richard (1979). *Philosophy and the Mirror of Nature*. Princeton:
Princeton University Press.

Rumelhart, David E., Paul Smolensky, James L. McLelland, & Geoffrey E. Hinton
(1986). Schemata and sequential thought processes in PDP models. In
J. L. McLelland & D. E. Rumelhart, eds, *Parallel Sequential Processing:
Exploration in the Microstructure of Cognition, Volume 2: Psychological and
Biological Models*. Cambridge: MIT Press.

Searle, John R. (1981). Minds, brains, and programs. In J. Haugeland (Ed.),
*Mind Design: Philosophy, Psychology, Artificial Intelligence*.
Cambridge: MIT Press.

Silvers, Stuart (1989). *Rerepresentation: Readings in the Philosophy of
Mental Representation*. Dordrecht: Kluwer.

Stallman, Richard M. & Gerald Jay Sussman (1977). Forward reasoning and
dependency-directed backtracking in a system for computer-aided circuit
analysis. *Artificial Intelligence*, 9, 135-196.

Suchman, Lucy A. (1987). *Plans and Situated Actions: The Problem of
Human-Machine Communication*. Cambridge: Cambridge University Press.

Vygotsky, L. S. (1978). *Mind in Society: The Development of Higher
Psychological Processes*. Edited by M. Cole, V. John-Steiner, S. Scribner
& E. Souberman. Cambridge: Harvard University Press. Originally published
in Russian in 1934.

Wallis, Brian (Ed.) (1984). *Art after Modernism: Rethinking
Representation*. New York: New Museum of Contemporary Art.

Wertsch, James W. (1985). *Vygotsky and the Social Formation of Mind*.
Cambridge: Harvard University Press.

White, Hayden (1973). *Metahistory: The Historical Imagination in
Nineteenth-Century Europe*. Baltimore: Johns Hopkins University Press.

Zimmerman, Don H. (1973). The practicalities of rule use. In J. D. Douglas
(Ed.), *Understanding Everyday Life: Toward the Reconstruction of
Sociological Knowledge*. London: Routledge and Kegan Paul.