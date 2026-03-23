---
id: red-rock-eater-digest-computation-and-human-experience
title: Red Rock Eater Digest - Computation and Human Experience
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/2000/RRE.Computation.and.Huma.html
importance: 6
research_status: partial
tags:
  - activism
  - ai
  - civil-liberties
  - cognitive-science
  - commerce
  - cryptography
  - education
  - environment
  - government-info
  - international
  - internet-policy
  - labor
  - law
  - media
  - military
  - religion
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/2000/RRE.Computation.and.Huma.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20000816232124/http://commons.somewhere.com/rre/) | **Most Recent Article: Tue, 15 Aug 2000** |

```
[Back in 1997 I published a book, "Computation and Human Experience",
that maybe five people have read.  It's not about the Internet and
it's not about politics.  It's about what computers are, in a deep
sense, and it proceeds through a relentless study of the dynamics of
research in one avant-garde subfield of computer science: artificial
intelligence (AI).  AI is the subject in which I received my PhD, and
I regard it simultaneously as a powerful way of looking at the world
and as dangerous nonsense.  (Neoclassical economics is the same way.)
I spent several years figuring out how to resolve this tension within
myself and in my relations with AI people, and though most of the AI
people no doubt think I'm a jerk, at least I can have a civil chat with
some of them.  The book reflects this tension, and tries to explain
in great depth the precise relationship between the dangerous-nonsense
aspects of AI and the powerful-way-of-looking-at-the-world aspects.
It's a long book, and with its equal recourse to the theories of
Derrida and Heidegger and to the notations and narrative conventions
of computer science it is guaranteed to offend just about everyone.

The chapter I've enclosed is an early discussion of what computers
are.  It is organized around the dialectical relationship in computer
science between "implementation" -- that is, the physical realization
of computers as objects in the physical world that obey the laws
of physics -- and "abstraction" -- the ideas and language that are
inscribed in the computer, and that need have no particular relation
to the laws of physics.  For those who don't know how computers work,
it provides an introduction to things like wires.  (Things like gates
have to wait until Chapter 5.)  For those who do know how computers
work, the chapter is supposed to defamiliarize any such knowledge,
so that commonplace technical constructs like variables start to seem
strange again.  Much of the chapter is taken up recounting various
controversies from the history of AI that readers will find unfamiliar.
But the deep purpose of the chapter is not to explain or settle those
controversies, which are not very important in the long run, but to
draw more fundamental conclusions about the nature of computation.

In particular, throughout the book I aim to deconstruct that mistaken
conception of people and their lives that I call "mentalism": the idea
(as, for example, in Descartes) that we have an internal space called
"the mind" that is radically different in nature from the outside
world, and yet that (precisely because of its radical difference from
the outside world) ends up mirroring the outside world in great detail
in the form of "knowledge".  This is not to say that people don't have
minds, don't have knowledge, don't set themselves apart from the world,
etc, much less that people don't have brains, aren't intelligent, etc.
Rather, it is to say that we cannot understand people's relationships
to their surroundings except against the background of a prior deep
embedding and immersion that should blow up received philosophical and
technical ideas about the mind, knowledge, and much else.  I aim to
demonstrate all of this by closely following the internal logic of AI
research and showing how it deconstructs itself.  The method is thus
closely related to Derrida's method of deconstruction as applied to
philosophical ideas, but it embraces none of the relativism, idealism,
nihilism, quietism, and other philosophical solecisms that Derrida is
often (and most often wrongly) accused of.  Anyway, I hope that you
will find this enclosed chapter useful on its own, and that it will
provoke you to buy the book, which despite its serious shortage of
commercial viability is still very much in print.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
You are welcome to send the message along to others but please do not use
the "redirect" option.  For information about RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html

---

Computation and Human Experience
Philip E. Agre
Cambridge University Press, 1997.

You are welcome to forward this chapter to others, but please do not
quote from it because it changed slightly in proof.  This version of
the chapter includes the complete text, but it is missing footnotes
and a lot of gnarly typesetting.

Chapter 4. Abstraction and implementation

Structures of computation

All engineering disciplines employ mathematics to represent the
physical artifacts they create.  The discipline of computing, however,
has a distinctive understanding of the role of mathematics in design.
Mathematical models can provide a civil engineer with some grounds
for confidence that a bridge will stand while the structure is still
on paper, but the bridge itself only approximates the math.  The
computer, by contrast, conforms precisely to a mathematically defined
relationship between its inputs and its outputs.  Moreover, a civil
engineer is intricately constrained by the laws of physics: only
certain structures will stand up, and it is far from obvious exactly
which ones.  The computer engineer, by contrast, can be assured of
realizing any mathematical structure at all, as long as it is finite
and enough money can be raised to purchase the necessary circuits.

The key to this remarkable state of affairs is the "digital
abstraction": the discrete 0s and 1s out of which computational
structures are built.  This chapter and the next will describe the
digital abstraction and its elaborate and subtle practical logic
in the history of computer engineering and cognitive science.  The
digital abstraction is the technical basis for the larger distinction
in computer work between abstraction (the functional definition of
artifacts) and implementation (their actual physical construction).
Abstraction and implementation are defined reciprocally: an
abstraction is abstracted from particular implementations and an
implementation is an implementation of a particular abstraction.
This relationship is asymmetrical: a designer can specify an
abstraction in complete detail without making any commitments about
its implementation.  The relationship is confined to the boundaries
of the computer; it does not depend on anything in the outside world.

Computer engineering uses abstraction to organize its work into a
hierarchy of relatively independent levels, each with its own research
community.  At the lowest level, device physicists can use any
materials they like to build their circuitry, as long as they can
support the most basic abstraction of binary arithmetic.  Computer
designers, likewise, can specify whatever architectures they like,
as long as they can be programmed in a general way.  The authors
of compilers (the programs that translate high-level programming
languages such as Fortran and Pascal into the machine languages that
computer hardware interprets directly) can explore a wide variety of
techniques, as long as their compilers support the semantics of some
language that programmers find congenial.  These programmers, finally,
can implement whatever abstractions they choose, simply by writing
programs.  These programs may employ several levels of abstraction as
well, each with a formally defined relationship to the levels below
and above it.

Philosophical accounts of computation and its relationship to AI
have placed much emphasis on the independence of the various levels
of a computational system (e.g., Haugeland 1985: 58).  And indeed,
a snapshot of computational practice at any given place and time
will probably resemble this picture of neatly separated levels of
abstraction.  The historical reality, though, is more complicated.
The practical logic of computing is driven by a variety of factors,
but the most pervasive factor is straightforward efficiency: the
amount of useful computational work that gets done in the service
of specified goals by a given amount of machinery in a given period
of time.  The demands of efficiency continually undermine the
independence of the various levels of abstraction in conventional
computer systems; more generally they undermine the separation between
abstraction and implementation.  At any given juncture in technical
history, this tension becomes manifest through the emergence of new
and often surprising design trade-offs, as well as a coevolutionary
pressure for mutual adaptation among the various levels of
abstraction.

In their everyday practice, few computer programmers must
consciously negotiate trade-offs between matters of abstraction
and implementation.  Programmers are very concerned with efficiency,
of course, and they have accumulated and codified a great deal of
experience in choosing the most efficient algorithms for a given
task.  Nonetheless, their design choices are heavily constrained by
the particular computer architectures with which they work.  The vast
majority of programmers work on computers with serial architectures.
A serial processor is called "serial" because it performs only a
single small operation, or "instruction," at a time.  It has often
been observed that a serial computer attempts to defy the demands of
physical implementation.  Though it might consist of several million
circuits distributed through a cubic foot of space, only a small
proportion of these circuits will actually be doing useful work at any
given time (Hillis 1985: 1-5).  Serial machines are thus located at
an extreme in the space of trade-offs between freedom of abstraction
and efficiency of implementation: they offer a maximum of freedom with
a minimum of efficiency.

As a result, many people have assumed that computers would be much
more efficient if they were highly parallel, that is, if they worked
by performing a large number of useful operations all the time.  A
highly parallel computer would distribute the useful work uniformly
throughout its circuitry rather than trying to cram it into a single
central processor.  Computational theorists and computer designers
have invested enormous effort into exploring the forms that
distributed computation might take (Almasi and Gottlieb 1994; Denning
and Tichy 1990; Hillis and Barnes 1987; Kitano and Hendler 1994).
But parallel computers have not become prevalent because programmers
have not been willing to give up the freedom of serial computing.
The performance of a serial machine might be tolerable for most tasks,
and so the computer market provides manufacturers with the enormous
amount of capital required to produce successive generations of serial
machines.  Any given parallel architecture, by contrast, will probably
occupy a niche market because its performance will be extremely
high on some categories of tasks and relatively poor on others.
For example, a computer that consists of a dozen serial processors
communicating over a network will perform well on tasks that can be
decomposed into a moderate number of roughly independent subtasks;
on other tasks, the processors will probably spend most of their time
waiting for the network rather than doing useful work.  Discovering
a suitable decomposition for a task is often difficult.  Specifically,
in order to benefit from parallel execution, a computation must
be organized so that it can be distributed in a natural way across
the spatial extent of a parallel machine (cf. Hillis 1985: 137-144).
On this view, *one foundation of efficient design is a natural
correspondence between the structure of a computation and the
structure of its physical implementation*.

An important example of this principle is found in the first several
stages of visual processing (known as "early vision"), according to
computational neurophysiologists such as Marr (1982).  According to
this theory, the visual cortex is organized, at least in part, as a
set of modules, each of which computes some function from one version
of the visual image to another.  Although the exact roster of these
computations is still uncertain, a typical proposal is that a certain
module takes in a slightly blurred version of the retinal image and
produces a map of where the edges in the image are located.  Another
module takes in these edge maps for both eyes (i.e., a stereo edge
map) and produces a map of "depth" (i.e., how far away the physical
edges actually are).  The salient aspect of these computations for
our purposes here is their physical organization.  Nature might
have implemented these modules in many ways, but in fact they are
constructed in accord with a natural correspondence between the
uniform two-dimensional structure of the images and the uniform
two-dimensional structure of the neural machinery itself.  That is,
each successive stage of the cortical circuitry that implements early
visual processing is organized as a flat sheet of computing elements.
As a result, most of the wires within a given stage can be fairly
short, transporting a signal from a given computing element to its
neighbors.

The resulting visual architecture has a striking simplicity: whereas
a serial computer must constantly shift its attention among different
processes and different data, every element of the early visual
system performs its single assigned task all the time.  But not
all computations will be so lucky.  When computations are less
naturally implemented, the work is distributed less evenly through
the circuitry.  Of course, a designer might have good reasons for
building a computer that implements its computations in a relatively
inefficient way: standardization, maintenance issues, functional
flexibility, conventional divisions of design labor, and so forth.
That these nonoptimal design options are available at all is testimony
to the power of computation: the separation between abstraction
and implementation remains perfectly valid as a conceptual matter,
regardless of how natural it is as a practical matter.

What makes the conceptual separation between abstraction and
implementation possible is a simple but profound invention: the wire.
By connecting two physically distant points in a circuit, wires allow
the designer the maximum latitude in choosing the manner in which
a given abstraction is to be implemented.  Given enough wires, a
computer designer can physically implement an arbitrary abstract
network of computing elements.  This is why technical papers about
computer architectures can provide functional specifications using
diagrams made of boxes and arrows without providing any clue as to
the actual physical geometry of the circuits that implement them.
And indeed, the people who finally build these computers spend
a large part of their time getting the sheer mass of wires under
control.  By loosening the constraints imposed on a designer by the
three-dimensional geometry of space, wires allow the designer to
decouple the causal patterns of an abstractly specified device from
the spatially localized causality of its physical implementation.

It is thus possible, as an engineering option, to implement one's
computations in perfect defiance of physical locality.  But in doing
so one pays a price in the efficiency of the resulting artifacts:
computers with shorter wires are faster, other things being equal,
because electrical signals travel along wires at a finite speed.
As computers grow larger and the pure velocity of computation becomes
a dominant design goal, the technology begins to break down and
reorganize itself within new, more rigorous correspondences between
abstraction and implementation.  Hardware designers, for example,
often cut wires to precise lengths, so that each signal will arrive
at its destination at the exact moment when it is needed.  Similarly,
even though a memory chip maintains the digital abstraction in its
outward behavior (if you store a 1 in a given memory location, you
will get a 1 back later on), most memory chips do not actually employ
the digital abstraction in their internal circuitry, which is in fact
a sophisticated analog circuit that takes advantage of the physical
properties of the materials from which it is made.  Furthermore, one
of the innovations of the IBM 801 computer, which started the trend
toward RISC (reduced instruction-set computing) processor architectures,
was that the processor and its compilers were codesigned, introducing
peculiar instructions that permitted the processor to keep more of its
circuitry usefully busy in complex situations (Hennessy and Patterson
1994; Radin 1983).  In each case, the drive for efficiency has brought
a more detailed understanding of the physical reality of computation
to bear on the problem of implementing digital abstractions.

The moral of the story is that abstraction and implementation, far
from being independent levels of technical description, are actually
engaged in a dialectical relationship.  Though one might wish to
define each of them without any heed to the other, their fates will
necessarily become intertwined as demands for efficiency intensify.
As technological development explores the endlessly ramifying space of
design trade-offs, implementation and abstraction will continue to be
pulled into a close and potentially complicated relationship.  Factors
of marketing and management have largely hidden this dialectic from
the consumers and philosophers of computation.  Yet, I would like to
argue, it is a fact with important and little-understood consequences
for computational psychology.

A case study: variables
	
The history of computer design can be understood in large part, then,
as the unfolding of dialectical interactions among various aspects
of implementation and abstraction.  A case study in this history
that will take on particular significance in later chapters of this
book concerns the development of two central abstractions of serial-
computer programming, pointers and variables.

Serial computers were originally designed to automate calculations
already performed in a routinized fashion by human beings --
themselves often called computers -- in military and business
environments.  Today this type of step-by-step calculation scheme
is probably most familiar, at least in the United States, from income
tax forms.  A typical calculation step, or "instruction," might be
glossed as "Add lines 31 and 40 and enter the result on line 41."
This instruction would be represented inside the machine using a
sequence of four numbers, one for the "add" operation and the other
three for the "addresses" of the "registers" containing the operands
(31 and 40) and the result (41).  This is the "register-transfer"
model of computation upon which virtually all modern computers are
based.  Each register, or "word," of the computer's "memory" is
implemented by an actual physical circuit that stores a sequence of
binary values.  The first computers had only a few hundred words of
memory, but memories of several million words are common today.  Each
register's address is itself a binary quantity.  In a thousand-word
memory an address can be specified with ten bits; in a million-word
memory twenty bits are required.  As a result, a single instruction
can require nearly seventy bits: half a dozen to specify the operation
("add," "subtract," "compare," etc.), twenty each for the operands and
result, and a few more for other miscellaneous purposes.

In practice this way of specifying instructions is too cumbersome.
Much space is wasted by instructions that do not require the full
three-operand format.  As a result, computer architects began
to reserve the word "register" for a small portion of the memory.
In the tax-form analogy, registers corresponded to scraps of paper
where individual operations were set up and performed, with the
results being copied back onto the indicated line of the tax form.
An instruction such as "Add words 31 and 40 and store the result in
word 41" would now be broken into three parts:

  1. Load word 31 into register 3.
  2. Add word 40 into register 3.
  3. Store register 3 into word 41.

Breaking instructions into smaller pieces permitted each instruction
to be specified in a single word of memory (perhaps five bits for
the operation, five bits for the register, twenty bits for the
memory address, and a few miscellaneous bits).  Furthermore, since
the registers could be implemented in faster circuitry than the
millions of general-purpose memory words, many computations could be
accelerated by keeping frequently used quantities in registers as long
as possible.  More generally, computer memory is now organized in a
hierarchy, with small numbers of faster memory elements close to the
central processor and large numbers of slower elements farther away.

An important extension to the register-transfer model of computation
was the invention of *indirect reference*.  In the conventional model,
a word of memory contains either an instruction or an item of data,
and these data refer to things in the outside world, such as an air
pressure or an adjusted gross income.  In the extended model, a word
of memory can also contain the address of another word of memory.
An instruction can now refer indirectly to a quantity in memory,
not by specifying its address but by specifying an address where its
address can be found.  For example, consider this instruction:

  Load word @7 into register 3.

The "@" symbol indicates indirect reference.  The execution of this
instruction proceeds in two steps: the processor first reads the
contents of register 7 and then, interpreting the resulting value as
a memory address, loads the value at that address into register 3.
Without indirect reference, any given serial-machine computation is
laid out across the machine's memory in a fixed configuration, in the
same way that an income-tax calculation is laid out across a piece of
paper; every word of memory has a fixed meaning ("dividend income,"
"social security benefits," "alternative minimum tax," etc.).
Indirect reference frees a computation from this fixed correspondence
to the underlying hardware.  In practice, programmers use indirect
reference in stereotyped ways, using a set of conventions that
collectively implement some useful form of abstraction.  As with all
abstractions, systematic use of indirect reference entails a decrease
in efficiency, since an additional memory "fetch" is now required
to load each value from memory.  Programmers have often argued about
the costs and benefits of programming innovations based on indirect
reference, but the cause of increased abstraction has usually won.

One such innovation is the use of "pointers" to create dynamically
linked record structures.  A particularly simple form of record
structure is the "list," in which each record includes the address
of the next record.  This address is called a pointer.  The records
can be located anywhere in memory, but a program can step through
them by following the pointers.  In the Lisp programming language,
for example, the simple list of four symbols that would be notated
as "(london paris zurich prague)" would be implemented using four
records, as follows:

address 704: 
  value = "paris"
  next = 1731

address 1030:
  value = "london"
  next = 704

address 1366:
  value = "prague"
  next = 0

address 1731:
  value = "zurich"
  next = 1366

A register could "point" at the list simply by containing the number
1030, which is the address of the first record in the list.  By
convention, the pointer to address 0 in the "prague" record indicates
that the list has ended (Knuth 1983).

By using enough interlinked lists, a programmer can construct
enormous symbolic structures.  These structures might be interpreted
as computer programs (in a compiler) or as syntactic structures (in
linguistics) or as a representation of the outside world (a "knowledge
base" or "world model").  Given some memory and the operations for
manipulating pointers, a program can build new structures, tear down
old ones, revise existing ones in accord with changing conditions, and
so forth.  This idea is the basis of symbolic programming (Abelson and
Sussman 1984; Newell 1961).

The notion of a variable is more subtle.  The problem is that the term
"variable" has no single definition.  In fact it has a wide variety
of definitions, some computational and some not.  Historically, the
algebraic notion of a variable arose slowly, acquiring a recognizably
modern form only during the Renaissance (Klein 1968).  This is the
kind of variable one encounters in middle school, in exercises such as

  3x - 4 = 5.

Here, at least on one conception, the variable x "stands in" for a
definite but currently unknown quantity.  Another mathematical use of
variables is in defining functions, as in

  f(x) = x^2 - 7x + 5.

In this case, the meaning is something more like "Whatever x is, f(x)
is this," where each occurrence of x is supposed to correspond to the
same value.  In set-theoretic terms, a function is simply a set of
pairs, each matching a value of x to the corresponding value of f(x).
The word "variable" does not refer to any part of this structure;
instead, it refers ambiguously to the symbol x and to the single
argument position of the function f (a "function of one variable").
Yet a third use of variables is quantification in formal logic, for
example:

  forall(x) person(x) -> exists(y) mother(y,x).
    "Everyone has a mother."

Even more obscure types of variables are found in higher branches of
mathematics.  Galois theory, for example, can be used to investigate
the solutions of polynomials; one begins by taking some field, F,
adding a symbol such as X, and then "closing" the resulting set under
the field's equivalents of addition and multiplication to obtain a new
extended field, F[X] of polynomial formulas (Goldstein 1973: 301-323).
This X, however, is not just an element of notation like the x's of
earlier examples; it also designates a symbol-like component of the
mathematical structures that are being investigated.

In each of these cases, the common element is a syntactic indication
of reference within some range of possibilities without a predetermined
choice among them.  But this is just a family relationship across a
disparate series of phenomena, each of which is perfectly well defined
in its own context.  Nonetheless, it will be useful to give this vague
general notion a name, so I will call it nonspecificity.

Programming languages employ a wide range of variable-like
mechanisms, each of which resolves the tension between abstraction and
implementation in its own way.  In each case, the purpose is to permit
an algorithm to be expressed without reference to particular numbers
or symbols.  Just as a million people can fill out the same tax form
and come up with different correct answers, so a million computers
can run the same program on different input data and return different
correct outputs.  Every programming language comes with its own
abstract conception of computation (its "virtual machine"), which may
or may not stand in any direct correspondence to the machinery that
will run the programs.  Programming languages are generally reckoned
as "low-level" or "high-level" according to the closeness of this
correspondence.  At the lowest extreme, a "machine language" consists
of the bit-patterns that a given computer architecture can execute
directly.  An "assembly language" provides the programmer with
comprehensible symbolic codes that can be translated straightforwardly
into a given machine language.  A slightly higher-level language,
like the widely used language C, maps closely onto the generic
register-transfer model of serial computing without being biased
toward any particular serial architecture.  And a truly high-level
language, like Lisp, will include a variety of abstract features
whose mapping onto a conventional register-transfer architecture
is not straightforward.  In order to execute a program in such a
language, the programmer provides the program as input to a compiler,
which translates it into a given architecture's machine language.

The "height," or degree of abstraction, of a programming language can
be measured in a rough way by the extent to which it uses indirect
reference to loosen the correspondence in time and space between the
program and the machinery that implements it.  In early programming
languages the correspondence was strong.  A variable in such a
language was implemented through a direct reference to a word of
memory whose contents could actually vary: it might have the value
of 23 at nine o'clock and the value of 31 a minute later.  Variables
seemed like mutable, physical things and bore little resemblance to
variables in mathematics.

The spatial and temporal correspondence between the program and its
implementation dissolved quickly with the development of high-level
languages.  These languages implement variables not in definite memory
locations but rather in *stack frames*, which allow several instances
of the same stretch of code to be in progress at the same time.
To load the value of a variable, the machine performs an indirect
reference within an area of memory known as a stack.  A given
instance of some variable has a definite lifetime, during which its
value is unlikely to change.  In general, the trend is for variables
to become less like physical things and more like the variables of
mathematics.  Indeed, in a language like Prolog the notion of time has
almost no place, so that variables become abstractions with complex
mathematical properties and a highly indirect relationship to the
underlying hardware.  (In practice, however, Prolog programmers are
vividly aware of the temporal order in which their programs will be
executed.)

The most extreme accomplishment in the general trend toward
computational abstraction is Smith's (1985) 3-Lisp language,
whose formal specification envisions an infinitely deep tower
of abstractions that never "grounds out" in physical hardware.
As a result, a 3-Lisp program can sustain the illusion of actually
modifying the machinery upon which it is running.  The actual running
system underwrites this illusion by quickly interpolating a new
layer of abstraction between the implementation and the previously
existing abstractions each time the immutable hardware threatens to
"show through."  The 3-Lisp language encounters the trade-off between
efficiency of implementation and freedom of abstraction in its most
radical form.

When high-level languages were first developed, it was not obvious
that they were worth the trouble.  Computers were still relatively
expensive to operate and the compiled programs were slow.  But
compiler technology has grown steadily more sophisticated, so that
little is lost by taking advantage of the convenience of high-level
languages.  As a result, assembly languages are used only for
exceptional purposes.  But compilers for serial computers have a
relatively easy job because they have little to gain by reasoning
about the relationship between the structure of a computation and the
structure of its physical implementation.  The compiler's only goal
is minimizing the number of instructions that are executed within the
extended register-transfer framework.

This issue is particularly crucial for computational theories
of cognition that rely on highly abstract notions of variables.
Competent agency requires a significant degree of nonspecificity: one
must be equally alert on Monday and Tuesday, in conversing with this
person or that, drinking from one cup or another, walking down one
street or the next.  Computational models have generally achieved this
nonspecificity of reference to the concrete particulars of thought
and action through the use of variables.  In some theories these
are explicitly the quantified variables of formal logic.  In other
theories, for example in production systems, the notion of variable is
tied to a specific mechanism in which nonspecific "rules" have certain
effects when the agent's database contains specific structures that
they "match."  (More of this in Chapter [x].)  In each case, the agent
represents the objects in specific situations by assigning them names,
or "constants," such as BLOCK-9 and CAR-37.  The agent applies its
nonspecific knowledge to particular individuals by "filling in" the
variables with the names.  Likewise, the agent formulates the general
lessons it learns in a given situation by replacing the constants with
variables, thus producing nonspecific knowledge that can be applied to
other individuals on another day.  In each case, the use of variables
induces a degree of seriality in a computation that might otherwise be
performed in parallel; the relatively complex mechanism that matches
variables with constants is a scarce resource that can only be
assigned to one purpose at a time (Newell 1980).  This understanding
of nonspecific knowledge will take on a deeper significance toward
the end of Chapter [x].  For the moment, the important point is its
great degree of abstraction from conventional computer architectures.
The steady increase in basic circuit speeds has long allowed computer
science to take advantage of the virtues of abstraction without the
costs of abstraction becoming obtrusive.  This trend has reinforced,
and has been reinforced by, the tendency of cognitive science to
understand a wide variety of concepts in abstract terms.  In each
case, I will argue, the result has been the steady entrenchment in
computational practice of a mentalist view of both human beings and
computation.

The example of variables demonstrates how such an entrenchment might
take place.  Recall that specific conceptions of human beings do not
inhere in machinery as such.  Instead, they adhere in design practices
whereby machines are built whose operations can be narrated in
intentional terms.  On this view, the variables of logic formalisms
and programming languages provide a way of building a machine
whose operation can be narrated as the application of a nonspecific
competence to specific circumstances.  Technical innovations might
someday supersede the use of variables, of course, but only if they
provide alternative discursive forms for narrating the operation of
an agent's machinery.  As a practical matter, any such innovations
will be available to designers only once the technical community
has routinized their use and integrated them into the whole support
network of factories, instruction manuals, technical standards,
repair facilities, programming language features, testing methods, and
so on.  The AI research community has historically invested enormous
energy in maintaining its own largely distinctive infrastructure,
including its own programming languages and computer architectures,
precisely to provide itself with the technical resources to construct
computer systems within its evolving repertoire of technical schemata.
But this infrastructure rests upon, and in recent times has been
increasingly subsumed by, the larger infrastructure of the computer
industry generally.

The connectionist movement makes the practical logic of this process
evident.  Starting in the late 1970s, computational psychologists
in the connectionist movement attempted to reinvent computation.
Rejecting the model of computation implicit in symbolic programming,
they began again from machinery whose form is modeled more closely
on the circuitry of animal and human nervous systems.  Instead of
employing the register-transfer model of computing, connectionist
models employ large networks of computationally simple "nodes"
(loosely modeled on neurons) that are connected by a mostly fixed set
of wires (loosely modeled on axons and dendrites) that are capable
of transmitting only simple codes (such as binary values or firing
rates).  In making these alternative commitments, the connectionists
lost access to the wide range of technical schemata that symbolic
programmers use to design systems whose operation can be narrated
in intentional terms.  Dreyfus and Dreyfus (1988), among others,
have hoped that connectionist research would develop an alternative
repertoire of technical schemata based on different, nonsymbolic
commitments about representation and cognition.  One starting place
is the idea of *distributed representation* (Rumelhart and McClelland
1986; van Gelder 1992), according to which the basic elements of
representation are inductively derived and semantically open-ended,
as opposed to the fixed categories of formal logic.  This idea, though
suggestive, immediately casts off most of the traditional means by
which the operation of cognitive models can be narrated.

To fill this vacuum, researchers immediately set to work fashioning
connectionist equivalents to conventional programming constructs
-- especially variable binding (Norman 1986).  Touretzky and Hinton
(1988), for example, built a connectionist production system, and
Smolensky (1987) built a variable-binding mechanism in which each
variable-constant pair was effectively represented by its own node.
Though highly cumbersome, these systems provided an existence proof
that inspired further refinements.  Ajjanagadde and Shastri (1989)
demonstrated that one could dynamically bind a handful of variables
using strobe signals that synchronized the firing of variables
and their values across long distances.  Lange and Dyer (1989)
and Sun (1992) described schemes in which relatively complex
codes, representing either variable-constant pairs or the constants
themselves, were passed along the wires.  This research explores a
space of trade-offs whose organizing principle is the tension between
the frequent changes in a variable's value, which invite a high degree
of abstraction, and the static connectivity of connectionist networks,
which invites a low degree of abstraction.  This research, in short,
is effectively reinventing the register-transfer model of computation
-- not because the register-transfer model is preferable on technical
or empirical grounds, but simply because it is the only model for
which a large repertoire of technical schemata has been developed.
The demands of narration and the demands of architecture, in other
words, are pulling connectionist research in opposite directions.

The purpose of this exercise is not to disparage connectionism but
simply to describe the tides of practical logic that threaten to sweep
it into the familiar channels of symbolic abstraction.  In preparing
the way for an interactionist alternative, Chapman (1991: 36-41) has
suggested a way of distinguishing the neurophysiological facts of

### essential connectionism*:

* * is made up of a great many components (about 10^11 neurons)* * each of which is connected to many other components (about 10^4)* * and each of which performs some relatively simple computation (whose
      nature is unclear)* * slowly (less than a kHz)* * and based mainly on the information it receives from its local
          connections.  (1991: 36)

from the empirically unsupported assumptions of many connectionist
models:

* * neurons are connected randomly or uniformly* * all neurons perform the same computation* * each connection has associated with it a numerical weight* * each neuron's output is a single numerical activity* * activity is computed as a monotonic function of the sum of the
          products of the activities of the input neurons with their
          corresponding connection weights.  (1991: 40, emphasis in the
          original)

The essential connectionist commitments are firmly grounded in
implementation.  As Chapman observes, however, they preclude the
use of pointers, and so they rule out virtually the whole tradition
of symbolic programming.  The models in later chapters will explore
the practical logic of AI model-building within the essential
connectionist commitments.  But first, let us consider the historical
development within AI of the divide between implementation and
abstraction.

Architectural and generative reasoning

In the founding documents of the cognitivist movement -- the works
from the early 1950s to the early 1960s by Chomsky, Lashley, McCarthy,
Miller, Minsky, Newell, Simon, and others -- the overwhelming
intellectual concern is the refutation of behaviorism (e.g., Chomsky
1959; Lashley 1951; Newell and Simon 1972).  The sharply focused
nature of the struggle against behaviorism lends these documents a
certain unity: they all argue for mental content as an explanatory
category in human psychology.  But as Chapter [x] has pointed out,
the cognitivist movement shared another kind of unity as well: the
background of assumptions against which the behaviorist-cognitivist
debate was constituted.  Among these background assumptions was the
mentalist metaphor system of inside and outside: both sides spoke of
stimuli and responses, or at least of input and output, debating only
whether anything "mental" could be found in between.  Another shared
assumption was a certain conception of science: since the behaviorists
had originally criticized introspectionism for its vagueness, the
cognitivists would demonstrate that their theories were precise.  In
these ways, the cognitivist movement could win the day by presenting
itself as a legitimate alternative to the stagnation of behaviorism.

Against the background of this commonality, the cognitivist movement
exhibited considerable internal diversity as well.  The leading
figures just mentioned took their inspiration in various proportions
from neurophysiology, feedback control, computer programming,
and formal language theory.  These various intellectual strands
take up different relationships to the themes of implementation
and abstraction: neurophysiology is concerned by definition with
implementation and had no systematic framework for theories of
abstraction; feedback control devices implemented a small set of
mathematical abstractions in a wide variety of ways; research on
computer programming developed abstractions that were ever more
distant from issues of physical implementation on computers; and
formal language theory was concerned almost entirely with abstraction,
investigating whether procedures related to the formal properties
of languages could be implemented without much concern for how.  All
of them had already been combined in other ways to form cybernetics,
recursion theory, and a dozen other less readily distinguishable
movements.  Having come together under the common flag of cognitivism,
they were now vigorously sorted out as each principal figure began
training students within his own synthesis.  It will be instructive
to look at some of these syntheses in relation to the tension between
implementation and abstraction.  Though all of them have great
historical significance, I will concentrate on the three that are
most immediately relevant to my project: Newell and Simon (who wrote
together during the 1960s), Chomsky, and Minsky.  Though all of these
authors have made steady progress on their respective projects over
the last thirty years, their basic premises have changed little.

Chapters [x] and [x] have already mentioned Newell and Simon's theory
of thought as search in a mathematically defined "problem space."
To test their Logic Theorist and GPS models (1963, 1972) against
the behavior of experimental subjects, they and their collaborator
Shaw wrote some of the most sophisticated computer programs of that
day.  Newell, Shaw, and Simon, though, did not regard these programs
themselves as models of human cognition, since human brains probably
do not implement serial architectures like the ones on which they
worked.  Their theoretical claims were not for their programs as such,
but simply for the abstractly defined problem-space scheme.  Their
programs are existence proofs for the possibility of implementing
their abstractions, as well as ways of mechanically generating
predictions from their theory, and they have only gradually been
working toward proposals about physical implementation (Newell 1990).

Chomsky, similarly, defined his project in linguistics in terms of
a distinction between "competence" and "performance."  Linguistic
competence is a mathematical abstraction expressing in ideal terms
the grammar of a given language.  Linguistic performance, by contrast,
concerns the actual situated employment of language by real people.
The relationship between competence and performance is different from
the software-hardware distinction in computer programming, since it
is not necessary for linguistic performance to implement linguistic
competence in precise detail.  (Actual speakers can experience slips
of the tongue, misunderstand complex sentences, suffer brain injuries,
make jokes by deliberately mangling grammar, etc.)

Newell and Simon's problem-space theory of thinking and Chomsky's
formal theory of grammatical competence are both generative
theories, meaning that they involve mathematical operations capable
of generating an infinite number of mental structures by the repeated
application of a small number of basic rules.  Chapter [x] has
introduced Newell and Simon's theory, in which one engages in a search
of a formally defined space of states, each of which provides a choice
among several operators.  In Chomsky's theory, each sentence has a
derivation, consisting of several steps, each of which permits
one to apply several different rules.  It is a characteristic of
generative theories that they envision an exponentially expanding
number of possible courses of reasoning.  Given four operators and
a single state, Newell and Simon will predict 4 possible outcomes
from the application of a single operator, 16 possible outcomes from
the application of two operators in sequence, 64 from the application
of three, 256 from four, and so forth (although some of these
multitudinous states might duplicate others).  Likewise, the iterative
application of the rules of linguistic competence can rapidly
produce an enormous variety of sentences.  Newell and Simon regarded
the generative application of operators as a psychologically real
phenomenon, whereas Chomsky was agnostic about whether people perform
grammatical derivations in their heads or whether they generate
and parse sentences by some other method whose results are simply
consistent with the grammar.  For Newell and Simon the empirical
question was whether their model applied the same operators as
experimental subjects.  For Chomsky the empirical question was whether
the iterative application of a grammar's rules produced exactly the
set of grammatical sentences, no more and no less.  Newell and Simon's
project was subject to experimental falsification in a way different
from Chomsky's.  But in each case, the possibility of generating
an infinity of possible mental structures was an emphatic point of
contrast with the relatively impoverished scope of human possibility
that seemed implicit in behaviorist theories.  Chomsky in particular
described grammars as making "infinite use of finite means" and
invoked the thought of Descartes as precedent for his rigorous
distinction between competence, qua abstract forms of thought, and
performance, qua implemented action (Chomsky 1966).

In contrast to the generative theorists, Minsky (1985) has
consistently been concerned with issues of implementation.  His
work represents the deepest and most sustained inquiry into the
practicalities and consequences of the physical implementation of
the various aspects of human intelligence.  Where the generativists
portray human reasoning as generating and exploring infinite
abstract spaces, Minsky's theories have been resolutely finite: he
has constantly reformulated his understandings of human intelligence
in accord with the constraints of physical implementation.  Though
intended as a foundation for neurophysiology, his models do not
invoke in any detail the claimed behavior of human neurons.  Instead,
he starts from the fundamental nature of physical implementation as
such: the locality of causal interactions, the nearly fixed structure
of physical artifacts, the logistical difficulties of centralized
control, and the inevitability of conflict and inconsistency in a
large system of any sort.

Minsky's theories employ an architectural style of reasoning.
Architectural reasoning attempts not merely to implement a given
abstraction but to discover abstractions that both do the required
work and admit of natural implementations.  Engineers who design
computer hardware engage in architectural reasoning all the time,
since it is their job to mediate between the abstractions that
programmers presuppose and the currently available circuit fabrication
and packaging technologies.  But, as I have explained, today's
computer designers are highly constrained by the expensive freedoms
of serial architectures.  The evolutionary processes that produced
the human brain were probably not under any comparable constraints.
Minsky views the human brain as a decentralized and massively
parallel computational system, with an enormous number of specialized
functionalities each occupying a localized region of neural circuitry.

The generative and architectural styles of research have led to
different views about the relationship between abstraction and
implementation in human cognition.  Generative theories posit large,
consistent abstractions that operate by their own formally specifiable
laws.  McCarthy and the other proponents of the reconstruction of
human knowledge in formal logic, for example, take as their starting
point the generative power of logical formalisms and the formal
consistency presupposed by their semantics (McCarthy 1958; Genesereth
and Nilsson 1987).  Some generativists have begun constructing large
abstract theories that they refer to as architectures.  Foremost
among these theorists is Newell (1990), who presents his SOAR
architecture as a "unified theory of cognition."  Yet such theories,
valuable as they are, are concerned primarily with abstraction.
They appeal to the practicalities of physical implementation only
in a general way, for example in the parallelism that ought to be
obtainable in the mechanism that selects rules to run.

Architectural theories, by contrast, hold that the demands of
physical implementation have profound consequences for the formulation
of abstract theories of cognition.  Minsky in particular emphasizes
physical locality so strongly that cognition becomes a large,
fragmentary collection of mutually inconsistent abstractions, each
bearing a different relationship to its physical implementation.
He formulates his theory not as a single unified mechanism, or
even as a single list of axioms of design, but as a constellation
of mini-theories, each examining some feature of human intelligence
-- whether language, reasoning, decision-making, memory, emotion,
imagination, or learning -- on the level of engineering intuition.
The emphasis on physical implementation and its consequences for
theories of cognition is also present in the connectionist movement.
Feldman (1985), for example, has offered architectures for the human
visual system that are compatible with both the phenomena of human
vision and the practicalities of architectural design.  Likewise,
research in cognitive neuroscience has made a principle of shaping its
abstractions in accord with the empirically discovered structures of
the brain (Churchland and Sejnowski 1992).  But whereas these projects
hypothesize mechanisms to explain detailed empirical data, Minsky uses
general principles of physical implementation to drive the formulation
of explanatory theories of cognitive architecture.

The dialectical relationship between abstraction and implementation is
evident in the patterns of dispute between generative and architectural
theorists.  Whereas the generative theorists promote the virtues of
abstract rigor and generality, the architectural theorists emphasize
physical realizability.  The literature on these disputes has focused
principally on the difficulty of reconciling the generative view of
cognition with connectionist implementation (Clark 1992; Fodor and
Pylyshyn 1988; Pinker and Prince 1988; van Gelder 1992).  The problem,
already apparent in the case of variables, is a conflict of metaphors:
whereas a connectionist network has a fixed pattern of connectivity,
general-purpose symbolic processing requires the continual
reconfiguration of the symbolic structures that implement the
agent's mental states.  It seems safe to predict that the dispute
will continue, and that the respective demands of abstraction and
implementation will continue to influence the models of both the
generative and architectural theorists.  I believe that this impasse
cannot be resolved without considerable rethinking of the generative
view of cognition.  My own project, however, is not to participate in
the debate but to explore alternatives to the hidden assumptions that
have determined its structure.

Generative reasoning and mentalism

The versions of computational research that I have surveyed differ
in their details, but all of them define their problems within
the framework of abstraction and implementation.  The dialectical
relationship between abstraction and implementation defines a
space within which various projects trace particular trajectories.
Though this history is complicated, a fundamental determinant of
its overall pattern is the metaphor system of mentalism within which
the distinction between abstraction and implementation makes sense.

Cognitivism and behaviorism, as we have seen, shared the mentalist
vocabulary of inside and outside, stimulus and response, contents and
behavior.  At issue was the question of whether scientific sense could
be made of the notion of abstract mental structures and processes:
thoughts and thinking, memories and remembering, plans and planning,
and a boundless repertoire of other nouns and verbs that shuttle
easily between the vernacular and scientific vocabularies of
psychology.  The conception of computation as implemented mathematics
provided the license that cognitivism needed.  Make it mathematical,
or make it seem likely to admit finite formalization, and it becomes
a valid psychological category.  As the project of AI accelerated,
the mind became a space for the free exercise of the theoretical
imagination.

The multiplication of mental constructs reached its point of greatest
fertility in the AI research of the 1970s: mental structures that
remain largely fixed or that continually change; mental languages
based on English, formal logic, programming languages, or some
composite of these; reasoning that proceeds through a detailed
simulation of the outside world or through the calculation of obscure
numerical functions; processing organized in a centralized or a
decentralized manner; processes that cooperate or compete; and so
forth.  The metaphor system of mentalism has lent itself to this
explosive unity in diversity for several reasons.  The first is that
everyone in Western culture, computationalists included, inherits a
substantial degree of mentalist self-understanding from the philosophy
that lies sedimented in the vernacular language.  The second is that
the computer itself arose within the discursive environment of a
cultural enthusiasm for the symbols of cognition, mentioned in Chapter
[x], that has waxed and waned from the manifestos of George Boole
to the popular images of Einstein and rocket scientists and "giant
brains" (Berkeley 1961) of the Cold War (Edwards 1996).  The third and
most important reason concerns the specific metaphors of mentalism.
The Cartesian mind is both inaccessible and transcendent: on the
one hand, it is the private domain of a unique individual who has
incorrigible access to its states; on the other hand, it is also
a perfectly generic cognitive essence found within every human
being.  This ambiguity is found as well in the phrase "the mind": in
announcing its intention to study the mind, with its singular form and
definite article, psychology does not assert that only one person in
the world has a mind, but rather that all minds are, in the relevant
sense, identical.  Laboratory scientists studied the mind with great
difficulty, but the practitioners of AI generated numerous personal
intuitions about their own minds and made them real, on a small scale,
in computational demonstrations (Turkle 1984: 265-267).

Abstraction, then, took on a special meaning within cognitivist
psychology.  The conceptual independence of mental abstractions from
their physical implementations was the modern computational version
of the soul's distinction from the body.  Computationalists emphasize
that an abstractly specified computation can be implemented on
any device capable of supporting the digital abstraction and the
register-transfer model, be it a supercomputer or a gadget made
of thread spools and rubber bands; and they identify a computation
with its abstraction, not its implementation.  In this way, AI has
reproduced in technological form the theological and philosophical
individualism that became radicalized in Descartes's method of
systematic doubt.  The object of inquiry was not the individual in
society or the person in the world, but the self-sufficient inner
realm of the mind.  The conceptual autonomy and infinite generative
power of mental computations has played the same role in the
computational theory of mind that the transcendence of the soul played
for so long in philosophy.

One might hope for an alternative conception of computation, one that
is better suited to an understanding of human beings as creatures
bound up in their environments.  An alternative to the mentalist
opposition of abstraction and implementation can perhaps be found in
the interactionist concepts of intentionality and embodiment.  Later
chapters will discuss these terms in detail, but I will offer minimal
definitions here to indicate what is at stake.  Intentionality relates
to the general phenomenon of an agent's taking up a relation to
something in the world: picking it up, drawing it, telling a story
about it, avoiding it, or trying to figure out where it is.  A theory
of intentionality must explain, for example, how to distinguish
intentional acts from ordinary causal events such as rocks rolling
down hills.  Intentionality includes representation as a special
case, but intentional relationships are not necessarily mediated
by representations.  From a computational point of view, embodiment
has four crucial (and conceptually interdependent) aspects: physical
realization, causal interaction with the world, the possession of
sensory and motor apparatus, and the necessity of making choices about
action (one cannot, for example, travel both north and south, or both
raise and lower one's hand).  More obvious but less fundamental issues
include the contingent attributes of various specific kinds of bodies:
motility, facing in a particular direction, anatomical organization,
and so forth.  Though abstraction and intentionality play analogous
theoretical roles, they differ in that abstract computations are
specifically removable from any concrete circumstances whereas
intentionality is defined in relation to an agent's activities in
the world.  Likewise, implementation and embodiment both refer to
the physical realizations of a computation, but they correspond to
different understandings of what is being realized: an abstract
process or a concrete form of activity.

The principal significance of this proposed shift from a mentalist to
an interactionist conception of computation is that intentionality and
embodiment do not imply the Cartesian mind-body opposition that lies
latent in the relationship between abstraction and implementation.
This is not to say that hard problems become easy, only that the
project of resolving them ought to suffer from different contradictions.
The next chapter plows some necessary ground: it reviews the ideas and
techniques that underlie contemporary computational practices, with a
view toward their systematic renovation within an interactionist framework.

end
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20000816232124/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20000816232124/mailto:webmaster@somewhere.com). |