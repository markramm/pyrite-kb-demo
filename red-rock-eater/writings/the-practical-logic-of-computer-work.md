---
id: the-practical-logic-of-computer-work
title: "The Practical Logic of Computer Work"
type: writing
writing_type: paper
url: "https://pages.gseis.ucla.edu/faculty/agre/practical.html"
coauthors: []
key_concepts: []
importance: 5
research_status: stub
tags:
  - paper
  - auto-imported
---

## Source

Automatically imported from: https://pages.gseis.ucla.edu/faculty/agre/practical.html

## Content

### The Practical Logic of Computer Work

#### Philip E. Agre Department of Information Studies University of California, Los Angeles Los Angeles, California 90095-1520 USA pagre@ucla.edu [http://polaris.gseis.ucla.edu/pagre/](https://web.archive.org/web/20200210084528/http://polaris.gseis.ucla.edu/pagre/) This is a chapter in Matthias Scheutz, ed, *Computationalism: New Directions*, Cambridge: MIT Press, 2002. Please do not quote from this version, which may differ slightly from the version that appears in print. 4700 words.

**1 Inscription errors**

In his reading of John Dee's sixteenth-century commentary on Euclid, Knoespel
(1987) describes what he calls the "narrative matter of mathematics": the
discursive work by which an artifact such as a drawing on paper is exhibited
as embodying a mathematical structure such as a Euclidean triangle. This
process, which is familiar enough to modern technologists as the work of
mathematical formalization, consists of a transformation of language into
something quite different from language, namely mathematics, and its challenge
is to circumvent or erase those aspects of language that are incompatible
with the claim of mathematics to represent the world in a transparent,
unmediated, ahistorical way. Knoespel explains the larger significance of the
point like this:
> ... the reification of geometry in architecture and technology has
> enormous implications for language. Once geometry becomes manifest
> in artifacts, these artifacts retain an authority radically different
> from that accessible to natural language. By virtue of their
> being manifested as physical objects they acquire what appears as an
> autonomy utterly separated from language. The apparent separation of
> both architecture and technology from language has great significance,
> for it works to repress the linguistic framework that has allowed them
> to come into being. (1987: 42)

Brian Smith (1996) makes a similar point when he speaks of "inscription
errors": inscribing one's discourse into an artifact and then turning around
and "discovering" it there. The hidden connections between artifacts and
language are particularly significant in the case of another large category
of artifacts, namely computers. The design of a computer begins with
formalization -- an intensive and highly skilled type of work on language.
A computer is, in an important sense, a machine that we build so that we
can talk about it; it is successful if its operation can be narrated using
a certain vocabulary. As the machine is set to running, we too easily
overlook the complicated reflexive relationship between the designer and user
on which the narratability of the machine's operation depends (see Suchman
and Trigg 1993). The corpus of language that was transformed in producing
the machine, like any discourse or text, is necessarily embedded in an
institutional and historical context, and the machine itself must therefore be
understood as being, in some sense, a text (see Woolgar 1991).

For practitioners of a computational research tradition such as artificial
intelligence (AI), however, the textuality of computers is a distraction at
best, to the extent that it is even comprehensible as an analysis of technical
work. Like John Dee, the practitioners of AI with whom I worked for several
years, and among whom I was trained, regarded formalization very differently,
as a means precisely of freeing their work from the unruliness and imprecision
of vernacular language. They believed that, by defining their vocabulary
in rigorous mathematical terms, they could leave behind the network of
assumptions and associations that might have attached to their words through
the sedimentation of intellectual history. As a result, I want to argue,
the field of AI has been left with no effective way of recognizing the
systemic difficulties that have arisen as the unfinished business of history
has irrupted in the middle of an intendedly ahistorical technical practice.
My purpose in diagnosing this situation is not to discredit mathematics,
technology, or even AI. Instead, I want to envision a critical technical
practice: a technical practice within which such reflection on language and
history, ideas and institutions, is part and parcel of technical work itself
(Agre 1995, 1997a).

**2 Patterns of dissociation**

My point of departure is what AI people themselves have taken to calling
Good Old-Fashioned AI (GOFAI) -- the complex of metaphors and techniques
from which the great majority of the AI literature until recently has begun.
Even those projects that do not fully embrace this standard theory are usually
well understood as incrementally relaxing its assumptions in an attempt to
resolve its seemingly inherent tensions.

This standard theory encompasses, among other things, particular theories of
representation, perception, and action:

> \* The theory of representation holds that knowledge consists in a model
> of the world, formalized (when it *is* formalized) in terms of the
> Platonic analysis of meaning in the tradition of Frege and Tarski. Individual
> things in the world (people, robots, places, tools, blocks, and so on) are
> represented on a one-for-one basis by constant symbols in a formal or informal
> logic, and regularities, conventions, and logical connections in the world are
> represented by quantified propositions.
>
> \* Perception is a kind of inverse optics (Hurlbert and Poggio 1988): building
> a mental model of the world by working backward from sense-impressions,
> inferring what in the world might have produced them. The computational
> neurophysiologist David Marr (1982) gave methodological form to this metaphor
> with his suggestion that the visual cortex consists of a set of modules
> that reconstruct a detailed three-dimensional model of the world by reasoning
> backward from sense impressions to the processes in the world that must have
> produced them.
>
> \* Action, finally, is conducted through the execution of mental constructs
> called plans, understood roughly as computer programs. Plans are constructed
> by searching through a space of potential future sequences of events, using
> one's world models to simulate the consequences of possible actions.

This theory is extraordinarily productive, in the sense that it provides a
plausible starting point for research and model-building on nearly any topic
of human or machine life. It is accordingly the basis of a vast literature.
It is founded in several oppositions, and I want to focus on the specific way
in which these oppositions figure in the history of the field. They are as
follows:

* mind versus world* mental activity versus perception* plans versus behavior* the mind versus the body* abstract ideals versus concrete things

Throughout AI, one encounters a certain pattern in the handling of these
oppositions. I will refer to this pattern as "dissociation". Dissociation
has two moments: an overt distinction between the two terms and a covert
conflation of them. As the language of overt and covert may suggest,
dissociation is not consciously avowed. It must be sought in the internal
tensions of texts and in the dynamics of technical work. Dissociation occurs
in many ways, none of which is fixed or stable. To the contrary, much of
the history of AI can be understood as attempts to comprehend and manage
the signs of trouble that originate in dissociation and that AI practitioners
can recognize within the conceptual system of the field. One purpose of a
critical technical practice is to recognize such troubles more fully and to
diagnose them more deeply.

It would be impossible to demonstrate in the entire literature of AI the
workings of the five dissociations that I enumerated above. Each AI text
needs to be treated on its own terms, and no strong generalizations are
possible. Instead, I will review the workings of the five dissociations
as they become manifest in particular texts and projects. It would require
a separate and much larger effort to trace the evolution of the various
dissociations through the historical development of the literature.

**3 Mind versus world**

The distinction between mind and world has obviously been construed in many
ways by different philosophical systems, but in AI it has been operationalized
in terms of a sharp qualitative distinction between the inside of the machine
and the world outside. This image of the mind as an internal space, what
Lakoff and Johnson (1980) call the "container" metaphor, underlies a large
proportion of the discourse of AI (Agre 1997a). The difficulty is that
it is hard to maintain accurate knowledge of a world that is understood to
be so distinct (compare Bordo 1987). Viewed at such a distance, the world
seems profoundly uncertain, and the likelihood that other people and things
will change the world according to their own agendas makes ordinary life seem
nearly impossible.

As a result, it is a common idealization in the field to suppose that
one's world model is complete in every relevant respect and stays up-to-date
automatically. Mind and world, having been distinguished at the outset, are
covertly conflated in the very concept of a world model -- a simulacrum of
the world in one's head. This conflation of mind with world is facilitated by
the use of research "domains", such as geometry, which are readily understood
in mathematical terms (compare Walkerdine 1988). This practice first took
hold with the work on logical theorem proving by Newell, Shaw, and Simon
(1960), and on chess by Newell and Simon (1963). Even in domains that
involve physical objects, it is common for AI people (and computer scientists
in general) to employ the same words to name both the representations in a
machine and the things that those representations represent. The erasure of
language that Knoespel discovered in Dee is here employed on a grand scale to
facilitate the conflation, not just of mathematics and the physical world, but
of representation and reality in general.

The point is not that AI researchers do this deliberately. Quite the
contrary, their work is well understood as an attempt *not* to do
it. Having acquired the conflation of mind and world through the discursive
practices they inherited from earlier intellectual projects, AI researchers
continually find the conflation reinforced through the practical logic of
their research. If I may risk a mathematical metaphor, the dissociative
relationship between mind and world is an attractor: although unsatisfactory
as a theory of human life, the dissociation is also difficult to escape by
incremental modifications because the covert conflation of mind and world
solves, even if pathologically, a problem for which no less pathological
solution is known. The mathematical metaphor here is misleading, though, in
that the terrain is a function of consciousness: which "moves" in the space of
research proposals seem comprehensible and well motivated is itself a function
of the critical awareness through which the symptoms of technical trouble are
perceived and interpreted. The point, therefore, is not that AI researchers
believe that the mind and world are the same, or that they are incapable
of grasping the idea that they are different. Rather, practices that tend
to conflate the two are dispersed throughout the discourse and practices
of the field; one is socialized into the discourse and practices through
one's training in the field, and field does not provide the critical tools
that would be necessary to detect this pattern and reverse it. So long as
the larger pattern remains ungrasped, the attractor retains its grip on the
research.

**4 Mental activity versus perception**

AI originated as part of the cognitivist movement whose other was behaviorism.
In combatting the behaviorist hegemony, the task of cognitivism was to present
itself as scientific by the same standard as behaviorism did, while also
opposing itself as squarely as possible to behaviorism on a substantive
level. As Karl Lashley noted in an influential early symposium paper (1951),
the behaviorist theory of action was stimulus-chaining: the idea that each
action in a serially ordered sequence arises as a response to, among other
things, the effects of the previous action in the sequence. Lashley, however,
observed that the elementary actions involved in speech -- individual phonemes
and words -- have no necessary relation to one another. The same phoneme,
for example, might be found adjacent to a large number of other phonemes in
the context of particular words (1951: 115-116). It is therefore impossible
that stimulus-response connections among particular linguistic elements could
explain the ways in which they are arranged in any particular utterance. He
therefore urged that serially ordered action must be understood in terms of an
internal organizing principle.

In his effort to oppose himself to the behaviorist story, Lashley equivocates
on the role of perception in organizing behavior. A fair-minded reader
will reconstruct his argument as advocating a two-factor theory of behavior:
continual perceptual inputs into the ongoing mental process (1951: 112, 131),
and continual outputs from that process in the form of spoken phonemes and
other actions drawn from a language-like repertoire. But in fact Lashley
provides little substantive account of the role of perception, emphasizing
instead that serial behavior is planned and organized in advance and performed
in scripted wholes. What is more, his use of language as a paradigm case
of action leaves little room for perceptual input. He imagines linguistic
utterances to arise through the interaction of three factors: the "expressive
elements", including phonemes and words, a "determining tendency" that encodes
the information to be conveyed without itself having any internal structure,
and the "syntax of the act", which he defines as:
> an habitual order or mode of relating the expressive elements; a
> generalized pattern or schema of integration which may be imposed
> upon a wide range and a wide variety of specific acts (1951: 122).

Thus begins the practice in cognitive science of using language, and
specifically the production of grammatical utterances, as the prototypical
case of human action. Note, however, that the resulting pattern of behavior
results solely from the idea one wishes one's actions to "express", and not
from any stimulus in the world. This restriction can go unnoticed in the
case of language because phonemes and words follow one another so rapidly,
and their formal relationships are so densely organized, that the outside
world has little time to influence their ordering. Of course, the ongoing
interaction between speakers and hearers *can* influence an utterance as
it unfolds (Goodwin 1981), but this idea plays no role in Lashley's argument,
nor indeed in the mainstream of cognitive science.

Dissociation in Lashley takes a distinct form: rather than uniting bodily
through systematic ambiguity, the two terms are brought together in two
separate theories that are then superimposed. One of these theories
envisions action arising through a formal order being imposed on a population
of expressive elements; this theory of the mental scripting of action is given
the more overt billing. The other theory imagines the mind to be a holistic
process -- "a great network of reverberatory circuits, constantly active"
(1951: 131) -- into which perception is simply one more influence among many.
The two theories are attached at various points, but not so closely that the
impossibility of perception's role ever becomes obtrusive.

**5 Plans versus behavior**

Although rarely cited in the modern literature, the locus classicus for
AI discussion of plans is Miller, Galanter, and Pribram's *Plans and the
Structure of Behavior* (1960). Miller, Galanter, and Pribram's starting
point, like Lashley's, was the intellectual dominance of behaviorism.
Their organizing question, therefore, is whether something must be imagined
to mediate between the observable categories of stimulus and response.
They find half of their answer in Boulding's (1956) notion of "the Image"
-- a vague precursor to the concept of a world model. They observe that the
Image explains knowledge and not action, and they ask why behavior has any
structure. The reason, they suggest (1960: 16), is because behavior arises
from a mental entity that has that same structure, namely a Plan. (They
capitalized the word.) They, like Lashley, would seem to have shifted from
a theory whose only explanatory factor is perception to a theory in which
perception, and thus the outside world as a whole, plays no role at all.

Although it is openly speculative and presents no computer demonstrations or
laboratory experiments of its own, *Plans and the Structure of Behavior*
served as a rhetoric for the emerging cognitivist movement. Its most
distinctive rhetorical device was a systematic conflation of behavior and
Plans. To this day, it is customary in AI research to refer to any structure
in behavior as a plan (lower case now, but with the same meaning), not as a
hypothesis but as a simple matter of terminology. Thus, for example, Cohen
et al (1989: 40; cited by Vera and Simon 1993: 26), echoing the earliest
arguments of Lashley and Miller, Galanter, and Pribram, ascribe to my own
work (Agre and Chapman 1987) the idea that "longer-term plans can emerge from
compositions of reflexes". The very suggestion is not coherent unless "plans"
(in the mind) are confused with "sequences of action" (in the world).

In fact, Miller, Galanter, and Pribram took Lashley's dissociation between
perception and thought a step further. Close reading demonstrates the
presence of two distinct theories: one speaking of discrete, prescripted Plans
and another speaking of a single Plan that unfolds incrementally through time.
Thus, for example, having defined their concept of a Plan as something like a
computer program that controls behavior, they casually amend their definition
by saying:
> Moreover, we shall also use the term "Plan" to designate a rough
> sketch of some course of action, just the major topic headings in the
> outline, as well as the completely detailed specification of every
> detailed operation (1960: 17).

The former theory, the one that describes a repertoire of discrete Plans, is
the official theory: it is the theory that explains the structure of behavior.
Yet it is an unsatisfactory theory in many ways. Computer programs, for
example, do need to be spelled out far in advance, and they must anticipate
every possible contingency of their execution; and so the official theory is
overlaid with the unofficial theory of a single Plan that can be constructed
in a more improvisational manner as an ongoing response to perception. The
authors return to the matter again by offering a theory of Plans based on
then-current ideas of servocontrol (1960: 26-39). This third theory -- the
so-called TOTE units (test, operate, test, exit) that supposedly provide a
"unit of analysis" for Plans -- is laid atop the earlier two with little overt
sense of their incompatibility; in any case, it is the equivocal relation
between the first two theories that set the agenda for subsequent research.

Most of this subsequent research focused exclusively on the construction of
discrete plans (Allen, Hendler, and Tate 1990; Georgeff 1987), thus obviating
the need for a theory of improvisation. It is, however, computationally very
difficult to construct a Plan that will work reliably in a world of any great
complexity. The problem is not precisely the size of the space of possible
plans, since subtle use of probabilistic search techniques can overwhelm even
quite large planning search problems (Gomes, Selman, and Kautz 1998). Rather,
in a dynamic world it is essentially impossible to know everything that
would be needed to conduct such a search. As a result, the second of Miller,
Galanter, and Pribram's theories -- the incremental, on-the-fly construction
of a partial Plan -- resurfaced in the form of "reactive planning" in the
1980's (e.g., Firby 1987, Fox and Smith 1984). One term of the dissociation,
having been suppressed, returned. Yet when it did so, its internal
relationship to the dominant theory was hardly recognized, and research
in that era saw several attempts to resynthesize the two approaches (e.g.,
Payton, Rosenblatt, and Keirsey 1990), reproducing in the architecture
of cognitive models the conflation that occurred more covertly in Miller,
Galanter, and Pribram's text.

**6 The mind versus the body**

The AI literature often dissociates mind and body, and here again the covert
conflation between the two terms takes a different form. It can be seen
in the first computer implementation of the plans-and-execution theory,
the STRIPS model of Fikes, Hart, and Nilsson (1972), which automatically
constructed plans and then executed them by directing the movements of a
robot. These authors' dilemma is that it is hard to predict in enough detail
how the world will unfold as the robot executes its plans, and yet it is so
expensive to construct a new plan that it seems necessary to execute as much
of each plan as possible. At one point they suggest simply executing the
first step of each new plan and then constructing a new plan from scratch,
but they reject the idea as impractical.
> One of the novel elements introduced into artificial intelligence
> research by work on robots is the study of execution strategies
> and how they interact with planning activities. Since robot plans
> must ultimately be executed in the real world by a mechanical
> device, as opposed to being carried out in a mathematical space
> or by a simulator, consideration must be given by the executor to
> the possibility that operations in the plan may not accomplish what
> they were intended to, that data obtained from sensory devices may
> be inaccurate, and that mechanical tolerances may introduce errors
> as the plan is executed.
>
> *Many of these problems of plan execution would disappear if
> our system generated a whole new plan after each execution step.
> Obviously, such a strategy would be too costly*, so we instead seek
> a plan execution scheme with the following properties:
>
> 1. When new information obtained during plan execution implies that
> some remaining portion of the plan need not be executed, the executor
> should recognize such information and omit the unneeded plan steps.
>
> 2. When execution of some portion of the plan fails to achieve the
> intended results, the executor should recognize the failure and either
> direct reexecution of some portion of the plan or, as a default,
> call for a replanning activity. (Fikes, Hart, and Nilsson 1972: 268;
> emphasis added)

The dissociation between the mind, which constructs plans, and the body, which
executes them, manifests itself here in a seeming attempt by planning and
execution to become reunited into a single compound process, or at least to
become intertwined with one another in rapid alternation. The impracticality
of the dissociation is revealed through the process of system-building.

It is here, in the design and construction of systems, that AI learns most
of its lessons, and not in formal experimentation with the systems once they
are running. If I seem to anthropomorphize the desire of mind and body to
reverse their dissociation, this is only to give voice to a common experience
of system designers: the tangible pressures that seem to push the design
process in one direction or another.

**7 Abstract ideals versus concrete things**

The final dissociation is between abstraction and concrete reality in the
tradition of Fregean semantics. Historically, theories of semantics have
drifted between two poles: psychologism, the theory that meanings are mental
entities, and Platonism, the theory that meanings reside in a timeless,
extensionless realm of ideals. Yet this distinction has made remarkably
little difference in practice. The mind, as it has been constructed through
the system of dissociations that I have already described, resembles the realm
of Platonic ideals in many ways. The use of mathematical domains helps to
blur the distinction between Platonic ideals and real human ideas, inasmuch as
mathematical entities resemble Platonic ideals and are now routinely employed
to formalize Platonic theories of the semantics of both language and logic.

The problem arises whenever the mind must be understood as participating
in the historical, causal world. The problem manifests itself in many ways,
but it can be clearly grasped already in Frege's own theory. Frege's theory
of sense, that is, the cognitive content of a representation, conflates
incompatible goals. The sense of a representation is supposed to be a
Platonic ideal, independent of place and time, and yet it is also held to
incorporate specific objects such as a car or a person. The problem is
particularly acute in the case of indexical representations, whose sense is
plainly dependent on the concrete historical circumstances of their use. I
can use words like "here" and "now" perfectly well without knowing where I am
or what time it is, and yet the sense of my utterance involves those specific
places and times. The trouble arises because Frege's theory of sense,
and a whole subsequent tradition of semantic theories, attempts to capture
the content of thoughts and utterances without reference to the embodied
activities and relationships with which they are used. Burge (1979: 426)
summarizes the problem:
> Frege appears to be caught between two objectives that he had for
> his notion of sense. He wanted the notion to function as conceptual
> representation for a thinker (though in principle accessible to
> various thinkers, except in special cases). And he wanted it uniquely
> to determine the referents of linguistic expressions and mental or
> linguistic acts. The problem is that people have thoughts about
> individuals that they do not individuate conceptually.

As the realm of Platonic abstractions is conflated with the realm of concrete
activity, the semantic formalism takes on a covertly material character and
the theory of mind takes on a covertly disembodied character.

**8 Conclusion**

These, then, are five dissociations that have organized the practical logic
of research within the leading tradition of artificial intelligence. The
interaction among these dissociations defines a complex and variegated field
whose contradictory pressures must be reconciled somehow in each project
in its own unique way. In most cases I have chosen particular projects to
illustrate the practical logic of dissociation. Other projects may well be
discovered to manage the tensions in a different way. Yet few AI projects,
if any, have reflected a systematic understanding of them, much less any
resolution.

Where do these dissociations originate? Do all conceptual distinctions lead
to dissociations when they are embodied in technical work? When AI work is
framed in terms of these dissociations, it becomes obvious that AI is part
of the history of Western thought. It has inherited certain discourses from
that history about matters such as mind and world, and it has inscribed those
discourses in computing machinery. The whole point of this kind of technical
model-building is conceptual clarification and empirical evaluation, and
yet AI has failed either to clarify or to evaluate the concepts it has
inherited. Quite the contrary, by attempting to transcend the historicity
of its inherited language, it has blunted its own awareness of the internal
tensions that this language contains. These tensions have gone underground,
emerging through substantive assumptions, linguistic ambiguities, theoretical
equivocations, technical impasses, and ontological confusions.

Yet the project of artificial intelligence has not been a failure. The
discipline of technical implementation, considered in another way, really has
done its job. The dissociations of AI have refused to go away, and in the
practical work of model-building they have ceaselessly reasserted themselves.
As AI practitioners have tried to manage all of the many cross-cutting
tensions in their work, they have made the generative principle of
those tensions ever more visible to those with the critical means to look.
This is the motivation for my advocacy of a critical technical practice and
the basis of my positive hopes for it. Bad theories of human existence, we
might conjecture, do not simply fail to correspond to the data; they are in
fact impracticable, in that nobody and nothing could live in the ways they
describe. As AI people learn to expand their understanding of the ways in
which a system can "work" or "not work", AI can perhaps become a means of
listening to reality and of learning from it. The key to this transition is
a reversal of the ideological function of technology that Knoespel described
at the outset. The texts that we inscribe in computing machinery are texts
in the fullest sense. In particular, they always have greater depths than we
are aware of, and they always encode sophisticated strategies for managing the
contradictory experience of the world that we have inherited from the past.
Computers and formalization do not eliminate all this; quite the contrary,
they make it more visible.

And what exactly has AI made visible in this fashion? Running through
all of the dissociations I mentioned is a recurring theme, a kind of
transcendentalism that attempts to hold something apart from and above
material reality. The transcendentalist philosophy of AI is that the outside
world is, to use the military language that AI took over during the 1980's
(Hendler 1990), uncertain, unpredictable, and changing. The dissociations
portray the world as a negative, chaotic principle and the mind as a positive,
ordering principle. What we might tentatively conclude, in the irreducibly
intuitive and practical way in which such conclusions might possibly be
drawn from technical work, is that it doesn't work that way. If not for
the positive ordering principles inherent in the world itself, life would
be impossible. Man, in this traditional sense, can live not by imposing
order, but only by participating in it. Only from this standpoint amid the
order of the world does the world itself become visible; only then does the
question usefully arise of how best to live in the world, and how best to
change it.

**Bibliography**

Philip E. Agre and David Chapman, Pengi: An implementation of a theory
of activity, *Proceedings of the Sixth National Conference on Artificial
Intelligence*, Seattle, 1987, pages 196-201.

Philip E. Agre, The soul gained and lost: Artificial intelligence as a
philosophical project, *Stanford Humanities Review* 4(2), 1995, pages
1-19.

Philip E. Agre, Toward a critical technical practice: Lessons learned in
trying to reform AI, in Geoffrey C. Bowker, Susan Leigh Star, William Turner,
and Les Gasser, eds, *Social Science, Technical Systems and Cooperative Work:
Beyond the Great Divide*, Erlbaum, 1997a.

Philip E. Agre, *Computation and Human Experience*, Cambridge: Cambridge
University Press, 1997b.

James Allen, James Hendler, and Austin Tate, eds, *Readings in Planning*,
Los Altos, CA: Morgan Kaufmann, 1990.

Susan Bordo, *The Flight to Objectivity: Essays on Cartesianism and
Culture*, Albany: State University of New York Press, 1987.

Kenneth E. Boulding, *The Image: Knowledge in Life and Society*, Ann
Arbor: University of Michigan Press, 1956.

Tyler Burge, *Sinning Against Frege*, Philosophical Review 88(4), 1979,
pages 398-432.

Paul Cohen, Michael L. Greenberg, David M. Hart, and Adele E. Howe,
Trial by fire: Understanding the design requirements for agents in complex
environments, *AI Magazine* 10(3), 1989, pages 32-48.

Richard E. Fikes, Peter E. Hart, and Nils J. Nilsson, Learning and executing
generalized robot plans, *Artificial Intelligence* 3(4), 1972, pages
251-288.

R. James Firby, An investigation into reactive planning in complex
domains, in *Proceedings of the Sixth National Conference on Artificial
Intelligence*, Seattle, 1987, pages 202-206.

Mark S. Fox and Stephen Smith, ISIS: A knowledge-based system for factory
scheduling, *Expert Systems* 1(1), 1984, pages 25-49.

Michael P. Georgeff, Planning, in Joseph F. Traub, Barbara J. Grosz, Butler
W. Lampson, and Nils J. Nilsson, eds, *Annual Review of Computer Science*
2, Palo Alto, CA: Annual Reviews Inc., 1987, pages 359-400.

Carla P. Gomes, Bart Selman, and Henry Kautz, Boosting combinatorial search
through randomization, *Proceedings of the Fourtheenth National Conference
on Artificial Intelligence*, Madison, WI, 1998.

Charles Goodwin, *Conversational Organization: Interaction between Speakers
and Hearers*, New York: Academic Press, 1981.

James Hendler, ed, *Planning in Uncertain, Unpredictable, or Changing
Environments, Proceedings of the AAAI Symposium at Stanford*, University
of Maryland Systems Research Center Report SRC TR 90-45, 1990.

Anya Hurlbert and Tomaso Poggio, Making machines (and artificial
intelligence) see, *Daedalus* 117(1), 1988, pages 213-239.

Kenneth J. Knoespel, The narrative matter of mathematics: John Dee's
preface to the *Elements* of Euclid of Megara (1570), *Philological
Quarterly* 66(1), 1987, pages 27-46.

George Lakoff, and Mark Johnson, *Metaphors We Live By*, Chicago:
University of Chicago Press, 1980.

Karl S. Lashley, The problem of serial order in behavior, in Lloyd
A. Jeffress, ed, *Cerebral Mechanisms in Behavior: The Hixon Symposium*,
New York: Wiley, 1951.

David Marr, *Vision*, San Francisco: Freeman, 1982.

George A. Miller, Eugene Galanter, and Karl H. Pribram, *Plans and the
Structure of Behavior*, New York: Henry Holt and Company, 1960.

Allen Newell, J. C. Shaw, and Herbert A. Simon, Report on a general
problem-solving program, in *Proceedings of the International Conference
on Information Processing*, Paris, 1960, pages 256-264.

Allen Newell and Herbert A. Simon, GPS, a program that simulates human
thought, in Edward A. Feigenbaum and Julian Feldman, eds, *Computers and
Thought*, New York: McGraw-Hill, 1963, pages 279-293. Originally published
in 1961.

David W. Payton, J. Kenneth Rosenblatt, and David M. Keirsey, Plan guided
reaction, *IEEE Transactions on Systems, Man, and Cybernetics* 20(6),
1990, pages 1370-1382.

Brian C. Smith, *On the Origin of Objects*, Cambridge: MIT Press, 1996.

Lucy A. Suchman and Randall H. Trigg, Artificial intelligence as craftwork,
in Seth Chaiklin and Jean Lave, eds, *Understanding Practice: Perspectives
on Activity and Context*, Cambridge: Cambridge University Press, 1993.

Valerie Walkerdine, *The Mastery of Reason: Cognitive Development and the
Production of Rationality*, London: Routledge, 1988.

Steve Woolgar, Configuring the user: The case of usability trials, in
John Law, ed, *A Sociology of Monsters: Essays on Power, Technology and
Domination*, London: Routledge, 1991.