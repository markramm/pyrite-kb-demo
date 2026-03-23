---
id: rre-wizards-of-os-2-2
title: "[RRE]\"Wizards of OS\" 2/2"
type: writing
writing_type: rre-post
url: "http://commons.somewhere.com:80/rre/1999/RRE.Wizards.of.OS.2.2.html"
importance: 6
research_status: partial
tags:
  - activism
  - ai
  - cognitive-science
  - commerce
  - cryptography
  - democracy
  - education
  - environment
  - government-info
  - international
  - internet-policy
  - labor
  - law
  - media
  - military
---



## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1999/RRE.Wizards.of.OS.2.2.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991008015458/http://www.somewhere.com/)

  

# [RRE]"Wizards of OS" 2/2

```
[This is part 2.  I have reformatted it.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html
or send a message to requests@lists.gseis.ucla.edu with Subject: info rre

---

Date: Sun, 10 Jan 1999 19:19:10 +0000
From: "Volker Grassmuck" <h0724elw@rz.hu-berlin.de>
To: pagre@alpha.oac.ucla.edu
Subject: "Wizards of OS" 2/2

                           "The Wizards of OS"
          Operating Systems and Social Systems
                House of World Cultures Berlin
                             July 15-17 1999

               http://www.mikro.org/Events/OS

                            Detailed Concept

Day One: From Monolithic to Distributed Operating Systems

  Achiving synchronization without centralization requires doing
  things in a different way from traditional operating systems.
  (Andrew S. Tanenbaum 1992: 464)

The computing tools of the founding generation had no operating
system.  The earliest OS- like software in the late Fifties were
called IOCS (Input/Output Control System) or Monitor.  The OS/360
developed by IBM in 1962 is generally considered the first "real" OS.
Its most important innovation was multiprogramming (in partitioned
storage areas, several jobs waited at any one time to be processed).
The point was always to make optimal use of the processor as a scarce
and expensive resource.  This economic motivation was also behind the
concept of time-sharing, first proposed by Christopher Strachey in
1959.  Time-sharing was an important turning point in the evolution
of the computer from a "numerical tool" to a "society of intelligent
agents".

Computer manufacturers and most representatives of the computer
science establishment believed that time-sharing was an inefficient
use of computing resources and that it shouldn't be pursued.  J.C.R.
Licklider, the architect of the MIT project MAC (Multiple-Access
Computer, aka Machine-Aided Cognition, aka Man and Computer), argued,
however, that computers were too fast and costly for real-time
interaction, for "cooperative thinking with a human," which is why
they should divide their time among many users.

In the early Sixties, Robert Fano and Fernando Corbato of MIT's
Computation Center developed the Compatible Time-Sharing System
(CTSS).  After three years of experience with the new way of using
computers, they asserted: "Most striking is the way the users have
built on one another's work...  More than half of the commands now
written into the system were developed by the users...  Whereas in
conventional computer installations one hardly ever makes use of
a program developed by another user, because of the difficulty of
exchanging programs and data, here the ease of exchange has encouraged
investigators to design their programs with an eye to possible use
by other people...  It is now easy to envision the use of the system
for education or for real-time collaboration between the members
of a research team...  The coupling between such a utility and the
community it serves is so strong that the community is actually a part
of the system itself." (1966)

An innovation motivated by the need to economize resources led to the
evolution of the computer as a medium while its users evolved into a
community.  In the technical computer science literature of the time,
terms such as communication and cooperation began to emerge.  There is
talk of a man-machine symbiosis (Licklider), synergy (Ulam, Engelbart,
1963), real time interactivity and a dialogue between machines and
users as well as among users via the machine (Fano/Corbato, 1966).

At the same time, the shift from line-switching to packet-switching
was taking place in telecommunications.  When, in 1969, two mainframe
computers at the universities of California and Utah were connected,
the history of the Internet began.  The networking of computers from
different manufacturers made open OSs that could run on a variety
of platforms necessary.  With the release of UNIX 4.2BSD in 1983 and
the integration of TCP/IP, the Net had its OS.  In the early Eighties,
Sun proclaimed, "The net is the computer," a vision that Larry Ellison,
head of Oracle, restated in the early Nineties with the network
computer (NC) supported by Java and containing no hard disk.  Today,
we can observe how computers, networks and embedded microprocessors in
electronic devices (robots, cars, kitchen appliances, cellular phones,
watches, etc.) are growing together into one distributed,
heterogeneous, interoperating, digital environment.

From the genealogy of the OS paradigms we know four ways to structure
OS software: monolithic systems (Unix, MS-DOS), layered systems
(Multics), virtual machines (VMS) and client-server models (Plan 9,
Amoeba, Mach, TRON).  The spread of microprocessors and LANs in the
Eighties led the transition to distributed systems with several
processors and client-server structures.  Distributed systems have
numerous advantages over centralized systems.  It was after all a
requirement by DARPA for the design of the Internet that the failure
of one component would not result in the failure of the whole system.
Performance-related and economic issues also speak for distributed
systems.

The movement away from a monolithic block of software toward smaller,
communicating units is rooted in developments in various areas of
computing.  In the design of programming languages, it's the change
from the top-down approach of structured programming to the bottom-up
object-oriented programming.  The Norwegian computer scientist
Kristen Nygaard is known as the originator of this concept.  Together
with Dahl and others he created Simula67, the first object-oriented
language.  Truly significant was the new way of thinking in Smalltalk
developed by Adele Goldberg (Xerox PARC).  C++ made it widely known.
In networks, the movement was from the star-shaped, line-switched
arrangement of "dumb" terminals toward packet-switched client-server
architectures.  In AI, it's from rule-based representations of
knowledge (expert systems, for example) toward connectionism (neural
networks, for example).  In interface design, it can be observed in
the current development from the WIMP paradigm (Windows, Icons, Menus,
Point and click) developed at Xerox PARC toward dialogue-based agent
systems, from manipulation toward delegation.

And in operating systems, the change is from the monolithic to
distributed models.  Early examples of the new way of thinking are
Oberon by Niklaus Wirth (ETH Zurich) and Plan 9 by Dennis Ritchie,
Ken Thompson, and others (Bell Labs), the original authors of Unix.
Today, distributed OSs such as Tron, Java-OS, Amoeba, GNU Hurd and
Inferno (the successor to Plan 9) point the way.

Modern conceptions of OSs are certainly a part of -- a reaction to,
and an impulse for -- further-reaching social and epistemological
concepts of dialogue and distribution.  This way of thinking appears
in other fields of study as well.  Ecology, for example, with its
networks of autonomous yet interdependent, heterogeneous elements is
important.  Also in management and organization theory, one speaks of
"flat hierarchies" and "decentralized, self-organizing units".

A revolution along the lines of the PC revolution and the Internet
revolution is being prophesied.  IBM's head, Lou Gerstner (whose
company brought a new NC onto the market), has just again declared
the death of the PC.  The concept of "intelligent" buildings and
"intelligent" cities, recently trumpeted on Potsdamer Platz, is also
a part of this movement toward distributed systems, right along with
talk of semi-intelligent, semi-autonomous software agents.

Several vectors point in the same direction.  Today's challenge is
to develop a distributed operating system for the distributed and
heterogeneous world of things, evolving in coordination with the
distributed and heterogeneous social systems.

Day Two: Social Systems

An OS and its design philosophy "exert an extremely strong influence
on the technical cultures that grow up around its host machines," as
the motto goes.  Passionate groups of devotees and cults form around
OSs, defending and promoting them with almost religious zealotry.
When Umberto Eco classified the Mac OS as catholic and DOS as
protestant, he unleashed a minor religious war.  "Technical cultures"
refers first to the cultures of technicians.  More generally, though,
all cultures that are based on media are always technical as well.
An argument could even be made that the phenomenon that is society
represents nothing other than an effect of the interconnections
created by media technology.

The second day will deal with the difficult question of the
relationship between the operating systems of technical systems and
what in a non-trivial analogy might be called the operating systems of
social systems.  Sociology of technology, research into the effects of
technology and similar approaches have shown that forcing technology
and culture into a dichotomy simply doesn't work.

In the design of a technical artifact such as an OS, non-technical
aspects come into play in a variety of ways: the culture of the
computer scientists within a culture of science; the forms of
social organization under which computer scientists work; general,
contemporary management and organization theories; broader
epistemological fields; the structures of the application domain
within which the software is to operate; models of various users of
the software (system administrators, programmers, end users -- each is
assigned his or her place in the system by their respective interface
to the OS), etc.  These aspects which work their way into the design
feed back into the social systems in the form of the artifacts where
in turn they effect changes.

The user interface -- from the desktop to systems for CSCW (Computer
Supported Cooperative Work) or groupware -- is the central link
through which psychological and social systems are mediated into
technical ones, and vice versa.  The most advanced instance of the
interface between man and machine, or more precisely, between humans
and digital information are agent systems, allowing the user to
train a software module which is able to learn according to his or
her wishes.  "This implies a two-sided relationship: in order to
create and shape the user model, the human has to express himself
in the agent; his inner value system has to be made explicitly
manifest (at least in the form of examples).  At the same time,
the phantasmagorical agent serves as a manifest image of the self.
It makes objective just how one perceives by regulating what one
encounters, and therefore, what one knows (of oneself)."  [Pfl=B3ger
97: 447 f.] It can't be made more clear just how intimately both sides
of the reciprocal constitution are interwoven.  And further, just how
problematic the position held by some cultural scientists is who use
and think of the computer as little more than a typewriter.

At the same time, social systems refer to OSs in their self-
description.  Thomas Wulffen unleashed the term "Betriebsystem Kunst"
("Art Operating System") to the world.  The term represents a flat
analogy relating more to the "functioning systems" of sociological
system theory than to computer science.  What's meant are collections,
museums, galleries, art schools and art publications, that is,
elements underlying the variety of possible "applications" which
define the total art system and keep it running.  If one were to carry
the analogy further, every institutionalization or differentiation
of a social functioning system would be based on the formation of
an OS, that is, a bundle of functionality, such as the allocation
of resources, scheduling and Input/Output (the institutionalized
communication with other functioning systems), forming the foundation
of a social system.  Could the legal system be viewed as the "OS of
society"? Or "communication"?  Or money? If capital can be seen as the
operating system of social systems, with the hardware on which it is
compiled (made "excecutable"), with its fundamental operations, its
application software and its interfaces to other system components?

Viewing technical and social systems together, thoroughly and deeply,
may turn up valuable insight.  Actor-Network Theory (Latour, Callon,
Law) seems at first glance to offer a vocabulary ideally suited
to describing distributed, object-oriented systems.  The discourse
analysis of technical systems (Friedrich Kittler) makes a subject-
centered bias avoidable.  System theory as well (Niklas Luhmann) and
its concepts of functioning systems which distinguish among various
tasks for society seems applicable for the observation of fundamental
operations which keep systems running.  Or, in the end, would a
Marxist reading, a capital analysis of the market and its checks and
balances be sufficiently to explain the system?

In any case, it is significant that the term "operating system" has
left the field of computer science and is beginning to be utilized by
social systems to describe themselves.  This alone reveals possible
points of departure concerning the construction of the identities of
systems in the age of digital media.

Computer scientists who make use of social models and cultural
observers who borrow from computing models -- in the field between
them, additional questions can be raised.  Questions about wealth
and poverty (which are behind the recent decision of the Mexican
government to install GNU-Linux in 140,000 elementary and middle
schools), educational questions (are children being socialized
into a Microsoft world during their computer lessons?), and last
but not least, political questions (who has read-access and who has
write-access to which information -- a question confronting anyone
who designs a multi-user, i.e. a social system).

The goal for this day can obviously not be so ambitious as
to completely clarify the relationship between "society" and
"technology".  It would be enough to show that a relationship exists,
to bring the OS out of the background and into the focus of attention
and show that this "ground" has social, psychological, cognitive
and world- constituting aspects.  If the first day proposes that the
paradigm shift of OSs takes us into a new phase in which decisions can
still be made, then the second day can show that these decisions have
an impact on all who have any relationship with media.

Day Three: Organization and Economy

Microsoft inherited its monopoly from IBM.  The sheer mass of
the colossus turned even non-IBM PCs in the Eighties into "IBM
compatibles" -- and thereby MS-DOS machines.  The U.S. Department of
Justice challenged IBM's monopoly in the courts for thirteen years,
but in the end the company lost its overwhelming position not to
federal prosecutors but because it slept through the PC revolution.
The pattern could be repeated now to the detriment of Microsoft:
the antitrust case could turn out to have no bite in it (as the legal
approval of the release of Windows98 with its integrated browser has
shown), while at the same time, the company is simply left behind by
a new generation of technology and a new organizational paradigm.  One
of the few opponents of the antitrust case writes that all the talk of
MS abusing its dominant position in OSs misses the point: "Microsoft
is desperately trying to keep its operating system from becoming
irrelevant." [Hume in Thierer, November 1997]

The new organizational paradigm sprang from neither sociological
theory nor a think tank.  The oft-sung sharing spirit of the Internet
has its roots in the OS innovation of time-sharing.  "Sharing"
meant open source code -- for hackers, as a fundamental element of
their ethic, for AT&T's Bell Labs, as the result of the antitrust
restrictions: because they were not allowed to market Unix, they gave
it to universities.  In turn, at the universities, the technical and
copyright preconditions for sharing met with the academic imperative,
"Publish or perish!", as well as with the spirit of the hippie
subculture.  Net historian David Bennahum points out that it was
no coincidence that Unix as well as the forerunners of the Internet
appeared in 1968 of all years.

Not so much as a loudly proclaimed revolutionary movement, but rather,
more or less unnoticed, the idea of a gift economy wandered from the
ethnological books of Levi-Strauss into the development of software.
Today it stands as competition to the classic political economy.  With
the communications protocols UUCP (Unix to Unix Copy) and TCP/IP, the
Net became an integral component of Unix, and the Usenet newsgroups
became an integral part of the community which developed it.  In
opposition to the closing of Unix after the deregulation of AT&T,
Richard Stallman of MIT started a project to create a freeware
Unix called GNU in 1984.  With Emacs as an editor and Hurd as an
OS, Stallman's Free Software Foundation created important products,
but most significantly, it formulated the GNU Public License (GPL),
the model for copyleft protected free software that spread throughout
the world.  Among the successes of open source software are GNU-Linux
(the most widely distributed Unix for PCs), Apache (the most widely
distributed Internet server software), PERL (the standard scripting
language of the Internet), BIND (the basis of theInternet domain name
system), Sendmail (the most widely distributed mail transfer software)
and Majordomo (the most widely distributed mailing list server,
written in PERL).  It's also no coincidence that all the above named
software projects are native to the Net.

There were always philosophers and evangelists, but there wasn't a
"manifesto" for the open source movement until early in 1998 when Eric
Raymond unleashed "The Cathedral and the Bazaar".  The essay outlines
the rules of thumb essential laws for a distributed, open, loosely
connected cooperation on the same complex software project among
thousands of people throughout the world.  His prime example for
the success of such an improbable form of organization is Linux,
initiated by Linus Torvalds.  "In fact, I think Linus's cleverest
and most consequential hack was not the construction of the Linux
kernel itself, but rather his invention of the Linux development
model."  [Raymond, C&B] Open source turned conventional logic on its
head: distributed groups of equals are more efficient than top-down
hierarchical systems.  Whoever gives away the fruit of his labor,
receives more in return.  Self-interest and recognition are more
effective motivations than money.

Among the most spectacular developments of the year was Netscape's
release of the source code for its browser and the deal between
IBM and the Apache Group for IBM's server package "WebSphere".  The
waves rolled so high that even MS ordered an in-house analysis of
open source.  When this confidential, so-called Halloween Document
was revealed, it became clear that MS perceives open source software
as a direct and short term threat to its profits and its platform.
Further, the author sees benefits in the free exchange of ideas that
MS is not able to replicate, and therefore, it represents a long term
threat to its hold on mindshare among software developers.  In order
to head off the danger, he recommends among others a strategy that
MS already uses against Java: MS takes an open standard, "enhances"
with its own proprietary functions, which it then tries make into the
"de facto" standard through the saturation of the market.  MS would
hardly be able to pull off the privatization of such public property
as TCP/IP, HTTP, Linux or Apache, as recommended in the Halloween
Document, but this is precisely what they are aiming to do in order
to avoid "becoming irrelevant".

When even Forbes magazine sang the praises of open source and hackers
in its August 1998 issue, one could be forgiven for wondering if the
end of capitalism was nigh.  Or, on the other hand, is open source
as the superior software development model most compatible with a
post-dogmatic, flexible capitalism? Is open source the equivalent
to the third sector in the political debate and to a shift from
"building" to "growing" in various scientific disciplines? In the
comparison to closed software development, is more efficiency and a
better business model all that matters or can a more viable idea of
the "public good" be established? Is the idea really so absurd that
the foundational infrastructure of our lives, including air, parks,
water fronts, libraries, museums and operating systems ought to be in
the public domain? Is a new order of knowledge being signified in this
open collaborative development?

In the early years of the railroads in England, each of the individual
companies laid tracks of differing width -- until all the parties
realized that a universal standard was in the interest of everybody:
the track manufacturers, the operators of transport services and
the passengers.  Such technical standards can be derived in three
ways.  They can be decreed by the state, as was the case with European
post offices, railroads, telecommunications, electric utilities
and so on.  They can be rammed through via monopolistic powers in
the so-called free market, which is what happened in the case of
the QWERTY keyboard, VHS, MS-Windows, etc.  Or they can be derived
via collaborative development in meta-national commissions.  Such
institutions can be trans-national (ISO, CCITT), occupational (IEEE),
industry-wide (W3 Consortium) or be completely open (IETF).

The first model of standardization has fallen out of fashion, and the
second has been discredited.  If one wanted to propose the development
of a standard for operating systems for a globalized, multifaceted,
distributed and networked world, the first thing one would probably
think of is try to register it with the International Standards
Organization (ISO).  The ISO was set up as an umbrella organization
over the national standards organizations, each of whom sends
delegates to the working groups.  Conflicts are resolved by voting,
which is why determining representation is critical.  Each step
in the process has to be approved by the national committees and
their clients whose interests have to be represented in the end
product.  The case of OSI (Open Systems Interconnection) showed
that this process cannot keep up with the rapid pace of technology.
Furthermore, while ISO standards are open (meaning that the
specifications are available to everyone at a price), they are not
free (meaning free from licensing fees paid to companies or research
institutions which have registered patents during the course of
standardization).

A different process of standardization is followed by the Internet
Engineering Task Force (IETF) which presides over the fundamental
technology on which the Internet is based.  Their working groups
are completely open to whomever is willing to pitch in.  Because
no authority is delegated, there is no voting; instead, decisions
are made by pragmatic consensus.  As opposed to the ISO, the goal
is not to develop a universal and complete standard with backward
compatibility and a sturdy future, but rather, "to scratch an itch"
(Raymond), that is, to quickly and simply solve an immediate problem.
The individual steps are documented in RFCs (Request for Comment)
which, like the email discussions of the participants, are open to
all.  Because the source code of the software standard is visible and
open to modification, it is tested by an incomparably larger number of
developers than in the ISO process.  Companies, too, assign employees
to the IETF working groups -- not because they hope to attain patents,
but because they want to sell cars and rest stops for a freely
accessible, stable and highly trafficked superhighway.

Also in the world of Unix and in the subworld of GNU-Linux, there
has been an effort towards standardization for some time.  From its
very beginnings, the Linux Kernel Project has maintained an OS kernel
which is binding for the whole of the Linux world.  The Linux Standard
Base (LSB) is now attempting to secure a similar model for retaining
the compatibility of applications across the various distributions.
Standardization makes for a unified world of Unix, which in turn makes
it very attractive for software manufacturers to port their products
to Unix and for hardware manufacturers to write drivers for.

Linux, in the role of David, has won the attention and acceptance
("mindshare") which Goliath, Microsoft, now fears.  But if the
analysis of the paradigm shift from centralized to distributed
social processes is correct, and this is paralleled by its "naturally"
appropriate paradigm shift from monolithic to distributed OSs,
thenUnix will have to change as well.  Indeed, the idea has already
been floated that Unix could be further developed with distributed
characteristics (the Beowulf Cluster, for example) and real time
capabilities.

These approaches in the Unix world would be included in the project
proposed here for an IETF-style development of an OS, just as all
the other distributed OSs (Plan 9, Java, Tron, Amoeba, etc.) as well
as the development in the TCP/IP world.  Because neither capital
nor numbers figure into this process, even MS developers could take
part without the danger of the corporation dominating the development
process.  Further, there is reason to believe that in such an open
process without direct monetary interests, the technology recognized
by the majority as superior would become the standard, and not -- as
in the now classic case of VHS vs. Beta -- the technology backed by
the most powerful player on the market.

As opposed to railroad tracks, an OS is not a product but an ongoing
process.  One of the most remarkable insights in the Halloween
Document is that in open source, MS doesn't have another company as
a competitor, but rather, a process.  More important than settling on
a certain standard is finding a procedure for further developing the
dynamic foundation of our media existence which promises the greatest
good for the greatest number.

On the first day, it was shown that OSs currently face a paradigm
shift, a new beginning.  MS is active in the field of distributed
OSs, but hasn't yet matched the dominance it has in the PC market.
So there is an opportunity to do things better this time around than
last time.

On the second day, it was made clear that decisions in the design of
OSs are not "extra- social", "extra-cultural" or "purely technical"
questions, but rather, deeply political and effected by every computer
user, even if only by his or her buying habits.  So it's up to us to
make the most of this opportunity.

After closed source and open source are contrasted on the third
day, and the advantages and disadvantages of the various models of
standardization models are presented, the closing panel will address
the question of whether or not it would be meaningful and possible to
set up an IETF-like working group to develop the next generation OS
standard.  Should such a project prove to be feasible and desirable
during the discussion, it would be the crowning achievement of the
event to celebrate the creation of such a body.

(translation by David Hudson)

---

   vgrass@rz.hu-berlin.de
   http://waste.informatik.hu-berlin.de/Grassmuck/
   http://www.mikro.org
   http://www.mikro.org/Events/OS

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991008015458/http://www.somewhere.com/)