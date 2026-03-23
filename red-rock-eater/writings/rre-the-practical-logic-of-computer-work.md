---
id: rre-the-practical-logic-of-computer-work
title: "[RRE]The Practical Logic of Computer Work"
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1998/RRE.The.Practical.Logic..html
coauthors: []
key_concepts: []
importance: 7
research_status: partial
tags:
  - auto-imported
  - rre
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1998/RRE.The.Practical.Logic..html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991004110334/http://www.somewhere.com/)

  

# [RRE]The Practical Logic of Computer Work

```
---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html
or send a message to requests@lists.gseis.ucla.edu with Subject: info rre

---

  The Practical Logic of Computer Work

  Philip E. Agre
  Department of Communication
  University of California, San Diego
  La Jolla, California  92093-0503
  USA

  phone: +1 (619) 534-6328
    fax: +1 (619) 534-7315
    net: pagre@ucsd.edu
   home: http://communication.ucsd.edu/pagre/

  Revised version of a paper presented at the Conference of the
  Society for Social Studies of Science, Tucson, October 1997.
  3400 words.

  Italics are in asterisks, book titles in underscores.

In his reading of John Dee's sixteenth-century commentary on Euclid,
Knoespel (1987) describes what he calls the "narrative matter of
mathematics": the discursive work by which an artifact such as a
drawing on paper is exhibited as embodying a mathematical structure
such as a Euclidean triangle.  This process, which is familiar enough
to modern technologists as the work of mathematical formalization,
consists of a transformation of language into something quite
different from language, namely mathematics, and its challenge is to
circumvent or erase those aspects of language which are incompatible
with the claim of mathematics to represent the world in a transparent,
unmediated, ahistorical way.  Knoespel explains the larger
significance of the point like this:

  ... the reification of geometry in architecture and technology
  has enormous implications for language.  Once geometry becomes
  manifest in artifacts, these artifacts retain an authority an
  authority radically different from that accessible to natural
  language.  By virtue of their being manifested as physical
  objects they acquire what appears as an autonomy utterly separated
  from language.  The apparent separation of both architecture and
  technology from language has great significance, for it works to
  repress the linguistic framework that has allowed it to come into
  being.  (1987: 42)

Brian Smith (1996) makes a similar point when he speaks of
"inscription errors": inscribing one's discourse into an artifact
and then turning around and "discovering" it there.  An example might
be the front door of an office building.  Beyond its functions in
controlling entry, the door also serves a narrative function: someone
happening upon it can recognize it as a door, and it is designed
in part to be recognizable as a door and to be narratable in
those terms.  The point is familiar from Schutz (1967 [1927?]) and
Garfinkel (1984 [1967]): the social reality of the square resides
in a reflexive relationship between designer and user, and the success
of that relationship lies precisely in the achieved unremarkability
of that relationship and the possibility of routinely locating the
"squareness" in the artifact itself.

This observation about geometry exercises and architecture may have
little import in itself, but its significance is more evident in
the case of another large category of artifacts, namely computers.
The design of a computer begins with formalization -- an intensive
and highly skilled type of work on language.  A computer is, in an
important sense, a machine that we build so that we can talk about it
in a certain way; it is successful if its operation can be narrated
using a certain vocabulary.  As the machine is set to running, we
too easily overlook the complicated reflexive relationship between
the designer and user upon which the narratability of the machine's
operation depends.  The corpus of language that was transformed in
producing the machine is necessarily, like any discourse or text,
embedded in an institutional and historical context, and the machine
itself must therefore be understood as being, in some sense, a text.

For practitioners of a computational research tradition such as
artificial intelligence, however, the textuality of computers is a
distraction at best, to the extent that it is even comprehensible as
an analysis of technical work.  Like John Dee, the practitioners of
AI with whom I worked for several years, and among whom I was trained,
regarded formalization very differently, as a means precisely of
freeing their work from what they regarded as the unruliness and
imprecision of vernacular language.  As a result, I want to argue, the
field has been left with no effective way of recognizing the systemic
difficulties that have arisen as the unfinished business of history
has irrupted in the middle of an intendedly ahistorical technical
practice.  My purpose in diagnosing this situation is not to discredit
mathematics, technology, or even AI.  Instead, I want to envision what
it would be like to have a critical technical practice: a technical
practice within which such reflection upon language and history, ideas
and institutions, is part and parcel of technical work itself.

My point of departure is what AI people themselves have taken
to calling Good Old-Fashioned AI -- the complex of metaphors and
techniques from which the great majority of the AI literature until
recently has begun.  Even those projects that do not fully embrace
this standard theory are usually well-understood as incrementally
relaxing its assumptions in an attempt to resolve its seeming inherent
tensions.  (Documentation of all of these characterizations of AI, and
details on many of the analyses of them, can be found in Agre (1998).)

This standard theory encompasses, among other things, particular
theories of representation, perception, and action.  The theory of
representation holds that knowledge consists in a model of the world,
formalized (when it is formalized) in terms of the Platonic analysis
of meaning in the tradition of Frege and Tarski.  Perception is a kind
of inverse optics: building a mental model of the world by working
backwards from sense-impressions, inferring what in the world might
have produced them.  Action, finally, is conducted through the
construction and execution of plans, understood roughly as computer
programs.  This theory is founded in several oppositions, and I want
to focus on the specific way in which these oppositions figure in the
history of the field.  They are as follows:

* * mind versus world,* * plans versus behavior,* * planning versus improvisation,* * the mind versus the body, and* * abstract ideals versus concrete things.

Throughout AI, one encounters a certain pattern in the handling of
these oppositions.  I will refer to this pattern as "dissociation".
Dissociation has two moments: an overt distinction between the two
terms and a covert conflation between them.  As the language of overt
and covert may suggest, dissociation is not consciously avowed.  It
must be sought in the internal tensions of texts and in the dynamics
of technical work.  Dissociation occurs in many ways, none of which
is fixed or stable.  To the contrary, much of the history of AI can be
understood as attempts to comprehend and manage the signs of trouble
that originate in dissociation and that AI practitioners can recognize
within the conceptual system of the field.  One purpose of a critical
technical practice is to recognize such troubles more fully and to
diagnose them more deeply.

Allow me to review the workings of dissociation in the five cases
I enumerated above as they become manifest in particular texts and
projects.  The distinction between mind and world has obviously
been construed in many ways by different philosophical systems, but
in AI it has been operationalized in terms of a sharp qualitative
distinction between the inside of the machine and the world outside.
The difficulty is that it is enormously difficult to maintain accurate
knowledge of a world that is understood to be so distinct and distant.
As a result, it is a common idealization in the field to suppose
that one's world model -- the mental structure that constitutes one's
knowledge of the world -- is complete in every relevant respect and
stays up-to-date automatically.  Indeed, it is common for AI people in
particular and computer people in general to employ the same words to
name both the representations in a machine and the things that those
representations represent.  This conflation between mind and world is
facilitated by the use of "domains" such a geometry and chess which
are readily understood in mathematical terms.  The erasure of language
that Knoespel discovered in Dee is here employed on a grand scale to
facilitate the conflation, not just of mathematics and the physical
world, but mental representation and the world.

The point is not that AI practitioners do this deliberately.  Quite
the contrary, their work is well understood as an attempt not to do
it.  Having acquired this conflation between mind and world through
the discursive practices they inherited from earlier intellectual
projects, AI people continually find the conflation reinforced through
the practical logic of their research.  If I may risk a mathematical
metaphor, the dissociative relationship between mind and world is
an attractor: although unsatisfactory as a theory of human life,
it is also difficult to escape by incremental modifications because
the covert conflation between mind and world solves, even if
pathologically, a problem for which no less pathological solution
is known.  The mathematical metaphor here is misleading, though, in
that the terrain is a function of consciousness: which moves in the
space of research proposals seem comprehensible and well-motivated is
itself a function of the critical awareness through which the symptoms
of technical trouble are perceived and interpreted.  So long as the
larger pattern remains ungrasped, the attractor retains its grip on
the research.

The second dissociation is between mental activity and perception.
AI originated as part of the cognitivist movement whose other was
behaviorism.  In combatting the behaviorist hegemony, the task of
cognitivism was to present itself as scientific by the same standard
as behaviorism did, while also opposing itself as squarely as possible
to behaviorism on a substantive level.  As Karl Lashley observed in
an influential 1951 symposium paper, the behaviorist theory of action
was stimulus-chaining: the idea that each action in a serially ordered
sequence arises as a response to, among other things, the effects of
the previous action in the sequence.  Lashley urged on psychophysical
grounds, however, that serially ordered action, for example in
language, must be understood in terms of an internal organizing
principle, which he understood as a holistic mental process.

In his effort to oppose himself to the behaviorist story, Lashley
equivocates on the role of perception in organizing behavior.  A
fair-minded reader will reconstruct his argument as advocating a
two-factor theory of behavior: continual perceptual inputs into the
ongoing mental process, and continual outputs from that process in the
form of spoken phonemes and other actions drawn from a language-like
repertoire.  But in fact Lashley provides little substantive account
of the role of perception, emphasizing instead that serial behavior
is planned and organized in advance and performed in scripted wholes.
Dissociation here takes a different form: rather than uniting bodily
through systematic ambiguity, the two terms are brought together
in two separate theories which are then superimposed.  One of these
theories, the mental scripting of action, is given the more overt
billing because of its simplicity and its polemical role, while the
other theory, the one that provides a clear place for perception,
floats indistinctly in the background.

A similar pattern can be observed in the case of the third
dissocation, which I have termed planning versus improvisation.
Remarkably, neither of these terms is prominent in the locus classicus
of AI's discourse of planning, Miller, Galanter, and Pribram's "Plans
and the Structure of Behavior" (1960).  Miller, Galanter, and Pribram
argue that behavior has a structure because it results from the
execution of a mental entity that has that same structure, namely
a Plan.  Although it is openly speculative and presents no computer
programs or laboratory experiments of its own, "Plans and the
Structure of Behavior" served as a rhetoric for the emerging
cognitivist movement.  Its most distinctive rhetorical device was
a systematic conflation between behavior and Plans.  To this day,
it is customary in AI research to refer to any structure in behavior
as a plan, not as a hypothesis but as a simple matter of terminology.

Miller, Galanter, and Pribram inherited the dissociation that was
already present in Lashley, and they took it a step further.  Close
reading demonstrates the presence of two distinct theories, one of
which speaks of discrete, prescripted Plans and another of which
speaks of a single Plan that unfolds incrementally through time.  The
former theory, the one that describes a repertoire of discrete Plans,
is the official theory: it is the theory that explains the structure
of behavior.  Yet it is an unsatisfactory theory in many ways, and so
it is overlaid with the unofficial theory of a single Plan that can
be constructed in a more improvisational manner as an ongoing response
to perception.  The authors return to the matter again by offering a
theory of Plans based on then-current ideas of servocontrol.  This
third theory is laid atop the earlier two with little overt sense
of their incompatibility; in any case, it is the equivocal relation
between the first two theories that set the agenda for subsequent
research.  Most of this research focused exclusively on the
construction of discrete plans, thus obviating the need for a theory
of improvisation.  It is computationally very difficult to construct
a Plan that will work reliably in a world of any great complexity,
however, and so the second of Miller, Galanter, and Pribram's theories
was rediscovered with great energy by AI researchers such as myself
in the 1980's.  One term of the dissociation, having been suppressed,
returned.  Yet when it did so, its internal relationship to the
dominant theory was hardly recognized, and research in that era saw
several attempts to resynthesize the two approaches, reproducing in
the architecture of cognitive models the conflation that occurred more
covertly in Miller, Galanter, and Pribram's text.

The fourth dissociation is between planning and execution, and here
again the covert conflation between the two terms takes a different
form.  It can be seen in the first computer implementation of the
plans-and-execution theory, the 1972 STRIPS model of Fikes and
Nilsson, which automatically constructed plans and then executed them
by directing the movements of a robot.  These authors' dilemma is that
it is hard to predict in enough detail how the world will unfold as
the robot executes its plans, and yet it is so expensive to construct
a new plan that it seems necessary to execute as much of each plan
as possible.  At one point they suggest simply executing the first
step of each new plan and then constructing a new plan from scratch,
but they reject the idea as impractical.  The dissociation between
planning and execution manifests itself here in a seeming attempt
by the two dissociated categories to become reunited, or at least
to become intertwined with one another.  The impracticality of the
dissociation is revealed through the process of system-building.
It is here, in the design and construction of systems, that AI
learns most of its lessons, and not in formal experimentation with
the systems once they are running.  If I seem to anthropomorphize the
desire of planning and execution to reverse their dissociation, this
is only to give voice to a common experience of system designers: the
very tangible set of pressures that seem to push the design process in
one direction or another.

The final dissociation is between abstraction and concrete reality
in the tradition of Fregean semantics.  Historically, theories of
semantics have drifted between two poles: psychologism is the theory
that meanings are mental entities, and Platonism is the theory that
meanings reside in a timeless, extensionless realm of ideals.  What
is most striking is how little difference this distinction has made
in practice.  The mind, as it has been constructed through the system
of dissociations that I have already described, resembles the realm
of Platonic ideals in many ways.  The use of mathematical domains
helps resolve this tension as well, inasmuch as mathematical entities
resemble Platonic ideals and are now routinely employed to formalize
Platonic theories of the semantics of both language and logic.

The problem arises whenever the mind must be understood as
participating in the historical, causal world.  The problem manifests
itself in many ways, but it can already be clearly grasped in Frege's
own theory.  Frege's theory of sense, that is, the cognitive content
of a representation, conflates incompatible goals.  The sense of
a representation is supposed to be a Platonic ideal, independent
of place and time, and yet it is also held to incorporate specific
objects such as a car or a person.  The problem is particularly acute
in the case of indexical representations, whose sense is plainly
dependent on the concrete historical circumstances of their use.
I can use words like "here" and "now" perfectly well without knowing
where I am or what time it is, and yet the sense of my utterance
involves those specific places and times.  The trouble arises because
Frege's theory of sense, and a whole subsequent tradition of semantic
theories, attempts to capture the content of thoughts and utterances
without reference to the embodied activities and relationships
with which they are used.  As the realm of Platonic abstractions is
conflated with the realm of concrete activity, the semantic formalism
takes on a covertly material character and the theory of mind takes on
a covertly disembodied character.

These, then, are five dissociations that have organized the practical
logic of research within the leading tradition of artificial
intelligence.  The interaction among these dissociations defines a
complex and variegated field whose contradictory pressures must be
reconciled somehow in each project in its own unique way.  In most
cases I have chosen particular projects to illustrate the practical
logic of dissociation.  Other projects may well be discovered to
manage the tensions in a different way.  Yet few AI projects, if
any, have reflected a systematic understanding of them, much less any
resolution.

Where do these dissociations originate?  Do all conceptual
distinctions lead to dissociations when they are embodied in technical
work?  When AI work is framed in terms of these dissociations, it
becomes obvious that AI is part of the history of Western thought.  It
has inherited certain discourses from that history about matters such
as mind and world, and it has inscribed those discourses in computing
machinery.  The whole point of this kind of technical model-building
is conceptual clarification and empirical evaluation, and yet AI has
failed either to clarify or to evaluate the concepts it has inherited.
Quite the contrary, by attempting to transcend the historicity of its
inherited language, it has blunted its own awareness of the internal
tensions that this language contains.  These tensions have gone
underground, emerging through substantive assumptions, linguistic
ambiguities, theoretical equivocations, technical impasses, and
ontological confusions.

Yet the project of artificial intelligence has not been a failure.
The discipline of technical implementation, considered in another
way, really has done its job.  The dissociations of AI have refused
to go away, and in the practical work of model-building they have
ceaselessly reasserted themselves.  As AI practitioners have tried
to manage all of the many cross-cutting tensions in their work, they
have made the generative principle of those tensions ever more visible
to those with the critical means to look.  This is the motivation
for my advocacy of a critical technical practice, and the basis of
my positive hopes for it.  Bad theories of human existence, we might
conjecture, do not simply fail to correspond to the data; they are in
fact impracticable, in that nobody and nothing could live in the ways
they describe.  As AI people learn to expand their understanding of
the ways in which a system can "work" or "not work", AI can perhaps
become a means of listening to reality and of learning from it.
The key to this transition is a reversal of the ideological function
of technology that Knoespel described at the outset.  The texts that
we inscribe in computing machinery are texts in the fullest sense.
In particular, they always have greater depths than we are aware
of, and they always encode sophisticated strategies for managing the
contradictory experience of the world that we have inherited from the
past.  Computers and formalization do not eliminate all this; quite
the contrary, they make it more visible.

And what exactly has AI made visible in this fashion?  Running through
all of the dissociations I mentioned a recurring theme, a kind of
transcendentalism that attempts to hold something apart from and above
material reality.  The transcendentalist philosophy of AI is that
the outside world is, to use the military language that AI took over
during the 1980's, uncertain, unpredictable, and changing.  In each
case, the world is a negative, chaotic principle and the mind is a
positive, ordering principles.  What we might tentatively conclude, in
the irreducibly intuitive and practical way in which such conclusions
might possibly be drawn from technical work, is that it doesn't work
that way.  If not for the positive ordering principles inherent in
the world itself, life would be impossible.  Man, in this traditional
sense, cannot live by imposing order, but only by participating in it.
Only from this standpoint amidst the order of the world does the world
itself become visible only then does the question usefully arise of
how best to live in the world, and how best to change it.

//* Bibliography

Philip E. Agre, Computation and Human Experience, Cambridge: Cambridge
University Press, 1997.

Harold Garfinkel, Studies in Ethnomethodology, Polity Press, 1984.
Originally published in 1967.

Kenneth J. Knoespel, The narrative matter of mathematics: John Dee's
Preface to the Elements of Euclid of Megara (1570), Philological
Quarterly 66(1), 1987, pages 27-46.

Karl S. Lashley, The problem of serial order in behavior, in Lloyd
A. Jeffress, ed, Cerebral Mechanisms in Behavior: The Hixon Symposium,
New York: Wiley, 1951.

George A. Miller, Eugene Galanter, and Karl H. Pribram, Plans and the
Structure of Behavior, New York: Henry Holt and Company, 1960.

Alfred Schutz, The Phenomenology of the Social World, translated by
George Walsh and Frederick Lehnert, Evanston: Northwestern University
Press, 1967.

Brian C. Smith, On the Origin of Objects, Cambridge: MIT Press, 1996.

end
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991004110334/http://www.somewhere.com/)
