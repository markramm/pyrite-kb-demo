---
id: tno-2-4
title: TNO 2(4).
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1995/TNO.2.4.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - administrative
  - auto-imported
  - rre
  - rre-post
---





## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1995/TNO.2.4.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009062019/http://www.somewhere.com/)

  

# TNO 2(4).

```
---

                T H E  N E T W O R K  O B S E R V E R

  VOLUME 2, NUMBER 4                                    APRIL 1995

---

  This month: Privacy in Intelligent Transportation Systems
              Readings on the institutions of public debate
              Using the net to teach students to write
              Lots and lots of useful Internet pointers

---

  Welcome to TNO 2(4).

  This issue is somewhat shorter than usual since I'm freaking out
  about a variety of deadlines.  Its primary focus is the pressing
  matter of privacy issues in Intelligent Transportation Systems
  (ITS).  ITS has the potential to provide a wide range of useful
  transportation related services, but it also has the potential
  to enable some very serious invasions of privacy.  For example,
  automatic toll collection systems are springing up all over the
  industrialized world.  Several of them in the United States cause
  statements to be created which list a driver's name, address, and
  the precise dates and times and places where tolls were charged.
  Such records can be abused in numerous ways, and the dangers will
  only multiply as the number of toll roads one traverses in the
  average day increases.  The time for constructive action on this
  issue is now, before privacy-invasive technical standards become
  entrenched and large institutional interests develop around
  the routine diversion of ITS-related personal information for
  secondary uses such as marketing.  This issue of TNO includes
  some remarks on this topic that I contributed to CFP'95.  This
  month's "Company of the Month" is developing prototype anonymous
  toll collection systems based on digital cash.  And this month's
  recommendations include an issue of the Santa Clara Computer and
  High Technology Law Journal on the topic.

  Also in this issue is a bibliography on the issues surrounding
  the industrial organization of public debate, a theme that I
  introduced in TNO 2(2) and will return to as soon as I can catch
  my breath.  This month's "wish list" describes a hypothetical
  system for moving certain elements of the jobs of college writing
  instructors offshore.  This worrisome idea provides an occasion
  to think through a whole variety of issues.  I hope that college
  teachers will take the possibilities of automation in their jobs
  seriously before it's too late to shape either the technologies
  or the institutions of teaching in ways that benefit everyone.

  Finally, a footnote on filthy e-mail.  I saw a report on the net
  that Vietnam's online services are having trouble getting their
  keyword-based smut detectors working because they can't represent
  Vietnamese diacritics accurately.  Perhaps the Communications
  Decency Act will bring such mechanisms to my own country as well.
  This would not be a happy result on the whole, but it would have
  certain virtues.  For example, Usenet pornographers would be
  required to write their stories without any of the hundred most
  obvious words for sexual acts, parts, feelings, and intentions.
  In general, I think it is healthy when writers learn not to rely
  on the condensed rhetorical force of individual keywords.

---

  Thinking about privacy in Intelligent Transportation Systems.

  [This is an edited transcript of remarks I contributed to a panel
  discussion at the Fifth Conference on Computers, Freedom, and
  Privacy in Burlingame, California in March 1995.]

  When we debate new technologies, we are necessarily arguing
  about the future.  Lacking direct knowledge of what the
  future will bring, we must tell stories -- stories about the
  complicated interactions between technologies and institutions.
  These stories have all sorts of origins, from science fiction to
  religion to sociological theory, and it is important for us to
  be aware of the nature of our stories and the habits of thought
  that they encode.  Some would say that it's useless to tell these
  stories, or by extension to worry about the social aspects of
  technology at all, given that we can't really predict the future.
  But to speak of "prediction" makes it sound like we have no
  choice in the matter -- like all we can do is wait around and see
  what happens.  But we do have choices, and indeed we inevitably
  make choices, and the choices we make set things in motion that
  we can in fact reason about to some significant degree.

  As Rob Kling has pointed out, the most common stories we tell
  about technology are utopian and dystopian.  Utopian stories may
  admit the potential for harm but are confident that appropriate
  safeguards will permit the new technologies to unleash enormous
  and almost unimaginable benefits -- a societal revolution whose
  outlines can be read off from the workings of the machinery.
  Dystopian stories about technology generally draw on images of
  authoritarian hell on earth in which technologies are employed
  solely for surveillance and control with few possibilities for
  liberation or redemption.

  In getting beyond these simple stories, the point is not to split
  the difference between them but to collect useful, substantive,
  medium-sized concepts that let us make theories about the
  interactions between technologies and institutions, where these
  theories depend in some detail on how the technologies and the
  institutions actually work.

  This kind of reasoning, I want to suggest, is urgently needed
  in the case of Intelligent Transportation Systems (ITS).  ITS
  architecture development to date has been driven by a large and
  subtle process of coalition-building among the companies and
  agencies that already manage transportation systems or that wish
  to develop new markets for existing technologies and systems
  integration skills.  Social issues have not been ignored by
  any means, but it is hard to find much evidence that privacy
  considerations, to take the topic at hand here today, have had
  any fundamental influence on architectural thinking, or indeed
  that they have been regarded as anything but, as one report
  recently put it, nontechnical constraints and barriers to ITS
  implementation.  And although I do not believe in dystopian
  stories about technology, at least in their pure, refined
  form, nonetheless I do believe that the ITS design process, if
  it continues on its current course, will lead to serious and
  systemic invasions of privacy.

  The raw material for dystopian visions of ITS is not hard
  to find.  Consider, for example, a 1992 report on ITS field
  trials by an OECD scientific expert group, which describes the
  "monitoring, teaching, and policing" functions of ITS as follows:

    "These functions are grouped together, although they are quite
    different, since they use the same technical basis.  Speeds
    and distances in relation to rules, road condition and other
    road users are monitored in connection with other functions.
    This information can be processed to provide the individual
    driver with immediate feedback on his behavior.  Such immediate
    reward and correction are known to be effective in teaching
    procedures.  It could serve to gradually improve driver
    behaviour and teaching performance.  In case a driver neglects
    these efforts to correct his misbehaviour, the same information
    could be used to enforce correct behaviour by various means,
    such as fines, license or speed limitation (policing)."

  Or consider this (considerably milder) passage from the DOT's
  1992 IVHS Strategic Plan Report to Congress:

    "The types of innovations [envisioned as part of ITS] include:

     [...]

* A variety of innovations within and outside of the motor
  vehicle to supplement the driver's efforts at vigilance
  and control, including new products which ensure the
  driver's own state of fitness, provide onboard road
  signing and visual enhancements, augment driver perception
  on a continuous basis, give warning of impending danger,
  intervene with emergency control if a crash is imminent,
  and over time, automate the driving process on specialized
  roadways."

(My thanks to Frank Durand <fwd@ix.netcom.com> for pointing these
  passages out to me.)  Clearly these scenarios, which it should
  be emphasized are just two among dozens, provoke some serious
  ambivalence.

  Further ambivalence derives from one major application of ITS,
  namely automatic toll collection.  On one hand, automatic toll
  collection should increase efficiency and convenience.  On the
  other hand, it threatens to create records of where you have
  been driving.  Although participation in such programs is usually
  described as voluntary, it will more likely become involuntary in
  practice as toll roads multiply, a concept called road pricing.
  Although rhetorically motivated by market allocation arguments,
  road pricing is better understood as a tax being sought by
  revenue-starved governments, for the simple reason that in most
  cases it is virtually impossible to create genuine markets for
  roadway services, in which prices could be set by competition
  rather than by the politics of taxation.  These privacy and
  taxation concerns led the citizens of Hong Kong to reject a road
  pricing scheme several years ago, and such resistance is a real
  possibility in other countries as well.

  With regard to the privacy issues in ITS, I think that the
  crucial issue is the capture of individually identifiable
  information about drivers and other transportation users.  ITS
  has the potential to generate enormous databases of individual
  travel information, and this information raises much more serious
  possibilities for abuse than the transactional information
  generated in supermarkets and other such consumer contexts.
  Although the paradigm here is the private citizen driving a
  privately owned car for noncommercial purposes, let me remark
  in passing that consumers have ITS privacy interests in a
  wide variety of contexts.  At least one rental car company,
  for example, is experimenting with GPS tracking of its cars,
  ostensibly to assist drivers with directions but more importantly
  to keep track of their property.  The information generated
  through this process will likely have a whole range of largely
  unforeseen secondary uses, both inside and outside the rental
  car company.  Insurance companies may take an interest in ITS
  information as well, perhaps to continue segmenting their markets
  based on the actuarial implications of individuals' travel
  patterns.

  The "fair information and privacy principles" being circulated
  by ITS America address these issues after a fashion.  They
  explicitly envision the creation of individually identifiable
  records and their secondary use.  Drivers will be permitted to
  opt out of these secondary uses.  Governments are explicitly
  envisioned as potentially providing law enforcement with the
  authorith to use ITS information as a surveillance means for
  enforcing traffic laws.  The full details are available on WWW
  at  http://weber.ucsd.edu/~pagre/its-privacy.html

  I think that technical professionals and other concerned citizens
  should ask a fairly long list of questions about these draft
  principles:

* What does "individually identifiable information" mean in

an ITS context?  What about information that is indexed by a
  vehicle identification or debit account number, which number
  is associated with your name in some other database?  What about
  the potential for reconstructing or narrowing down an individual
  driver's likely identity using ITS information together with
  information from other databases?

* Why should drivers have to take action to opt out of

the dissemination of such potentially dangerous information?
  Few deny the potential economic benefits of secondary uses of
  such information, but surely the technology exists to provide
  a user-friendly way for consumers to opt in to such uses by
  explicitly requesting certain kinds of offers, perhaps using
  pseudonyms to do so.

* Should ITS privacy guidelines have the force of law?* Who should be liable when ITS information is employed to

violate an individual's privacy?  ITS developers?  States?
  Both of them?  What statutory framework is required to ensure
  that violated individuals can pursue adequate legal remedies?

* How will the adequacy of ITS privacy safeguards be determined?

Who will make this determination?  Will there be an ongoing
  evaluation?

* Is it reasonable that these guidelines are being formulated by

a private organization, albeit one serving as an advisory board
  to DOT, rather than by the government itself?

  (My thanks to Marc Rotenberg for his help with these questions.)

  I regard these questions as fairly serious and urgent, and I
  think we should ask whether ITS development should proceed until
  they have been answered.  But more fundamentally, I think we
  should reconsider the whole premise of the "Fair Information
  and Privacy Principles", which is that privacy can be protected
  through a set of policy guidelines developed independently of the
  system architecture.  History shows clearly that when databases
  of information begin to accumulate, imaginations start working
  overtime to think up new uses for them.  In the case of ITS
  information, this is an accident waiting to happen.  And it
  is a wholly unnecessary accident as well.  The fact is that
  new technologies have arisen that should make the collection of
  individually identifiable information in ITS wholly unnecessary.
  Perhaps the prototype for these technologies is digital cash, a
  mathematical scheme based on public key cryptography that allows
  a buyer and seller in electronic commerce to transact business
  without necessarily identifying themselves to one another.  In
  particular, digital cash should make it possible for drivers to
  pay for transportation services such as the use of toll roads
  anonymously.  Digital cash is an improvement over other "smart
  card" systems because it is not based on an account that can be
  used to connect different uses of an ITS system together, and
  potentially to connect those uses back to the individual driver
  through the account's connection to the credit card or bank
  account that might periodically be used to transfer credit to it.
  (See this month's "Company of the Month" below.)  It's best to
  think of digital cash not as a single technology, but rather as
  one amidst a whole world of technologies that can be assembled
  from the building blocks of public key cryptography and
  intelligent agents.

  How will we ensure that ITS employs these 21st century
  privacy technologies?  The bad news is that the main tradition
  of computer system design requires human activities to be
  progressively reorganized so that distributed computer systems
  can "capture" them in real time.  This is what will happen
  with ITS unless privacy protection is redefined as a central
  functionality of those systems.

  The good news is that the business and government entities that
  have been central to the ITS initiative do not plan on making
  their money, at least most of it, through secondary uses of
  personal information but by providing useful transportation
  related services.  These people realize that privacy issues are
  a potential show-stopper through the resistance they can provoke
  from an informed public, and they are likely to be open to
  constructive proposals that provide genuine privacy protection
  while permitting everyone to enjoy the benefits of ITS.

  Technically informed professionals will play a crucial role in
  this process.  I would suggest that we need an Internet-based
  ITS Watch, with volunteer citizen-activists using on-line forums
  like the Privacy Digest to pool reports on the privacy aspects
  of the hundreds of national, state, and local initiatives,
  while also raising awareness within the architecture development
  and standards-setting processes both of the new technologies of
  privacy protection and the risks of public resistance that may
  attend the failure to use them.  Will these things happen?  It's
  our choice, right now.

---

  Bibliography on industrialized public debate.

  I hope that my TNO articles about industrialized public debate
  will inspire others to inform themselves and join the crusade
  to restore the health of democracy.  Although these articles
  are informal and not part of the scholarly literature, they are
  influenced in various ways by others' work.  Here are some books
  that you might find useful.  They are an extremely mixed bag,
  including both journalism, advocacy, and scholarship from a wide
  variety of political perspectives.  I find them all valuable, but
  in different ways -- some as sociological specimens and others as
  serious accounts of our current dilemma.  I'll let you decide for
  yourself which ones are which.

  Eric Alterman, Sound and Fury: The Washington Punditocracy and
  the Collapse of American Politics, New York: HarperCollins, 1992.

  Jeffrey H. Birnbaum, The Lobbyists: How Influence Peddlers Get
  Their Way in Washington, New York: Times Books, 1992.

  Craig Calhoun, ed, Habermas and the Public Sphere, Cambridge: MIT
  Press, 1992.

  Bill Cantor, ed, Experts in Action: Inside Public Relations, New
  York: Longman, 1984.

  Charles T. Clotfelder and Michael Rothschild, Studies of Supply
  and Demand in Higher Education, Chicago: University of Chicago
  Press, 1993.

  Cynthia Crosson, Tainted Truth: The Manipulation of Fact in
  America, New York: Simon and Schuster, 1994.

  Edwin J. Feulner, Jr., Waging and Winning the War of Ideas,
  Washington: Heritage Foundation, 1986.

  Oscar H. Gandy, Jr., Beyond Agenda Setting: Information Subsidies
  and Public Policy, Norwood, NJ: Ablex, 1982.

  William Greider, Who Will Tell the People: The Betrayal of
  American Democracy, New York: Simon and Schuster, 1992.

  Joseph R. Gusfield, The Culture of Public Problems: Drinking-
  Driving and the Symbolic Order, Chicago: University of Chicago
  Press, 1981.

  Jurgen Habermas, The Structural Transformation of the Public
  Sphere: An Inquiry into a Category of Bourgeois Society,
  translated by Thomas Burger, Cambridge: MIT Press, 1989.

  Robert L. Heath, ed, Strategic Issues Management: How
  Organizations Influence and Respond to Public Interests and
  Policies, San Francisco: Jossey-Bass, 1988.

  Robert Jackall, ed, Propaganda, New York: New York University
  Press, 1995.

  Barry Mitnick, ed, Corporate Political Agency: The Construction
  of Competition in Public Affairs, Newbury Park, CA: Sage, 1993.

  Vincent Mosco and Janet Wasko, eds, The Political Economy of
  Information, Madison: University of Wisconsin Press, 1988.

  David M. Ricci, The Transformation of American Politics: The
  New Washington and the Rise of Think Tanks, New Haven: Yale
  University Press, 1993.

  James Allen Smith, The Idea Brokers: Think Tanks and the Rise of
  the New Policy Elite, New York: Free Press, 1991.

  Elizabeth L. Toth and Robert L. Heath, eds, Rhetorical and
  Critical Approaches to Public Relations, Hillsdale, NJ: Erlbaum,
  1992.

  Bruce C. Wolpe, Lobbying Congress: How the System Works,
  Washington, DC: Congressional Quarterly Press, 1990.

  Slavoj Zizek, ed, Mapping Ideology, London: Verso, 1994.

---

  Wish list.

  Why don't students learn to write better?  All sorts of reasons,
  I suppose, but one of them is that teaching people to write well
  is labor-intensive.  You can teach introductory chemistry in big
  lectures and graduate-student-led problem sections, but nobody
  learns to write unless someone copy-edits their writing with a
  red pen.  You don't learn to write by writing but by revising
  something you've written, and revisions start with someone else's
  well-informed comments and tailored advice about the problem
  areas to work on right now.  Students who come to my classes from
  the community college system are often particularly ill-served in
  this regard, given that savage budget cuts most often mean very
  large community college classes.

  In my own preferred world, we would decide as a democracy
  that it is important for students to learn how to write well,
  and we would train and hire enough writing instructors for
  them.  Some writing instructors would be career professionals and
  others would be students commenting on the work of less advanced
  students.  Although writing instructors as a profession generally
  do not get the respect they deserve, this is more or less the
  system we already have.  We just don't have enough of it, and
  maybe we're not going to get any more.

  There is an alternative.  Perhaps our students can write
  their essays on WorldWide Web pages, and the copy-editing and
  advice-giving can be done in India.  India has a good higher
  educational system and more educated people than jobs.  We would
  effectively be moving certain components of writing instruction
  offshore, just as an increasing amount of software development
  is moving offshore.  The difference here is that the work would
  be less project-oriented and more job-oriented, so that any given
  worker would sit at a terminal marking up papers and writing
  comments on them without having any very complicated contact with
  the student whose work is being marked up.  The web provides a
  nice, convenient interface for this process, though it would need
  to be augmented with a good interface for the mark-up notations.
  (Isn't that what a mark-up language is supposed to be for?  I
  guess the phrase "mark-up" has different meanings.)

  I expect that many people reading this suggestion are upset by
  it.  Moving people's jobs offshore to low-wage parts of the world
  usually does not make them happy.  Perhaps they would emphasize
  the intricacy of the relationship between writing instructor
  and student, the importance of face to face interaction in
  talking about an essay, and so forth.  It's an empirical question,
  certainly, how the costs and benefits of the different approaches
  compare.  And if people in India are willing to do the work
  then why deprive them of it?  One issue would be the contrast in
  cultural backgrounds; if you've grown up in a culture whose stock
  of cultural references is rooted in the Mahabharata then perhaps
  it's hard to mark up a manuscript written by someone whose stock
  of cultural references is rooted in Shakespeare and the Bible.
  We shall see.

  My point is not to present this speculation as a Good Thing, or
  even as a Prediction.  It's a fantasy, like all of the fantasies
  in this department of TNO, offered as an occasion to reflect on
  the nature of technological fantasies.  This one, like most, is
  no doubt way too simple.  We can be sure, I think, that computer
  network based work reorganization is coming to academia, and not
  just to writing instruction: introductory chemistry seems like
  an obvious place to look as well.  Once professors are obliged
  to think about their courses as "courseware" (ugh), the world is
  going to change.  But not in obvious ways, simply by replacing
  a person doing job X by a machine that does the same job.  More
  likely job categories will get shuffled and rearranged.  Most
  of this will get presented as lightening the load, leaving the
  skilled employees to do the more highly skilled parts of their
  jobs, expanding the job definitions of employees in lower job
  categories, and so forth.  It will take much trial and error
  to figure out precisely which part of writing instruction, for
  example, really can be moved offshore to India, and which part
  must be left to the (presumably fewer) professionals and trained
  student workers back on the university campus.

  In my experience, academic workers are generally oblivious to the
  ongoing projects aimed at reorganizing university institutions
  and teaching activities through the application of technology.
  For professors in particular, tenure is a narcotic.  And even
  more narcotic is the idea that each individual professor succeeds
  or fails on his or her own individual merits and networking and
  publication and general hustle.  But times of radical change tend
  to make explicit the unarticulated assumptions that underlie the
  previous order of things.  Once this happens at the university,
  it will probably be too late.

  The issues are enormous.  As conservative rhetor Thomas Sowell
  points out, once most university classes are taught through
  video, it will be possible to document the political views that
  are being taught in class and explose the unpopular views to
  criticism.  (He thinks that this is a good thing.)  On the other
  hand, it would be excellent if a professor who wishes to offer a
  course on meter in Chaucer can assemble a large enough class of
  students by assembling the geographically scattered enthusiasts
  of that specialized topic into a networked virtual classroom.
  Let's get it into our heads that university teaching work, at
  all levels, is work, and that like any other kind of work it
  can change radically for better or worse.  It is not a matter of
  "predicting" these changes, since the whole idea of prediction
  presupposes that we can only wait passively and see what happens.
  Instead, I think it is important for university workers to learn
  the emerging technology and get busy organizing themselves to
  shape both the technology and the institutions of education in
  accord with the values that are important to them.

---

  This month's recommendations.

  Bill Morrissey, Night Train (Philo/Rounder).  I mentioned this
  record in passing in TNO 1(5) as part of my list of excellent
  new records from middle-aged white guys.  I've been listening
  to it ever since, and it just keeps getting better and better.
  Bill Morrissey is a folk singer from New Hampshire who is just
  about the best song-writer in the world.  His perfectly honest,
  achingly beautiful, utterly unpretentious songs concern small
  epiphanies in the lives of people with genuine emotions.  Each
  one is a precisely drawn picture with no extra stuff left over.
  For example, "Cold, Cold Night", a gently quick-tempo number
  about the heightening of senses in new love, breathes striking
  clarity into a series of small things and clocks in at 2:13.

  Computer Supported Cooperative Work, Kluwer (ISSN 0925-9724).
  This is an academic journal about people working together using
  computers.  It is rare among journals in focusing with equal
  seriousness on both the technical and social aspects of computer
  work, balancing a sophisticated critical consciousness with a
  commitment to building real, useful things.  (Look for my own
  article about the business discourse of "empowerment" sometime
  later this year.)  Library budgets for journals are in crisis
  these days, but even so I really recommend that you tell your
  local academic or corporate library about CSCW.  As more and
  more activities come to be mediated by long-distance computing
  and communications, the work being reported in this journal is
  precisely what we're going to need to help build tools in way
  that's informed by real ideas about people's lives.

  Santa Clara Computer and High Technology Law Journal, special
  issue on privacy issues in Intelligent Transportation Systems
  (volume 11, number 1, March 1995).  It derives from a symposium
  on this topic that Dorothy Glancy organized at Santa Clara
  University in July, 1994.  Contributions include: Hon. Norman
  Y. Mineta, "Transportation, technology, and privacy"; Jeffrey
  H. Reiman, "Driving to the Panopticon"; Sheldon W. Halpern, "The
  traffic in souls"; Robert Weisberg, "IVHS, legal privacy, and the
  legacy of Dr. Faustus"; Sheri A. Alpert, "Privacy and intelligent
  highways"; Ronald D. Rotunda, "Computerized highways and the
  search for privacy in the case law"; Philip E. Agre, "Reasoning
  about the future"; and Dorothy Glancy, "Privacy and intelligent
  transportation technology".  According to the order form in
  the journal, single issues may be purchased for US$20 (or US$25
  for foreign addresses) from: Computer and High Technology Law
  Journal; School of Law; Santa Clara University; Santa Clara,
  California 95053; (408) 554-4197; scchtlj@scuacc.scu.edu.

  Second Annual Report of the Privacy Rights Clearinghouse, Center
  for Public Interest Law, University of San Diego, January 1995.
  The Privacy Rights Clearinghouse (PRC) is a consumer education
  project on privacy issues that operates a toll-free phone number
  that California residents can call with questions and concerns
  about privacy issues.  They also produce a large number of highly
  regarded fact sheets about specific privacy related topics --
  a remarkable feat given the murky state of most of the relevant
  law.  Their Second Annual Report features 47 excellent real-life
  horror stories drawn from the thousands of phone calls they have
  answered.  The PRC is on the web at http://www.acusd.edu/ and on
  gopher at gopher.acusd.edu (under "USD Campuswide Info. Svcs.").
  Their e-mail address is prc@acusd.edu.  Their hotline number is
  (800) 773-7748 (in California only) or +1 (619) 298-3396.

---

  Company of the month.

  This month's company is:

  Amtech Systems Corporation
  17304 Preston Road, Building E-100
  Dallas, Texas  75252

  phone: +1 (214) 733-6600
    fax: +1 (214) 733-6699

  Elsewhere in this issue of TNO you've read about the potential
  for serious privacy violations in Intelligent Transportation
  Systems.  No doubt someone will tell you, "hey, that's just the
  price of progress" or "those privacy paranoids just don't like
  technology".  The truth is that the privacy invaders are the
  ones who are against technology -- the powerful technologies of
  privacy protection that are rapidly becoming available.  Amtech,
  one of the major providers of equipment for automatic vehicle
  identification (AVI) for highway toll collection, has developed a
  prototype of an AVI system based on the "digital cash" methods of
  David Chaum's company Digicash.  This system will permit people
  to pay for tolls automatically and with complete privacy through
  the use of cryptography.  Amtech is planning to market the system
  in Europe and Japan, but at present they have no plans to market
  it in the United States for the simple reason that the highway
  authorities who are implementing ITS systems are not terribly
  unconcerned about privacy.  That's not necessarily because they
  are evil; often it is because they are simply not aware of the
  magnitude of the dangers and the availability of technological
  solutions.  I encourage you to do research on the ITS systems
  that are coming to a highway near you (and I promise that ITS
  is definitely coming to a highway near you), contact the local
  highway authority administrators (they usually answer their
  own phones), politely ask them whether they plan to employ
  technologies based on digital cash for their toll collection, and
  when they say "huh?, what's that mean?", politely tell them about
  the virtues of digital cash, its wide acceptance in Europe, and
  the progress of Amtech's digital cash AVI technology.

  I am sure that Amtech would be happy to send you information
  about their technology.  Please, though, don't ask for it unless
  you have a serious reason to want it.  Doing research on the
  privacy aspects of ITS systems in your area is a serious reason.

---

  Follow-up.

  My notes on the industrial organization of public debate provoked
  some correspondence.  Bill Dickens <wdickens@brook.edu> at the
  Brookings Institution did not like my general orientation toward
  the pursuit of self-interest in the funding of think tanks and
  the like.  And he was certainly right that I went over the top
  with one parenthetical comment about think tanks, namely:

    (It's an awful phrase -- a common euphemism is "research
    institutes", though that latter phrase includes some scientific
    and technical institutions that do more than produce ammo for
    public debates.)

  This comment is bogus enough that I've actually removed it from
  the archival versions of TNO 2(2).  Many difficult issues arise
  here, not least when we are faced with people working in think
  tanks who are sincerely trying to do the right thing.  I wouldn't
  want to impugn those people's motives or enter into any sort
  of straightforward reductionism about the people who contribute
  money to think tanks.  Further analysis, though, will have to
  wait until I get some time to think clearly again.

  I was a little unclear in TNO 2(3)'s mention of Ellen Spertus'
  WWW list of non-profit organizations.  The list is at MIT and
  Spertus herself used to be at MIT, but now she's at Microsoft.

  In TNO 2(3) I mentioned my "wish list" idea for a web-based
  system for letting booksellers know about author's publicity
  schedules.  Frank Kroger <fkroger@halcyon.com> kindly pointed
  me at an embryonic version of something similar called BookWire:
  http://www.bookwire.com:80/

  The journal Information Technology and People has recently
  published a special issue, edited by Roger Clarke, entitled
  "Identification Technologies and Their Implications for People".
  Christine Harbs and I have an article in this issue entitled
  "Social Choice About Privacy: Intelligent Vehicle-Highway Systems
  in the United States".  You can see the full set of abstracts by
  sending a message that looks like so:

    To: rre-request@weber.ucsd.edu
    Subject: archive send identification

  Or on WWW at http://weber.ucsd.edu/~pagre/identification.html

  Also, I have coedited (with Stan Rosenschein) a special double
  volume of Artificial Intelligence on "Computational Theories of
  Interaction and Agency".  The first volume has appeared, and the
  abstracts for the articles in both volumes, along with contact
  information for all of the authors, are available on the web.
  The URL is  http://weber.ucsd.edu/~pagre/aij-abstracts.html

  The Australian Privacy Charter Council has released a very
  interesting list of privacy principles that improves considerably
  on the principles that have been suggested in the United States
  and many other countries.  It will be a valuable reference for
  anyone trying to articulate the conceptual basis for privacy
  protection in specific contexts such as transportation, banking,
  and medical records.  The URL, which I've split over two lines,
  is:  http://commerce.anu.edu.au/comm/staff/RogerC/Dataveillance/
  PrivacyCharter

  Jerry Werner is editing an on-line newsletter on Intelligent
  Transportation Systems.  It will be valuable for people who
  are concerned about the privacy implications of this enormous,
  potentially worrisome project.  The URL is  http://io.com/~itsol/
  Check out the interview on ITS with Newt Gingrich.

  Voters' Telecom Watch is at  http://anansi.panix.com:80/vtw/
  They're leading the charge against the Communications Decency
  Act (the Exon bill, recently incorporated by the Senate into the
  telecom deregulation bill).

  In case you haven't seen it, the very funny "Useless WWW Pages"
  site is at  http://www.primus.com/staff/paulp/useless.html

  The US government has declassified a batch of Cold War era
  satellite intelligence photographs of the Soviet Union.  The
  photographs are of fairly low resolution and seem part of an
  advertising campaign aimed at finding civilian uses for military
  spy satellite technologies, but they are certainly interesting
  documents.  They've put a few of them on the web, and they
  claim they'll make the whole batch available on-line eventually.
  The URL is  http://edcwww.cr.usgs.gov/dclass/dclass.html

  An Irish friend passed along to me and twenty other acquaintences
  the URL for the "framework document" released by the British and
  Irish governments for negotiations over Northern Ireland.  He
  says that the document was hard to get in paper form, and the web
  site provides a fine example of the power of the net in getting
  information out and opening political processes to the public.
  The URL is  http://netman.ul.ie/ITD/framework.html

  Lew Rose has a good web site of materials on advertising law.
  The URL is  http://www.webcom.com/~lewrose/home.html

  The Senate Democrats have a skeletal but decently maintained web
  site at ftp://ftp.senate.gov/committee/Dem-Policy/general/dpc.html

  The hotel industry has set up some web pages that are more
  interesting than most non-computer industry pages.  They're
  called TravelWeb and the URL is  http://www.travelweb.com/

  Gleason Sackman's exhaustive net-happenings mailing list of net
  resources on education now has a searchable index on the web.
  The URL is  http://www.mid.net:80/NET/

  There's a pretty impressive collection of educational resources
  at http://inform.umd.edu:86/Educational_Resources/

  Another web index of conservative stuff is under construction at
  http://www.moscow.com/~bmdesign/tcl/conhome.html

  A good guide to newspapers that have web pages can be found at
  http://marketplace.com/e-papers.list.www/e-papers.home.page.html

  A site of resources for WWW developers, including a page of
  advice on how to publicize your web pages, is located on WWW
  at  http://www.uwtc.washington.edu/Computing/WWW/General.html

  A very interesting set of web resources in Spanish is located
  at  http://www.sccs.swarthmore.edu/~justin/jornada/index.html
  And a flamboyant guide to web stuff in French is located at
  http://www.cam.org/~hugo/francais.html

  Here are the pointers to web sites on the Oklahoma City bombing
  that the LA Times reported on April 21st:
    http://www.coast.net/~emv/tubed/ok-bomb.html
    http://www.ionet.net/explode.html
    http://www.uoknor.edu/okdaily/bombing.html
    http://www.cpb.uokhsc.edu/okwww.html
    http://qns1.qns.com/kwtv/news/bombing.html
    http://pathfinder.com/

---

  Phil Agre, editor                                pagre@ucsd.edu
  Department of Communication
  University of California, San Diego           +1 (619) 534-6328
  La Jolla, California  92093-0503                   FAX 534-7315
  USA

---

  The Network Observer is distributed through the Red Rock Eater
  News Service.  To subscribe to RRE, send a message to the RRE
  server, rre-request@weber.ucsd.edu, whose subject line reads
  "subscribe firstname lastname", for example "Subject: subscribe
  Jane Doe".  For more information about the Red Rock Eater, send
  a message to that same address with a subject line of "help".
  For back issues etc, use a subject line of "archive send index".
  TNO is also on WWW at http://communication.ucsd.edu/pagre/tno.html

---

  Copyright 1995 by the editor.  You may forward this issue of The
  Network Observer electronically to anyone for any non-commercial
  purpose.  Comments and suggestions are always appreciated.

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009062019/http://www.somewhere.com/)