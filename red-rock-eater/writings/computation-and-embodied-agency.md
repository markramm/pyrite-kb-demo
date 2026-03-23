---
id: computation-and-embodied-agency
title: Computation and Embodied Agency
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1995/Computation.and.Embodied.html
coauthors: []
key_concepts: []
importance: 4
research_status: partial
tags:
  - forwarded-content
  - internet-culture
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1995/Computation.and.Embodied.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991005040936/http://www.somewhere.com/)

  

# Computation and Embodied Agency

```
[This is a brief survey of some new developments in artificial intelligence.
It's in LaTeX format for those who have LaTeX, but those who do not can easily
enough ignore the back-slashed formatting commands.  It's about 15 pages.]

\documentstyle[11pt]{article}

\title{Computation and Embodied Agency}
\author{Philip E. Agre \\
  Department of Communication \\
  University of California, San Diego \\
  La Jolla, California  92093-0503 \\
  \tt{pagre@ucsd.edu} \\
  (619) 534-6328, fax (619) 534-7315}

%  Copyright 1995 by the author.
%
%  To appear in a special issue of Informatica on computational theories of
%  mind.  For details contact Matjaz Gams <matjaz.gams@ijs.si>.
%
%  Please do not quote from this version, which will probably change slightly
%  in proof.  Paper reprints will be available from the author at the address
%  above when the article appears in print.

\begin{document}

\maketitle

\section{Introduction}

{}From its origins in a small number of well-funded laboratories, the field
of artificial intelligence has been undergoing steady structural changes:

\begin{itemize}
  \item The field's scope has grown more precise as various neighboring
    fields have matured.  These include disciplines such as artificial life
    and neural network modelling that use computational methods to study
    animal and human activities but that do not identify themselves as part
    of AI. 
  \item AI has also witnessed the development of specialized subfields such
    as machine learning, natural language processing, and computational logic
    with their own literatures, meetings, and disciplinary cultures.  These
    subfields develop distinctive cultures, particularly with regard to the
    standards by which research projects are judged.
  \item Research communities have arisen to apply AI methods to particular
    domains such as manufacturing and medicine.  These communities respond to
    their domains in a more complex and realistic way than mainstream AI has
    usually done, but as a consequence they often have less freedom to explore
    new methods that are still poorly understood.
\end{itemize}

Many projects cross the borders among these areas of research.  Many of these
communities, moreover, have been heavily influenced by ideas and methods
from outside AI as well, giving them a hybrid character.  By choosing which
disciplinary communities to associate themselves with, researchers have some
flexibility in deciding, for example, whether they are engaged in scientific
discovery or engineering design (or perhaps both).

As the field of AI has decentralized, its growing pluralism has made room
for a variety of critical interventions and interdisciplinary dialogues.  
It becomes possible for groups of researchers to discover common threads 
in their work and to explore these collectively without needing to struggle
against prestructured disciplinary boundaries or to proclaim the existence 
of a new, permanent institution.  This article describes one such initiative,
which draws together research from several fields to propose alternatives
to some of the basic concepts of AI.  The idea that unifies in this emerging
style of research is not architectural -- work is included from a remarkable
variety of technical research programs.   Rather, the unifying idea is
conceptual and methodological:

\begin{quote}
  using principled characterizations of interactions between agents and their
  environments to guide explanation and design
\end{quote}

The theme of interaction, of course, has a long history.  Systems described in
the AI literature have interacted with their environments (physical or social,
real or simulated) for a long time, Simon (1970: 24-25) famously pointed out
that simple ants can engage in complex interactions with complicated beaches,
and the concepts of cybernetics had a significant influence in the original
founding of the field (Edwards 1996).  The point is to bring new tools to the
analysis of these interactions and to make new uses of the resulting analyses.
Some rough initial explication of the key words may help orient the reader to
the detailed discussions below.

\begin{description}
  \item{interactions}: The focus of this research is on activities that take
    place in the material world.  The agents may or may not be understood
    as having internal mental processes that play roles in shaping the
    activities, but the focus is on the activities themselves.
  \item{environments}: The environments in which these activities take place
    will generally have both physical and social aspects.  The research
    described here, though, is primarily concerned with embodied activity in
    simplified versions of the physical world.
  \item{agents}: The research might concern people, animals, or robots.  The
    point is certainly not to equate people to animals or robots, but simply
    to establish dialogue among research projects with different goals.
    Serious ideas about conversational interaction and its consequences for
    computational modelling of human beings, for example, may inspire clearer
    thinking about other kinds of interaction as well.
  \item{characterizations}: Attempts to conceptualize interactions between
    agents and their environments will require theorists to draw clear
    distinctions between the theorist's ``aerial view'' of an activity and
    the agent's ``ground view'' of that same activity.  Agents that are not
    omniscient or omnipotent will necessarily engage in activities that are
    not wholly scripted, and that therefore have emergent structures that can
    be studied and understood.
  \item{principled}: Both formal/mathematical and informal/qualitative kinds
    of characterizations are included.  The important thing is that they be
    grounded in the intellectual disciplines of some field of research.
  \item{guide}: It is impossible to determine in advance what forms these
    characterizations might take, what lessons might be learned from them,
    or what kinds of guidance they might offer to research.  Some of this
    guidance will take the form of knock-down arguments, formal or otherwise,
    and the rest will be a heuristic matter of probabilities.  Both types of
    guidance are valuable.
  \item{explanation and design}: The goals of the research might include both
    scientific explanation of existing agents-in-environments and engineering
    design of new ones.  Despite their distinct goals, the activities of
    science and engineering have a long history of cross-fertilization in
    computational research; the important thing is simply to be aware of which
    is which.
\end{description}

Stanley J. Rosenschein and I have recently (1995) edited a special double
volume of the journal {\sl Artificial Intelligence} that explores this
approach to AI research in detail, including seventeen papers that develop the
approach in particular directions.  The purpose of this article is to explore
some of the intellectual background to this research (Section 2), to summarize
some of what has been learned from it (Section 3), and to reflect on how this
research may portend the emergence of a critical cognitive science, grounded
in computational experiment but simultaneously guided by critical research on
its own practices and their place in history (Section 4).

\section{Agents in the world: Cognition and planning}

Every research community, whether it knows it or not, inherents an extensive
network of ideas from its predecessors.  This inheritance may be regarded
as a type of historical memory, carried across generations in the language 
and artifacts and interactional forms of a community, and it matters whether
the memories are conscious or unconscious.  Unconsciously inherited ideas 
will continue to shape thought and research in the present day, structuring
agendas and methods and interpretations while making it difficult to
conceptualize alternatives.  Although it is probably impossible for any
research community to become encyclopedically aware of its intellectual
heritage, critical research can make a community aware of patterns that have
gone unnoticed and options that it did not know it had.

This view of the role of critical reflection is common sense in many fields,
particularly philosophy.  Yet it is still unfamiliar in most scientific and
technical fields, which are accustomed to understanding themselves as wholly
aware of their own ideas and methods.  The tendency of scientific fields
to reconstruct their history within present-day frameworks has been long
remarked (Kuhn 1962); in technical fields this sort of organized forgetting
is manifested in the ``state of the art'' which is nowise defined by its
origins.  While we might be suspicious of such an assumption in chemistry or
ecology or antenna physics, it is particularly implausible in the case of AI,
which clearly draws upon an ancient and complex tradition of Western thought
about such categories as ``the mind'' (Agre 1995a).  Concepts of mental life
have been central to AI since its beginnings; its whole premise was that
computations occurring inside a computer might be regarded as modeling or
mimicking the thoughts occurring inside a human being's mind.

The root metaphor here is spatial: the mind/computer as a container with an
inside and an outside.  Perceptions might pass into the container and willed
actions might pass out of it, but the unit of analysis is the process going on
inside it, as opposed to the interactions with an environment that it enters
into.  This way of framing AI's subject matter is understandable, given that
the computers of the 1950's had only the crudest capabilities for interacting
with their environments.  But this framing was not a fully conscious choice;
it was part of the philosophical tradition from which the psychology of that
day had itself descended.  Behaviorists and mentalists argued about whether
it was alright to posit any mechanisms in the space between stimulus and
response, but they did not argue about the stimulus-response paradigm and the
container metaphor it implied.

To be sure, the lines of descent which provided AI with its root metaphors
were not wholly straight.  Perhaps the field's most influential founder,
Herbert Simon, had previously embraced a more complex view of human beings
and their lives in his writings on public administration.  In his first major
book, {\sl Administrative Behavior}, Simon (1957) described numerous measures
through which organizations compensate for the ``limited rationality'' of
their members.  The creation of stable job descriptions and the overall
division of labor, for example, compensate for finite human abilities.
Deliberately designed communication channels, likewise, compensate for
individuals' limited knowledge and limited capacities to absorb new
information.  And hierarchical organizations provide individuals with
bounded goals while providing for overall coordination.  Simon portrays
people and their organizational environments as fitted to one another.
Metaphorically, the jagged edges of individuals' capabilities are met by
the complementary shape of the world around them.  Individuals are treated
not as self-sufficient and self-defining but as participants in a larger
organizational metabolism.

Although this theory may tend to underestimate the scope of human agency,
it at least begins to comprehend people as participants in a larger world.
In particular, it provides a positive theory of the attributes of that larger
world which interact constructively with the complex pattern of strengths
and weaknesses found in individual cognition.  Yet when Simon went on to
collaborate with Allen Newell in the first symbolic models of human thought
(e.g., Newell and Simon 1963), the only element of it that remained is the
assumption that people get their goals from their hierarchical superiors --
or, more to the point, from the psychologists who are running the experiment.
{\sl Administrative Behavior} was a study of decision-making in an environment
that provided the conditions for satisfactory choices despite limitations of
individual rationality; {\sl Human Problem Solving} (Newell and Simon 1972)
was a study of problem-solving in an ``environment'' defined in terms of
the formal structure of a ``problem'' as a ``search'' through an abstract
``space.''

AI ideas about action have generally been framed in terms of ``planning,''
which is roughly the notion of conducting one's life by constructing and
executing computer programs (Allen, Hendler, and Tate 1990).  Somewhat
confusingly, this term originally entered the AI lexicon from Newell
and Simon's work, but with a different meaning -- it was a mechanism for
shortening searches through a hierarchy of search spaces representing
different degrees of detail.  But its more common denotation was influenced by
Newell and Simon's work as well, the idea being roughly that one constructs a
plan by conducting a search through the space of possible plans, looking for
the one that reaches a recognized goal state.

The development of the concept of planning provides an instructive lesson in
the workings of technical ideas.  The most elaborate and widely influential
early articulation of it was found in George Miller, Eugene Galanter, and Karl
Pribram's book {\sl Plans and the Structure of Behavior} (1960).  According to
Miller, Galanter, and Pribram:

\begin{quote}
  A Plan is any hierarchical process in the organism that can control the
  order in which a sequence of operations is to be performed (1960: 16).
\end{quote}

This definition is remarkably vague, speaking not of a symbolic structure but
of a ``process.''  (The process is hierarchical in the sense articulated by
Newell and Simon in their own concept of ``planning.'')  In practice, though,
Miller, Galanter, and Pribram constantly shifted back and forth between two
concepts of a Plan.  According to the first concept, a Plan is a recipe that
someone might retrieve from memory and execute as a single choice; the day's
repertoire of habitual routines might be understood as a library of these
Plans.  This concept provides an easy explanation of why behavior has a
structure: this structure is caused by a Plan that has that same structure.
But it provides no explanation of how complex patterns behavior of respond
to the unfolding complexities of the environment.  This was the purpose of
second concept, usually referred to as {\sl the\/} Plan, which was a large
hierarchical structure in the individual's mind, assembled from bits and
pieces of Plans.  At any given time the Plan would be partially assembled,
well worked out in some areas and sketchy in others.  The only requirement
was that any given section of the Plan be completely filled in when the
time comes to execute it.  These two distinct concepts responded to distinct
needs that Miller, Galanter, and Pribram did not know how to reconcile. 
Their text betrays no evidence that they were aware of the internal tension
in their ideas; nor was the problem discussed in the extensive literature
that they inspired.  Instead, later computational research focused heavily
on the construction of single Plans, with little attention to the more
improvisational aspects of human activity that required the incremental
assembly of the longer-term Plan.

In retrospect, much conceptual trouble in AI has arisen through a subtle
tendency to conflate two logically distinct points of view: (1) that of the
observer or theorist investigating an agent-environment system; and (2) that
of the agent being studied or designed.  Thus, for example, Miller, Galanter,
and Pribam failed to distinguish consistently between two of their central
theses: (1) that behavior has a structure; and (2) that behavior has the
structure it does because it is caused by a Plan that has that same structure.
Perhaps in consequence of this, it has become common in AI to use the term
``plan'' to refer either to a behavioral phenomenon or a mental entity. 
This usage makes it difficult to conceptualize any other explanation for the
recurring structures of behavior, for example that they might arise through
the repeated interaction of particular agents (which may or may not employ
plans) with particular environments (which are probably arranged to facilitate
beneficial forms of interaction).

The AI literature has also failed to distinguish consistently between
the observer's view of the world and the agent's own model of the world.
Agents are often said to possess ``world models'' which stand in systematic
point-by-point correspondence with the outside world, and programs often
receive correct, complete, consistent, up-to-date models automatically.  It is
of course possible that some real agents employ world models of this type, or
that artificial agents might benefit from them.  But the case for world models
becomes less automatic once we recognize that real, situated, finite agents
can only maintain models of the world by piecing together bits and pieces
of information perceived at distant places and times, often without precise
knowledge of their location.  Likewise, it is important to distinguish two
uses of the word ``situation,'' which can be used to refer to the totality of
the state of the world at a given moment or else to the agent's own knowledge
or immediate sense perceptions of the world at that moment.

Throughout this history, the unrecognized root metaphor of mind-as-container
frustrated clear thinking about computational theories of action.  It is
clear in retrospect that action should be a promising site for reexamination
of basic AI ideas, precisely because action constantly crosses the boundaries
between the mind-inside and the world-outside.  Yet this realization came
slowly to the AI community, largely through a series of experiments with
``situated'' or ``reactive'' systems that effectively reinvented the second,
neglected half of Miller, Galanter, and Pribram's ambiguous concept (Agre and
Chapman 1987, Brooks 1986, Georgeff and Lansky 1987, Rosenschein and Kaelbling
1986, Schoppers 1987).

\section{Structural coupling}

In the context of this history, the ambition of the approach to AI that 
I sketched at the outset -- characterizing interactions in principled
ways -- is to reconcile the two demands that pulled the ``planning''
theory in contradictory directions: explaining the sense in which activity
has a structure and explaining how activity responds to a steady stream
of environmental contingencies.  These explanations will not be simple,
nor would it be desireable to force them into a single vocabulary.  Early
projects in this area have been primarily concerned with mapping the territory
and identifying specific, relatively modest results that can provide models 
for further research.  This section summarizes some of these early projects,
with special reference to the work described in Agre and Rosenschein (1995).

A unifying theme for this results is Maturana and Varela's (1987) notion of
structural coupling.  Structural coupling is a difficult concept to understand
within the theories of causality that have been implicit in the majority 
of AI research.  But it is easier to understand in its original context 
of evolutionary biology.  Any given ecosystem, consisting of a number of
species and a certain physical environment, will exhibit a great deal of
mutual adaptation as the various species have coevolved while constantly
having effects on their surroundings.  Over time, the ``design'' of each 
species becomes increasingly interlocked with the rest of the ecosystem, so
that its structure becomes well-adapted to particular forms of interaction
while contributing certain ongoing influences in turn.  In this sense, the
structures of the various species and their environments become ``coupled''
-- implying one another through their mutual adaptation and their roles in
creating the conditions of continued existence for one another.  As a result,
it makes little sense to study an organism in isolation from its environment.
Simple descriptive anatomy might provide a useful source of reference
material, but it will not provide concepts to explain how the organism
functions in its natural surroundings or why it is structured as it is.

The notion of structural coupling might be extended to other spheres, for
example in understanding the systems of cultural practices by which people
conduct their lives.  It would be a serious mistake to reduce these practices
to a simple matter of biological adaptation or survival, thereby converting AI
into a type of sociobiology, but the biological metaphor has heuristic value
nonetheless.  Computational research on human interactions with the physical
world suggests exploring the specifically cognitive dimension of these
practices -- the ways that they bridge the gap between the structure of an
underlying architecture and the structure of an environment of activity.

\subsection{Horswill}

Horswill (1995) offers a framework for thinking about the adaptation of a
robot's perceptual architecture to its environment.  Research in AI has most
often aimed at building extremely general architectures to match the seemingly
infinite flexibility of human intelligence.  This emphasis on generality
discourages attention to environmental adaptation.  Horswill, by contrast,
seeks general methods for building specialized systems.  Intuitively, one
might imagine a lattice structure in which general-purpose systems are located
toward the top and very specialized systems are located toward the bottom.
The partial order that induces the lattice is ``works correctly in a broader
range of environments than.''  The discovery of new forms of structure in the
environment -- for example, a geometric structure or property of reflected
light (cf Marr 1982) -- should allow the designer to move downward in the
lattice, selecting a design that employs simpler machinery.

Horswill uses this framework to describe the workings of a robot that provides
visitors with tours of a floor of an office building.  This environment has
special properties whose computational significance may not be evident at
first.  For example, the floors in this environment have no low-frequency
surface markings since they consist of square floor tiles of uniform color,
whereas all other objects do have such small markings.  As a result, a simple
bandpass filter, together with information from stereo matching about an
object's distance from the camera, suffices to distinguish between floors 
and other objects.  Other such environmental constraints remove the necessity
of calibrating the camera, since analysis of the necessary computations
reveals that, in order to make the specific decisions that it needs to make 
in carrying out its purpose, the robot need only calculate a function that is
monotonically related to a correct measurement of the world.  The final result
of these discoveries is that the robot can be built with simple hardware. 
The point, however, is not to promote simple hardware as such, nor to suggest
any particular type of hardware is universally applicable, but to provide
principled means for choosing the simplest hardware that is compatible with a
given environment and (desired or observed) pattern of interaction.

This method does not provide a mechanical formula for system design, since 
it takes considerable thought and post-hoc rationalization to discover 
which environmental constraints actually permit a given system's calculations
to be simplified.  Nonetheless, experience with this process ought to provide
designers with a library of instructive case studies in both the design of
adapted systems and the explanation of natural systems.

\subsection{Kirsh}

Whereas Horswill's design methods produce essentially passive perceptual
systems, Kirsh (1995) describes and categorizes a wide variety of measures
through which people actively manage their physical environments to assist
their perception and cognition.  Gathering the tools and ingredients needed 
to cook a particular dish into a specific area of the kitchen, for example,
reduces the amount of visual discrimination needed to select the right object
to pick up; it also provides reminders of steps that might otherwise have been
forgotten.  When disassembling a bicycle, arranging the parts in the order in
which they were removed effectively serves as a mnemonic device to guide the
process of putting them back on again (Chapman and Agre 1986).  By analogy
with manufacturing automation, in which workspaces are frequently provided
with ``jigs'' that hold parts in place while other operations are performed on
them, Kirsh refers to these tricks as ``informational jigging.''

The phenomenon of informational jigging provides numerous clues about the
strengths and limitations of human cognition.  It is easier, for example, 
to discern the length of a row than the volume of a pile.  As a result, when
arranging various foods on a tray it is helpful to place them in parallel
lines across the countertop to ensure that one is using them in steady
proportions.  Capture errors are common when two common tasks provide similar
patterns of visual cues; it helps to differentiate these tasks by performing
them in different places or with different tools.

\subsection{Hammond, Converse, and Grass}

This pattern of reasoning generalizes the pattern found in Horswill's work.
In each case, recourse to very general architectures is avoided by looking for
structure in the relationship between agent and environment.  For Horswill,
this structure is a matter of perceptual patterns that permit computations 
to be simplified.  For Kirsh, it is a matter of active interventions in 
the environment that produce the same effect.  Hammond, Converse, and Grass
(1995) take this line of reasoning further, investigating much longer-term
relationships between agents and their environments.  This is a striking
departure from AI planning research, which has generally understood activity
in terms of the pursuit of single, discrete goals.

The starting-point for Hammond, Converse, and Grass's argument is a 
particular kind of architecture: ``case-based'' systems that work by treating
previously encountered situations as precedents for reasoning about new 
ones.  Case-based systems offer an explanation of why ordinary activities can
proceed so smoothly despite their great complexity -- most of the complexity
has  been encountered elsewhere before.  A great deal of research has explored
the memory structures needed to support case-based reasoning (Schank 1982),
and Hammond, Converse, and Grass wished to apply these results to the modeling
of long-term activities.  Doing so, though, required some account of why newly
situations are likely to be similar to old ones.  The answer, in large part,
is that people actively ``stabilize'' their environments.  A simple example of
stabilization is putting tools away and cleaning up when a task is finished.
That way, the work environment will look largely the same at the beginning of
each task.

\subsection{Agre and Horswill}

With the work of both Kirsh and Hammond, Converse, and Grass, the ``principled
characterization'' of the environment takes the form of a heuristic argument
and the classification of a broad range of example phenomena.  Although
this kind of theory is valuable, it does not support strong forms of proof.
One cannot use these concepts, for example, to demonstrate formally that
a particular kind of agent will necessarily enjoy all of the reminders and
perceptual distinctions necessary to perform a given task.  The theorist
faces a trade-off: formal proofs usually require that the agent and world be
understood in relatively simple and unrealistic ways.

The work of Agre and Horswill (see Agre 1995b, Agre and Horswill 1992)
provides a case study in the formalization of cultural practices.  They
explore tasks that involve operations on artifacts, for example the artifacts
found in Western kitchens during the preparation of simple customary meals.
One might try formalizing these tasks in terms of the various states that
each type of object might occupy (a fork might be clean or dirty; eggs might
be intact, broken, beaten, or cooked; and so on) and the operations that
cause objects to move from one state to another (beating an broken egg with
a fork causes the egg to become beaten and the fork to become dirty).  Each
type of object would thus have a state-graph similar to the graphs found
in conventional formalizations of planning as a matter of search.  It is
possible to conceive of kitchens, on another planet perhaps, in which these
state-graphs are extremely tangled, so that the cook must consider a vast
range of combinatorial possibilities before making any moves.  But the
kitchens that have evolved in human cultures do not cause such problems.  An
investigation of the state-graphs for familiar tools and materials suggests
one reason why: these graphs fall into a small number of simple formal
categories which permit a simple mechanism to determine what actions to take
next.

Cooking is not always this simple, of course, but a formal analysis predicts
when difficulties are likely to arise -- for example when the interleaving of
several complex recipes makes it necessary to schedule the use of a limited
resource such as the oven.  For most purposes, though, culture has evolved
tools that serve cognitive functions: they help make it simple to decide what
to do next, thereby reducing the need for the complex forms of state-space
search that planning research has developed.

Considered together, these research projects begin to paint a picture quite
different from that found in the cognitive tradition AI research.  Instead
of disembodied thinking, this research discovers embodied agents engaged
in intricate interactions with their environments, and the properties of
these interactions turn out to have substantial consequences for the agents'
architectures.  Just as Simon's {\sl Administrative Behavior} had imagined
organization members as fitted to their cognitive environments in complex
ways that compensated for their limited rationality, this research paints
human beings as fitted to their physical environments.  More importantly,
this research breaks down the conventional concept of cognition: cognition,
it turns out, is not usefully understood as something that happens inside
an individual's head.  The natural unit of analysis, rather, is to be found
in the interactional patterns that arrange the world as someplace that is
good to think in.  Research can reconstruct the structural coupling between
architectures and environments by moving back and forth analytically between
them, investigating the environmental structures and customary practices
that might compensate for the limitations that an architecture might seem to
possess when considered in isolation.

\section{Critical cognitive science}

The research I have described suggests an alternative conceptualization of
the field of artificial intelligence.  On a substantive level it suggests
new units of analysis for AI, starting with the principled characterization
of interactions between agents and their environments and proceeding to an
exploration of the structural coupling between them.  On a critical level it
suggests a more sophisticated awareness of the inner conceptual workings of
the field: the inheritance the field has received from its forebears and the
technical difficulties that persist when this inheritance is not reexamined
in the light of experience.  It is conceivable that the research reported
here has stumbled upon the best possible set of substantive concepts to
guide future research.  But this is unlikely, and it would be unfortunate
to simply create a rigid new framework to replace the old one.  The focus on
interactions arose through reflexive study of the ideas and recurring tensions
in AI research, and this habit of reflection should be codified and taught.

Although this critical approach might be brought to the design of robots or
the study of insects, my own principal concern is with the study of human
beings.  The purpose of a ``critical cognitive science,'' I would propose,
is to employ computational techniques to study people and their lives while
simultaneously cultivating an awareness of the implicit theory of humanity
that this research presupposes and discovers.  A critical cognitive science
would be marked by the following six activities:

\begin{enumerate}
  \item taking computational ideas seriously {\sl as\/} ideas and
    investigating their place in the history of both ideas and institutions;
  \item studying the discursive forms (the metaphors, narratives, grammar, and
    so on) of computational research against this same background;
  \item using engineering methods as tools but doing so critically, not
    permitting them to import whole philosophical worldviews into the
    research;
  \item embracing technical difficulties and impasses as potentially
    instructive symptoms of internal tensions in the underlying ideas;
  \item critically interrogating the concepts of human beings and their lives
    that are implicit in technical ideas; and
  \item establishing dialogue with a wide variety of other fields, according
    equal value to technical and non-technical interlocutors.
\end{enumerate}

Measured against these standards, the research reported here provides simple,
inevitably flawed starting points.  The focus on interactions between agents
and their environments, for example, permits this research to enter into
dialogue with a wide variety of other research programs which also regard
interaction as constitutive of humanity.  Most of these research programs have
considerably more sophisticated ideas about interaction than computational
research can accommodate using the technical methods that have arisen to
date.  On the other hand, computational research provides powerful tools for
submitting theoretical concepts to practical tests.  The process of building
something regularly reveals issues that have been glossed over in descriptive
research, or even in formal laboratory research that has not fully enumerated
the assumptions that allow laboratory phenomena to be treated as evidence for
or against a theory.  Critical cognitive science will have matured when the
interdisciplinary dialogue routinely provides intellectual challenges in both
directions.

\thebibliography{99}

\bibitem
Philip E. Agre and David Chapman, Pengi: An implementation of a theory
of activity, Proceedings of the Sixth National Conference on Artificial
Intelligence, Seattle, 1987, pages 196-201.

\bibitem
Philip E. Agre and Ian Horswill, Cultural support for improvisation,
Proceedings of the Tenth National Conference on Artificial Intelligence, Los
Altos, CA: Morgan Kaufmann, 1992.

\bibitem
Philip E. Agre and Stanley J. Rosenschein, eds, Special Double Volume on
Computational Theories of Interaction and Agency, {\sl Artificial Intelligence}
72-73, 1995.

\bibitem
Philip E. Agre, The soul gained and lost: Artificial intelligence as a
philosophical project, Stanford Humanities Review 4(2), 1995a, pages 1-19.

\bibitem
Philip E. Agre, Computational research on interaction and agency, Artificial
Intelligence 72(1-2), 1995b, pages 1-52.

\bibitem
James Allen, James Hendler, Austin Tate, eds, Readings in Planning, San Mateo,
CA: Morgan Kaufmann, 1990.

\bibitem
Rodney A.~Brooks, A robust layered control system for a mobile robot, {\sl
IEEE Journal of Robotics and Automation} 2(1), 1986, pages 14-23.

\bibitem
David Chapman and Philip E. Agre, Abstract reasoning as emergent from concrete
activity, in Michael P. Georgeff and Amy L. Lansky, eds, Reasoning about
Actions and Plans: Proceedings of the 1986 Workshop, Morgan-Kaufmann
Publishers, Los Altos, CA, 1986.

\bibitem
Paul Edwards, The Closed World: Computers and the Politics of Discourse, MIT
Press, 1996.

\bibitem
Michael P. Georgeff and Amy L. Lansky, Reactive reasoning and planning,
Proceedings of the Sixth National Conference on Artificial Intelligence,
Seattle, 1987, pages 677-682.

\bibitem
Kristian J. Hammond, Timothy M. Converse, and Joshua W. Grass, The
stabilization of environments, Artificial Intelligence 72(1-2), 1995, pages
305-327.

\bibitem
Ian Horswill, Analysis of adaptation and environment, Artificial Intelligence
73(1-2), 1995, pages 1-30.

\bibitem
David Kirsh, The intelligent use of space, Artificial Intelligence 73(1-2),
1995, pages 31-68.

\bibitem
Thomas S. Kuhn, The Structure of Scientific Revolutions, Chicago: University
of Chicago Press, 1962.

\bibitem
David Marr, Vision, San Francisco: Freeman, 1982.

\bibitem
Humberto R. Maturana and Francisco J. Varela, The Tree of Knowledge: The
Biological Roots of Human Understanding, Boston: New Science Library, 1987.

\bibitem
George A. Miller, Eugene Galanter, and Karl H. Pribram, Plans and the
Structure of Behavior, Henry Holt and Company, 1960.

\bibitem
Allen Newell and Herbert A. Simon, GPS: A program that simulates human
thought, in Edward A. Feigenbaum and Julian Feldman, eds, Computers and
Thought, McGraw-Hill, 1963, pages 279-296.

\bibitem
Allen Newell and Herbert A. Simon, Human Problem Solving, Englewood Cliffs,
N.J., Prentice-Hall, 1972.

\bibitem
Stanley J. Rosenschein and Leslie Pack Kaelbling, The synthesis of digital
machines with provable epistemic properties, in Joseph Halpern, ed,
Proceedings of the Conference on Theoretical Aspects of Reasoning About
Knowledge, Monterey, CA, 1986.

\bibitem
Roger C. Schank, Dynamic Memory: A Theory of Reminding and Learning in
Computers and People, Cambridge University Press, 1982.

\bibitem
Marcel Schoppers, Universal plans for reactive robots in unpredictable
environments, Proceedings of the Tenth International Joint Conference on
Artificial Intelligence, Milan, 1987, pages 1039-1046.

\bibitem
Herbert A. Simon, Administrative Behavior: A Study of Decision-Making
Processes in Administrative Organization, second edition, New York, Macmillan,
1957.

\bibitem
Herbert A. Simon, The Sciences of the Artificial, Cambridge: MIT Press, 1970.

\end{document}
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991005040936/http://www.somewhere.com/)