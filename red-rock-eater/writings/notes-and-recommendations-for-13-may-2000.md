---
id: notes-and-recommendations-for-13-may-2000
title: "Notes and Recommendations for 13 May 2000"
type: writing
writing_type: paper
date: 2000-05-13
url: "https://pages.gseis.ucla.edu/faculty/agre/notes/00-5-13.html"
coauthors: []
key_concepts: []
importance: 5
research_status: stub
tags:
  - paper
  - auto-imported
---

## Source

Automatically imported from: https://pages.gseis.ucla.edu/faculty/agre/notes/00-5-13.html

## Content

```
Further notes on Microsoft's irresponsibility, design spaces, eBay,
systems analysis courses, and the new jargon, plus recommendations
and yet another high-quality batch of URL's.  This message is even
more indebted than usual to the excellent RRE readers who send me
stuff, and I again ask everyone to send me good stuff for the list.

In response to my notes on the slippery language Microsoft has used to
evade responsibility for the security problems that were exploited by
the most recent e-mail virus, RRE readers sent me a slew of additional
quotes from Microsoft personnel, including some that are astounding.

We can begin with another example of defocusing: redefining the issue
by eliding certain elements of critics' arguments:

  "The issue here isn't scripting.  It's the social phenomenon of
  virus writing.  That virus could have been written as an executable
  or on any platform or in a nonscripting language.  Just because this
  virus was written in a scripting language, and we happen to support
  scripting in our operating system, doesn't make it a security issue."

  http://news.cnet.com/news/0-1003-200-1823167.html

Read this passage closely.  Leave aside the question -- hard to even
discuss because it is so conveniently vague -- of whether "that virus"
could possibly have been written in another language or even on another
platform and still been the same virus.  The problematic part starts
with "Just because ...".  It's conceivable that someone, somewhere has
argued that the problem is the simple existence of scripting languages.
That person would be a convenient foil, but would hardly represent the
mainstream of critical opinion.  The problem, as everyone knows, is
not scripting languages, but email clients that can execute attachments
that contain scripts that can perform a wide variety of potentially
damaging actions.  Blaming "the social phenomenon of virus writing"
is not reasonable.  A product that can be subverted by a random college
student to cause massive worldwide damage is not secure.  That's what
"secure" means.

Given the scope of the recent disaster, some people were surprised to
find the following text in a Microsoft "knowledge base" page entitled
"General Information About Using VBScript with Outlook":

  VBScript is designed to be a secure programming environment.  It
  lacks various commands that can be potentially damaging if used in
  a malicious manner.  This added security is critical in enterprise
  solutions.

  http://support.microsoft.com/support/kb/articles/Q167/1/38.ASP

(In case the page changes, I copied and pasted above passage on the
evening of 5/8/00.)

Rereading the passage I've quoted, one notices that no claim is made
that VBScript includes no commands that can cause damage -- only that
"various commands" are not included -- and likewise that no claim
is made that VBScript under Outlook is secure -- it only has "added
security".  It sounded good when I read it the first time, though.

Or consider the following passages from a message from Microsoft,
dated 5/8/00 and entitled "Special Edition -- Office News Service --
Virus Alert":

  Last week a new virus began circulating through e-mail that has the
  potential to affect a wide range of e-mail users including those
  users running Microsoft Outlook.  If run, the virus could overwrite
  .jpg, .mp3 and other file types, and attempt to send a copy of
  itself to everyone in the recipient's address book.

The language here attempts to break any mental association between
the virus vulnerability and Outlook.  The virus, we are told, "has the
potential to affect a wide range of e-mail users including those users
running Microsoft Outlook".  A hurried reader would take away the
impression that the problem is not Outlook-specific.  But two seconds'
thought will raise doubts.  First, the virus will only work on a
machine that can execute Visual Basic scripts.  That narrows it down
quickly to a small range of Microsoft platforms.  One might ask, do
other Microsoft mailers execute Visual Basic scripts in attachments?
But that's not what the passage says.  It says only that the virus
"has the potential to affect a wide range of e-mail users".  Someone
who uses a Windows 98 mail client besides Outlook could for whatever
reason save the attached VBS file and then specifically execute it
from the desktop.  This could "affect" the user's machine (damaged
files, modified startup, reset Explorer homepage), but it wouldn't
propagate the virus because the propagation mechanism relies on the
Outlook address book.  This particular claim turns out to be correct,
but you have to read it carefully.

At least the passages I have quoted so far are just evasive.  Some
of Microsoft's statements have been outright false.  Here is a later
passage in the same text:

  1) Customers can avoid being affected by this and other viruses by
  following standard best practices:
  ++ Never run an executable from someone you don't know.
  ++ Always have a good-quality virus scanner.
  ++ Always keep the virus scanner's signature files up to date.

This is just not true.  The messages that contained this virus were
from people who had you in their address books; they are therefore
likely to be people that you know.  The suggested policy of not
opening attachments (now called "running executables" -- even though
the idea that opening an attachment is running an executable will
be counterintuitive for most normal users) from people you don't
know will not prevent this virus from spreading.  Nor will the other
suggested policies prevent the virus: the best widely used virus
scanners (for some weird reason) do not stop this sort of virus
without it being included in a signature file, and the signature files
in this case (as in other cases) were not updated until the virus had
already spread far and wide.  It is little wonder, then, that the same
Microsoft message included the following disclaimer:

  INFORMATION PROVIDED IN THIS DOCUMENT IS PROVIDED 'AS IS' WITHOUT
  WARRANTY OF ANY KIND.  The user assumes the entire risk as to the
  accuracy and the use of this document.

The following astonishing passage is from an online column about
Microsoft's irresponsibility by Hiawatha Bray of the Boston Globe.

  When I raised the issue with Microsoft spokesman Adam Sohn last
  week, he described his idea of how companies could improve the
  security of Outlook.  "They should commence by beating their
  employees", Sohn declared.

  He chuckled to signify that he was kidding -- but only about the
  floggings.  Sohn was dead serious about Microsoft's utter lack
  of responsibility for the Love Bug fiasco.  Instead, he blamed
  the silly computer users who go opening e-mail attachments.
  "People shouldn't open them", said Sohn.  "That's the problem."

  http://www.digitalmass.com/columns/software/0508.html

A Microsoft spokesman is joking that employees should be beaten
for opening an attachment -- an attachment from a friend no less.
I am not making this up.

Finally, listen to this quote from Microsoft's inescapable Scott Culp:

  In this case the virus author chose to target Outlook probably
  because it gave him better reach.  There isn't a security
  vulnerability in Outlook involved in this at all.

  http://dailynews.yahoo.com/h/nm/20000504/wr/virus_love_11.html

Mr. Culp thinks he is playing a game.  Look everyone!  I've managed
to spin this situation into being something good about Microsoft!
Never mind the lack of logical connection between the two sentences.
This is the company whose products are being used to rebuild the
productive infrastructure of the entire world, including large parts
of the US military.  We are insane to be doing business with them.

What really causes these endless computer security disasters?  We've
talked about economic factors, but now I think we have to talk about
another factor: weenies.  Weenies come in two varieties, tech and
marketing.  Tech weenies think they're smart but aren't mature enough
to do real engineering.  Marketing weenies mechanically apply the
marketing dogmas of product differentiation but aren't capable of
having a real vision for their products.  Multics was designed by
real engineers and the Mac was designed by marketing visionaries,
but Windows was designed by weenies.  The most distinctive feature of
weenies is the worship of features.  Tech weenies want everything to
be cool: that means hypergeneral, hyperprogrammable, hyperextensible,
no matter what hazards might result.  Marketing people obsessively
look at the complete list of features in their competitors products
and command the tech weenies to include all of them, and then to
differentiate the product by adding more.

The tech weenies and marketing weenies typically hate each other, but
they have this in common: neither of them will ever voluntarily remove
a feature from a product, even if it causes billions of dollars in
damage.  Tech weenies are basically designing for themselves, and have
no conception of human beings and their relationships -- and thus no
coherent trust model in their products.  Marketing weenies are frantic
to get products to market, and have the shortest possible time horizon
-- and thus no concern for the world in which their products will soon
enough become ineradicable legacy systems.  Weenies too often win in
high-technology competition because a critical mass of their customers
lacks detailed knowledge of the products.  (Keep in mind that the real
customers of a company like Microsoft -- the ones who sign the checks
-- are generally neither the technical people nor the users.)  Security
catastrophies will not disappear until the weenies are all under adult
supervision.  This will never happen at Microsoft, which is managed by
two-year-olds who hire people just like themselves.  One more reason to
shut it down.

The Daily Howler has begin a month-long examination of the terrifying
pathology of the media in the ongoing presidential campaign.

  http://www.dailyhowler.com/

Strongly recommended.

A few people asked for a list of references for my set of informal
notes on the new design space.  Here are some relevant books, some of
which I have recommended here before:

  James N. Danziger, William H. Dutton, Rob Kling and Kenneth
  L. Kraemer, Computers and Politics: High Technology in American
  Local Governments, New York: Columbia University Press, 1982.
  Still remarkably relevant, this book is the origin, so far as I
  know, of the observation that computing is a malleable technology.

  William H. Dutton, Society on the Line: Information Politics in
  the Digital Age, Oxford: Oxford University Press, 1998.  Advertised
  with extensive exerpts here on RRE, this book has a framework
  for analyzing the social construction of "access" that is broadly
  compatible with my notion of people using information technology
  to amplify existing social forces, as well as with my discussion
  in other articles of problems with online boundaries.

  Andrew Feenberg, Critical Theory of Technology, New York: Oxford
  University Press, 1991.  Feenberg observes that computers are a dual
  technology that can be viewed either as mirroring the world in their
  representations or as a medium of communication.

  Batya Friedman, ed, Human Values and the Design of Computer
  Technology, Cambridge: Cambridge University Press, 1997.  My
  argument presupposes in a rough way that information technologies
  are not neutral, that they embody values and views of the world.
  This volume collects papers that explicate this idea.

  John Chris Jones, Internet and Everyone, London: Ellipsis, 2000.
  The celebrated experimental designer's lengthy meditations on the
  Internet, told largely through letters about design experiments
  involving spontaneity and chance.

  David G. Messerschmitt, Networked Applications: A Guide to the New
  Computing Infrastructure, San Francisco: Morgan Kaufman, 1999.  This
  is an introduction to modern networked applications architecture,
  written in plain English by a hard-core engineer.  It is a good
  source for all the stuff about layered systems and components etc.

  Mary Anne Moser and Douglas MacLeod, eds, Immersed in Technology:
  Art and Virtual Environments, Cambridge: MIT Press, 1996.  This is
  the standard text about environments that are immersive in the sense
  that I am sort of deprecating.

  Donald A. Norman, The Invisible Computer: Why Good Products
  Can Fail, the Personal Computer Is So Complex, and Information
  Appliances Are the Solution, Cambridge: MIT Press, 1998.  A polemic
  against the archaic world of personal computing with its excessive
  generality and physical clumsiness and in favor of computers that
  melt into the woodwork and let you get on with your life.

  Donald A. Schon, The Reflective Practitioner: How Professionals
  Think in Action, New York: Basic Books, 1983.  When I refer to the
  processes of "design" in the artistic sense, this is what I have in
  mind.  Schon's description of the iterative reconceptualization that
  goes on in the teaching of architecture -- what he calls design as
  a "reflective conversation with the materials" -- has been justly
  influential.

  Douglas Schuler and Aki Namioka, eds, Participatory Design:
  Principles and Practices, Hillsdale, NJ: Erlbaum, 1993.  This is
  a good collection of articles about designers collaborating with
  users.

  Carl Shapiro and Hal Varian, Information Rules: A Strategic Guide
  to the Network Economy, Boston: Harvard Business School Press, 1998.
  This is the most accessible reference for the stuff about standards
  and the reflexivity of network effects.

  Marc Smith and Peter Kollock, eds, Communities in Cyberspace, London:
  Routledge, 1999.  This is perhaps the most useful book about the the
  Internet and community, including both the online and offline sorts.

  Etienne Wenger, Communities of Practice: Learning, Meaning and
  Identity, Cambridge: Cambridge University Press, 1998.  In an
  Internet context, the word "community" has unfortunately come to
  mean "online community", even though the great majority of real
  communities employ a wide variety of media including the Internet.
  Wenger's book presents a productive analytic framework for looking
  at communities of people who share collective identities and
  practices.

That's a partial list, and it doesn't dig very deeply into the design
literature on either the arts side or the technology side.  But it's a
start.

The announcement of Bob Smith's book "Ben Franklin's Web Site: Privacy
and Curiosity from Plymouth Rock to the Internet" somehow included the
wrong e-mail address (it should be privacyjournal@prodigy.net) and the
wrong Web site URL (it should be ).

In response to my notes on eBay, Paul Resnick directed me to his online
directory of researchers on the subject of trust systems:

  http://databases.si.umich.edu/reputations/

Giorgos Zacharia also directed me to his master's thesis on reputation
mechanisms whose algorithm design is influenced by problems with the
eBay-like feedback mechanisms:

  http://ecommerce.media.mit.edu/reputations/complete_thesis.pdf

And a dealer in postage stamps sent me the following description of
the Byzantine small world of online stamp auctions.  I've reformatted
it.  He asked to remain anonymous for obvious reasons...

  You're going to get a lot of commentary.  I'm going to confine
  myself to one argument and be relatively brief in my observations.
  In addition to my other lives, I am a partner in a philatelic
  joint venture ....  We are running an expanding business on eBay.

  RE: Argument 5

  Factors not taken into account include the behavior of multiple
  bidders probing each others' maxima and the perceived status and
  needs of other bidders.  This is a Byzantine game as complex as
  any played out in the elite auction houses of London and New York
  (which are rapidly adopting the on-line mode).  The similarities
  are actually very extensive.

  Incidentally, all philatelic auctions (brick-and-mortar, mail,
  telephonic, etc.) have maximum-bid provisions.  Unlike eBay, many
  physically based auctions also have provision for cumulative maxima,
  allowing a bidder to win lots in a particular sale until a specific
  figure is reached or closely approached.

  a) eBay bidders have access to the recent bidding histories of
  all competing bidders, including bidding times and other pattern-
  revealing information.

  b) eBay bidders have access to the recent sales history of the
  seller, including a record of all last bids from each bidder on
  each auction, with bidding times.  Knowledge of bidders as buyers
  and sellers permits extrapolation of their assessments of item
  value, while knowledge of THEIR bidders behavior as buyers and
  sellers permits .... {{{ INFINITE REGRESS: the calculus of Maya }}

  c) The professional trade on eBay is semi-collegial and has its own
  practical ethics: for example, I rarely bid against my clients until
  they are outbid, nor do I bid against my preferred vendors unless
  I am bidding for a particular client to repurchase by private treaty
  and believe the vendor is bidding for stock (the latter is one of
  the few cases in which I will place an early maximum bid to indicate
  that I have a firm pricepoint).

  d) I can bid in multiple auctions on multiple continents almost
  simultaneously by opening multiple browser windows.  I can also
  watch other auctions in which competitors for a given lot are
  bidding: if I know their spending patterns, I can gage their
  willingness to chase a lot in light of their other current bids
  and recent expenses.

  e) I can select auctions for bidding that close at times inconvenient
  for particular possible competitors.  I can schedule my auctions
  to close at times most favorable to bidders in a particular country
  (e.g., I have a lot of clients in the Benelux region but few in
  former Dutch possessions in the Orient: if I have censored wartime
  Indonesian covers, I will schedule them to close at prime buying
  hours in Jakarta, in an effort to expand out clientele in the region).

  There are many other wrinkles peculiar to the philatelic business,
  but market making in this field is just as complicated on eBay as in
  the world at large.  The one huge advantage to both buyer and seller
  is the ability to display an item on line at no cost: I live by
  my reputation for honest grading and descriptions, and photographs
  enable me to substantiate it before a purchase is ever made.

What most struck me is how the online practices of stamp dealers are
both embedded in the existing complex social world, and the detail in
which these practices nonetheless depend on the workings of the online
auction mechanism.  Other readers described similar complexities in
their own fields.

A while back I called for the creation of Stats Watch, a nonprofit
organization of statisticians who issue press releases and conduct
publicity stunts when they spot abuses of statistics in the media.
Well, the other day I noticed an AP wire report about an organization
called Statistical Assessment Service  that
claimed to have determined in a scientific manner that Al Gore's
statistics were bad and George W. Bush's statistics were just fine.
Looking more closely, I found that this organization is a partisan
conservative activist group that uses public relations tactics but
pretends to be scientific and neutral.  I was depressed at this
disingenuous stuff, which illustrates why it's so hard to main any
standards of rationality in a world of public relations.

In response to the course materials from my ongoing systems analysis
and design course, Rich Giordano described his own attempt to overthrow
the orthodoxy in that area.  Our correspondence really brings out the
underlying reasons for the difficulty of the project, so I've included
an edited version of it here.  I've omitted the initial back-and-forth
messages in which Rich says "I'm doing something similar and it worked
well" and I say "tell me more".

  Date: Thu, 20 Apr 2000 10:44:21 -0400 (EDT)
  From: Richard Giordano 

  It might be easier to ask me some questions about the course.  The
  course is hard to teach because I have to combine the social with
  the technical.  The way that I do this is to group the students into
  teams (as you have done), and ask them to be reflective on their
  collaborations.  Each student keeps a journal which they give to me
  at the end of the course.  The purpose isn't to grade the journal,
  but to help students to reflect on what they are doing.  Moreover,
  at the very beginning of the course, we do a role-play.  A group
  of students act as systems designers and clients, and they have to
  re-design (or re-do) an existing information system.  They have a
  "preliminary meeting" for about 40 minutes while the entire class
  observes them.  This serves a few purposes: First, it breaks down
  whatever barriers exist in the class; second, it allows the students
  to think like designers; third, it allows the class to observe a set
  of hothouse designers in action.  After the role-play, we discuss
  what we observed.  What alliances were forming; what were the power
  relationships; what effect did existing technologies and solutions
  have on the design; who controlled the meeting? etc. etc.  The
  students dread doing this, but they love it afterwards.

  Like you, I ask them to observe information in-use.  The notion here
  is that information in use is messy -- go to any train station.  I ask
  the students to take something of a constructivist stance.  Regarding
  what they observe -- why is it like this instead of some other way?
  For example, they can go to Piccadilly Station in Manchester and
  observe what's happening there, and then ask "Why does it look like
  this?  What's the process behind it all?"  Then I go through some
  tools to help them capture processes -- it used to be the normal
  SSADM stuff, but I've changed it all to modelling.  The idea is that
  you need to create some form of documentation which can serve as an
  object for both historical purposes, but mainly to allow stakeholders
  to participate in a process -- and they can see their participation
  in some tangible object. (My underlying idea is that the emerging
  model is something of a boundary object.  I can't go into the use
  of boundary objects or cross-functional communities of practice
  in the calss in detail because I don't have the time -- but I do
  get the students to think about the social role of documentation.)
  Then we go through the object-oriented paradigm -- but I start big,
  looking at a generic system that consists of resources and services.
  The connection between resources and services leads to a discussion
  interfaces and standards.  Then we get back to the social again
  by looking at methods of evaluation.  I am guided in that regard
  principally by participative stakeholder evaluation techniques.
  [Ray Pawson and Nick Tilley, Realistic Evaluation, Sage, 1997. -- PA]

  The students give a presentation every single class meeting.  What
  they do is not so much present their work, but they present their
  thinking behind the work.  For instance, if a group models something
  in a certain way, the question is why this way instead of some
  other way?  Or why model this at all?  These are principally English
  and Commonwealth kids education to the A-level standard.  They are
  trained to write on paper, not to speak.  Giving presentations helps
  them to build their presentation skills, on the one hand, and to be
  critical on the other.  It also helps them see their work in relation
  to others, and to see that there are many ways of approaching the
  same problem.

  I can honestly say that the students love the course.  This is
  partly the result of their having something very different from
  their other CS courses, and partly because they like being taught
  by an American.  But many of them are still in contact with me years
  later and they say that the course helps them put their current work
  in perspective.  A substantial number have written to say that the
  experiences in the course helped them when they went on their first
  job interviews.  Although this may not seem like a lofty goal for
  the course, it does help demonstrate that what we do in the classroom
  has some relation to what people experience in the world.

  Date: Sun, 23 Apr 2000 12:59:17 -0700 (PDT)
  From: Phil Agre 

  Cool.  I assume you're on the semester system, since you're covering
  so much more material.  The formal analogies between our courses
  are extensive, but you're trying much harder to make the course map
  onto the relationships and activities that they'll be engaged in
  as working systems developers, where I'm going for a more abstract
  and generalizable experience of design. ...  Even though I believe
  strongly in the stuff about participation and politics, we just
  don't have time to do that, and the industrial design paradigm
  we're using doesn't draw out the aspects of social embedding that
  you rightly emphasize.  You're trying to get them to do the existing
  system developer job the right way, where I'm blowing that stuff
  away, largely I'll admit because I personally have no patience for
  it.  And as you say, you're getting them to use the technical tools
  they'll use on the job, where many of my students are probably not
  going to be using tools like that.

  But I think the most important thing you're doing in your course
  that I'm not is the stuff with the model of the situation-of-use
  that serves as a boundary object in the design process.  In general
  it sounds like you're teaching them good representational schemes,
  where I'm encouraging them to invent their own.  Each approach is
  valid enough, but yours has the massive advantage that they really
  do have this experience of a substantial representation that talks
  back to them throughout the design process, whereas my students
  really won't have more than a fragmentary representation of the
  situation they're designing for.  This may reflect my own lack of
  knowledge, but my problem with the modeling approaches that I've
  heard about is that they impose false models of the work process
  (or play process, etc), coming from industrial automation with its
  emphasis on fixed work routines, rigidly defined divisions of labor,
  etc.  My main purpose in having the students look at real people
  using information is to break some of these false models and instil
  a sense of the complexity of that embedding.  But I can't go on
  forever just breaking up intuitions; at some point the conversation
  can't proceed useful until you get a model in front of everyone.
  Can you suggest what I read to educate myself on this?

  Date: Mon, 24 Apr 2000 12:51:06 -0400 (EDT)
  From: Richard Giordano 

  Thanks so much for the kind words.  I think you exactly understand
  what I'm trying to do.  I did teach a more speculative systems
  analysis and design course -- a seminar -- called something like
  "Topics in Information Systems Design" where the students critically
  looked at the process of analysis, design and implementation.
  We also looked at case studies involving fraud, conflict, etc.  I
  liked teaching this course quite a lot, but left Manchester before
  I could really develop it.  This was given to graduate students in
  a combined CS/MBA program.

  The problem I have with modelling is that the tools you use to
  create the model work to reproduce the world in the image of
  the tools (or the underlying concepts of the tools themselves).
  Thus, object-orientation has been used as a foundation for process
  modelling and business process reengineering with, I think, horrible
  social results.  I've written about this to some extent in a piece
  with Martin Lea -- "Representations of the Group and Group Processes
  in CSCW Research: A Case of Premature Closure?" in Bowker, Star,
  Gasser & Turner, eds. "Social Science, technical Systems and
  Cooperative Work."  Since you have a piece in this volume, you might
  have it on your bookshelf.  The part I'm referring to is on pages
  9-14.  My general orientation toward modelling has been informed
  by various work in the social construction of technology.  I think
  you know this literature well, so I won't make specific references.
  Generally, I'm interested in how social forces influence the shape
  of tools with in turn influence social forces.  Some of this, as you
  know, is structuration theory, and in that regard I am influenced by
  Anthony Giddens and, to some extent, Wanda Orlikowski.

  I don't have any time to get into this in any detail in the class I
  teach.  For one, the course I teach used to last an entire semester,
  but the CS Department has changed the MSc timetable--the course
  lasts one intensive week.  (It's hard on everybody, and I'm not sure
  what the students learn in such a short period.  To make it easier
  for the kids, they know in advance what they have to do, and they
  get background readings.)  For another, the CS MSc students don't
  know anything about modelling, so I need to give them a foundation
  from which to move on.  I try to have them be critical of what
  I'm teaching while I'm teaching it, so the kids should know my
  reservations with modelling and the tools to do this.

  About readings related to models as boundary objects.  I don't know
  of any offhand. ...  My sources on boundary objects begin with Leigh
  Star.  How boundary objects might transform knowledge in practice
  (particularly because knowledge in practice is bounded-up with power
  -- and this is especially true in the process of systems analysis
  and design, as you know...) I lean somewhat on Bourdieu -- and a
  colleague named Paul Carlyle at the Sloan School at MIT -- for this.

The deep issue here is that the representational practices of computer
science -- data structures, at least as conventionally understood --
presuppose a rigid relationship between the "system" and the reality
that it represents.  System design methodologies have a way of
imposing their own view of the world, and that view is usually wrong.
That's one reason why I've moved toward design processes taken from
industrial design and architecture.  But ultimately one has to contend
with seemingly inherent problems with formalism.

When I tell the truth on this list, I sometimes get hate mail.  Not
that much, really, but enough.  When I do get nasty messages, they are
obviously from people who have had a lot of practice.  And I always
go through the same cycle: I send a short, intemperate response; I
delete the message; I breathe several times to get the anger out of my
system; I regret responding at all; an hour passes; I realize just how
sophisticated the rhetoric of the hate message was; and I regret not
having saved it.  This happens over and over.  My last round of notes,
however, got so many responses so quickly that one hate message was
still retrievable an hour later as I worked my way through subsequent
messages.  I enclose it here not to seek sympathy, which I truly do
not deserve, but because I find it interesting.  Note, above all, that
at no point does it make logical sense.  At the risk of interrupting
its trance-like flow, I have interleaved my own commentary.

  There was a time when I gleaned much that I considered worthwhile
  from your articles, but that time has passed.  In my opinion, you
  have put on blinders that restrict your view(s) as much to leftist
  dogmas and propaganda as any of the "conservative paranoia" you
  describe.

The high-toned first sentence melodramatically posits the high ground
from which he issues the abuse to follow.  Then he's right into it.
The illogic begins right away, as the second sentence can't decide
whether it's accusing me of spouting left-wing views or of blinding
myself to them.  It falls strangely into the middle, so that I can't
figure out what I'm being accused of.

  I gather that we should criticize George Bush for never having held
  a "real job", but the same condition in the life of Bill Clinton is
  perfectly acceptable.

This is extremely common.  Conservatives are trying to bring back the
culture of deference in which double standards are a routine way of
life, and to this end they continually manufacture bogus accusations
of double standards against the egalitarians who have long pointed
out double standards as a way of insisting that everyone be treated
equally.  In this case, the accusation is bogus in a straightforward
factual sense; before becoming President, Bill Clinton had at least
two real jobs -- as a law professor and as governor of Arkansas -- and
pointing that out surely doesn't make one a raving liberal.  (Because
of conservative media bias, many people are unaware that the Texas
constitution, unlike that of Arkansas and most other states, assigns
the governor very little power.)  Most likely this guy is fabricating
his double-standard accusation by distoring, in the blurry fashion of
lizard-brain thinking, the conservative accusation that Bill Clinton
never held a job in the private sector before he become President.
Or perhaps he is twisting language by secretly redefining a "real job"
as one in the private sector.  In either case he is twisting language.

Notice, too, the routinized innuendo: "I gather", he says, that he
is to believe a certain thing, even though I never said that thing
or anything like it.  "I gather" is one of many devices in the new
jargon for poking anything one likes into the mind and mouth of
one's opponent.  And the innuendos are about to start coming fast
and furious.

  Regardless of the issues surrounding so-called "father's rights",
  (and given that no father currently has any say in whether his
  child is to be born or aborted, I doubt that there is any such thing
  as "father's rights" in the U.S. law), are you at all concerned
  about the legal and constitutional aspects of the recent "rescue"
  of Elian Gonzalez?  Or of the lives lost in Waco and the "factory"
  in the Sudan?

These questions are really accusations; he already knows the answer
and isn't waiting around.  But because the accusations have been
framed as questions, I am left with no way to disprove them.  That's
the nature of an innuendo.

Look, too, at the logic here, or the lack of it.  First of all, it
does not follow logically that a man who cannot compel a woman to
carry his child has no rights as a father.  He claims to "doubt" a
buzz phrase ("father's rights") that, like many phrases of the new
jargon (e.g., "special rights"), has no real definition, just a hazy
set of associations.  To rebut this, one would have to enumerate the
possible definitions.  And note in particular that his rhetoric here
depends on a conflation of two such definitions: rights as a father
as against the rights of a mother (not at issue in the present case
because the mother is not alive) and rights that a father has for being
a living parent (which obviously exist in US law in great abundance).

Having stumbled through all that, I next find myself not-quite-accused
of indifference to "the legal and constitutional aspects of the recent
'rescue' of Elian Gonzalez" -- the scare-quoted "rescue" being my own
word.  This is another technique of the new jargon: create a "message",
call it M, utter a few random "facts" that would seem to support M,
and then immediately start repeating M over and over without mentioning
the facts that support it, as if M were fully established.  The device
works precisely by not laying its cards on the table: one cannot rebut
it without reconstructing the full set of "facts" and patiently taking
them all apart.  As so often, the sophistry takes a few words to say
and hours of labor and logic to refute.  Of course, society does often
come to conclusions whose supporting facts need not be repeated forever
afterward, but it's characteristic of the new jargon to pretend that
a "message" has been established beyond doubt almost instantaneously
after it has been introduced.  If one complains that, for example, the
most common assertion that is used to support the message is actually
false -- in this Tom DeLay's seriously lizard-brained assertion that
"This is a frightening event, that American citizens now can expect
that the executive branch on their own can decide on whether to raid
a home" (AP 4/23/00) -- then you'll get no contrition at all, just
a prefabricated line such as "that doesn't matter; what matters is M"
or else another "fact" that needs to be laboriously checked out.

But at least the business about Elian Gonzalez was connected in some
way to something I said.  The next rhetorical question -- "Or of the
lives lost in Waco and the 'factory' in the Sudan?" -- has no logical
connection at all.  One cannot even begin to interpret this question,
much less answer it, without providing some account of what it is
even doing there.  And clearly it is there because this guy, with
his lizard brain logic, imagines me to be on the Clinton side, so
to speak, and to defend every bad deed and tolerate every lie that
that side has ever told.  (Also notice the weirdness of putting scare
quotes around the word "factory".  I'm not aware of anyone having
denied that the building that Clinton bombed in Sudan was a factory.)
This is the lizard brain at work: it understands only associations.
Every possible bad thing is associated with Clinton, and everyone
who gets themselves associated with Clinton is also transitively
associated with every last one of those bad things.  This is another
purpose of the rhetorical question: the transitive association and
the accusation it implies are not to be rationally investigated;
they are left simply to hang in the air.  It is the work of innuendo:
create a mental association and then stash it on a shelf just beyond
the reach of rational inquiry, in this case by first posing it as a
rhetorical question and then packing and leaving.

  What is the Constitution to you?  Does it matter to you that lacking
  any will or effort on the part of the federal government to enforce
  it, the Constutution is just another piece of paper?  Or that, so
  far, the "oath" to defend and uphold it, at least for the present
  administration, has turned out to be just so much hot air?

This guy has been at the hard stuff.  A primitive kind of mental
electricity is passing through his chain of associations, so that my
reference to "the administration's motives in rescuing a Cuban boy who
was being held by conservatives in Miami" is enough to create a spiral
that leads in a couple of short steps to the conclusion -- another
rhetorical question, another innuendo -- that I have no regard for the
Constitution.  For the lizard brain, a person is either For or Against
a powerful symbol such as the Constitution -- always necessarily an
emotionally primitive extreme with no in-betweens allowed -- and in
this person's lizard brain Clinton is Against the Constitution and
so am I.  It matters for nothing that I have defended the Constitution
against several conservative assaults -- such data cannot even be
processed.  (Other cultivators of the lizard brain have responded to
such things with, "How can you defend that so-and-so?", the innuendo
being that I have thereby chosen to associate myself with him in every
possible way.)

  In your opinion, is there any such thing as "right" or "wrong" in
  any context that will continue beyond the term of a single President?

Now we reach the ground zero of the lizard brain, for which it's
just a few quick steps from a complex issue to the most primitive
dichotomy there is.  To me, the Elian Gonzalez case is the purest
possible example of how primitive the conservative lizard brain has
become.  Here you have your basic hard case: one where several strong
moral imperatives apply equally well and yet contradict one another.
Normal people understand that the world is a complicated place, and
that this sort of conflict is pretty much the norm.  But the lizard
brain believes in absolutes.  And if the absolutes conflict with
one another, the lizard brain is programmed to respond to whichever
arbitrary choice of absolutes the most primitive of media screamers
happens to make.

This is what is so dangerous about the conservative lizard brain: its
judgements are very often absolutely arbitrary.  This arbitrariness
is not an accident.  Conservative society works by breaking down the
rational mind and replacing it with a set of primitive associations
that can be activated selectively by those in power.  People who
might otherwise have been rational, powerful, caring human beings
are reduced to barking dogs who bark at whoever their master tells
them to, all the while shrieking both inwardly and to the world that
they are upholding everything that is good and pure and moral against
everything that is the absolute opposite.  The point is not that
all conservatives are in this state, or that conservative philosophy
is necessarily expressed in the anti-logic of the lizard brain.  The
point, rather, is that a conservative society of orders and classes
requires ordinary people to internalize a system of arbitrariness
and prejudice that cannot be justified, and that such a society
cannot exist without crushing the rational mind.  That's what's going
on right now.  The modern technology of crushing the rational mind
originated with the associationism of public relations, and it has
lately matured in the hands of the professional language-twisters of
the punditry.  We all have lizard brains, and all of us automatically
respond to the strong emotions and vague associations of the new
jargon.  But some people's rational minds have not yet been fully
extinguished, and those people have a responsibility to speak out.

  I wonder.

He wonders.  Except he doesn't, of course.  He has framed the issues
to his satisifaction in the anti-rational haze of the lizard brain, in
which it suffices to issue innuendos and walk away.

  Meanwhile, please arrange for my name and address to be removed from
  your distribution list.  I do not have time to plow through the kind
  of crap you sent me today.

And walk away he does, gone off to abuse someone else.  It used to be
that I responded to obnoxious people said "take me off your mailing
list" with "take yourself off".  Now, having grown older and wiser, I
have a form letter that I send, explaining at length and with vacuous
good cheer how to take themselves off.  This is a trick I learned from
Amazon.com: it not only saves your soul, but it also makes the flamer
much angrier than an angry response would.

Conservatives have the most highly evolved jargon, but they haven't
cornered the market on nastiness.  I also got this message from
someone who evidently works for the state of North Carolina:

  You know, Mr. Pagre, this 'worm design' email may have positive
  ironic and political undertones, show up the establishment's
  hypocrisy and all other sorts of positive things.

  However, adding one more black mark to rack up to Pagans makes your
  Karma that much more problematic.

  Samhain is a holy time of the year.  Why not pick on the Christians?
  Most of the group you are targeting belong to that group.  You've
  just managed to piss off the witches of the world, and there are a
  lot more of them than you think.

Having no tolerance for anything that resembles a threat, I reported
this message to the sender's site administrator.

Having tired of paying new-book prices on Amazon.com, I've been using
online comparison-shopping mechanisms for used bookstores.  The one
that works best for me is .  Of course it's
mostly older and better-known books that are available cheaply this
way, but I've gotten about forty books this way at an average price
well under $10.  Just to give you an idea, here is what I've bought:

  Peter Ackroyd, The Life of Thomas More, Doubleday, 1998.

  Armen A. Alchian, Economic Forces at Work, Liberty Press, 1977.

  Carl L. Becker, The Heavenly City of the Eighteenth Century
  Philosophers, Yale University Press, 1932.

  Frederick C. Beiser, The Sovereignty of Reason: The Defense of
  Rationality in the Early English Enlightenment, Princeton University
  Press, 1996.

  Robert H. Bork, The Antitrust Paradox: A Policy at War With Itself,
  Basic Books, 1978.

  Taylor Branch, Parting the Waters: America in the King Years,
  1954-63, Simon and Schuster, 1988.

  Owen Chadwick, The Secularization of the European Mind in the
  Nineteenth Century: The Gifford Lectures in the University of
  Edinburgh for 1973-4, Cambridge University Press, 1975.

  Alfred D. Chandler, Jr., The Visible Hand: The Managerial Revolution
  in American Business, Harvard University Press, 1977.

  Alfred D. Chandler, Jr., Scale and Scope: The Dynamics of Industrial
  Capitalism, Harvard University Press, 1990.

  John R. Commons, Myself, University of Wisconsin Press, 1963.

  Ulrich Conrads, Programs and Manifestoes on 20th-Century
  Architecture, translated by Michael Bullock, MIT Press, 1970.

  Edward G. Corrigan and Pearl-Ellen Gordon, eds, The Mind Object:
  Precocity and Pathology of Self-Sufficiency, Aronson, 1995.

  Claude S. Fischer, America Calling: A Social History of the
  Telephone to 1940, University of California Press, 1992.

  Anthony Giddens, The Constitution of Society: Outline of the Theory
  of Structuration, University of California Press, 1984.

  Louis Hartz, The Liberal Tradition in America: An Interpretation
  of American Political Thought Since the Revolution, Harcourt Brace,
  1955.

  David Held, Democracy and the Global Order: From the Modern State to
  Cosmopolitan Governance, Stanford University Press, 1995.

  Richard Hofstadter, Anti-Intellectualism in American Life, Knopf,
  1963.

  Richard Hofstadter, The Paranoid Style in American Politics, and
  Other Essays, Knopf, 1965.

  Arthur R. Hogue, Origins of the Common Law, Indiana University
  Press, 1966.

  John Keane, Tom Paine: A Political Life, Little, Brown, 1995.

  Russell Kirk, The Roots of American Order, Open Court, 1974.

  Jack Knight, Institutions and Social Conflict, Cambridge University
  Press, 1992.

  Paul Krugman, The Accidental Theorist: And Other Dispatches from the
  Dismal Science, Norton, 1998.

  Arthur O. Lovejoy, The Great Chain of Being: A Study of the History
  of an Idea, Harvard University Press, 1936.

  Robert Markley, Fallen Languages: Crises of Representation in
  Newtonian England, 1660-1740, Cornell University Press, 1993.

  Carolyn Merchant, The Death of Nature: Women, Ecology, and the
  Scientific Revolution, Harper and Row, 1980.

  Rene Moses-Hrushovski, Deployment: Hiding Behind Power Struggles as
  a Character Defense, Aronson, 1994.

  Geoff Mulgan, Connexity: How to Live in a Connected World, Harvard
  Business School Press, 1998.

  Douglass C. North and Robert Paul Thomas, The Rise of the Western
  World: A New Economic History, Cambridge University Press, 1973.

  Douglass C. North, The Economic Growth of the United States,
  1790-1860, Prentice-Hall, 1961.

  Robert S. Peck, ed, To Govern a Changing Society: Constitutionalism
  and the Challenge of New Technology, Smithsonian Institution Press,
  1990.

  Virginia Postrel, The Future and Its Enemies: The Growing Conflict
  over Creativity, Enterprise, and Progress, Free Press, 1998.

  Andras Sajo, Limiting Government: An Introduction to
  Constitutionalism, Central European University Press, 1999.

  Charles Sellers, The Market Revolution: Jacksonian America,
  1815-1846, Oxford University Press, 1991.

  Darren Staloff, The Making of an American Thinking Class:
  Intellectuals and Intelligentsia in Puritan Massachusetts, Oxford
  University Press, 1998.

  Cass R. Sunstein, After the Rights Revolution: Reconceiving the
  Regulatory State, Harvard University Press, 1990.

  Karen Kissel Wegela, How to Be a Help Instead of a Nuisance:
  Practical Approaches to Giving Support, Service, and Encouragement
  to Others, Shambhala, 1996.

I realized that I've turned into a book collector, which is a scary
thought.  That's something that middle-aged college professors do.
I suppose I'll write a deserving East European library into my will.

Some URL's.

Emerging Antitrust Issues in Electronic Commerce
http://www.ftc.gov/speeches/other/ecommerce.htm

Red Escolar Linux
http://redesc.linux.org.mx/

Quality of Service: Fact or Fiction?
http://www.cisco.com/warp/public/759/ipj_3-1/ipj_3-1_qos.html

venture capitalists' response to the stock market crash
http://www.forbes.com/forbes/00/0515/6511182a.htm

FCC Opens Door for New Wireless Technology
http://news.cnet.com/news/0-1004-200-1857730.html

Research Council Calls for More Study of Large Information Systems
http://chronicle.com/free/2000/05/2000051101t.htm

Internet Explorer "Open Cookie Jar"
http://www.peacefire.org/security/iecookies/
http://slashdot.org/articles/00/05/11/173257.shtml

Digital Storytelling
http://tech-head.com/dstory.htm

Microsoft's proposed antitrust remedy
http://news.cnet.com/News/Pages/Special/Microsoft/issue_of_remedy.html

Rethinking Antitrust Policies for the New Economy
http://www.usdoj.gov/atr/public/speeches/4707.htm

for Metallica fans with guilty consciences
http://www.paylars.com/

Center for Digital Discourse and Culture
http://www.cddc.vt.edu/

Biosphere Data Project
http://sims.berkeley.edu/biosphere/

Consumer Financial Privacy Act
http://www.epic.org/privacy/financial/HR4380.html

Switches Raise Prospects for Tiny Technology
http://www.nytimes.com/library/tech/00/05/biztech/articles/08mems.html

So Far, Big Brother Isn't Big Business
http://www.nytimes.com/library/financial/personal/050700personal-privacy.html

Backbone Bottlenecks Burst Broadband Bubble
http://www.zdnet.com/zdnn/stories/news/0,4586,2550556,00.html

end
```