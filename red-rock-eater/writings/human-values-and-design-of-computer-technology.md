---
id: human-values-and-design-of-computer-technology
title: Human Values and Design of Computer Technology
type: writing
writing_type: rre-post
url: http://commons.somewhere.com/rre/1997/Human.Values.and.Design..html
coauthors: []
key_concepts: []
importance: 6
research_status: partial
tags:
  - HCI
  - activism
  - democracy
  - education
  - internet-culture
  - media
  - social-computing
---




## Source

Automatically imported from: http://commons.somewhere.com/rre/1997/Human.Values.and.Design..html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](http://www.somewhere.com/)

  

# Human Values and Design of Computer Technology

```



          Human Values and Design of Computer Technology

   edited by Batya Friedman

published by CSLI Publications and 
             Cambridge University Press

             January 1998

   hardcover $64.95 ISBN 1-575-86081-3
   paperback $24.95 ISBN 1-575-86080-5


Contents

        Introduction
        Batya Friedman

PART I
Conceptualizing Human Values in Design

1       Bias in Computer Systems
        Batya Friedman and Helen Nissenbaum

2       Accountability in a Computerized Society
        Helen Nissenbaum

3       Disability, Inability and Cyberspace
        John Perry, Elizabeth Macken, Neil Scott, and Janice L. McKinley

4       Do Categories Have Politics? The Language/Action Perspective
        Reconsidered
        Lucy Suchman

5       Categories, Disciplines, and Social Coordination
        Terry Winograd

6       Commentary on Suchman Article and Winograd Response
        Thomas W. Malone

7       Social Impact Statements: Engaging Public Participation in
        Information Technology Design
        Ben Shneiderman and Anne Rose

PART II 135
Computers as Persons? -- Implications for Design

8       Computers Are Social Actors: A Review of Current Research
        Clifford I. Nass, Youngme Moon,  John Morkes, Eun-Young Kim,
        and B.J. Fogg

9       When the Interface Is a Face
        Lee Sproull, Mani Subramani, Sara Kiesler, Janet Walker, and
        Keith Waters

10      'Social' Human-Computer Interaction
        Sara Kiesler and Lee Sproull

11      Reasoning About Computers As Moral Agents: A Research Note
        Batya Friedman and Lynette I. Millett

12      Interface Agents: Metaphors with Character
        Brenda Laurel

13      Human Agency and Responsible Computing: Implications for
        Computer System Design
        Batya Friedman and Peter H. Kahn, Jr.

PART III
Practicing Value-Sensitive Design

14      Workplace Database Systems: Difficulties of Data Collection
        and Presentation
        Harry Hochheiser

15      Eliminating a Hardware Switch: Weighing Economics and Values
        in a Design Decision
        John C. Tang

16      Steps toward Universal Access Within a Communications Company
        John C. Thomas

17      Social Choice About Privacy: Intelligent Vehicle-Highway
        Systems in the United States
        Philip E. Agre and Christine A. Mailloux


Introduction
Batya Friedman

Many of us when we design and implement computer technologies focus
on making a machine work -- reliably, efficiently, and correctly.
Rarely do we focus on human values.  Perhaps we believe in value-
neutral technology.  Perhaps we believe that issues of value belong
only to social scientists, philosophers, or policy makers.  Neither
belief is correct.  In their work, system designers necessarily
impart social and moral values.  Yet how?  What values?  Whose values?
For if human values -- such as freedom of speech, rights to property,
accountability, privacy, and autonomy -- are controversial, then
on what basis do some values override others in the design of, say,
hardware, algorithms, and databases?  Moreover, how can designers
working within a corporate structure and with a mandate to generate
revenue bring value-sensitive design into the workplace?

This volume brings together leading researchers and system designers
who take up these questions, and more.  In this introduction, I
situate these questions within a larger conceptual framework.  I also
motivate the need to embrace value-sensitive design as part of the
culture of computer science.  Then I offer an overview of each of
the chapters.  Roughly half of the chapters are new material, and the
remainder are reprints of pivotal articles from recent years.  For
readers with specialized interests, Table 1 arranges the chapters by
technical topic; Table 2 by core human value.

Does Technology Have Values?

Does technology have values?  Consider a few examples.  In the
early 1900s, missionaries introduced a technological innovation --
steel ax heads -- to the Yir Yoront of Australia, a native people.
The missionaries did so without regard for traditional restrictions
on ownership, and indiscriminately distributed the ax heads to
men, women, old people, and young adults alike.  In so doing, they
altered relationships of dependence among family members and reshaped
conceptions of property within the culture (Sharp, 1952/1980).
Another example: About four decades ago, snowmobiles were introduced
into the Inuit communities of the Arctic, and have now largely
replaced travel by dog sleds.  This technological innovation thereby
altered not only patterns of transportation, but symbols of social
status, and moved the Inuit toward a dependence on a money economy
(Houston, 1995; Pelto, 1973).  Or a computer example.  Electronic
mail rarely displays the sender's status.  Is the sender a curious
lay person, system analyst, full professor, journalist, assistant
professor, entry level programmer, senior scientist, high school
student?  Who knows until the e-mail is read, and maybe not even
then.  This design feature (and associated conventions) has thereby
played a significant role in allowing electronic communication to
cross traditional hierarchical boundaries and to contribute to the
restructuring of organizations (Sproull & Kiesler, 1991).  The point
is this: In various ways, technological innovations do not stand
apart from human values.  But, still, what would it mean to say that
technology has values?

Endogenous and exogenous views have emerged in recent years. 
The endogenous view holds that through the process of designing
and implementing technology, the very meaning and intentions that
we designers and builders bring to our task literally become a part
of the technology (cf. Appadurai, 1988; Cole, 1991).  But this view
seems false in the sense that it imputes mental states to things which
do not have the capacity to have them.  Is the claim, for example,
that a gun itself intends to kill someone?  That proposition seems
incorrect.  Although arguable, it similarly seems incorrect to impute
mental states to computational systems.  In chapter 13, Friedman and
Kahn discuss this position in more detail.  In contrast, the exogenous
view holds that values reside with the users, not the technology.
Proponents of this view are likely to say "guns don't kill people,
people do"; or similarly, "hammers don't pound nails, people do" or
"computer databases don't track workers, people do." But this view
ignores our everyday experience that particular tools lend themselves
to particular tasks in particular ways; otherwise, one tool would
serve all purposes well and we know this is not the case.  Try
pounding a nail with a computer database.

A third view -- which I think is correct -- holds that the way people
design tools makes the tools more suitable for some uses over others.
Scheffler (1991) suggests, for example, that a hammer is well suited
for driving nails, poorly suited as a soup ladle, and perhaps amenable
as a doorstop, bookend, or paper weight.  In other words, human
activity is constrained and perhaps even prodded by features of the
technology, but not determined by it.

In terms of computer system design, we are not so privileged as to
determine rigidly the values that will emerge from the systems we
design.  But neither can we abdicate responsibility.  For example,
let us for the moment agree with Perry et al. in chapter 3 that
disabled people in the workplace should be able to access technology,
just as they should be able to access a public building.  As system
designers we can make the choice to try to construct a technological
infrastructure which disabled people can access.  If we do not make
this choice, then we single-handedly undermine the principle of
universal access.  But if we do make this choice, and are successful,
disabled people would still rely, for example, on employers to hire
them.  Suitability (as a feature of the technology) is necessary for,
but does not assure equal access (a human value).

Users, of course, are not always powerless when faced with unwelcomed
value-oriented features of a technology.  For example, students in
one of my classes conducted an informal ethnographic investigation
of computer use in a local accounting firm.  The previous year, this
firm had acquired an off-the-shelf packaged software program for
preparing tax returns that automatically reported the number of tax
returns completed by each employee.  But such overt comparisons among
employees resulted in office discord.  Employees did not believe that
the numbers fairly portrayed their overall value to the firm, let
alone the real income they generated.  Note that this problem arose
unsolicited because of the built-in features of the software.  This
firm operated within a cooperative family-style work culture.  Thus,
in this situation, the firm members agreed to destroy the comparative
data when it was produced.  However, it takes courage to turn away
from quantitative data that tell us how things are going even if we
rationally believe the numbers are misleading and incomplete.

Human Values: A Working Definition

In some sense, we can say that any human activity reflects human
values.  I drink tea instead of soda.  I recently attended a Cezanne
exhibit instead of a ball game.  I have personal values.  We all do.
But these are not the type of human values which this volume takes
up.  Rather, this volume is principally concerned with values that
deal with human welfare and justice.

This demarcation between personal and moral values follows from
the psychological literature which has investigated empirically
what have been referred to as three domains of social knowledge: the
moral, conventional, and personal (Nucci, 1996; Smetana, 1983; Turiel,
1983).  The moral domain refers to prescriptive judgments which people
justify based on considerations of justice, fairness, rights, or
human welfare.  Conventional issues refer to behavioral uniformities
designed to promote the smooth functioning of social interactions.
Personal issues refer to those which lie under the jurisdiction of the
self.  Over eighty-five empirical studies, in western and nonwestern
countries, have demonstrated that young children, adolescents, and
adults differentiate these three forms of knowledge (for reviews
of the literature, see Smetana, 1995; Tisak, 1995; Turiel, 1983,
in press; Turiel, Killen, & Helwig, 1987).  In addition, many of
these studies have analyzed how social issues can often embody all
three aspects (Smetana, 1982; Turiel, Hildebrandt, & Wainryb, 1991).
Abortion, for example, is a particularly controversial social issue
not only because it involves a controversial assumption about when
life begins, but because personal values (that a woman has personal
jurisdiction over her own body) can conflict with moral values (that
involve the potential welfare and rights of a fetus).  It is also
the case that personal and conventional issues can become moral,
in specific contexts.  For example, most people in western countries
believe that if a man chooses to wear a bathrobe, that is his personal
choice.  But in certain contexts there are also conventions about
appropriate dress.  Thus, if a man wears his bathrobe to a dignitary's
funeral, many people would judge the act not only as a conventional
violation, but a moral violation -- as a sign of disrespect.

This form of analysis can bring clarity into understanding the social
aspects of computing.  For example, a particular feature of a computer
system (the positioning of the track ball on a laptop computer)
may make a system easier to use.  But unless the difficulty of use
systematically prevents certain groups of individuals from using the
technology, ease of use per se is not a moral value, but a personal
one.  Or consider a voting booth for use in national elections.  A
person may prefer to cast his or her vote by marking an old-fashioned
"X" next to a candidate's name instead of using an electronic voting
system that requires punching out a dot on a voting card.  But if the
person can easily vote with the latter system, then preferring one
system over the other reflects a personal value.  On the other hand,
if the system requires a short voter to pull a lever that is above his
or her reach, as has actually happened (Roth, 1994), then the system
prevents fair participation in the voting process.  Accordingly, the
human values at stake become moral, not simply personal.

When designing computer systems, conflicts also often arise between
conventional and moral considerations.  Think of standardization. 
On the one hand, standardization relies on conventional uniformities
to enhance the smooth functioning among different components of a
system or among different users of a system.  Imagine if communication
protocols on the internet were not standardized.  In this light,
standardization is vital.  On the other hand, standardization requires
individuals to give up some degree of control over the technology.
Think of the frustrations some workers encounter when companies
require every worker to use the identical word processor.  Indeed,
the debate in this volume between Suchman (chapter 4) and Winograd
(chapter 5) can be understood in these terms.  Suchman objects to
standardized communication on the grounds that individuals are coerced
by the system.  Winograd counters that through the social conventional
coordination of communication, more successful and beneficial
communication is supported (and individual welfare increases).

The human values addressed in this volume principally refer to moral
values.  But I prefer to use the broader term "human values" instead
of simply moral values to highlight the complexity of social life, and
to provide the basis for analyses wherein personal and conventional
values can become morally implicated.

Distinguishing Value-Sensitive Design from Usability

Some system designers have a tendency to conflate value-sensitive
design with usability.  This problem arises with good reason.  
Namely, usability is itself a human value, although not always a
moral one.  But when it is, both can be addressed by the same design.
For example, systems which can be modified by users to meet the needs
of specific individuals or organizations enhance their usability
(cf. Adler & Winograd, 1992).  At the same time, such systems can help
users to realize their goals and intentions through their use of the
technology -- a human value which Nissenbaum and I (Friedman, 1996)
refer to as autonomy.

Sometimes, however, usability conflicts with value-sensitive design.
Nielsen (1993), for example, asks us to imagine a computer system
that checks for fraudulent applications of people who are applying
for unemployment benefits by asking applicants numerous personal
questions, and then checking for inconsistencies in their responses.
Nielsen's point is that some people may not find the system socially
acceptable (based on the value of privacy) even if the system receives
high usability scores -- that is, it is easy to learn, easy to use,
error free, efficient, and so on.  Indeed, in this volume, Tang
(chapter 15) provides a case study of just such a conflict.  Tang
describes the issues which a design team faced in deciding how to
power a microphone.  The solution they settled upon was to power a
microphone directly from the workstation.  They thereby eliminated a
separate hardware on/off switch on the microphone.  From a usability
perspective, Tang points to benefits from this design decision
insofar as a separate battery could wear down, and thereby cause an
inconvenience to the user.  Moreover, to preserve the battery users
would no longer need to remember to turn the microphone off when it
was not in use.  However, despite these usability advantages, Tang
also shows that the design undermined the moral values which some
users placed on privacy and security.

In short, our language and conceptualizations within the field
currently provide solid means by which to pursue issues of usability
(cf. Adler & Winograd, 1992; Norman, 1988; Norman & Draper, 1986;
Nielsen, 1993).  This work is important.  At a minimum, usability
represents social organizational values needed to make systems work
in a functional sense.  At times, usability can also support human
values of moral import.  But at times we need to give ground on
usability to promote human values, and, conversely, at times we
need to give ground on human values to promote usability.  Such
optimizations require judicious decisions, carefully weighing and
coordinating the advantages of each.

About This Book

 From a variety of perspectives, there has been increasing interest
in the social implications of computer technology.  Methods from
anthropology, sociology and psychology, for example, have been used
in understanding computing and human values from individual and
organizational perspectives (Kling, 1980; 1996; Nass & Reeves, 1996;
Sproull & Kiesler, 1991; Suchman, 1987; Zuboff, 1988).  The literature
on computer ethics has revealed the philosophical dimensions of
computing (Ermann, Williams, & Gutierrez, 1990; Forester, 1989;
Johnson, 1994; Johnson & Nissenbaum, 1995; Ladd, 1989; Moor, 1985).
The computer-supported cooperative work (CSCW) and participatory
design (PD) communities have enhanced collaboration and the democratic
participation of individuals within organizations (Blomberg, Suchman,
& Trigg, 1996; Bodker, 1991; Clement & Van den Besselaar, 1994; Ehn,
1988; Greenbaum & Kyng, 1991; Greif, 1988; Kuhn, 1996; Schular &
Namioka, 1993).  More broadly, the human-computer interaction (HCI)
community has been increasingly aware of and concerned about the
social dimensions of design (Baecker, Grudin, Buxton, & Greenberg,
1995; Brown & Duguid, 1994; Fernandes, 1995; Laurel, 1990;
Shneiderman, 1992; Tognazzini, 1995; Winograd, 1996; Winograd &
Flores, 1986).  All of these perspectives have offered important if
not crucial lines of inquiry.  This volume adds to this growing body
of literature by offering a principled and practical framework for
promoting human values in system design, particularly values with
moral import.

Part I: Conceptualizing Human Values in Design

The papers in this first section examine computer technology in
relation to the values of accountability, autonomy, freedom from bias,
privacy, and universal access.  Some of these papers illustrate how
value-oriented problems can be closely tied to technical decisions.
For example, Friedman and Nissenbaum (chapter 1) include an analysis
of Corbats's multi-level scheduling algorithm which has been
implemented in a variety of timesharing systems.  They suggest that
when systems are placed under heavy use, the algorithm may unfairly
discriminate against users with long-running computations.  Other
value-oriented problems are more deeply embedded within a social
context.  For example, Nissenbaum (chapter 2) analyzes systems which
are constructed out of modules or modified from previously existing
code in order that no single individual understands the entire system.
In such situations, it can be difficult to identify the locus of
responsibility for computer-mediated action.  Similarly, Perry et
al. (chapter 3) show that in order to solve the problem of access for
the disabled, designers may need to find the best (or a reasonable)
balance between the responsibilities of the individual user and the
responsibilities of the computer industry, if not the larger society.

Over forty years ago, Norbert Wiener said that in the coming years
access to information would be relatively easy, and that the hard
problem for computer science would be to provide access to useful
information.  Today, Wiener would find little disagreement.  Just note
some of the millions of users as they try (often unsuccessfully) to
meaningfully access the billions of accessible words on the World Wide
Web.  Many of the emerging solutions to this problem currently depend
on filters of some sort.  Filters, in turn, depend on the activity of
categorization: being able to identify items which are similar along
one or more dimensions, and different along others.  It is here that
the three chapters on categorization by Suchman, Winograd, and Malone
are of great importance.

Suchman (chapter 4) begins by offering strong words of caution: that
whoever determines the categories -- and how those categories can
be used -- imputes their own personal values into the system and has
power over the user.  As noted above, Winograd (chapter 5) responds
to Suchman by pointing to the frequent need for socially coordinated
activity in which groups of people seek to share information and
technology.  In such activity, Winograd argues that we need some
degree of standardization wherein designers impose categories.
That is their job.  The key, according to Winograd, is to cultivate
regularized activity without becoming oppressive: or, in a sense,
to use power wisely.  In turn, Malone (chapter 6) responds to Suchman
by arguing that not only are categories often useful, but to some
extent they are necessary given the structure of human cognition.
At the same time, Malone suggests that no category system is complete,
and therefore designs need to be adaptable, often by their users.

Consider this debate in terms of this present introduction.  Recall
that Table 1 categorizes the chapters by technical topic, and Table
2 categorizes the chapters by human value.  Suchman would have us
recognize that as the editor of this volume, I have imposed my own
categories onto these chapters.  For example, I categorized the
chapters by Suchman, Winograd, and Malone as involving the human
value of autonomy.  But at least three other decisions were possible.
First, I could have chosen one or more other categories: following
Suchman, perhaps that of politics or power.  Such a choice would
lead in different, and interesting, directions.  Second, I could
have provided no categorization.  But following Winograd and Malone,
categories can serve as an effective way to quickly orient readers
to the subset of chapters (aka the subset of information) that might
be of greatest interest to them.  Third, I could have asked the
contributors to categorize their own chapters, either according
to a predetermined set of categories or to a category of their
choosing.  While such delegation was certainly possible, it would have
transformed my role from one of editor, seeking to shape and provide
coherence to this volume, to one of coordinator seeking to reflect the
perspectives of the contributors.  Since multi-authored volumes often
suffer from a lack of coherence, I decided that delegating control was
on balance a poor choice.  My point is that the tensions encountered
in using and selecting categories to characterize the chapters in this
volume illustrate the same issues we face with the use of categories
in system design: that appropriate, if not good, resolutions depend on
finding in context the right balance between competing values.

Shneiderman and Rose (chapter 7) move this discussion on value-
sensitive design to the level of codification.  Based on the idea
of an environmental impact statement, they propose that designers be
encouraged, if not required, to provide a "social impact statement"
which assesses the social impact of their designs on direct and
indirect users.  A key toward developing one's social impact statement
would be the early identification and involvement of stakeholders
in the design.  Shneiderman and Rose discuss this proposal in the
context of their current design for the Maryland Department of
Juvenile Justice.  Agre and Mailloux (chapter 17) also recommend such
stakeholder involvement in their discussion of intelligent vehicle
highways.

Part II: Computers as Persons? -- Implications for Design

Whether a designer chooses to present the technology to the user as
an "agent," "person," "persona," or some other anthropomorphized form,
might not appear to be a heavily laden value question.  After all, we
rarely think of the anthropomorphism of automobiles, sailing vessels,
or stuffed animals as cause for alarm.  The concern with computer
technology arises, however, from the way in which people engage with
computer technology as if it were a person to a greater extent than
previously realized.  Thus, as system designers, we need to understand
how anthropomorphism occurs, and then decide whether or not to design
features which promote it.  This is the distinction I was making
earlier between suitability (design features) and values (promoting
computers as persons).  Possibly for the first time in one place, this
part brings together the growing body of work on this topic.

Typically, we think of social interaction as involving two or more
people, even if people are physically distant from one another,
as when talking on the telephone, reading electronic mail, or even
having an internal dialogue with a friend.  But can an interaction
be social, or at least fully social, with computer technology?  Nass
et al. (chapter 8) lean toward an affirmative response.  They begin
by documenting that with minimal social cues (e.g., text-only), people
will exhibit behavior with computers that in comparable situations
parallels their behavior with other human beings (e.g., following
politeness norms).  Accordingly, they suggest that there may be
a place to design, for example, "likable" computers which flatter
their users and that adhere to human conventions of politeness.
More boldly, following the title of their chapter, "Computers are
Social Agents", they suggest that in system design interpersonal
communication should become the metaphor and mechanism for
human-computer interaction.

Sproull and Kiesler and their colleagues (chapter 9) provide evidence
which support Nass et al.'s initial claim.  In their study, subjects
changed their personas and behavior in the presence of a simulated
face (e.g., they presented themselves more positively to the simulated
face than to a text interface) and attributed some personality traits
to the simulated face.  Other results reported by Kiesler and Sproull
(chapter 10, which expands on their work in chapter 9) show that
people will trust and behave cooperatively with a computer partner.
Yet, in contrast to Nass and his colleagues, Kiesler and Sproull offer
a more cautious interpretation of the data.  It is one thing to say,
as they do, that when the interface takes on a human persona through
characteristics people typically associate with people -- such as
human speech and physiognomy -- then it is likely to elicit what looks
like social behavior in users.  It is another thing to say, which they
do not, that people think of machines as people.

Part of the difficulty in interpreting the above studies arises
by trying to use data on human social behavior in interaction with
computers to infer human cognition.  Thus Friedman and Millett
(chapter 11) offer a different methodology: social-cognitive
interviews.  Based on this method, they assessed individuals'
reasoning about computer agency and computer capabilities, and their
judgments of moral responsibility in two situations that involved
delegation of decision making to a complex computer system.  Results
showed a complex pattern of results.  On the one hand, most of
the individuals attributed either decision making or intentions to
computers, and over one-fifth of the individuals explicitly held
computers morally responsible for error.  On the other hand, most
of the individuals judged computer decision making and computer
intentions to be different from that of humans.  Reasoning focused on
rule-based systems (e.g., "[the computer] can decide in a sense that
somebody has programmed rules, which it follows, and in that sense it
chooses a course") and algorithmic processes (e.g., "[the computer] is
deciding based on a very clear strict algorithm... it's a decision but
not an open-ended one").  Based on these and other data, this study
does not support the stronger claims by Nass et al. that people treat
computers as social actors.  It does suggest that in certain respects
people attribute agency to computer technology, and that such
attributions go well beyond superficial use of language.

Laurel (chapter 12) would probably be neither surprised nor
bothered by a user's attribution of agency to a computer.  In her
chapter, written in 1990 before all of the other writings in this
section, Laurel distinguishes between full-bodied and unidimensional
characters.  By characters she means something like portrayals of
people, as in characters in a play.  Full-bodied characters, like
real people, are complex and at times engage in unpredictable behavior.
Accordingly, Laurel suggests that as a metaphor for interface design
full-bodied characters lead to ineffective designs.  She proposes that
the appropriate metaphor should be that of an unidimensional character
(or caricature): simple and predictable.  Laurel suggests that such
an interface would facilitate usability by minimizing ambiguity.
It would also build on a user's inclination to attribute agency to a
computer.

Alternatively, Friedman and Kahn (chapter 13) are reluctant to
build on such user inclinations.  Their reasoning follows from
the philosophical position that computers, as they are known today
in material and structure, are not persons capable of moral agency. 
They also show how serious problems arise when human beings believe
to the contrary and hold computers responsible for computer-mediated
action.  Similar arguments are made by Nissenbaum (chapter 2) in
the broader context of her discussion on maintaining accountability
in a computerized society.  If this line of reasoning is correct,
then it follows that the use of social cues in computer systems to
elicit social behavior constitutes a form of deception.  Of course,
deceptions may not always be wrong.  A social psychologist, for
example, may initially deceive his or her subjects on the nature of
an experiment in order to collect certain types of social-scientific
data.  Thus, even if one argued that encouraging a social interaction
with a computer counts as a form of deception, a decision would still
need to be made on whether such deception is warranted.  Yet, in most
cases, Friedman and her colleagues argue it is not.  This does not
mean that all agent technology need be abandoned.  Rather, Friedman
and her colleagues argue for system design that clarifies and makes
salient to the user that the computer is an "it" and not a "who" --
a machine and not a person -- and that only people can be responsible
for computer-mediated action.

Part III: Practicing Value-Sensitive Design

Until now, a designer working within a corporate structure might say
something like "nice theory, but so what?" How is it really possible
to bring value-sensitive design into the workplace?  The four chapters
within Part III take up this question.  The chapters report on diverse
work environments, including hardware development in a medium-sized
hardware company (SunSoft), research and development efforts in a
communications corporation (NYNEX), in-house software development
in a large urban hospital (the name is being kept anonymous), and
policy analysis of intelligent vehicle highway systems at an academic
institution (University of California, San Diego).

As a collection, these chapters call attention to three common
questions that arise when designers explicitly address human values.
First, how can one design proactively so as to minimize harm and
injustice to human lives?  Hochheiser (chapter 14) discusses his
efforts to do so in the design of a database to aid instrument repair
technicians in a large urban hospital.  Part of Hochheiser's challenge
was to anticipate abuses which had not yet occurred and to convince
potential users and management that preventing such abuses are worthy
of design time and resources.  Second, is there an economic benefit
to attending to human values in design?  Tang (chapter 15) says
that in most cases the answer is yes; and that it is the designer's
responsibility to examine these benefits, and to speak the economic
language of the corporate world.  Toward estimating the economic
benefits of value-sensitive design, Tang suggests that one can
estimate lost revenue from potential buyers who would otherwise
not purchase the product.  In Tang's case, buyers with concerns
for security, such as the federal government, might not purchase
a workstation that lacked a hardware on/off switch on a microphone.
Third, when in the design process is the right time to address human
values?  In what way?  In all four chapters, the authors agree that
the time to get involved is as early in the design process as possible
and to continue that involvement throughout the project.  Moreover,
both Hochheiser (chapter 14) and Tang (chapter 15) show how important
it is to address human values in the context of one's own design
projects; Thomas (chapter 16) shows how to influence organizational
practice and culture; and both Thomas (chapter 16) and Agre
and Mailloux (chapter 17) show how to influence professional
organizations, standards, and policy.

Conclusion

I have sought to convey some of the challenges and controversies
which are arising in this emerging field of human values and system
design.  I have also suggested that as a community we need to embrace
value-sensitive design as part of the culture of computer science.
To do so moves us in important directions.  It moves us toward
the conceptualizations needed to identify shortcomings in current
designs and to seek remedies which promote human well-being.  It moves
us toward the language needed to discuss the often immense social
consequences of our work with the public at large.  And it moves us
toward holding out value-sensitive design as a criterion -- along with
the traditional criteria of reliability, efficiency, and correctness
-- by which systems may be judged poor and designers negligent.  As
with the traditional criteria, we need not require perfection, but
commitment, which contributors to this volume demonstrate, with verve.

References

Adler, P.S., and T. Winograd, eds. 1992. Usability: Turning
Technologies into Tools. Oxford: Oxford University Press.

Appadurai, A., ed. 1988. The Social Life of Things. New York:
Cambridge University Press.

Baecker, R., J. Grudin, W. Buxton, and S. Greenberg,
eds. 1995. Readings in Human-Computer Interaction: Toward the Year
2000 (2nd edition). San Francisco: Morgan Kaufmann.

Blomberg, J., L. Suchman, and R.H. Trigg. 1996. Reflections on a
Work-Oriented Design Project. Human-Computer Interaction,
11(3):237-265.

Bodker, S. 1991. Through the Interface: A Human Activity Approach to
User Interface Design. Hillsdale, NJ: Lawrence Erlbaum.

Brown, J.S., and J. Duguid. 1994. Borderline Issues: Social and
Material Aspects of Design. Human-Computer Interaction, 9(1):3-36.

Clement, A., and P. Van den Besselaar. 1993. A Retrospective Look at
PD Projects. Communications of the ACM, 36(4):29-37.

Cole, M. 1991 (April). Discussant to B. Friedman and P. H. Kahn,
Jr. (Presenters). Who is Responsible for What? and Can What be
Responsible? The Psychological Boundaries of Moral
Responsibility. Paper session at the biennial meeting of the Society
for Research in Child Development, Seattle.

Ehn, P. 1988. Work-Oriented Design of Computer Artifacts. Stockholm:
Arbetslivscentrum. (Distributed by Lawrence Erlbaum, Hillsdale, NJ).

Ermann, M.D., M.B. Williams, and C. Gutierrez, eds. 1990. Computers,
Ethics, and Society. Oxford: Oxford University Press.

Forester, T., ed. 1989. Computers in the Human Context. Cambridge, MA:
The MIT Press.

Fernandes, T. 1995. Global Interface Design. Boston: AP Professional.

Friedman, B. 1996. Value-Sensitive Design. Interactions, III(6):17-23.

Greenbaum, J., and M. Kyng. 1991. Design at Work. Hillsdale, NJ:
Lawrence Erlbaum.

Greif, I., ed. 1988. Computer-Supported Cooperative Work: A Book of
Readings. San Mateo, CA: Morgan Kaufmann.

Houston, J. 1995. Confessions of an Igloo Dweller. New York: Houghton
Mifflin.

Johnson, D.G. 1994. Computer Ethics (2nd edition). Englewood Cliffs,
NJ: Prentice Hall.

Johnson, D.G., and H. Nissenbaum, eds. 1995. Computers, Ethics and
Social Values. Englewood Cliffs, NJ: Prentice Hall.

Kling, R. 1980. Social Analyses of Computing: Theoretical Perspectives
in Recent Empirical Research. Computing Surveys, 12(1):61-110.

Kling, R., ed. 1996. Computerization and Controversy: Value Conflicts
and Social Choices (2nd edition). Boston: Academic Press.

Kuhn, S. 1996. Design for People at Work. In Bringing Design to
Software, ed. T. Winograd, 273-289. Reading, MA: Addison-Wesley.

Ladd, J. 1989. Computers and Moral Responsibility: A Framework for
Ethical Analysis. In The Information Web: Ethical and Social
Implications of Computer Networking, ed. C. Gould, 207-227. Boulder,
CO: Westview Press.

Laurel, B., ed. 1990. The Art of Human-Computer Interaction. Reading,
MA: Addison-Wesley.

Moor, J.H. 1985. What is Computer Ethics? Metaphilosophy(16):266-275.

Nass, C., and B. Reeves. 1996. The Media Equation: How People Treat
Computers, Television and New Media Like Real People and
Places. Stanford, CA: CSLI Publications.

Nielsen, J. 1993. Usability Engineering. Boston: AP Professional.

Norman, D.A. 1988. The Psychology of Everyday Things. New York: Basic
Books.

Norman, D.A., and S. W. Draper, eds. 1986. User Centered System
Design. Hillsdale, NJ: Lawrence Erlbaum.

Nucci, L. 1996. Morality and the Personal Sphere of Actions. InValues
and Knowledge, eds. E.S. Reed, E. Turiel, and T. Brown, 41-60. Mahwah,
NJ: Lawrence Erlbaum.

Pelto, P.J. 1973. The Snowmobile Revolution: Technology and Social
Change in the Arctic. Menlo Park, CA: Cummings Publishing Company.

Roth, S.K. 1994. The Unconsidered Ballot: How Design Affects Voting
Behavior. Visible Language(28):48-67.

Scheffler, I. 1991. In Praise of the Cognitive Emotions. New York:
Routledge.

Schuler, D., and A. Namioka, eds. 1993. Participatory Design:
Principles and Practices. Hillsdale, NJ: Lawrence Erlbaum.

Sharp, L. 1980. Steel Axes for Stone-Age Australians. In Conformity
and Conflict, eds. J. P. Spradley and D. W. McCurdy, 345-359. Boston:
Little, Brown, & Company. (Reprinted from Human Organization, 1952(11)
17-22.)

Shneiderman, B. 1992. Designing the User Interface: Strategies for
Effective Human-Computer Interaction (2nd edition). Reading, MA:
Addison-Wesley.

Smetana, J.G. 1982. Concepts of Self and Morality: Women's Reasoning
about Abortion. New York: Praeger.

Smetana, J.G. 1983. Social-Cognitive Development: Domain Distinctions
and Coordinations. Developmental Review(3):131-147.

Smetana, J.G. 1995. Morality in Context: Abstractions, Ambiguities and
Applications. In Annals of Child Development (Vol. 10), ed. R. Vasta,
83-130. London: Jessica Kingsley.

Sproull, L., and S. Kiesler. 1991. Connections: New Ways of Working in
the Networked Organization. Cambridge, MA: The MIT Press.

Suchman, L. 1987. Plans and Situated Actions. Cambridge, UK: Cambridge
University Press.

Tisak, M.S. 1995. Domains of Social Reasoning and Beyond. In Annals of
Child Development (Vol. 11), ed. R. Vasta, 95-130. London: Jessica
Kingsley.

Tognazzini, B. 1995. Tog on Software Design. Reading, MA:
Addison-Wesley.

Turiel, E. 1983. The Development of Social Knowledge. Cambridge, UK:
Cambridge University Press.

Turiel, E. In press. The Development of Morality. To appear in
Handbook of Child Psychology, 5th Ed., Vol. 3, ed. W. Damon :
ed. N. Eisenberg, Social, Emotional, and Personality Development. New
York: Wiley.

Turiel, E., M. Killen, and C.C. Helwig. 1987. Morality: Its Structure,
Functions and Vagaries. In The Emergence of Morality in Young
Children, eds. J. Kagan and S. Lamb, 155-244. Chicago: University of
Chicago Press.

Turiel, E., C. Hildebrandt, and C. Wainryb. 1991. Judging Social
Issues: Difficulties, Inconsistencies, and Consistencies. Monographs
of the Society for Research in Child Development 56(2, Serial
No. 224).

Winograd, T., ed. 1996. Bringing Design to Software. Reading, MA:
Addison-Wesley.

Winograd, T., and F. Flores. 1987. Understanding Computers and
Cognition: A New Foundation for Design. Reading, MA: Addison-
Wesley. (First issued by Ablex, 1986.)

Zuboff, S. 1988. In the Age of the Smart Machine. New York: Basic
Books.

end

```

  

This web service brought to you by
[Somewhere.Com, LLC.](http://www.somewhere.com/)