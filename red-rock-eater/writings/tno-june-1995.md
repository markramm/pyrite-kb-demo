---
id: tno-june-1995
title: "TNO June 1995"
type: writing
writing_type: paper
date: 1995-06-07
url: "https://pages.gseis.ucla.edu/faculty/agre/tno/june-1995.html"
coauthors: []
key_concepts: []
importance: 5
research_status: stub
tags:
  - paper
  - auto-imported
---

## Source

Automatically imported from: https://pages.gseis.ucla.edu/faculty/agre/tno/june-1995.html

## Content

```
--------------------------------------------------------------------

                T H E  N E T W O R K  O B S E R V E R

  VOLUME 2, NUMBER 6                                     JUNE 1995

--------------------------------------------------------------------

  This month: Reforming computer science
              The Exon bill -- the day after
              Computing and the people
              Stealth spam
              Corporate privacy policies

--------------------------------------------------------------------

  Welcome to TNO 2(6).

  This issue of TNO includes three short articles by the editor.
  The first one prescribes a change in attitude for the field of
  computer science, from automating other people's lives to working
  with the people who have deep knowledge of the particular worlds
  where computers are used.  The second reflects on the conflict
  between Republicans over the Communications Decency Act, which
  may be a model for many other such conflicts among conservatives
  down the road.  And the third offers some first thoughts on the
  sense in which computer technology is increasingly "popular" --
  that is, shaped by the collective action of ordinary people for
  their own purposes.  Plus two short notes: one on electronic junk
  mail and another on conspiracy theories about the Oklahoma City
  bombing.

  This month's wish list gathers a batch of small items that have
  been bothering me, mostly about books and magazines.  I've also
  included a review of Jeff Smith's book "Managing Privacy" that
  Wired magazine wouldn't print.

  David Henkel-Wallace <gumby@cygnus.com> (who doubts that he's
  the first one to have noticed this) points out that "information
  superhighway" is an anagram for "New utopia?  Horrifying sham."

  A footnote.  Reporters have to stop confusing the Internet with
  Usenet and acting as if the Internet were coextensive with the
  public discussion groups that reporters can easily listen in on.
  Both of these problems are evident in the following article:

    Julie Chao, Internet pioneers abandon world they created,
    Wall Street Journal, 7 June 1995, page B1.

  It's an article about physicists who have stopped reading the
  Usenet discussion groups on physics because they're full of
  uninformed speculation and polemics.  Gee whiz -- I'm surprised
  that the physicists didn't forget those groups a decade ago.
  But the idea of physicists literally abandoning the Internet
  is like -- like what? -- like the idea of Chicagoans abandoning
  sports.  Who, for example, invented the Web?  Let's encourage
  reporters to look at the real uses of the Internet in scientific
  communities -- and every other kind of community.  It's just
  that doing so requires a little more effort than listening in
  on a news group.

--------------------------------------------------------------------

  Computer science is dead.

  I have a doctoral degree in computer science, but I now teach
  in a social sciences department.  Though I would like to think
  I'm starting a trend, the evidence is not strong.  Even so, the
  evidence *is* strong that the academic discipline of computer
  science is in trouble.  I was first alerted to this fact a few
  years ago when my officemate from graduate school quit a top-rank
  computer science faculty position to work for Microsoft because
  he wanted to be where the action is.  He's right: the agenda for
  computer science research has shifted from academia to industry.

  But the problem runs deeper than that, and I think that computer
  science needs to fundamentally reinvent itself to avoid shrinking
  into irrelevance.  Here's the problem: we are told that computer
  technology is being continually revolutionized, but it doesn't
  really work that way.  Instead, computer science has historically
  laid down one layer after another of settled art, little of which
  must be greatly revised later on.  Lots of people got tenure for
  designing parsers, for example, and now we know how to do that.
  An earthquake did occur at the fault line between processor
  design and compiler design in the 1980's, but that has settled
  down.  Programming language design was a difficult matter once,
  but now it isn't, and the market has decided that it's satisfied
  with C and C++ anyway.  There's no accounting for taste, but
  there it is.  (For a more general analysis see Andrew Friedman's
  brilliant historical book "Computer Systems Development", which
  I recommended in TNO 1(9).  See also Peter Denning's recent
  articles about the future of the engineering field generally.)

  So what happens next?  The technical methods of computing are
  like a lake that is silting: once somebody finally figures out
  how to make distributed operating systems, it'll be all over.
  The most likely exception is in the theory of computation -- the
  mathematical foundations of the field, where really interesting
  research on "interactive proof" methods will probably bring
  us a lot more useful stuff from the same place that public-key
  cryptography came from.  Plenty of other computer research
  will remain to be done, of course, but the emphasis may shift
  elsewhere.  No longer will the world need hordes of computer
  scientists who know a little about medicine or engineering or
  business; instead, it will need hordes of doctors and engineers
  and business people who know a little about computers and a great
  deal about a particular world where computers are used.

  The field of computer science can save itself, though, if it
  gets a new attitude.  It has to stop looking at the whole world
  as a bunch of technology-driven "application domains" and instead
  develop a spirit of partnership with people who know substantive
  things -- things about organizations, about managing information,
  about sickness and health, about democracy.  Although numerous
  computer people are sympathetic to such an approach, many of the
  basic concepts and methods of computer science make it difficult
  to put into practice.  One obstacle is the field's understanding
  of formalization: to implement something on a computer, you have
  to translate it into mathematical terms that can be coded.  But
  the resulting formalisms rarely correspond to the way that users
  think about things.  Furthermore, computer scientists know almost
  nothing about how computer use fits into the lives and activity
  systems of the people who use them.  Instead, generations of
  systems analysts have used models that derive from industrial
  automation -- rather than from the intention of providing support
  for skilled people with complex lives.  The approach, whether
  explicitly or implicitly, is not "we will work with you and help
  you build tools" but "we will represent you and replace you".

  But an attitude of symmetrical partnership, necessary as it is,
  will not suffice in itself.  We also need what I call "bridging
  concepts" -- that is, medium-sized concepts that make it easy to
  move back and forth between serious ideas about technology and
  serious ideas about the social worlds where technology is used.
  Listening to the speakers at the conference on Society and the
  Future of Computing that we recently organized in Colorado, and
  reflecting on other valuable things I've read lately, I managed
  to articulate ten candidates for these bridging concepts, which
  I'll present here in the form of imperatives for the field of
  computer science:

    (1) Designers must rethink the physical forms of interaction
    with computers.

  At the conference, Joy Mountford from Interval described some of
  the ways that professional designers were doing just this.  The
  existing physical forms of interaction with computers (keyboards
  and screens) are alright for some purposes, but for many others
  they lead to hand and eye injuries.  Though I am hardly the most
  overworked computer user in the world, I had prescription glasses
  made (out of my own pocket) to help correct an atrophy in the eye
  muscles that shift focus from near to far.  Computer scientists
  don't think much about the physical form of interaction with
  computers because, by and large, they imaginatively identify with
  the systems themselves rather than with the lives of the people
  using them.  Research on interfaces for people with disabilities
  is helping to stimulate thinking about alternatives, but much
  more remains to be done for everyone else.

    (2) Systems must fit into users' diverse ways of life.

  People from different backgrounds -- cultures, professions,
  and so on -- live different lives, and so it seems likely that
  they will need different computers.  But how do computers and
  ways of life fit together?  A focus on individual users' thought
  processes does not suffice to answer the question; indeed, it
  can contribute to weird stereotypes about the different thought
  styles or learning rates of different groups of people.  What
  about people who must switch back and forth between tasks on
  their computer and tasks on other machines?  What about people
  who share a computer with several others?  What about people
  who maintain relationships with others through several different
  media, including both computer and non-computer media?  How do
  different cultures organize the teaching and learning of family
  members?  And so on.  A major problem is that nobody can get
  tenure in a computer science department, at least in the United
  States, for investigating such questions.  This needs to change.

    (3) Workplace computing must provide tools for people, not
    automation that replaces people.

  Much of computer science derives historically from industrial
  automation, and the idea that computers are meant to replace
  people is more deeply ingrained in the field's methods and
  concepts than many computer scientists want to admit.  The big
  news, though, is that the old assumptions behind automation no
  longer hold.  So many activities have become automated by now
  that today's jobs require highly skilled workers to keep track
  of complex processes while participating in constant change.
  Interface designers like Ben Shneiderman have emphasized this
  shift from the technical side, while industrial researchers
  like Patricia Sachs and labor researchers like Joel Yudken
  are remarkably unanimous about the point as well.  Computer
  scientists often do make representations of people's work, but
  these representations have largely been preludes to software
  specs -- to automation.  The hard problem, which new research
  is only beginning to address, is how such representations can
  support work by supporting the thinking and group effort of the
  people who are doing the work.

    (4) Interface design must move beyond a focus on users to a
    focus on learning communities.

  Even when they live or work alone, people are very much bound
  up in social networks.  As Jonathan Grudin has pointed out,
  "the user" is a dangerous fiction.  This fiction did have some
  truth to the extent that computer-using jobs were rationalized,
  using the "one best way" prescribed by time and motion experts.
  But in the new world, the emphasis is shifting to continual
  learning.  The best learning is that which takes place through
  dealing with actual problems.  People who work together routinely
  teach and learn informally, for example, by telling stories
  about their experiences.  How can technology support this kind of
  informal learning in communities?  Roy Pea and Elliot Soloway are
  studying this question in classroom settings, and Julian Orr and
  others are studying it in workplace settings.  Computer science,
  though, has a hard time conceiving of social relationships and
  processes that are not directly captured by computers.  This will
  need to change.

    (5) The new technologies of privacy protection must replace
    system designers' habit of tracking human activities in
    ever-greater detail.

  Public-key cryptography and the whole world of related emerging
  privacy technologies have, as Marc Rotenberg points out, changed
  the way we think about technology itself.  Many theorists have
  associated technology with social oppression, so that critics of
  oppression have found themselves positioned as anti-technology.
  Now the tables are turned: the bureaucracies that resist strong
  cryptography are the real anti-technologists.  But the field
  of computer science has plenty of catching up to do as well.
  For the most part, the use of computers to invade privacy
  doesn't result from a conscious decision to invade privacy.
  The situation is actually much worse, since the most basic step
  in system design is to choose which entities in the world to
  represent (people, vehicles, packages, transactions, etc) and
  to create identifiers for them.  The resulting records end up in
  databases that then get reused for secondary purposes and merged
  with other databases.  But public-key cryptography lets us start
  over by designing in privacy protection from the start.  This
  won't be easy, and it will require much more innovation so that
  designers can produce systems that collect precisely the minimum
  amount of information necessary to serve a given function.  But
  I think it can be done.

    (6) Technologists must respect and support the extensive
    expertise of information management professionals.

  ... that is to say, librarians.  It is embarrassing to watch
  computer scientists reinvent indexing and retrieval technologies
  that librarians discarded in the 1950's.  I don't think most
  computer scientists have realized that, as Christine Borgman and
  others have persuasively argued, managing large collections of
  information is a specialized skill that is quite independent of
  the (equally valuable) skills of computer people.  The emergence
  of digital library research may redress the problem; the big
  question is whether computer scientists will pay attention and
  give due respect, or whether this research will move into other
  fields and other departments.

    (7) As distributed information technology is used to reduce
    transactions and coordination costs, it must not undermine
    workers and their families.

  Electronic commerce promises to interconnect buyers' and sellers'
  computers, thereby removing a lot of useless paperwork from the
  world's business operations.  As Rolf Wigand points out, one
  effect of this innovation is to reduce transaction costs: the
  costs of making contracts in the market.  This is good when it
  brings lower prices at the consumer's end of the whole pipeline.
  But economic theory predicts that reduced transaction costs will
  have other effects.  One of these, potentially, is an increase
  in contingent work: that is, work that people do on a "flexible"
  short-term contract basis.  This system is great for people who
  want flexibility in their working lives.  But it's lousy for
  people who need stability -- most especially people with kids.
  Children need security, and we should worry whether they can get
  it in a world where parents must change jobs every few months,
  weeks, or days.  Distributed computing also reduces coordination
  costs, which are the costs of holding a far-flung business
  operation together.  To some extent this effect counteracts the
  reduction in transaction costs.  But it also gives centralized
  management much better tools for controlling work at a distance.
  Computer people should become aware of how these forces play out
  in practice, and they should investigate how their systems might
  help increase efficiency without also increasing the control and
  instability in people's lives.

    (8) Technical standards-setting processes must be opened to
    a broader range of stakeholders --- long before the standards
    become irreversibly entrenched in the market.

  Technological markets need standards so that products can
  work together and so that people can know what they are buying.
  Standards have enormous consequences, since it is easy for a
  standard to become entrenched in the market without necessarily
  being compatible with the best technical solution or the most
  humane social arrangements.  Standards are still largely set
  by remarkably informal voluntary arrangements.  Plenty of
  power politics is often going on behind the scenes, of course,
  but standards-setting processes still seem like one venue where
  social concerns can be explored before designs become faits
  accomplis.  It is possible, for example, that many standards can
  be influenced toward privacy protection -- simply because nobody
  had been thinking about privacy before, or because nobody had
  been adequately informed about technical options for protecting
  privacy.  Who, we might ask, are the full range of stakeholders
  in technical standards-setting, and what would it take to get
  them a place at the table?  Some plane tickets would help, and
  regular reports about standards activities on the Internet would
  help too, but substantive dialog is needed as well.

    (9) Citizens and professionals alike must become aware of
    the ways that information infrastructure architectures either
    support or inhibit democratic participation.

  Computer people have been talking about democracy a lot lately,
  influenced in part by organizations like CPSR and EFF who have
  articulated connections between information infrastructure and
  democratic participation.  The Clinton administration has done
  little of substance, but their NII rhetoric has stimulated some
  remarkably broad-based discussion of telecommunications policy
  issues.  At the top of the list is the distinction between a
  symmetrical switched architecture, in which anyone can produce
  their own content, and an asymmetrical architecture like the
  US regional phone companies want to use to deliver "interactive"
  video services.  Of course, only a few percent of the population
  understand this distinction.  But that's a good start, and more
  can be done to spread the word.

    (10) Information technologists must recognize that the success
    of democracy depends most crucially on citizens' experience of
    empowerment and skills of organizing.

  All this talk about democracy, though, can get shallow.  Langdon
  Winner has pointed out the sometimes facile connections between
  information, knowledge, power, and democracy that often make
  the issues seem easier than they are.  In the end, what really
  matters is whether people feel empowered to organize themselves
  to exert some control over their own lives.  The best technology
  you can possibly build is useless unless people have these social
  and political skills and feel that it would make some difference
  to try using them.  Perhaps learning how to use the net can be
  an occasion to reinvent the skills of democracy, and perhaps
  the skills of democracy will help us understand what kinds of
  information infrastructure we should be building next.

--------------------------------------------------------------------

  The conservative culture wars.

  After the Internet community and civil libertarians spent months
  busting their butts trying to defeat the Communications Decency
  Act, Newt Gingrich just about killed it with one breath.  Never
  mind that the bill was introduced by a retiring Democrat; the
  real political action around the CDA was among conservatives.
  By threatening to shut down the whole Infobahn in the name of
  morality, the Act precisely diagnosed a huge division within the
  conservative movement.

  The conservatives have assembled a formidable coalition around
  an anti-government agenda.  But simmering beneath this relatively
  smooth surface is a cultural division between authoritarians
  and libertarians.  Once the conservative coalition destroys the
  liberal establishment -- for example by sending the auditors from
  hell after every liberal non-profit organization that ever got a
  dime from the government -- then American politics will turn into
  a subterranean battle between these two forces.  Each side will
  call itself conservative, but they will mean different things
  by the term.  Most corporate leaders, for example, are economic
  conservatives and cultural libertarians who want opportunities
  for their daughters and worry that nationalist xenophobia will
  interfere with the country's participation in the global economy.
  Many of them are concerned that Pat Robertson and his followers
  might actually believe the things he writes in his books.

  Likewise, the ideological libertarians who define the culture
  of the high tech world are generally focused on entrepreneurship,
  contemptuous of government economic intervention, supportive
  of gay rights, and more interested in freedom for kids than
  in patriarchal family values.  The problem, of course, is that
  these folks don't have the votes.  Libertarian think tanks have
  unprecedented visibility, but that just means that their ideas
  are selectively harvested in support of a culturally conservative
  agenda.  Privatization, yes -- but forget about legalizing drugs.
  The people who run the Republican Party -- including the pundits
  and theorists and the conservative foundations who fund them --
  are well aware that conservative Christians control dozens of
  state Republican party organizations, and they take great care
  to make the ideology appeal to them.  This leads to some strange
  results -- for example, the libertarian conservative magazine
  The National Review has run articles fretting over university
  radicals' antipathy to science *and* explaining the threat to
  society posed by the theory of evolution.

  The Exon bill provided another such result.  Its main grassroots
  support came from the Christian Coalition, whose lobbyists were
  squarely focused on pedophiles "stalking" children on the net.
  Now, I happen to believe that pedophiles are real and dangerous.
  But did the Christian Coalition people understand that the Exon
  bill would have basically no effect against pedophiles, who are
  surely smart enough to confine themselves to innocent-sounding
  interactions in cyberspace?  I don't know.  While the Senate
  debate was going on, it was certainly frustrating to have people
  (small numbers of them to be sure) respond to the Voters' Telecom
  Watch alerts on the CDA with messages like, "So you're against
  decency?".  On the other hand, why did it take the Exon bill for
  the major net providers to address people's concerns by getting
  visible about their efforts to implement real technical solutions
  to the potential problems?  This issue will be back.

--------------------------------------------------------------------

  Computing as a popular technology.

  Computing, perhaps more than any other technology in history,
  is a popular technology.  By "popular" I don't mean "popular"
  as in "so-and-so is a popular movie star".  Instead I mean the
  original sense of the word -- "of the people".  Although we think
  of computers as impossibly esoteric, the fact is that ordinary
  people have begun to take hold of computing at a tremendous rate.
  Computing is a highly plastic technology, meaning that its forms
  can be changed and adapted endlessly, and it is time to start
  tracing all the ways in which people taken hold of computing
  for their own purposes and have then had an influence on their
  design.  Here are a few:

   * User groups.  People are getting together in groups for mutual
  assistance, exchanging software, grouching about bugs, helping
  one another find good deals and avoid bad deals, and so forth.
  User groups are becoming powerful distribution channels in the
  market, like the buyers' cooperatives that have been an important
  part of community organizing forever.

   * Resistance.  People can put up a fuss when computers are used
  to invade their privacy or otherwise offend them.  Sometimes this
  resistance is organized, as when telephone workers have tried to
  reduce surveillance of their work by managers.  Sometimes it is
  spontaneous and unorganized, as when people avoid entering data
  into machines, use the machines in a superficial manner, modify
  the programming to suit them, and so on.

   * Free software.  Lots of free software is circulating in the
  world, much of it written by people who just want to share.  A
  program circulated on the Internet can be used by many thousands
  of people in short order, and a whole volunteer distribution
  system has arisen.

   * Market choice.  As individual consumers, people can buy stuff
  that's good and refuse to buy stuff that's lousy.  To do this, of
  course, they need to talk to one another.  As computer knowledge
  diffuses through communities and social networks, markets will
  have to respond better to people's needs.  Informed people can
  also make a difference in their workplaces by politicking for the
  purchase of good systems that support productivity rather than
  lousy ones that drive people crazy.

   * Guerilla networking.  Fidonet began as a political project
  to provide cheap digital communications to everyone.  Regardless
  of what you think of its quality control, Usenet is very much a
  democratic "underground".  Hundreds of social movements across
  the political spectrum are getting on the net, supported by
  specialized organizations such as the Institute for Global
  Communications.  Thousands and thousands of individual computer
  enthusiasts have set up BBS's in their communities, often with
  the intention of serving particular interest groups such as SF
  readers or labor unionists.

   * Interest-group organizing.  The 1994 Communications Act, which
  failed in the last minutes of that Congress despite bipartisan
  support, was shaped in some ways by a remarkably broad alliance
  of public interest groups, many of which coordinated their
  efforts under the umbrella of the Telecommunications Policy
  Roundtable.  Similar projects have begun regionally.  Other
  groups, such as the Electronic Privacy Information Center and
  Voter's Telecom Watch, have fought legislation that would have
  antidemocratic effects on information infrastructure, and a wide
  variety of people have responded to their calls for political
  action on these issues.

   * Community networking.  As I reported in TNO 2(5), people
  building computer networks to support their communities are
  rapidly learning what it takes to actually serve people with
  technology.  Their experience will increasingly feed back into
  the design of software to support communities.

  I think this is a pretty impressive list.  Many others will
  disagree, either because they think that technology charges
  forward according to its own internal logic or because they
  think that the whole world is totally dominated by corporations.
  There's a grain of truth in each of these assertions, of course,
  but if we believe them then we might as well give up now.  It's
  important to believe that people can act together to take some
  control over their lives, not only because it's a necessary
  belief to stay sane -- but also because it's true.

--------------------------------------------------------------------

  Stealth spam.

  Lately I've been noticing a new variety of junk mail on the net,
  much more sophisticated than the noisy Canter-and-Siegel variety
  and much more worrisome for that reason.  I call this new junk
  mail "stealth spam".  It's e-mail that seems to be addressed
  to me as an individual, but which could equally well have been
  addressed to hundreds or thousands of other people.  It achieves
  this effect through vagueness: "we've heard your name as a good
  person to talk to", "I think you might find this interesting",
  and so on.  The big problem with these messages is that it takes
  real work to determine whether they are junk or not, and they
  increase the risk that actual/real/serious messages might get
  mistaken for junk.  This has happened to me at least once so far.
  And these "stealth spam" messages are not all from obscure shady
  operators.  At least one was sent by a salesman from Silicon
  Graphics -- a salesman who will rue the day he heard about the
  Internet if he bothers me again.

  I've seen some other variants.  Someone sent a message to the
  Risks Digest, for example, recounting the good experience he had
  had with a negative ion machine.  Later on, someone else sent a
  message to Risks explaining that the first message was identical
  to others that had been posted to many other lists, and that the
  sender in fact sells ion machines.  The new spin was that these
  messages weren't sent all at once, but were rather dribbled out
  to one list after another very slowly.

  This phenomenon has set me thinking about genres.  Paper junk
  mail is usually easy to distinguish from paper non-junk mail.
  Why is this?  One reason is that it's very hard to make paper
  junk mail truly indistinguishable from paper non-junk mail.  So
  in order to make sure their mail gets read and not tossed out
  straightaway, the paper junk mail people have evolved a highly
  distinctive genre of document, based on elaborate theories and
  much experimentation, that mutates the traditional business letter
  genre with special uses of color and formatting and postscripts
  and inserts -- and even those yellow sticky notes whose generic
  name is a trademark.

  Why doesn't this happen with electronic junk mail?  Maybe it's
  because, courtesy of the wonder of digital technology, you
  can make electronic junk mail that's indistinguishable from
  electronic non-junk mail.  This is a real problem.

--------------------------------------------------------------------

  One more note on the Oklahoma City bombing.

  Over the few weeks, I am told, right-wing activists and
  journalists will unveil their fully matured conspiracy theories
  about the Oklahoma City bombing.  The original theories were
  pretty wacky, but the latest ones are starting to edge into the
  realm of plausibility.

  Here's a composite: The BATF, and maybe the FBI as well, wanting
  to create terrorist threats to justify their budgets, decided to
  frame someone from the militia movement.  So they got some fringe
  characters and fixed them up with provocateurs who pretty much
  did all the work.  The plan was to arrest the guy(s) on the site
  early in the morning before the bomb blew up.  But something went
  wrong; the guy(s) arrived late and actually managed to carry out
  the plan.  The bomb, furthermore, created much more damage than
  it had any right to.  The reason for this is that a bunch of
  explosives were stored in the basement of the building, having
  been kept there by BATF people who were practicing (somehow --
  this bit isn't clear to me) for the operation.  These explosives
  were set off by the original explosion and were responsible for
  much of the structural damage to the building.

  Okay, so that's the theory.  At least it's one theory; I'm sure
  that I will get a bunch of messages elaborating or changing or
  criticizing this version one way or another.  Aside from the mass
  of circumstantial evidence, all of which may be true or not true
  or covered up or not covered up, this theory is within the realm
  of plausibility because things like this have happened before.
  You can go back as far in history as you like and pick your
  favorite examples.  Take, for instance, the Earth First! people
  who were arrested getting set to blow up an electrical pylon;
  those folks were pretty thoroughly set up by a government agent.
  (That does not in itself mean that they were not guilty of a
  crime, but it does change the picture.)  Of course, right-wing
  activists are not likely to appeal to this precedent, or to the
  whole long history of government sabotage and harassment against
  left-wing activists, violent and nonviolent alike.  Instead,
  they will frame the conspiracy in terms of their theory that the
  United States is actually a socialist dictatorship in which the
  Constitution has long been nullified.  And they will get a lot
  of deliberate but indirect cover for this view from mainstream
  politicians and pundits.  At least that's what I predict, based
  on what I've heard on the net.  What if their facts are even half
  right?

--------------------------------------------------------------------

  Wish list.

  This month's wishes are small things that have been bothering me
  forever.  It's just possible that they have not been done because
  nobody ever thought of them.

  On-line library catalogs are great.  I cannot imagine how anybody
  did research without them.  Their biggest hole, in my experience,
  is that they do not include tables of contents for edited volumes
  or anthologies.  I can issue commands to search for journal
  articles by a given author, but I would also like to search for
  book chapters by that author.

  I also devoutly wish that I had an easy way to obtain all of
  the published reviews of a given book -- or at least a list of
  citations to all of the reviews.  To do this, of course, it would
  be necessary for on-line periodical catalogs to know what book
  is actually being reviewed in a given article.  In practice, the
  name of the book being reviewed simply appears in the title of
  the review, without the machine having an actual pointer to the
  book's own catalog entry.

  Ever tried to cancel a subscription to a magazine?  Why does it
  take six to eight weeks to change your address?  Magazines do not
  care much about their subscription operations, and I'm convinced
  that they outsource them to the lowest fly-by-night bidder no
  matter how poor the service.  After all, they've got your money,
  so why pay any attention to you afterward?  We'd all like to
  think that this is a short-sighted strategy, but maybe the market
  just isn't interested in fixing this particular problem.  In case
  it is, though, maybe on-line services are part of the solution.
  It would be nice to check on my magazine subscriptions through a
  nice GUI interface; this approach may even increase single-copy
  sales.  Of course, there's the security problem ...

  I read a lot of newspapers and magazines, and often I wish to
  save a pointer to a particular article for future reference.  If
  all newspapers and magazines are someday published in electronic
  form then this will be easy, though a lot of other things will
  become hard.  As it is, I have to save the publication, throw it
  in a box in my office, and then pay somebody to make photocopies
  that I can use later in my research or for class readers.  This
  is cumbersome and expensive, so I only do it when I'm pretty
  sure I want to use the article again.  Another approach would be
  for each article to carry, perhaps above the title somewhere, a
  discreet barcode-like set of dots or lines that I could scan with
  a simple scanner that could be about the size of two credit cards
  back-to-back.  Then periodically I could aim the scanner at my
  personal computer and press a button, whereupon it would download
  all the codes it had scanned recently through an infrared LED.
  My computer would then look these codes up in a general database
  over the net and tell me how much it would cost to have a copy of
  each article neatly printed up and mailed to me.

  It bothers me when someone takes a perfectly good paper directory
  (phone book, Books in Print, parts catalog, etc) and puts it on a
  computer with one of those low-tech search engines where you have
  to type in some of the fields, and then it offers to show you a
  few of the entries in the database.  Unless you frequently need
  to do sideways searches (like looking people up by their phone
  numbers), this is unbelievably worse than the interface you
  get with the paper version, which lets you scan whole pages of
  entries quickly.  Why can't the computer-based interfaces look
  more like the paper interface?  Why can't we get whole pages,
  nicely formatted, to appear on our screens, easily flippable
  forward and backward?  Maybe we couldn't get that when the
  computers all had 286-grade processors, but starting soon even
  your basic Nintendo will have more than enough computing power
  to get us back to the decent interface we started out with.  I'm
  hardly the first person to complain about this, but maybe now is
  the time to really raise heck about it.

  I am so accustomed to e-mail that I often think of the telephone
  as a variant of e-mail rather than the other way around.  (Stop
  laughing.  I'll bet you do this too.)  In particular, I often
  wish that I could call someone and get their voicemail even if
  they are present and able to answer the phone.  Why?  Because
  sometimes the message I have for them is not urgent and requires
  no dialogue, so that it's better for the recipient to hear it
  when they're ready to get messages.  As it is, when someone picks
  up the phone we have to do a little negotiation about whether
  my message is more important than whatever my phone call has
  interrupted.  So it would be nice if I could push an extra button
  on the phone, or dial an easy prefix (one that's written down on
  a simple, clear reference card that's posted right on the phone)
  that will ensure that I get the voicemail instead of the person.

--------------------------------------------------------------------

  This month's recommendations.

  Carl F. Cargill, Information Technology Standards: Theory,
  Process, and Organizations, Digital Press, 1989.  It seems to me
  that the future of the networked world depends to a great extent
  on the market dynamics of technical standards.  Once a standard
  becomes entrenched in the marketplace, it's very hard to change.
  Just look at ASCII, for example.  The market needs standards
  because products have to work together.  But entrenched standards
  can also create monopolies, retard technical progress, foreclose
  technical possibilities, facilitate invasions of privacy, or
  limit the options available for participation in society.  So
  I encourage everyone to become aware of information technology
  standards.  This is the basic book on the subject.  It's not
  the most inherently thrilling topic in the world, but the book is
  written in a clear, simple fashion that is rooted in the author's
  experience.  It has no references, though, which is irritating.
  Other interesting authors on the strange economics of standards
  are Paul David and Brian Arthur.

  Richard Saul Wurman, Access Guides.  Yet more proof, if any were
  needed, that architects are cooler than normal people.  Although
  they have started to drift back toward the breathless tone of
  their competitors in recent years, the Access guides are still
  the only "tour guides" that you would want for the city you live
  in.  Their claim to fame is that they are organized spatially,
  so that you can open them to the block you're currently standing
  on and find out what's there.  They include lots of architectural
  information and generally reliable restaurant and shop reviews.
  They aren't cheap, but I keep finding that each volume pays for
  itself the first day I use it.  Think of it as the paper version
  of "augmented reality"; the fantasy is that someday these guides
  will be software for your heads-up display and the whole world
  will be annotated the way it is for the Terminator.

  Maritza Pick, How To Save Your Neighborhood: The Sierra Club
  Guide to Community Organizing, San Francisco: Sierra Club Books,
  1993.  This is the best all-around practical guide to community
  organizing that I have seen lately.  What would it be like to
  apply its lessons to an Internet community?  Or to organize your
  geographic community over telecommunications policy issues like
  cable television regulation, library facilities and hours, or
  local government information?

--------------------------------------------------------------------

  Review of Jeff Smith's "Managing Privacy: Information Technology
  and Corporate America", University of North Carolina Press, 1994.

  [Despite having published several of my book reviews, Wired
  magazine wouldn't publish this one.  I gather that the phrase
  "serious and thoughtful analysis of corporate policy-making"
  didn't push the right buttons for them.]

  "Managing Privacy" is a serious and thoughtful analysis of
  corporate policy-making about privacy.  Based on interviews
  with managers and observers in several pseudonymous American
  banking and insurance firms, its centerpiece is a simple but
  valuable model of organizational responses to privacy issues.

  Smith argues that the firms he investigated have generally
  dealt with privacy issues in an improvised, decentralized, and
  inconsistent way until provoked into action by some external
  threat -- usually the possibility of new regulatory legislation.
  Lacking such a threat, he observes that individual managers
  have little incentive to explore responsible privacy policies.

  He pulls few punches in describing the inadequate approaches to
  privacy at most of the companies.  Few have adequate policies
  to protect sensitive personal information from being used
  improperly.  And he interviews focus groups of ordinary citizens
  to document the magnitude of the danger facing these firms:
  many people are outraged when informed about the practices of
  companies they deal with.  If the public became widely informed
  about these practices, regulatory legislation would clearly
  become more likely.

  He uses his analysis to motivate some solutions.  Since he
  believes that the threat of regulation is the motivating force
  behind the implementation of good privacy policies, he proposes
  that the United States set up a data protection commission.
  This commission would not have authority to license firms that
  maintain files of personal information.  Instead, it would
  oversee the creation of industry-wide privacy standards, so the
  threat of regulation would be available but not normally acted
  upon.

  Despite the rigors of these arguments, Smith's book is
  fundamentally sympathetic to the dilemmas that confront both
  companies and individual managers in addressing privacy issues.
  He retains a tacit faith in the efficacy of internal privacy
  policies even though genuinely responsible policies might
  decrease the companies' revenues.  Of course, some companies have
  adopted reasonably substantive privacy-protection policies to
  avoid public displeasure.  Yet in emphasizing the reactive nature
  of corporate policy-making, Smith underestimates the amount of
  perfectly proactive obfuscation that certain companies exert
  on privacy issues through their public relations programs.
  Smith's book helps us cut through some of this fog, but much work
  remains to be done.  If we really want to control our personal
  information, first we'll have to clear our minds of the soothing
  language that is circulated by companies involved in privacy
  controversies.

--------------------------------------------------------------------

  Company of the month.

  This month's company is:

  New Society Publishers
  New Society Educational Foundation
  4527 Springfield Avenue
  Philadelphia, PA  19143

  phone: (800) 333-9093

  In TNO I have continually argued that democracy is fundamentally
  a cultural matter, and that the Internet community can contribute
  to a revival of democracy by spreading the skills of community
  and organizing.  Some of the best practical books on these skills
  have come out of church-based movements for peace and social
  justice.  New Society Publishers produces some of the best books
  in the genre, and if you have a serious interest in learning more
  then I encourage you to write for a catalog.

--------------------------------------------------------------------

  Follow-up.

  My complaints about Internet discussion groups in TNO 2(5)
  drew mixed reactions.  Some people thought I was saying that
  *all* Internet discussion groups exhibit the pathologies I was
  complaining about.  That's not so.  An awful lot of them do, and
  what needs explaining is the ones that do not.  Some groups are
  successful, as I pointed out, because they have a steady stream
  of external events to react to, so that endless back-and-forth
  discussions about last week's news get forgotten in favor of
  fresh events.  What are the other dynamics that make groups work?
  And more importantly, what structures can groups adopt that make
  these dynamics work right?

--------------------------------------------------------------------
  Phil Agre, editor                                pagre@ucla.edu
  Department of Information Studies
  University of California, Los Angeles         +1 (310) 825-7154
  Los Angeles, California  90095-1520                FAX 206-4460
  USA
--------------------------------------------------------------------
  Copyright 1995 by the editor.  You may forward this issue of The
  Network Observer electronically to anyone for any non-commercial
  purpose.  Comments and suggestions are always appreciated.
--------------------------------------------------------------------
```

 [*Go back to the top of the file*](#top)