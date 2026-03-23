---
id: computational-theories-of-interaction-and-agency
title: Computational Theories of Interaction and Agency
type: writing
tags:
- agre-primary
- ai-critique
- deictic-representation
- grammars-of-action
- embodied-cognition
- edited-volume
importance: 10
metadata:
  writing_type: edited-volume
  date: &id001 1995-02-01
  url: https://pages.gseis.ucla.edu/faculty/agre/aij-abstracts.html
  coauthors: &id002
  - Stanley Rosenschein
  key_concepts: &id003
  - deictic-representation
  - grammars-of-action
  importance: 10
  research_status: partial
writing_type: edited-volume
date: *id001
url: https://pages.gseis.ucla.edu/faculty/agre/aij-abstracts.html
coauthors: *id002
key_concepts: *id003
research_status: partial
---

## Source

Automatically imported from: https://pages.gseis.ucla.edu/faculty/agre/aij-abstracts.html

## Content

## Computational Theories of Interaction and Agency

### edited by Philip E. Agre University of California, San Diego Stanley J. Rosenschein Teleos Research MIT Press, 1996

The field of artificial intelligence has developed an "agent perspective",
expanding its focus from thought to action, from search spaces to physical
environments, and from problem-solving to long-term activity. Originally
published in February 1995 as volumes 72 and 73 of the journal Artificial
Intelligence, this book brings together seventeen papers by researchers
in artificial intelligence, neural networks, computer science, robotics,
and cognitive science on the themes of interaction and agency. Each paper
develops a distinct conceptual framework for the principled characterization
of interactions between agents and their environments, as well as the use
of such characterizations to guide the analysis of existing agents and the
synthesis of artificial agents.

Each abstract is accompanied by its full citation as a journal article.

---

**Computational Research on Interaction and Agency**

```
  Philip E. Agre
  Department of Communication
  University of California, San Diego
  La Jolla, California  92093-0503
  pagre@ucsd.edu
```

Recent research in artificial intelligence has developed computational
theories of agents' involvements in their environments. Although inspired
by a great diversity of formalisms and architectures, these research projects
are unified by a common concern: using principled characterizations of agents'
interactions with their environments to guide analysis of living agents
and design of artificial ones. This article offers a conceptual framework
for such theories, surveys several other fields of research that hold the
potential for dialogue with these new computational projects, and summarizes
the principal contributions of the articles in this special double volume.
It also briefly describes a case study in these ideas -- a computer program
called Toast that acts as a short-order breakfast cook. Because its designers
have discovered useful structures in the world it inhabits, Toast can employ
an extremely simple mechanism to decide what to do next.

Full citation: Philip E. Agre, [Computational research
on interaction and agency](https://web.archive.org/web/20200210084525/http://dlis.gseis.ucla.edu/people/pagre/aij-intro.html), Artificial Intelligence 72(1-2), 1995, pages
1-52.

---

**Sensorimotor Transformations in the Worlds of Frogs and Robots**

```
  Michael Arbib
  Center for Neural Engineering
  University of Southern California
  Los Angeles, California  90089-2520
  arbib%pollux.usc.edu@usc.edu

  Jim-Shih Liaw
  Center for Neural Engineering
  University of Southern California
  Los Angeles, California  90089-2520
  liaw@rana.usc.edu
```

The paper develops a multilevel approach to the design and analysis of
systems with "action-oriented perception", situating various robot and animal
"designs" in an evolutionary perspective. We present a set of biological
design principles within a broader perspective that shows their relevance
for robot design. We introduce schemas to provide a coarse-grain analysis
of "cooperative computation" in the brains of animals and the "brains" of
robots, starting with an analysis of approach, avoidance, detour behavior,
and path planning in frogs. An explicit account of neural mechanism of
avoidance behavior in the frog illustrates how schemas may be implemented
in neural networks. The focus of the rest of the article is on the relation
of instinctive to reflective behavior. We generalize an analysis of the
interaction of perceptual schemas in the VISIONS system for computer vision
to a view of the interaction of perceptual and motor schemas in distributed
planning which, we argue, has great promise for integrating mechanisms for
action and perception in both animal and robot. We conclude with general
observations on the lessons on relating structure and function which can be
carried from biology to technology.

Full citation: Michael A. Arbib and Jim-Shih Liaw,
Sensorimotor transformations in the worlds of frogs and
robots,
Artificial Intelligence 72(1-2), 1995,
pages 53-79.

---

**Learning to Act Using Real-Time Dynamic Programming**

```
  Andrew G. Barto
  Computer Science Department, LGRC
  University of Massachusetts
  Amherst, Massachusetts  01003-4610
  barto@envy.cs.umass.edu

  Steven J. Bradtke
  GTE Data Services
  One E Telecom Parkway, DC F4M
  Temple Terrace, Florida  33637
  bradtke@envy.cs.umass.edu

  Satinder Pal Singh
  Department of Brain and Cognitive Sciences
  Massachusetts Institute of Technology, E10-243
  Cambridge, Massachusetts  02139
  singh@psyche.mit.edu
```

Learning methods based on dynamic programming (DP) are receiving increasing
attention in artificial intelligence. Researchers have argued that DP
provides the appropriate basis for compiling planning results into reactive
strategies for real-time control, as well as for learning such strategies when
the system being controlled is incompletely known. We introduce an algorithm
based on DP, which we call Real-Time DP (RTDP), by which an embedded system
can improve its performance with experience. RTDP generalizes Korf's
Learning-Real-Time-A\* algorithm to problems involving uncertainty. We invoke
results from the theory of asynchronous DP to prove that RTDP achieves optimal
behavior in several different classes of problems. We also use the theory of
asynchronous DP to illuminate aspects of other DP-based reinforcement learning
methods such as Watkins' Q-Learning algorithm. A secondary aim of this
article is to provide a bridge between AI research on real-time planning and
learning and relevant concepts and algorithms from control theory.

Full citation: Andrew G. Barto, Steven J. Bradtke, and Satinder P. Singh,
Learning to act using real-time dynamic programming,
Artificial Intelligence 72(1-2), 1995,
pages 81-138.

---

**Learning Dynamics:   
System Identification for Perceptually Challenged Agents**

```
  Kenneth Basye
  Department of Math and Computer Science
  Clark University
  950 Main Street
  Worcester, Massachusetts  01610
  kbasye@black.clarku.edu

  Tom Dean
  Box 1910, Computer Science Department
  Brown University
  Providence, Rhode Island  02912
  tld@cs.brown.edu

  Leslie Pack Kaelbling
  Box 1910, Computer Science Department
  Brown University
  Providence, Rhode Island  02912
  lpk@cs.brown.edu
```

From the perspective of an agent, the input/output behavior of the environment
in which it is embedded can be described as a dynamical system. Inputs
correspond to the actions executable by the agent in making transitions
between states of the environment. Outputs correspond to the perceptual
information available to the agent in particular states of the environment.
We view dynamical system identification as inference of deterministic
finite-state automata from sequences of input/output pairs. The agent can
influence the sequence of input/output pairs it is presented by pursuing a
strategy for exploring the environment. We identify two sorts of perceptual
errors: errors in perceiving the output of a state and errors in perceiving
the inputs actually carried out in making a transition from one state to
another. We present efficient, high-probability learning algorithms for
a number of system identification problems involving such errors. We also
present the results of empirical investigations applying these algorithms to
learning spatial representations.

Full citation: Ken Basye, Tom Dean, and Leslie Pack Kaelbling,
Learning dynamics: System identification for perceptually
challenged agents,
Artificial Intelligence 72(1-2), 1995,
pages 139-171.

---

**A Dynamical Systems Perspective on
Agent-Environment Interaction**

```
  Randall D. Beer
  Department of Computer Engineering and Science
  Case Western Reserve University
  Cleveland, Ohio  44106-7071
  beer@cthulhu.ces.cwru.edu
```

Using the language of dynamical systems theory, a general theoretical
framework for the synthesis and analysis of autonomous agents is sketched.
In this framework, an agent and its environment are modeled as two coupled
dynamical systems whose mutual interaction is in general jointly responsible
for the agent's behavior. In addition, the adaptive fit between an agent
and its environment is characterized in terms of the satisfaction of a given
constraint on the trajectories of the coupled agent-environment system. The
utility of this framework is demonstrated by using it to first synthesize and
then analyze a walking behavior for a legged agent.

Full citation: Randall D. Beer,
A dynamical systems perspective on agent-environment
interaction,
Artificial Intelligence 72(1-2), 1995,
pages 173-215.

---

**On Information Invariants in Robots**

```
  Bruce Randall Donald
  Computer Science Department
  Cornell University
  Ithaca, New York  14850
  brd@cs.cornell.edu
```

We consider the problem of determining the information requirements to perform
robot tasks, using the concept of *information invariants*. This paper
represents our attempt to characterize a family of complicated and subtle
issues concerned with measuring robot task complexity. We also provide a
first approximation to a purely operational theory that addresses a narrow but
interesting special case.

We discuss several measures for the information complexity of a task: (a) How
much internal state should the robot retain? (b) How many cooperating agents
are required, and how much communication between them is necessary? (c) How
can the robot change (side-effect) the environment in order to record state or
sensory information to perform a task? (d) How much information is provided by
sensors? and (e) How much computation is required by the robot? We consider
how one might develop a kind of "calculus" on (a) -- (e) in order to compare
the power of sensor systems analytically. To this end, we attempt to develop
a notion of information invariants. We develop a theory whereby one sensor
can be "reduced" to another (much in the spirit of computation-theoretic
reductions), by adding, deleting, and reallocating (a) -- (e) among
collaborating autonomous agents.

Full citation: Bruce R. Donald,
On information invariants in robotics,
Artificial Intelligence 72(1-2), 1995,
pages 217-304.

---

**The Stabilization of Environments**

```
  Kristian J. Hammond
  Computer Science Department
  University of Chicago
  1100 East 58th Street
  Chicago, Illinois  60637
  kris@cs.uchicago.edu

  Timothy M. Converse
  Computer Science Department
  University of Chicago
  1100 East 58th Street
  Chicago, Illinois  60637
  converse@tartarus.uchicago.edu

  Joshua W. Grass
  Computer Science Department
  University of Chicago
  1100 East 58th Street
  Chicago, Illinois  60637
  grass@tartarus.uchicago.edu
```

In planning and activity research there are two common approaches to matching
agents with environments. Either the agent is designed with a specific
environment in mind, or it is provided with learning capabilities so that
it can adapt to the environment it is placed in. In this paper we look at
a third and underexploited alternative: designing agents which adapt their
environments to suit themselves. We call this *stabilization*, and we
present a taxonomy of types of stability that human beings typically both rely
on and enforce. We also taxonomize the ways in which stabilization behaviors
can be cued and learned. We illustrate these ideas with a program called
*FixPoint*, which improves its performance over time by stabilizing its
environment.

Full citation: Kristian J. Hammond, Timothy M. Converse, and Joshua W. Grass,
The stabilization of environments,
Artificial Intelligence 72(1-2), 1995,
pages 305-327.

---

**An Architecture for Adaptive Intelligent Systems**

```
  Barbara Hayes-Roth
  Knowledge Systems Laboratory
  Department of Computer Science
  Stanford University
  Stanford, California  94305
  bhr@camis.stanford.edu
```

Our goal is to understand and build comprehensive agents that function
effectively in challenging niches. In particular, we identify a class of
niches to be occupied by "adaptive intelligent systems (AISs)". In contrast
with niches occupied by typical AI agents, AIS niches present situations
that vary dynamically along several key dimensions: different combinations
of required tasks, different configurations of available resources, contextual
conditions ranging from benign to stressful, and different performance
criteria. We present a small class hierarchy of AIS niches that exhibit these
dimensions of variability and describe a particular AIS niche, ICU (intensive
care unit) patient monitoring, which we use for illustration throughout the
paper. To function effectively throughout the range of situations presented
by an AIS niche, an agent must be highly adaptive. In contrast with the
rather stereotypic behavior of typical AI agents, an AIS must adapt several
key aspects of its behavior to its dynamic situation: its perceptual strategy,
its control mode, its choices of reasoning tasks to perform, its choices
of reasoning methods for performing chosen tasks; and its meta-control
strategy for global coordination of all its behavior. We have designed and
implemented an agent architecture that supports all of these different kinds
of adaptation by exploiting a single underlying theoretical concept: *An
agent dynamically constructs explicit control plans to guide its choices among
situation-triggered behaviors*. The architecture has been used to build
experimental agents for several AIS niches. We illustrate the architecture
and its support for adaptation with examples from Guardian, an experimental
agent for ICU monitoring.

Full citation: Barbara Hayes-Roth,
An architecture for adaptive intelligent systems,
Artificial Intelligence 72(1-2), 1995,
pages 329-365.

---

**Analysis of Adaptation and Environment**

```
  Ian Horswill
  MIT Artificial Intelligence Laboratory
  545 Technology Square
  Cambridge, Massachusetts  02139
  ian@ai.mit.edu
```

Designers often improve the performance of artificial agents by specializing
them. We can make a rough, but useful distinction between specialization to
a task and specialization to an environment. Specialization to an environment
can be difficult to understand: it may be unclear on what properties of the
environment the agent depends, or in what manner it depends on each individual
property. In this paper, I discuss a method for analyzing specialization into
a series of *conditional optimizations*: formal transformations which,
given some constraint on the environment, map mechanisms to more efficient
mechanisms with equivalent behavior. I apply the technique to the analysis of
the vision and control systems of a working robot system in day to day use in
our laboratory.

The method is not intended as a general theory for automated synthesis
of arbitrary specialized agents. Nonetheless, it can be used to perform
*post-hoc* analysis of agents so as to make explicit the environment
properties required by the agent and the computational value of each
property. This *post-hoc* analysis helps explain performance in normal
environments and predict performance in novel environments. In addition, the
transformations brought out in the analysis of one system can be reused in the
synthesis of future systems.

Full citation: Ian Horswill, Analysis of adaptation and environment,
Artificial Intelligence 73(1-2), 1995,
pages 1-30.

---

**The Intelligent Use of Space**

```
  David Kirsh
  Department of Cognitive Science
  University of California, San Diego
  La Jolla, California  92093-0515
  kirsh@cogsci.ucsd.edu
```

The objective of this essay is to provide the beginning of a principled
classification of some of the ways space is intelligently used. Studies of
planning have typically focused on the temporal ordering of action, leaving
as unaddressed, questions of where to lay down instruments, ingredients,
work-in-progress, and the like. But, in having a body, we are spatially
located creatures: we must always be facing some direction, have only certain
objects in view, be within reach of certain others. How we *manage*
the spatial arrangement of items around us, is not an afterthought; it
is an integral part of the way we think, plan and behave. The proposed
classification has three main categories: spatial arrangements that simplify
choice; spatial arrangements that simplify perception; and spatial dynamics
that simplify internal computation. The data for such a classification is
drawn from videos of cooking, assembly and packing, everyday observations in
supermarkets, workshops and playrooms, and experimental studies of subjects
playing Tetris, the computer game. This study, therefore, focusses on
interactive processes in the medium and short term: on how agents set up their
*workplace* for particular tasks, and how they continuously manage that
workplace.

Full citation: David Kirsh,
The intelligent use of space,
Artificial Intelligence 73(1-2), 1995,
pages 31-68.

---

**Indexical Knowledge and Robot Action: A Logical Account**

```
  Yves Lespérance
  Department of Computer Science
  University of Toronto
  6 Kings College Road, Room 283
  Toronto, Ontario M5S 1A4
  Canada
  lesperan@cs.toronto.edu

  Hector J. Levesque
  Department of Computer Science
  University of Toronto
  6 Kings College Road, Room 283
  Toronto, Ontario M5S 1A4
  Canada
  levesque@ai.toronto.edu
```

The knowledge required for action is generally indexical rather than
objective. For example, a robot that knows the relative position of an
object is generally able to go and pick it up; he need not know its absolute
position. Agents may have very incomplete knowledge of their situation in
terms of what objective facts hold and still be able to achieve their goals.
 [This paper](https://web.archive.org/web/20200210084525/ftp://ftp.cs.toronto.edu/pub/cogrob/indexmodal.ps.Z)
presents a formal theory of knowledge and action, embodied in a modal logic,
that handles the distinction between indexical and objective knowledge and
allows a proper specification of the knowledge prerequisites and effects of
action. Several kinds of robotics situations involving indexical knowledge
are formalized within the framework; these examples show how actions can be
specified so as to avoid making excessive requirements upon the knowledge
of agents. Various other papers on related issues can be found in our
[repository](https://web.archive.org/web/20200210084525/ftp://ftp.cs.toronto.edu/pub/cogrob/README.html).

Full citation: Yves Lespérance and Hector J. Levesque,
Indexical knowledge and robot action: A logical account,
Artificial Intelligence 73(1-2), 1995,
pages 69-115.

---

**Exploiting Patterns of Interaction to Achieve Reactive Behavior**

```
  Damian Lyons
  A. J. Hendriks
  Philips Laboratories
  Philips Electronics North America Corporation
  Briarcliff Manor, New York  10510
  dml@philabs.philips.com
```

This paper introduces an approach that allows an agent to *exploit*
inherent patterns of interaction in its environment, so-called dynamics,
to achieve its objectives. The approach extends the standard treatment of
planning and (re)action in which part of the input to the plan generation
algorithm is a set of basic actions and perhaps some domain axioms. Real
world actions are typically difficult to categorize consistently and are
highly context dependent. The approach presented here takes as input a
procedural model of the agent's environment and produces as output a set of
action descriptions that capture how the agent can exploit the dynamics in
the environment. An agent constructed with this approach can utilize context
sensitive actions, "servo" style actions, and other intuitively efficient ways
to manipulate its environment.

A process-algebra based representation, *RS*, is introduced to model
the environment and the agent's reactions. The paper demonstrates how to
analyze an *RS* environment model so as to automatically generate a set
of potentially useful dynamics and convert these to action descriptions. The
output action descriptions are designed to be input to an Interval Temporal
Logic based planner. A series of examples of reaction construction drawn
from the *kitting robot* domain is worked through, and the prototype
implementation of the approach described.

Full citation: Damian M. Lyons and A.J. Hendriks,
Exploiting patterns of interaction to achieve reactive
behavior,
Artificial Intelligence 73(1-2), 1995,
pages 117-148.

---

**A Situated View of Representation and Control**

```
  Stanley J. Rosenschein
  Teleos Research
  576 Middlefield Road
  Palo Alto, California  94301
  stan@teleos.com

  Leslie Pack Kaelbling
  Box 1910, Computer Science Department
  Brown University
  Providence, Rhode Island  02912
  lpk@cs.brown.edu
```

Intelligent agents are systems that have a complex, ongoing interaction
with an environment that is dynamic and imperfectly predictable. Agents are
typically difficult to program because the correctness of a program depends on
the details of how the agent is situated in its environment. In this paper,
we present a methodology for the design of situated agents that is based on
*situated-automata theory*. This approach allows designers to describe
the informational content of an agent's computational states in a semantically
rigorous way without requiring a commitment to conventional run-time symbolic
processing. We start by outlining this situated view of representation,
then show how it contributes to design methodologies for building systems that
track perceptual conditions and take purposeful actions in their environments.

Full citation: Stanley J. Rosenschein and Leslie Pack Kaelbling,
A situated view of representation and control,
Artificial Intelligence 73(1-2), 1995,
pages 149-173.

---

**The Use of Dynamics in an Intelligent Controller for a Space Faring Rescue Robot**

```
  Marcel Schoppers
  Robotics Research Harvesting
  P.O. Box 2111
  Redwood City, California  94063
  mjs@hpp.stanford.edu
```

The NASA Extra Vehicular Activity Retriever (EVAR) robot is being designed to
retrieve astronauts or objects that become detached from the orbiting Space
Station. This task requires that the robot's intelligent controller must rely
heavily on orbital dynamics predictions, without becoming blind to the wide
variety of anomalies that may occur.

This article describes the controller's Universal Plan (U.P.) and some
technical lessons learned from it. The U.P. reacts not to actual current
states but to estimated states, which are obtained using goal-directed active
perception. A modal logic formalization of discrete-event dynamics allows us
to finely analyze and specify the interactions of knowledge, belief, sensing,
acting, and time within the U.P. The U.P. now acts like a hands-off manager:
it makes regular observations, grants some leeway for unobservable or
ill-modelled processes, has faith in subsystem dynamics, and takes action only
to manipulate subsystems into delivering desired progress. Most of the time,
the appropriate action is to do nothing.

Finally we examine properties of the application that allowed the U.P. to
deliver robust goal achievement despite misleading state estimates, weak
models of relevant processes, and unpredictable disturbances.

Full citation: Marcel Schoppers,
The use of dynamics in an intelligent controller for a space
faring rescue robot,
Artificial Intelligence 73(1-2), 1995,
pages 175-230.

---

**On Social Laws for Artificial Agent Societies: Off-Line Design**

```
  Yoav Shoham
  Department of Computer Science
  Stanford University
  Stanford, California  94035
  shoham@flamingo.stanford.edu

  Moshe Tennenholtz
  Faculty of Industrial Engineering and Management
  Technion -- Israel Institute of Technology
  Haifa 32000
  Israel
  moshet@ie.technion.ac.il
```

We are concerned with the utility of social laws in a computational
environment, laws which guarantee the successful coexistence of multiple
programs and programmers. In this paper we are interested in the off-line
design of social laws, where we as designers must decide ahead of time on
useful social laws. In the first part of this paper we suggest the use of
social laws in the domain of mobile robots, and prove analytic results about
the usefulness of this approach in that setting. In the second part of this
paper we present a general model of social law in a computational system,
and investigate some of its properties. This includes a definition of the
basic computational problem involved with the design of multi-agent systems,
and an investigation of the automatic synthesis of useful social laws in the
framework of a model which refers explicitly to social laws.

Full citation: Yoav Shoham and Moshe Tennenholtz,
On social laws for artificial agent societies: Off-line
design,
Artificial Intelligence 73(1-2), 1995,
pages 231-252.

---

**Instructions, Intentions and
Expectations**

```
  Bonnie Webber
  Norman Badler
  Barbara Di Eugenio
  Chris Geib
  Libby Levison
  Michael Moore 
  Department of Computer and Information Science
  University of Pennsylvania
  200 South 33rd Street
  Philadelphia, Pennsylvania  19104-6389
  bonnie@central.cis.upenn.edu
```

Based on an ongoing attempt to integrate Natural Language instructions with
human figure animation, we demonstrate that agents' understanding and use
of instructions can complement what they can derive from the environment
in which they act. We focus on two attitudes that contribute to agents'
behavior -- their intentions and their expectations -- and shown how Natural
Language instructions contribute to such attitudes in ways that complement
the environment. We also show that instructions can require more than one
context of interpretation and thus that agents' understanding of instructions
can evolve as their activity progresses. A significant consequence is that
Natural Language understanding in the context of behavior cannot simply
be treated as "front end" processing, but rather must be integrated more
deeply into the processes that guide an agent's behavior and respond to its
perceptions.

Full citation: Bonnie Webber, Norman Badler, Barbara Di Eugenio, Chris Geib,
Libby Levison, and Michael Moore, Instructions, intentions and expectations,
Artificial Intelligence 73(1-2), 1995, pages 253-269.

---

**Reinforcement Learning in Non-Markov Environments**

```
  Steven Whitehead
  STMS, Adaptive Systems Department
  GTE Laboratories Incorporated
  40 Sylvan Road
  Waltham, Massachusetts  02254
  swhitehead@gte.com

  Long Ji Lin
  Siemens Cororate Research Inc
  755 College Road East
  Princeton, New Jersey  08540
  lgl@learning.scr.siemens.com
```

Techniques based on reinforcement learning (RL) have been used to build
systems that learn to perform nontrivial sequential decision tasks. To
date, most of this work has focused on learning tasks that can be described
as Markov decision processes. While this formalism is useful for modeling a
wide range of control problems, there are important tasks that are inherently
non-Markov. We refer to these as *hidden state* tasks since they
arise when information relevant to identifying the state of the environment
is *hidden* (or missing) from the agent's immediate sensation. Two
important types of control problems that resist Markov modeling are those
in which (1) the system has a high degree of control over the information
collected by its sensors (e.g., as in active vision), or (2) the system
has a limited set of sensors that do not always provide adequate information
about the current state of the environment. Existing RL algorithms perform
unreliably on hidden state tasks.

This article examines two general approaches to extending reinforcement
learning to hidden state tasks. The *Consistent Representation (CR)
Method* unifies recent approaches such as the Lion algorithm, the
G-algorithm, and CS-QL. The method is useful for learning tasks that
require the agent to control its sensory inputs. However, it assumes that,
by appropriate control of perception, the external states can be identified
at each point in time from the immediate sensory inputs. A second, more
general set of algorithms in which the agent maintains internal state over
time is also considered. These *stored-state* algorithms, though quite
different in detail, share the common feature that each derives its internal
representation by combining immediate sensory inputs with internal state which
is maintained over time. The relative merits of these methods are considered
and conditions for their useful application are discussed.

Full citation: Steven D. Whitehead and Long-Ji Lin,
Reinforcement learning of non-Markov decision processes,
Artificial Intelligence 73(1-2), 1995,
pages 271-306.

---
