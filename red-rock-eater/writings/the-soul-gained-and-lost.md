---
id: the-soul-gained-and-lost
title: "The Soul Gained and Lost"
type: writing
tags:
- agre-primary
- ai-critique
- philosophy
- phenomenology
- split-identity
- planning-paradigm
links:
- target: ai-s-philosophical-unconscious
  relation: develops
  note: Primary essay developing the concept
  kb: red-rock-eater
- target: critical-technical-practice
  relation: develops
  note: Philosophical grounding for why CTP is necessary
  kb: red-rock-eater
- target: lessons-learned-in-trying-to-reform-ai
  relation: related_to
  note: Companion essays — Soul is philosophical, Lessons is methodological
  kb: red-rock-eater
metadata:
  importance: 5
  writing_type: paper
  url: "https://pages.gseis.ucla.edu/faculty/agre/shr.html"
  coauthors: &id001 []
  key_concepts: &id002 []
  research_status: stub
importance: 5
writing_type: paper
url: "https://pages.gseis.ucla.edu/faculty/agre/shr.html"
coauthors: *id001
key_concepts: *id002
research_status: stub
---

## Source

Automatically imported from: https://pages.gseis.ucla.edu/faculty/agre/shr.html

## Content

### The Soul Gained and Lost: Artificial Intelligence as a Philosophical Project

#### Philip E. Agre Department of Information Studies University of California, Los Angeles Los Angeles, California 90095-1520 USA pagre@ucla.edu [http://polaris.gseis.ucla.edu/pagre/](https://web.archive.org/web/20191212194545/http://polaris.gseis.ucla.edu/pagre/) This paper appeared in a slightly different form in a special issue of the Stanford Humanities Review, entitled "[Constructions of the Mind: Artificial Intelligence and the Humanities](https://web.archive.org/web/20191212194545/http://www.stanford.edu/group/SHR/4-2/text/toc.html)", edited by Guven Guzeldere and Stefano Franchi. The official citation is *Stanford Humanities Review* 4(2), 1995, pages 1-19. 9400 words.

**1 Introduction** 

When I was a graduate student in artificial intelligence, the humanities
were not held in high regard. They were vague and woolly, they employed
impenetrable jargons, and they engaged in "meta-level bickering that never
decides anything". Although my teachers and fellow students were almost
unanimous in their contempt for the social sciences, several of them (not
all, but many) were moved to apoplexy by philosophy. Periodically they would
convene impromptu Two-Minute Hate sessions to compare notes on the arrogance
and futility of philosophy and its claims on the territory of AI research.
"They've had two thousand years and look what they've accomplished. Now it's
our turn." "Anything that you can't explain in five minutes probably isn't
worth knowing." They distinguished between "just talking" and "doing", where
"doing" meant proving mathematical theorems and writing computer programs. A
new graduate student in our laboratory, hearing of my interest in philosophy,
once sat me down and asked in all seriousness, "Is it true that you don't
actually do anything, that you just say how things are?" It was not, in fact,
true, but I felt with great force the threat of ostracism implicit in the
notion that I was "not doing any real work".

These anecdotes may provide some sense of the obstacles facing any attempt at
collaboration between AI and the humanities. In particular, they illustrate
certain aspects of AI's conception of itself as a discipline. According to
this self-conception, AI is a self-contained technical field. In particular,
it is a practical field; to do AI is to prove theorems, write software,
and build hardware whose purpose is to "solve" previously defined technical
"problems". The whole test of these activities lies in "what works". The
criterion of "what works" is straightforward, clear, and objective in the
manner of engineering design; arguments and criticisms from outside the field
can make no claim at all against it. The substance of the field consists
in the "state of the art" and its history is a history of computer programs.
The technical methods underlying these programs might have originated in other
fields, but the real work consisted in formalizing, elaborating, implementing,
and testing those ideas. Fields which do not engage in these painstaking
activities, it is said, are sterile debating societies which do not possess
the intellectual tools -- most particularly mathematics -- to do more than
gesture in the general direction of an idea, as opposed to really working it
out.

I will be thought to exaggerate. Technicians will protest their respect
for great literature and the attitudes I have reported will be put down to
a minority of fundamentalists. Yet the historical record makes plain that
interactions between AI and the humanities have been profoundly shaped by
the disciplinary barriers that such attitudes both reflect and reproduce.
Serious research in history and literature, for example, has had almost
no influence on AI. This is not wholly due to ignorance on the part of
technical people, many of whom have had genuine liberal educations. Rather
AI, as a technical field, is constituted in such a way that its practitioners
honestly cannot imagine what influence those fields *could* have.

Philosophy has had a little more influence. Research on AI's constitutive
questions in the philosophy of mind is widely read and discussed among AI
research people, and is sometimes included in the curriculum, but these
discussions are rarely considered part of the work of AI, judging for example
by journal citations, and any influence they might have had on the day-to-day
work of AI has been subtle at best. Contemporary ideas from the philosophies
of language and logic have been used as raw material for AI model-making,
though, and philosophers and technical people have collaborated to some degree
in specialized research on logic.

Perhaps the principal humanistic influence on AI has derived from a small
number of philosophical critics of the field, most particularly Hubert
Dreyfus (1972). For Dreyfus, the project of writing "intelligent" computer
programs ran afoul of the critique of rules in Wittgenstein (1968 [1953])
and Heidegger's (1961 [1927]) analysis of the present-at-hand way of relating
to beings (in this case, symbolic rules). The use of a rule in any practical
activity, Dreyfus argues, requires a prior participation in the culturally
specific form of life within which such activities take place. The attempt
to fill in the missing "background knowledge" through additional rules would
suffer the same problem and thus introduce a fatal regress [[1](#endnote1)]. Although most senior AI researchers of my acquaintance
stoutly deny having been affected by Dreyfus' arguments, a reasonable amount
of research has addressed the recurring difficulties with AI research that
Dreyfus predicted. One of these is the "brittleness" of symbolic, rule-based
AI systems that derives from their tendency to fail catastrophically in
situations that depart even slightly from the whole background of operating
assumptions that went into the system's design. For the most part, the
response of AI researchers to these difficulties, and to Dreyfus' analyses
generally, is to interpret them as additions to AI's agenda that require no
fundamental rethinking of its premises [[2](#endnote2)].

Within the field itself, critical reflection is largely a prerogative of the
field's most senior members, and even these papers are published separately
from the narrowly technical reports, either in non-archival publications like
the *AI Magazine* or in special issues of archival publications devoted
to the founders' historical reflections. In 1990 I received a referee's
report on a AAAI (American Association for Artificial Intelligence) conference
paper that read in part,
> In general, avoid writing these "grand old man" style papers until you've
> built a number of specific systems & have *become* a grand old man.

The boundaries of "real AI research", in short, have been policed with great
determination.

Yet this is now changing. In part the current changes reflect sociological
shifts in the field, in particular its decentralization away from a few
heavily funded laboratories and the resulting, albeit modest, trend toward
interdisciplinary pluralism. But the change in atmosphere has also been
influenced by genuine dissatisfactions with the field's original technical
ideas. AI's practices of formalizing and "working out" an idea constitute
a powerful method of inquiry, but precisely for this reason they are also
a powerful way to force an idea's internal tensions to the surface through
prolonged technical frustrations: excessive complexity, intractable
inefficiency, difficulties in "scaling up" to realistic problems, and so
forth. These patterns of frustration have helped clear the ground for a
new conception of technical work, one that recognizes the numerous, deep
continuities between AI and the humanities. Although these continuities
reach into the full range of humanistic inquiry, I will restrict myself here
to the following five assertions about AI and its relationship to philosophy:

1. AI ideas have their genealogical roots in philosophical ideas.- AI research programs attempt to work out and develop the philosophical
     systems they inherit.- AI research regularly encounters difficulties and impasses that derive
       from internal tensions in the underlying philosophical systems.- These difficulties and impasses should be embraced as particularly
         informative clues about the nature and consequences of the philosophical
         tensions that generate them.- Analysis of these clues must proceed outside the bounds of strictly
           technical research, but they can result in both new technical agendas and in
           revised understandings of technical research itself.

In short, AI is philosophy underneath. These propositions are not entirely
original, of course, and some version of them underlies Dreyfus' early
critique of the field. My own purpose here is to illustrate how they might
be fashioned into a positive method of inquiry that maintains a dialogue
between the philosophical and technical dimensions of AI research. To this
end, I will present a brief case study of one idea's historical travels from
philosophy through neurophysiology and into AI, up to 1972. Although much of
this particular story has been told many times, some significant conclusions
from it appear to have escaped analysis. It is an inherently difficult story
to tell, since it requires a level of technical detail that may intimidate the
uninitiated without nearly satisfying the demands of initiates. It is a story
worth telling, though, and I will try to maintain a firm sense of the overall
point throughout. I will conclude by briefly discussing recent developments
that have been motivated in part by critical reevaluations of this tradition,
and by sketching the shape of the new, more self-critical AI that is emerging
in the wake of this experience.

**2 Rene Descartes: Criteria of intelligence** 

In a famous passage in his *Discourse on Method*, Descartes summarizes a
portion of his suppressed treatise on *The World* as follows:
> ... the body is regarded as a machine which, having been made by the hands
> of God, is incomparably better arranged, and possesses in itself movements
> which are much more admirable, than any of those which can be invented by
> man. ... if there had been such machines, possessing the organs and outward
> form of a monkey or some other animal without reason, we should not have
> had any means of ascertaining that they were not of the same nature as those
> animals. On the other hand, if there were machines which bore a resemblance
> to our body and imitated our actions as far as it was morally possible to do
> so, we should always have two very certain tests by which to recognize that,
> for all that, they were not real men. The first is, that they could never
> use speech or other signs as we do when placing our thoughts on record
> for the benefit of others. For we can easily understand a machine's being
> constituted so that it can utter words, and even emit some responses to
> action on it of a corporeal kind, which brings about a change in its organs;
> for instance, if it is touched in a particular part it may ask what we wish
> to say to it; if in another part it may exclaim that it is being hurt, and
> so on. But it never happens that it arranges its speech in various ways, in
> order to reply appropriately to everything that may be said in its presence,
> as even the lowest type of man can do. And the second difference is, that
> although machines can perform certain things as well as or perhaps better
> than any of us can do, they infallibly fail short in others, by the which
> means we may discover that they did not act from knowledge, but only from
> the disposition of their organs. For while reason is a universal instrument
> which can serve for all contingencies, these organs have need of some special
> adaptation for every particular action. From this it follows that it is
> morally impossible that there should be sufficient diversity in any machine
> to allow it to act in all the events of life in the same way as our reason
> causes us to act (page 116).

It is worth quoting Descartes' words at such length because they contained
the seeds of a great deal of subsequent intellectual history. Distinctions
between the body and the soul were, of course, of great antiquity, as was the
idea that people could be distinguished from animals by their reasoned use of
language. Descartes, though, extended these ideas with an extremely detailed
physiology. His clearly drawn dualism held that automata, animals, and the
human body could all be explained by the same mechanistic laws of physics,
and he set about partitioning functions between body and mind [[3](#endnote3)] [[4](#endnote4)]. In establishing this
partition, one of the tests was the conventional distinction between animal
capabilities, which reside in the body, and specifically human capabilities,
which required the exercise of the soul's faculties of reason and will.
Thus, for example, automata or animals might utter isolated words or phrases
in response to specific stimuli, but lacking the faculty of reason they
could not combine these discrete units of language in an unbounded variety of
situationally appropriate patterns. The soul itself has ideas, but it has no
physical extent or structure. Thus, as Descartes explains in *The Passions
of the Soul* (Articles 42 and 43), memory is a function of the brain; when
the soul wishes to remember something, it causes animal spirits to propagate
to the spot in the brain where the memory is stored, whereupon the original
image is presented once again to the soul in the same manner as a visual
perception.

The attraction of Descartes' proposals lay not in their particulars, many of
which were dubious even to his contemporaries. Rather, Descartes provided
a model for a kind of theory-making that contrasted with late scholastic
philosophy in every way: it was specific and detailed, it was grounded in
empirical physiology, and it was written in plain language.

**3 Karl Lashley: Language as a model for action** 

The American cognitivists of the 1950's often modeled themselves after
Descartes, and they intended their research to have much of the same appeal.
Despite the intervening three centuries, the lines of descent are indeed
clear. This is evident in the case of Chomsky, for example, who argued in
explicitly Cartesian terms for a clear distinction between the physiology
of speech, including the biological basis of linguistic competence, and the
capacity for actually choosing what to say. While not a dualist, Chomsky
nonetheless epitomized his conception of human nature in terms of "free
creation within a system of rule" (1971: 50). Miller (1956) used Descartes'
*Rules for the Direction of the Mind* to motivate his search for ways
that people might more efficiently use their limited memories.

The first and most influential revival of research into mental mechanisms,
Karl Lashley's 1951 paper "The problem of serial order in behavior",
did not acknowledge any sources beyond the linguistics, psychology, and
neurophysiology of the 1940's. Nonetheless, the underlying continuities are
important for the computational ideas that followed. Despite his own complex
relationship to behaviorism, Lashley's paper argued clearly that behaviorist
psychology could not adequately explain the complexity of human behavior.
Lashley focused on a particular category of behavior, namely speech. He
pointed out that linguists could demonstrate patterns to the grammar and
morphology of human languages that are hard to account for using the theory
of "associative chains", whereby each action's effects in the world give rise
to stimuli that then trigger the next action in turn. The formal structures
exhibited by human language, then, were sufficient reason to restore some
notion of mental processing to psychology.

Moreover, Lashley suggested that *all* action be understood on the
model of language. He regarded both speech and physical movement as having a
"syntax", and he sought the physiological basis of both the syntax of movement
and the choice of specific movements from among the syntactically possible
combinations. This suggestion was enormously consequential for the subsequent
development of cognitivist psychology, and particularly for AI. Lashley
summarized the idea in this way:
> It is possible to designate, that is, to point to specific examples of, the
> phenomena of the syntax of movement that require explanation, although those
> phenomena cannot be clearly defined. A real definition would be a long step
> toward solution of the problem. There are at least three sets of events
> to be accounted for. First, the activation of the expressive elements
> (the individual words or adaptive acts) which do not contain the temporal
> relations. Second, the determining tendency, the set, or idea. This
> masquerades under many names in contemporary psychology, but is, in every
> case, an inference from the restriction of behavior within definite limits.
> Third, the syntax of the act, which can be described as an habitual order
> or mode of relating the expressive elements; a generalized pattern or schema
> of integration which may be imposed upon a wide range and a wide variety of
> specific acts. This is the essential problem of serial order; the existence
> of generalized schemata of action which determine the sequence of specific
> acts, acts which in themselves or in their associations seem to have no
> temporal valence (Lashley 1951: 122).

Two things are new to cognitive theorizing here, grammar as a principle of
mental structure and the generalization of grammatical form to all action.
But a great deal in Lashley's account is continuous with that of Descartes.
To start with, it is an attempt at an architecture of cognition. Indeed, it
is considerably less detailed than Descartes' architecture, although Descartes
provided no account of the mechanics of speech. Both Lashley and Descartes
assign the ability to speak individual words -- or in Lashley's case, to make
individual discrete physical movements -- to individual bits of machinery,
without being very specific about what these bits of machinery are like.
And they both view the human capacity for putting these elements together as
the signature of the mind. To be sure, Lashley's argument rests on the formal
complexity of speech whereas Descartes points at the appropriateness of each
utterance to the specific situation. In each case, though, what counts is the
capacity of the mind to order the elements of language in an unbounded variety
of ways.

The continuities go deeper. Lashley, as a neurophysiologist, shows no signs
of believing in an ontological dualism such as Descartes'. Yet the conceptual
*relations* among the various components of his theory are analogous to
those of Descartes. In each case, the brain subserves a repertoire of bodily
capacities, and on every occasion the mind orders these in accord with its
choices, which themselves are not explained. For Descartes the mind's choices
simply *cannot* be explained in causal terms, though its operations can
be described in the normative terms of reason, as for example in his *Rules
for the Direction of the Mind*. Lashley does not express any overt
skepticism about his "determining tendency", but neither does he have anything
very definite to say about it; the concept stays nebulous throughout. This is
not simply an incompleteness of Lashley's paper but is inherent in its design:
the purpose of the determining tendency is not to *have* structure in
itself but to *impose* structure upon moment-to-moment activities from
the repertoire of action schemata made available to it by the brain.

In retrospect, then, Lashley's paper makes clear the shape of the challenge
that the cognitivists had set themselves. They wished to rout their sterile
behaviorist foes in the same way that Descartes had routed the schoolmen,
by providing a scientific account of cognitive processes. The problem, of
course, is that Descartes was not a thoroughgoing mechanist. So long as the
cognitivists retained the relational system of ideas that they had inherited
from Descartes, and from the much larger tradition of which Descartes is a
part, each of their models would include a component corresponding to the
soul. No matter how it might be squeezed or divided or ignored, there would
always remain one black box that seemed fully as intelligent as the person
as a whole, capable of making intelligent choices from a given range of
options on a regular basis. As the field of AI developed, this recalcitrant
box acquired several names. Dennett (1978: 80-81), for example, spoke of the
need for "discharging the homunculus", something he imagined to be possible by
dividing the intelligent homunculus into successively less intelligent pieces,
homunculi within homunculi like the layers of an onion, until one reached a
homunculus sufficiently dumb to be implemented in a bit of computer code. AI
researchers' jargon spoke of subproblems as being "AI-complete" (an analogy:
so-called NP-complete computational problems are thought to be unsolvable
except through an enumeration of possible solutions -- an efficient algorithm
for any one such problem would yield efficient algorithms for all of them).
And several exceedingly skilled programmers devised computer systems that
were capable of reasoning about their own operation -- including reasoning
about their reasoning about their own operation, and so on *ad infinitum*
(e.g., Smith 1985). In each case, the strategy was reducing the soul's
infinite choices to finite mechanical means.

But beyond sketching the shape of a future problem, Lashley also sketched
the principal strategy of a whole generation for solving it. The operation
of the determining tendency might be a mystery, but the general form of its
accomplishment was not. While the linguistic metaphor for action envisions
an infinite variety of possible actions, it also imposes a great deal of
structure on them. In mathematical terms the possible actions form a "space".
The generative principle of this space lies in the "schemata of action", which
are modeled on grammatical rules. A simple schema for English sentences might
be

> Sentence -> NounPhrase IntransitiveVerb .

That is, roughly speaking "one way to make a sentence is to utter a noun
phrase followed by an intransitive verb". Other rules might spell out these
various "categories" further; for example,
> NounPhrase -> Article Noun   
> Article -> a   
> Article -> the   
> Noun -> cat   
> Noun -> dog   
> IntransitiveVerb -> slept   
> IntransitiveVerb -> died

These mean, roughly, "one way to make a noun phrase is to utter an article
followed by a noun", "some possible articles are "a" and "the" ", "some
possible nouns are "cat" and "dog" ", and "some possible intransitive verbs
are "slept" and "died" ". And there might be other ways to make sentences;
for example,
> Sentence -> NounPhrase TransitiveVerb NounPhrase   
> TransitiveVerb -> saw   
> TransitiveVerb -> ate

This particular set of grammatical rules generates a finite space of English
sentences; for example,
> the cat saw a dog   
> a dog ate a dog

The process of "deriving" a sentence with these rules is simple and orderly.
One begins with the "category" Sentence, and then at each step one makes two
choices: (1) which category to "expand", and (2) which rule to apply in doing
so, until no categories are left. For example, one might proceed as follows:
> 1. Sentence   
> 2. NounPhrase TransitiveVerb NounPhrase   
> 3. NounPhrase TransitiveVerb Article Noun   
> 4. NounPhrase saw Article Noun   
> 5. Article Noun saw Article Noun   
> 6. the Noun saw Article Noun   
> 7. the Noun saw Article dog   
> 8. the cat saw Article dog   
> 9. the cat saw a dog

The space of possible sentences, then, resembles a branching road with a
definite set of choices at each point. The process of choosing a sentence
is reduced to a series of much smaller choices among a small array of
alternatives. The virtue of this reduction becomes clearer once the grammar
generates an infinite array of sentences, as becomes the case when the
following grammatical rules are added to the ones above:
> Sentence -> NounPhrase CognitiveVerb that Sentence   
> CognitiveVerb -> thought   
> CognitiveVerb -> forgot

It now becomes possible to generate sentences such as
> the cat thought that the dog forgot that a cat slept

Chomsky (1965: 8) in particular made a great deal of this point; following
Humboldt, he spoke of language as making "infinite use of finite means".
And although he believes that the mind ultimately has a biological (and
thus mechanical) explanation (1979: 66, 97), he has focused his research
on the level of grammatical competence rather than trying to uncover this
explanation himself.

**4 Allen Newell and Herbert Simon: The mechanization of the soul**

Instead, the first steps in mechanizing this idea of a generative space
were due to Newell and Simon (1963). Whereas Chomsky was concerned simply
with the precise extent of the generative space of English grammar, Newell
and Simon's computer program had to make actual choices within a generative
space. And whereas Lashley posited the existence of a "determining tendency"
whose genealogical origins lay in a non-mechanical soul, Newell and Simon
had to provide some mechanical specification of it. Here the generative
structure of the space was crucial. Newell and Simon did not employ
linguistic vocabulary. Nonetheless, just as grammatical rules and derivations
provide a simple, clear means of generating any grammatical sentence, the
application of "operators" provided Newell and Simon with a simple, easily
mechanized means of generating any possible sequence of basic actions.
Choosing *which* sequence of actions to adopt was a matter of "search".
The mechanism that conducted the search did not have to make correct choices
all the time; it simply had to make good enough choices eventually as it
explored the space of possibilities.

Newell and Simon placed enormous significance on this idea (see, for
example, Newell's comments in Agre (1993: 418)), and justifiably so. While
maintaining the system of conceptual relations already found in Descartes,
Lashley, and Chomsky, their program nonetheless embodied a serious proposal
for the mechanization of the soul (cf Gallistel 1980: 6-7). Their strategy
was ingenious: rather than endow the soul with an internal architecture
-- something incomprehensible within the system of ideas they inherited
-- they effectively proposed interpreting the soul as an epiphenomenon.
Ironically, given Descartes' polemics against scholastic philosophy, the
idea is approximately Aristotelian: the soul as the form of the person, not a
discrete component. More specifically, rather than being identified with any
particular device, the soul was *contained* by the generative structure
of the search space and *manifested* through the operation of search
mechanisms. These search mechanisms were "heuristic" in the sense that no
single choice was ever guaranteed to be correct, yet the overall effect of
sustained searching was the eventual discovery of a correct outcome. Despite
the simplicity and limitations of their early programs, Newell and Simon were
willing to refer to these programs' behavior as "intelligent" because they met
this criterion. And they regarded their proposal as promising because so many
human activities could readily be cast as search problems.

Up to this point, the story of the mechanization of the soul is a conventional
chapter in the history of ideas: to tell this story, we trace the unfolding
of an intellectual project within an invariant framework of continuities
or analogies among idea-systems. With Newell and Simon's program, though,
the story clearly changes its character. But how exactly? So far as the
disciplinary culture of AI is concerned, the formalization and implementation
of an idea bring a wholly new day -- a discontinuity between the prehistory
of (mere) questions and ideas and the history, properly speaking, of problems
and techniques. Once this proper history has begun, technical people can put
their proposals to the test of implementation: either it works or it does not
work.

Yet despite this conception, and indeed partly because of it, the development
of technical methods can be seen to continue a along trajectory largely
determined by the defining projects and internal tensions of the ancestral
systems of ideas. In particular, these projects and tensions continue to
manifest themselves in the goals and tribulations of AI's technical work. In
the case of Newell and Simon's proposal, the central goals and tribulations
clustered around the "problem" of *search control* -- that is, making
heuristic search choices well enough -- not perfectly, just well enough --
to allow the search process to "terminate" with an acceptable answer within
an acceptable amount of time. An enormous AI subliterature addresses this
problem in a wide variety of ways. Within this literature, searches are
said to "explode" because of the vastness of search spaces. It should be
emphasized that mediocre search control ideas do not kill a mechanism; they
only slow it down. Yet this research has long faced a troubling aporia: the
more complicated the world is, the more choices become possible at each point
in the search, and the more ingenuity is required to keep the search process
under control. The metaphors speak of a struggle of containment between
explosion and control. Such a struggle, indeed, seems inherent in any theory
for which action is said to result from formal reason conducted by a finite
being (Cherniak 1986).

Newell and Simon's achievement thus proved tenuous. So long as AI's
self-conception as a self-sufficient technical discipline has remained intact,
however, these difficulties are readily parsed as technical problems seeking
technical solutions. An endless variety of solutions to the search control
problem has indeed been proposed, and each of them more or less "works"
within the bounds of one or another set of "assumptions" about the world of
practical activity.

**5 Richard Fikes and Nils Nilsson: Mechanizing embodied action**

To watch the dynamics of this process unfold, it will help to consider one
final chapter: the STRIPS program (Fikes and Nilsson 1971). The purpose
of STRIPS is to automatically derive "plans" for a robot to follow in
transporting objects around in a maze of rooms. The program constructs
these plans through a search process modeled on those of Newell and Simon [[5](#endnote5)]. The search space consists of partially specified
plans, with each "operator" adding another step to the plan. Returning to
the linguistic metaphor, the authors of STRIPS understand the robot's action
within a grammar of possible plans. They refer to the units of action that
Lashley called "expressive elements" as "primitive actions", and the "syntax
of the act" strings these actions into sequences that can be "executed" in the
same manner as a computer program. In Descartes' terms, the soul's faculty of
reason specifies an appropriate sequence of bodily actions, each of which may
well be complicated, its faculty of will decides to undertake them, and the
body then physically performs them.

To those who have had experience getting complex symbolic programs to work,
the STRIPS papers make intense reading. Because the authors were drawing
together so many software techniques for the first time, the technically
empathetic reader gets a vivid sense of struggle -- the unfolding logic
of what the authors unexpectedly felt compelled to do, given what seemed
to be required to get the program to work. A detailed consideration of the
issues would take us much too far afield, but the bottom line is easy enough
to explain. As might be expected, this bottom line concerns the technical
practicalities of search control. A great deal is at stake: if the search
can be controlled without making absurdly unrealistic assumptions about the
robot's world, then the program can truly be labeled "intelligent" in some
non-trivial sense.

Consider, though, what this search entails. The STRIPS program is searching
for a correct plan -- that is, a plan which, if executed in the world as it
currently stands, would achieve a given goal. This condition -- achieving a
given goal -- is not simply a property of the plan; it is a property of the
robot's interactions with its world. In order to determine whether a given
plan is correct, then, the program must effectively conduct a simulation of
the likely outcome of each action. For example, if a candidate plan contains
the primitive action "step forward", it matters whether the robot is facing
a wall, a door, a pile of rubbish, or an open stretch of floor. If "step
forward" is the *first* step in the plan then the robot can predict its
outcome simply by activating its video camera and looking ahead of itself.
But if "step forward" is the seventh step in the plan, subsequent to several
other movements, then complex reasoning will be required to determine its
likely outcome.

This is a severely challenging problem, and Fikes and Nilsson approached it,
reasonably enough given the state of computer technology in 1971, through
brute force: they encoded the robot's world in the form of a set of formulae
in the predicate calculus, and they incorporated into STRIPS a general-purpose
program for proving predicate-calculus theorems by means of a search through
the space of possible formal proofs. This approach "works" in the same sense
that any search method works: if the search ever terminates then the answer
is correct, but how long this takes depends heavily on the perspicacity of
the program's search control policies. And adequately perspicuous search
control policies are notoriously elusive. As programmers like Fikes and
Nilsson quickly learned, the trick is to design the world, and the robot's
representations of the world, in such a way that long, involved chains of
reasoning are not required to predict the outcomes of actions.

Yet predicting the outcomes of actions was, as programmers say, only the
"inner loop" of the plan-construction process. Recall that the overall
process of choosing possible actions is also structured as a search problem;
extending Lashley's linguistic metaphor, it is as if the grammaticality of
a spoken sentence depended on the listener's reaction to each successive
word. Moreover, the space of possible plans is enormous: at any given
time, the robot can take any of about a dozen primitive actions, depending
on its immediate circumstances, and even a simple plan will have several
steps. Once again, search control policies are crucial. At each point in
the search process, the program must make two relatively constrained choices
among a manageable list of options: it must choose a partially specified
plan to further refine, and it must choose a means of further refining it --
roughly speaking, it must add another primitive action to the plan.

As with any search, making these choices correctly every time would require
"intelligence" that no mechanism could probably possess. The point, instead,
is to make the choices correctly *often enough* for the search to settle
on a correct answer in a reasonable amount of time. This, once again, is the
appeal of heuristic search: intelligent action emerges from a mass of readily
mechanizable decisions. In other words, the problem for Fikes and Nilsson was
that they had to write bits of code whose outcomes approximated two hopelessly
uncomputable notions: "partially specified plan most likely to lead to a
correct plan" and "best primitive action to add to this subplan". Their
solution to these problems was unsurprising in technical retrospect, and the
details do not matter here. Briefly, they chose whatever partially specified
plan seemed to have gotten the furthest toward the goal with the smallest
number of primitive actions, and they chose a new primitive action that
allowed the theorem-proving program to make further progress toward proving
that the goal had been achieved. Both of these criteria are virtually
guaranteed to lead the plan-construction process down blind alleys (such as
telling the robot to head for the door before getting the key). The important
point is that these blind alleys did not hurt the robot; they only kept the
robot waiting longer to be given a plan to execute.

How big a step was the STRIPS program toward mechanized intelligence?
Reasonable people could disagree. It is certainly an impressive thing to
watch such a program in operation -- provided you have long enough to wait.
But the question of search control was daunting. To the AI research people
of that era, search control in STRIPS-like plan-construction programs was a
"problem" to be addressed through a wide variety of technical means. Yet this
approach accepts as given the underlying structure of the situation: a steep
trade-off between the complexity of the world and the practicality of the
search control problem. If the robot can perform many possible actions, or
if the results of these actions depend in complex ways on the circumstances,
then the search space grows rapidly -- in mathematical terms, exponentially
-- in size. And if it is impossible to predict the outcomes of actions -- say
because the robot is not the only source of change in the world -- then the
search space will have to include all of the *possible* outcomes as well.
In a prescient aside in the sequel to the original STRIPS paper, Fikes, Hart,
and Nilsson (1972) pointed this out:
> One of the novel elements introduced into artificial intelligence research
> by work on robots is the study of execution strategies and how they interact
> with planning activities. Since robot plans must ultimately be executed in
> the real world by a mechanical device, as opposed to being carried out in
> a mathematical space or by a simulator, consideration must be given by the
> executor to the possibility that operations in the plan may not accomplish
> what they were intended to, that data obtained from sensory devices may be
> inaccurate, and that mechanical tolerances may introduce errors as the plan
> is executed.
>
> Many of these problems of plan execution would disappear if our system
> generated a whole new plan after each execution step. Obviously, such a
> strategy would be too costly, so we instead seek a plan execution scheme with
> the following properties:
>
> (1) When new information obtained during plan execution implies that some
> remaining portion of the plan need not be executed, the executor should
> recognize such information and omit the unneeded plan steps.
>
> (2) When execution of some portion of the plan fails to achieve the
> intended results, the executor should recognize the failure and either
> direct reexecution of some portion of the plan or, as a default, call for
> a replanning activity (1972: 268).

Thus, although they recognized the tension that was inherent in the system of
concepts they had inherited, the technical imagination of that time provided
Fikes, Hart, and Nilsson with no other way of structuring the basic question
of intelligent action. It was fifteen years before the inherent dilemma
of plan-construction was given definite mathematical form, first by Chapman
(1987) and then more compactly by McAllester and Rosenblitt (1991). This
kind of research does not decisively discredit the conceptual framework of
planning-as-search; rather it clarifies the precise nature of the trade-offs
generated by that framework. And indeed, productive research continues to
this day into the formal structure of plan-construction search problems.

**6 Beyond the Cartesian soul** 

The previous sections offer a critical reconstruction of a single strand
of intellectual history, a single intellectual proposition worked out in
increasingly greater technical detail so that its internal tensions become
manifest. To diagnose the resulting impasse and move beyond it, it will be
necessary to transcend AI's conception of itself as a technical, formalizing
discipline, and instead to reconsider the larger intellectual path of which
AI research has been a part. No matter how esoteric AI literature has become,
and no matter how thoroughly the intellectual origins of AI's technical
methods have been forgotten, the technical work of AI has nonetheless been
engaged in an effort to domesticate the Cartesian soul into a technical
order in which it does not belong. The problem is not that the individual
operations of Cartesian reason cannot be mechanized (they can be) but that
the role assigned to the soul in the larger architecture of cognition is
untenable. This incompatibility has shown itself up in a pervasive and ever
more clear pattern of technical frustrations. The difficulty can be shoved
into one area or another through programmers' choices about architectures and
representation schemes, but it cannot be made to go away.

This impasse, though, is not a failure. To the contrary, tracing the precise
shape of the impasse allows us to delineate with particular confidence the
internal tensions in the relational system of ideas around the Cartesian soul.
According to this hypothesis, the fundamental embarrassment of Descartes'
theory does not lie in the untenability of ontological dualism. Rather, it
lies in the soul's causal distance from the world of practical action. As
this world grows more complex (or, more precisely, as one's representational
schemes reflect this world's complexity more fully), and as one becomes more
fully immersed in that world, the soul's job becomes astronomically difficult.
Yet Descartes performed his analysis of the soul in sedentary conditions:
introspecting, visualizing, and isolating particular episodes of perception.
When he did discuss complex activities, he focused not on the practicalities
of their organization but on the struggles they engendered between the body
and the soul (see, for example, *Passions of the Soul*, Article 47).

In order to impose intelligent order on its body's actions, the Cartesian
soul faces a stern task. For example, to visualize a future course of events,
the soul must stimulate the brain to assemble the necessary elements of
memory. The reasoning which guides this visualization process must be based
in turn upon certain knowledge of the world, obtained through the senses --
enough information to visualize fully the outcomes of the individual's planned
sequence of actions. Our judgement that such a scheme places an excessive
burden on the soul -- or, as technical people would say, makes the soul
into a "bottleneck" -- is not a logical refutation; it is only an engineer's
embodied judgement of the implausibility of a design. But within the logic of
Descartes' project that is a lot.

The underlying difficulty takes perhaps its clearest form in Lashley. At
the beginning of his lecture, he opposes his own view to the behaviorist and
reflexological tale of stimuli and responses as follows:
> My principal thesis today will be that the input is never into a quiescent
> or static system, but always into a system which is already actively excited
> and organized. In the intact organism, behavior is the result of interaction
> of this background of excitation with input from any designated stimulus.
> Only when we can state the general characteristics of this background of
> excitation, can we understand the effects of a given input (page 112).

In contradistinction to a scheme that focuses upon the effects of an
isolated stimulus, Lashley proposes giving due weight both to a stimulus
and to the ongoing flux of brain activity in which the stimulus intervenes.
People, in other words, are always thinking as well as interacting with
the world. Having said this, though, he immediately gives priority to the
internal "background" of neural activity, and his paper never returns to any
consideration of external stimuli and their effects. As with his silence
about the nature of the determining tendency, this is not a simple omission
but is intrinsic to his relational system of concepts. His analysis of action
on the model of speech portrays speakers as laying out a complex series of
sounds through internal processing and then producing them in a serially
ordered sequence, without in any way interacting with the outside world
[[6](#endnote6)]. As we have already seen in the case of STRIPS,
this obscurity about the relationship between "planning" (of action sequences)
and "interaction" (with the world while those actions are going on) structured
cognitive theorizing about action, and AI research in particular, for many
years afterward [[7](#endnote7)].

It is precisely this pattern of difficulty that has impelled an emerging
interdisciplinary movement of computational modelers to seek a conception of
intelligent behavior whose focal point is the fullness of embodied activity,
not the reticence of thought. An organizing theme of this movement is
the principled characterization of interactions between agents and their
environments, and the use of such characterizations to guide design and
explanation. When the "agents" in question are robots, this theme opens
out onto a systems view of robotic activity within the larger dynamics of
the robot's world. When the "agents" are animals, it opens out onto biology,
and specifically onto a conception of ethology in which creatures and their
behavior appear thoroughly adapted to the dynamics of a larger ecosystem.
When the "agents" in question are people, it opens out onto philosophical and
anthropological conceptions of human beings as profoundly embedded in their
social environments. In lieu of detailed references to these directions
of research, allow me to me direct the reader to an issue of *Artificial
Intelligence* on Computational Theories of Interaction and Agency that will
appear in 1995.

**7 AI and the humanities** 

I have argued that AI can become sterile unless it maintains a sense of
its place in the history of ideas -- and in particular unless it maintains
a respect for the power of inherited systems of ideas to shape our thinking
and our research in the present day. At the same time, AI also provides a
powerful means of forcing into the open the internal structure of a system of
ideas and the internal tensions inherent in the project of getting those ideas
to "work". Thus, AI properly understood ought to be able to participate in
a constructive symbiosis with humanistic analyses of ideas.

Putting this mode of cooperative work into practice will not be easy. The
obstacles are many and varied, but I believe that the most fundamental ones
pertain to the use in AI of mathematics and mathematical formalization. This
is not the place for a general treatment of these topics, but it is possible
at least to outline some of the issues. The most obvious issue, perhaps, is
the symbolic meaning attached to mathematics in the discursive construction
of technical disciplines. Technical people frequently speak of mathematics
as "clean" and "precise", as opposed to the "messy" and "vague" nature of
the social world and humanistic disciplines. These metaphors clearly provide
rich points of entry for critical research, but the important point here is
that their practical uses go beyond the simple construction of hierarchies
among disciplines. Most particularly, the notion of mathematics as the telos
of reason structures AI researchers' awareness in profound ways.

To see this, let us briefly consider the role that mathematics plays in AI
research. The business of AI is to build computer programs whose operation
can be narrated in language that is normally used in describing human
activities (Collins 1990). Since the function of computers is specified
in terms of discrete mathematics, the daily work of AI includes the complex
and subtle discursive practice of talking about human activities in ways
that assimilate them to mathematical structures [[8](#endnote8)].
In the case of the computational models of action described above, this
assimilation is achieved by means of a linguistic metaphor for action.
This metaphor is not specific to AI; in fact it structures a great deal of
the practice of applied computing (Agre 1994) [[9](#endnote9)].
And this fact in turn points to an inherent source of intellectual
conservatism in AI: the field is not restricted *a priori* to speaking
of human beings in particular terms, but it *is* restricted to speaking
in terms that someone knows how to assimilate to mathematical structures
that can be programmed on computers. In this way, the existing intellectual
infrastructure of computing -- its stock of discursive forms and technical
methods -- drags like an anchor behind any project that would reinvent AI
using language drawn from alternative conceptions of human beings and their
lives.

This observation goes far toward explaining the strange appearance that AI
presents to fields such as literature and anthropology that routinely employ
much more sophisticated and critically reflective conceptions of human life.
The first priority for AI research is to get something working on a computer,
and the field does not reward gnawing doubts about whether the conceptions
of human life being formalized along the way are sufficiently subtle,
accurate, or socially responsible -- thus the emphasis, mentioned at the
outset, on "doing" as opposed to "just talking". Critical methods from the
humanities are likely to appear pointless, inasmuch as they do not immediately
deliver formalizations or otherwise explain what programs one might write.
AI people see formalization as a trajectory with an endpoint, in which the
vagueness and ambiguity of ordinary language are repaired through mathematical
definition, and they are not greatly concerned with the semantic violence that
might be done to that language in the process of formal definition. A word
like "action" might present real challenges to a philosophical project that
aims to respect ordinary usage (e.g., White 1968), but the assimilation of
action to formal language theory reduces the word to a much simpler form: a
repertoire of possible "actions" assembled from a discrete, finite vocabulary
of "expressive elements" or "primitives". Having thus taken its place in
the technical vocabulary of AI, the word's original semantic ramifications
are lost as potential resources for AI work. The ideology surrounding
formalization accords no intrinsic value to these left-over materials. As
a result, formalization becomes a highly organized form of social forgetting
-- and not only of the semantics of words but of their historicity as well.
This is why the historical provenance and intellectual development of AI's
underlying ideas claim so little interest among the field's practitioners.

What would a reformed AI look like? It would certainly not reject or replace
mathematics. Rather, it would draw upon critical research to cultivate a
reflexive awareness of how mathematical formalization is used as part of
the engineer's embodied work of building things and seeing what they do.
In particular, it would cultivate an awareness of the cycle of formalization,
technical working-out, the emergence of technical impasses, the critical work
of diagnosing the impasse as reflecting either a superficial or a profound
difficulty with the underlying conception of action, and the initiation
of new and more informed rounds of formal modeling. The privilege in this
cycle does not lie with the formalization process, nor does it lie with the
critical diagnosis of technical impasses. Rather, it lies with the cycle
itself, in the researcher's "reflective conversation with the materials" of
technical and critical work (Schon 1983).

Humanistic critical practice can take up numerous relationships, cooperative
or not, to this cycle of research. My own analysis in this paper has employed
a relatively old-fashioned set of humanistic methods from the history of
ideas, tracing the continuity of certain themes across a series of authors
and their intellectual projects. Since formalization is a fundamentally
metaphorical process, discursively interrelating one set of things with
another, mathematical set, it can be particularly fruitful to trace the
historical travels of a given metaphor among various institutional sites
in society, technical and otherwise (Martin 1987, McReynolds 1980, Mirowski
1989). The purpose in doing so is not simply to debunk any claims that
technical institutions might make to an ahistorical authority, but to prevent
the passage to formalism from forgetting the underlying commitments that a
given way of speaking about human activities draws from its broader cultural
embedding [[10](#endnote10)]. This contextual awareness will
be crucial when the technical research reaches an impasse and needs to be
diagnosed as a manifestation of internal tensions of the underlying system
of ideas. Any given set of ideas will be more easily given up when they are
seen as simply one path among many others not taken. Indeed this awareness of
context will be crucial for recognizing that an impasse may have occurred in
the first place. Viewed in this way, technical impasses are a form of social
remembering, moments when a particular discursive form deconstructs itself and
makes its internal tensions intelligible to anyone who is critically equipped
to hear them.

The cycle of reaching and interpreting technical impasses, moving back and
forth between technical design and critical inquiry, can be practiced on a
variety of scales, depending upon the acuity of one's critical methods. The
example I traced in the body of this paper was extremely coarse: whole decades
of research could be seen in hindsight to have been working through a single,
clear-cut intellectual problem. The difficulty was not that AI practitioners
were insulated from the philosophical critiques of Cartesian reason that
might have provided a diagnosis of their difficulties and defined the contours
of alternative territories of research. To the contrary, Hubert Dreyfus was
articulating some of these critiques all along. The real difficulty was that
the critical apparatus of the field did not provide its practitioners with a
living, day-to-day appreciation for the contingent nature of their formalisms.
Although they viewed formalization as conferring upon language a cleanliness
and precision that it did not otherwise possess, the effect was precisely
the reverse. Lacking a conscious awareness of the immense historicity of
their language, they could not understand it as it called out to them the very
things they had discovered. A reformed technical practice would employ the
tools of critical inquiry to engage in a richer and more animated conversation
with the world.

**\* Footnotes** 

[1]
For a detailed analysis of this argument see Preston (1993).

[2]
Dreyfus, in joint work with Stuart Dreyfus, has been cautiously supportive
of one alternative AI research program, the "connectionist" attempt to build
simulations of neural circuitry without necessarily formulating "knowledge"
in terms of symbolic "rules" (Dreyfus and Dreyfus 1988). But as the Dreyfuses
points out, this research program still faces a long, difficult learning curve
and will not be discussed here.

[3]
The terms "mechanism" and "mechanistic" require further analysis than
space permits here. Suffice it to say that a mechanism is a physical object
whose workings are wholly explicable in causal terms. To speak of something
as a mechanism, furthermore, is to insert it into a rhetoric of engineering
design, whether divine or human, and whether on the model of the clockmaker
or the computer programmer. For the modern mathematical intepretations of
the term, which are obviously relevant to the foundations of computing if not
immediately to the genealogy being traced here, see Webb (1980).

[4]
Note that the intellectual culture of Descartes' day did not
distinguish between "mind" and "soul", and the two terms continue to be used
interchangeably in Catholic philosophy to this day; see for example Holscher
(1986). Even in the present day, these terms are usually not so much opposed
as simply employed in different discourses with overlapping genealogies.

[5]
Chapman (1987) presents a genealogy of the AI "planning" systems in this
lineage.

[6]
Actual human speakers frequently do interact with their addressees and
others during the real-time production of their utterances (Goodwin 1981),
but this fact is rarely taken into account in cognitive theories of grammar
and speech.

[7]
It is particularly clear in the opening chapter of Miller, Galanter, and
Pribram's influential book *Plans and the Structure of Behavior* (1960).

[8]
This is obviously an attribute that AI shares with a wide variety of other
fields, for example mathematical economics, and much of the analysis here
applies to these other fields as well. It should be noted that AI people
themselves place great emphasis on a distinction between "neat" forms of AI,
which openly avow their commitment to mathematical formalization and employ
large amounts of mathematical notation in their papers, and "scruffy" forms,
which do not (Forsythe 1993). My argument, though, applies equally to both
forms of AI research. Regardless of whether its author was consciously
thinking in terms of mathematics, a computer program is a notation whose
operational semantics can be specified in mathematical terms. While the
formalizations in "neat" research are frequently more consistent, systematic,
and explicit than those of "scruffy" research, the design of any computer
program necessarily entails a significant level of formalization.

[9]
Different linguistic metaphors for human action are obviously possible,
if perhaps equally problematic; see for example Ricoeur (1971).

[10]
For an impressive cultural analysis of the origins of AI, see Edwards
(1996).

**\* Acknowledgements** 

This paper has been improved by comments from Harry Collins, Guven Guzeldere,
Scott Mainwaring, Beth Preston, and Joszef Toth.

**\* References** 

Philip E. Agre, Interview with Allen Newell, *Artificial Intelligence*
59(1-2), 1993, pages 415-449.

Philip E. Agre, Surveillance and capture: Two models of privacy, *The
Information Society* 10(2), 1994, pages 101-127.

David Chapman, Planning for conjunctive goals, *Artificial Intelligence*,
32(3), 1987, pages 333-377.

Christopher Cherniak, *Minimal Rationality*, Cambridge: MIT Press,
1986.

Noam Chomsky, *Aspects of the Theory of Syntax*, Cambridge: MIT Press,
1965.

Noam Chomsky, *Problems of Knowledge and Freedom: The Russell Lectures*,
New York: Pantheon, 1971.

Noam Chomsky, *Language and Responsibility*, translated from the French
by John Viertel, New York: Pantheon, 1979.

Harry M. Collins, *Artificial Experts: Social Knowledge and Intelligent
Machines*, Cambridge: MIT Press, 1990.

Daniel Dennett, Why the law of effect will not go away, in *Brainstorms:
Philosophical Essays on Mind and Psychology*, Montgomery, VT: Bradford
Books, 1978.

Rene Descartes, *The Philosophical Works of Rene Descartes*, translated
by Elizabeth S. Haldane and G. R. T. Ross, volume 1, Cambridge: Cambridge
University Press, 1972.

Hubert L. Dreyfus, *What Computers Can't Do: A Critique of Artificial
Reason*, New York: Harper and Row, 1972.

Hubert L. Dreyfus and Stuart Dreyfus. Making a mind vs. modeling the brain:
AI back at a branchpoint, *Daedalus* 117(1), 1988, pages 15-43.

Paul Edwards, *The Closed World: Computers and the Politics of Discourse in
Cold War America*, Cambridge: MIT Press, 1996.

Richard E. Fikes and Nils J. Nilsson, STRIPS: A new approach to the
application of theorem proving to problem solving, *Artificial
Intelligence* 2(3), 1971, pages 189-208.

Richard E. Fikes, Peter E. Hart, and Nils J. Nilsson, Learning and executing
generalized robot plans, *Artificial Intelligence* 3(4), 1972, pages
251-288.

Diane E. Forsythe, Engineering knowledge: The construction of knowledge in
artificial intelligence, *Social Studies of Science* 23(3), 1993, pages
445-477.

C. R. Gallistel, *The Organization of Action: A New Synthesis*,
Hillsdale, NJ: Erlbaum, 1980.

Charles Goodwin, *Conversational Organization: Interaction Between Speakers
and Hearers*, New York: Academic Press, 1981.

Martin Heidegger, *Being and Time*, translated by John Macquarrie and
Edward Robinson, Harper and Row, 1961. Originally published in German in
1927.

Ludger Holscher, *The Reality of the Mind: Augustine's Philosophical
Arguments for the the Human Soul as a Spiritual Substance*, London:
Routledge, 1986.

Karl S. Lashley, The problem of serial order in behavior, in Lloyd A.
Jeffress, ed, *Cerebral Mechanisms in Behavior: The Hixon Symposium*,
New York: Wiley, 1951.

Emily Martin, *The Woman in the Body: A Cultural Analysis of
Reproduction*, Boston: Beacon Press, 1987.

David McAllester and David Rosenblitt, Systematic nonlinear planning,
*Proceedings of the National Conference on Artificial Intelligence*,
Los Altos, CA: Morgan Kaufmann Publishers, 1991, pages 634-639.

Paul McReynolds, The clock metaphor in the history of psychology, in Thomas
Nickles, ed, *Scientific Discovery: Case Studies*, Dordrecht: Reidel,
1980.

George A. Miller, Information and memory, *Scientific American* 195(2),
1956, pages 42-46.

George A. Miller, Eugene Galanter, and Karl H. Pribram, *Plans and the
Structure of Behavior*, New York: Henry Holt and Company, 1960.

Philip Mirowski, *More Heat Than Light: Economics as Social Physics, Physics
as Nature's Economics*, Cambridge: Cambridge University Press, 1989.

Allen Newell and Herbert A. Simon, GPS: A program that simulates human
thought, in Edward A. Feigenbaum and Julian Feldman, eds, *Computers and
Thought*, New York: McGraw-Hill, 1963.

Elizabeth F. Preston, Heidegger and artificial intelligence, *Philosophy and
Phenomenological Research* 53(1), 1993, pages 43-69.

Paul Ricoeur, The model of the text: Meaningful action considered as a text,
*Social Research* 38, 1971, pages 529-562.

Donald A. Schon, *The Reflective Practitioner: How Professionals Think in
Action*, New York: Basic Books, 1983.

Brian C. Smith, Prologue to *Reflection and Semantics in a Procedural
Language*, in Ronald J. Brachman and Hector J. Levesque, eds, *Readings
in Knowledge Representation*, Los Altos, CA: Morgan Kaufmann, 1985.

Judson Chambers Webb, *Mechanism, Mentalism, and Mathematics: An Essay on
Finitism*, Dordrecht: Reidel, 1980.

Alan R. White, ed, *The Philosophy of Action*, London: Oxford University
Press, 1968.

Ludwig Wittgenstein, *Philosophical Investigations*, third edition,
translated by G. E. M. Anscombe, New York: Macmillan, 1968. Originally
published in 1953.
