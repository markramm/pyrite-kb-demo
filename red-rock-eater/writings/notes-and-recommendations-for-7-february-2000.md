---
id: notes-and-recommendations-for-7-february-2000
title: "Notes and Recommendations for 7 February 2000"
type: writing
writing_type: paper
date: 2000-02-07
url: "https://pages.gseis.ucla.edu/faculty/agre/notes/00-2-7.html"
coauthors: []
key_concepts: []
importance: 5
research_status: stub
tags:
  - paper
  - auto-imported
---

## Source

Automatically imported from: https://pages.gseis.ucla.edu/faculty/agre/notes/00-2-7.html

## Content

```
Some notes on the US elections and computer science, followed by
a batch of follow-up items and several recommendations, plus URL's.
Some of the follow-ups and most of the URL's draw on subscribers'
notes, so you should regard the whole thing as a collective effort.

As a periodic reminder, you can unsubscribe by sending a message that
looks like this:

  To: requests@lists.gseis.ucla.edu
  Subject: unsubscribe rre

RRE messages can be forwarded electronically to anyone, except for a
rare few that are clearly marked to the contrary.  In fact I strongly
encourage you to forward RRE messages to everyone who can use them.
All I ask is that Eudora users not use the "redirect" command to
do the forwarding.

I much appreciate everyone's comments on "Networking on the Network".
I've made a batch of revisions and will send out an announcement for
it this week.  I've been working on NotN for years now, and I really
want you to help me get it in into the hands of every PhD student
in the world.  So please think hard and come up with ways to get the
NotN announcement to people who can use it.  The new version adds a
bunch of new material, most of which I've already mentioned.  I've
also deleted some passages that weren't working, like the shamanic
and Reichean stuff that weirded people out.  My next project, which
probably won't happen until I get some more books written, is a long
section toward the end of NotN that relates the sociology of social
networks to a sort of spiritual philosophy.  It's all in my notebook,
but not quite in presentable form.

John McCain is the strongest Republican candidate in forty years.
So why is the Republican establishment terrified of him?  One reason
is obvious enough: having committed themselves to George Walker Bush,
they will look like idiots if McCain wins.  But pride alone does not
explain the evidence.  The real reason is that McCain has discovered
a fault line through the middle of the Republican coalition.  It's
a line between two very different kinds of conservatives.  On one
side are conservatives in the mold of Edmund Burke.  These people
want to restore a society of orders and classes -- a divine order in
which everyone knows their place.  They know that George Walker is a
dim-witted aristocrat who owes everything to his father's connections,
but that's precisely why they support him.  Despite his dissolute
youth, sleazy business dealings, and indifferent performance as the
governor of Texas, they regard him as the model of "character" because
of his breeding.  That's how they think.

That kind of conservatism obviously holds a limited appeal for the
great majority of voters, however, and so the establishment has spent
the last twenty years building up its think tanks and propagating its
pundits to sell working people on another kind of conservatism, one
based on the verities of decency and self-reliance.  Come the election
year, then, the establishment thought they had it all figured out:
having created a gaggle of nebulous enemies to keep working people
in a froth, they could nominate one of their own, persuade the voter-
unfriendly theocrats to return to their closet strategy of stealth,
fake left with empty talk about inclusiveness and compassion, cruise
to victory on working-class conservatives' votes, treat themselves
to some great big tax cuts, and implement all of the institutional
changes they had ever dreamed of.  First they'd repeal the 1960s,
then they'd repeal the 1930s, then they'd repeal the 1790s, and then
if they got a second term they'd repeal the Renaissance.

But along comes John McCain, the ultimate product of the working-class
conservative culture of the military.  McCain is a conservative, no
doubt about it.  But McCain understands something: that the average
American does not want a society of orders and classes, does not want
a return to the Middle Ages, and thinks that the whole reason why
people like themselves died in the American Revolution and a bunch of
subsequent wars was to get away from that sort of thing.  So McCain is
campaigning on conservativism: not the pundit conservatism that blurs
things together, but the conservatism of decency and self-reliance
that a lot of normal Americans, unlike their establishment betters,
actually believe in.  The establishment is freaking because McCain is
calling them on their game.  It has a decent paper trail by now, this
establishment conservatism, and that paper trail is all about special-
interest pork.  But normal Americans don't like special-interest pork.
So it doesn't matter whether McCain's own paper trail lives up to the
hype: the fact is that, by really being the candidate that Ross Perot
was in his dreams, John McCain has found the key to American politics
in the year 2000.

So put yourself in the shoes of the Republican establishment.  Let's
say that John McCain raises $10 million on the Internet and then wins
in South Carolina.  Then perhaps McCain wins the nomination, in which
case the establishment is hosed.  Having gone on to crush Gore, McCain
will have completely discredited both of the country's major political
machines.  His power fulcrum will be awesome.  Or, alternatively, the
establishment puts on a giant display of money and machinery to stifle
the popular rebellion, in which case it is discredited just as badly.
Al Gore goes on to win in November, and the establishment operatives
disembowel themselves.  In either case, the establishment will spend a
lot of money telling Senator McCain's supporters that they are actually
liberals.  They might actually start to believe it, and we will return
to a 19th-century style of morally centrist class-based politics.

Democrats have a lot to fear in this.  Bill Bradley does not remotely
have the demographics to win in the fall, and the liberals who support
him are living in dreamland.  Even supposing that Bill Bradley were
a real liberal, as opposed to a guy who last week decided to reinvent
himself one small notch to the left of Gore, liberals don't have the
luxury of picking the candidate of their dreams because they aren't
out there rebutting the pious cliches of doctrinaire conservativism in
public debate.  Liberals can't afford to lose this one, for the simple
reason that the next Republican President will throw a legal switch
that effectively makes it impossible for labor unions to represent
their members in the political process.  And that will be it for the
Democratic party.  The liberals must therefore throw everything behind
Al Gore, they must hope that McCain and Walker annihilate one another,
and they must pray that their man gets his act together real soon.
In particular, they must pray that Al Gore proves himself equal to the
opportunity that Bill Clinton clearly saw but just as clearly screwed
up: building an inclusive politics on spiritual values.  George Walker
maybe they can beat.  But if John McCain intercepts that pass then it's
all over.

Can I ask computer scientists to help me out with something?  ALthough
I got a PhD in computer science in 1989, since then I have been out of
the academic computer science loop.  My research works best, however,
when I can build conceptual bridges between computer science and other
parts of the world, and so I need your help in getting back into the
loop.  Looking around at the increasingly wired world, I keep noticing
a pattern: the technical and institutional problems of connecting
everyone to everyone else.  These problems recur on many levels:

  * Packet switching is a decentralized mechanism for connecting anyone
to anyone else at any time; of course a packet-switched network has no
architectural conception of "connection", but one can easily construct
such a conception on a higher service layer. If the network does
not have to provide any latency guarantees then this is easy enough.
But if such guarantees are required then suddenly all of the world's
routers have to share information intensively enough to make promises
they can deliver on.

  * Transaction processing "connects" everyone to everyone else, in the
sense that everyone in the world is potentially in contention for the
same seat on the airplane, the same box in the inventory, the right to
submit the $120.00 bid in the auction, and so on. The problem, then,
is that everyone needs to be connected to some central point so that
incompatible transactions are not processed. And if a transaction
requires several operations to be performed as an atomic bundle, then
all of the operations that may ever need to be performed as a bundle
need somehow to be within hailing distance of one another. Connecting
six billion people to a single point is obviously a challenge that is
best avoided, if only one can figure out how.

  * Databases are often used simultaneously by thousands of people
all over the world. A database's designer faces a dilemma: either the
heavily used parts of the database are cached in numerous distributed
locations, in which case changes to the database become cumbersome
and even dangerous, or else those parts of the database are stored in
centralized locations, in which case users experience slow responses
to their queries. Lots of fancy handshaking is required in practice.

I gather that much computer science these days is concerned with this
problem. It's hard to imagine any general solutions because of the
difficulty of characterizing the highly distributed patterns of use.
I don't imagine that I can solve the problem; instead, I want to write
about the institutional (legal, economic, organizational, political)
aspects of it. I see people's lives and relationships increasingly
bound together by these "switchboards", as I call them, and I want to
understand the consequences. For example, when do these switchboards
tend to become monopolies because of network effects? And then what
follows from that? What I want are analytically deep computer science
articles about various "connecting everyone to everyone" types of
problems, and about architectural and conceptual approaches to solving
them. These articles could be from the networking literature, or
databases, or groupware, or any number of other subfields. Although
I can handle the technical literature perfectly well, I particularly
want articles that I can recommend to relatively nontechnical people.
I also particularly want articles that throw light on the problem but
do not fit the characterization of it that I've given. I would greatly
appreciate any references or other clues you can offer.

I got another death threat. It was in response to the message whose
subject line read "spam self-regulation is one of the really bad
ideas". It consisted a long tirade about how regulation would stop
progress, and how if I persisted in advocating regulation then I
would be better off dead. Aren't we taking ourselves just a little too
seriously here? I'm not going to be deterred by conservative threats,
and I hope that you won't be either. In fact, I think that one reason
why the Internet has been making so little progress is that there
haven't been enough lawsuits. In economic terms, legal decisions
are public goods -- everyone benefits from the guidance they provide
-- and so it stands to reason that not enough of them will be
produced. In fact, lawsuits produce public goods even when they are
settled, simply by providing the parties to other disputes a preview
of how the issues would sort out. We've had some excellent lawsuits
against spammers, and we need more of them. People who denounce
"lawsuits" are really just denouncing lawsuits against people like
themselves. They have no problem filing lawsuits of their own. That
particular sort of hypocrisy is very 20th century, and we're all bored
with it.

In discussing the commercial forces arrayed against the Internet's
open platform model, for example in the proprietary networks of AOL
and Time Warner, I messed up my biology a little. The mollusc that
attaches itself to the insides of pipes and sucks out the nutrients
that go by, reproducing until it clogs the pipe, is called a zebra
mussel, not a tiger mussel. I was writing quickly and got my striped
animals mixed up. If you search for "zebra mussel" on the Web, you
will discover a minor industry of research on this pest, a nonnative
species in the US where it is causing a lot of trouble, for example
in the Great Lakes. I think it makes an excellent metaphor.

I mentioned a freeware program called NetCD that plays CDs on one's
CD-ROM drive, automatically downloading song titles from a server when
it can't find them on your machine. In response, an RRE subscriber
wrote this, which I've revised only slightly:

  The application you mentioned, NetCD, accesses the cddb database.
  Therein lies a story that might show why distributed applications
  aren't as successful as expected. cddb has been hugely popular for
  years, and there are dozens of applications on every platform that
  were programmed to use the database. Then cddb's owners decided
  that applications must conform to certain restrictions in order to
  access the database (e.g., display a cddb logo for a certain number
  of seconds, provide a link to cddb, etc). That caused enough of an
  uproar in the user community that a clone service, dubbed freedb,
  was started using an old version of the cddb database. (Note that
  the cddb was and still is at least partially supported by user
  submission of information.) cddb is now working on a new enhanced
  version of the cddb protocol that will provide access to more
  information (more credits, weblinks, genre info, etc.); using this
  protocol for some developers will require a license.

  This, to me, is the problem with distributed applications like
  cddb. They can provide a wonderful service, but eventually, someone
  will want to own the data. Judging by all the corporate activity
  around this problem, they will soon be able to legally own
  collections of data like CD #3413241324 is Michael Jackson's Bad.

  So I guess I don't know how it's going to get any better either, but
  for different reasons.

For more information, see:

http://slashdot.org/articles/99/03/08/0945228.shtml
http://slashdot.org/articles/99/03/09/0923213.shtml
http://www.freedb.org/why/ http://www.cddb.com/dev/faq.html/page=all

In response to my cri de coeur about Doubleclick's new policy of
collecting individually identifiable information, some people asked
why I recommended turning cookies off altogether, and why I did not
suggest a half-way measure such as changing one's cookies file to
read-only. Here's the answer. I talk with a lot of reporters about
online privacy issues, and the reporters continually bring home to me
the fact that normal people don't know about esoteric stuff like files
being read-only. Normal people shouldn't have to know about that sort
of stuff. The whole problem with cookies, as with much else about the
interface between personal computers and public networks, is that the
data flows are not transparent. Heaven only knows what data any of the
applications on your personal computer is uploading to some random
computer in the Cayman Islands.

I was willing to tolerate this situation so long as the Web was, for
a really complicated and accidental set of historical and technical
reasons, more or less anonymous. (For example, the average person
cannot be tracked effectively using IP addresses. This is surprising,
given that the Internet protocols depend on having those addresses.
Why is it? It's because most normal people dial in to ISP's that
assign IP addresses to them dynamically on a per-session basis, so
that Web sites and other Internet servers cannot use the IP address to
track them from one session to another unless they can somehow attach
an identity to each of the dynamic addresses. This is a seriously
esoteric fact, and yet it is fundamental to the significant degree of
privacy that normal people do in fact retain today on the Internet.)
Now that Doubleclick has decided to subvert the existing anonymous
system, it's time for an uprising against the lack of transparency
that is unfortunately fundamental to the World Wide Web as we know
it. The philosophy of the Web is to obscure the interface between
client and server, but the philosophy is wrong. That interface
is a sensitive personal boundary that needs to be visible and
comprehensible to the individual that it affects. The Web is broken,
and will remain so until this problem is fixed.

If the latest fiasco with cookies is the last straw for you, you might
want to investigate Freedom, a well-regarded Internet privacy program
from Zero-Knowledge Systems. The following description borrows
liberally from their Web site: Freedom is an encrypted, anonymous
Internet presence system that lets you create multiple pseudonymous
digital identities (nyms) which interact in cyberspace exactly the
way your regular online identity always has, but cannot be associated
to your real-world self. By hiding your IP address and intercepting
cookies, it prevents people from tracking your movements on the
web. That way, you can have the benefits of cookies (remembering
passwords, your personalization of sites, etc) without letting
the site owners learn the real world person's habits. Freedom
also makes it easy to view and delete the cookies sent to each nym.
It's available at .

In response to my essay on the cooperative publication of journals,
the most common response was, "you're not accounting for a wide range
of costs, like typesetting, printing, distribution, and marketing".
But the whole point of Web-based cooperative journal publishing is
that those costs are all reduced and shifted so that they needn't pass
through the hands of the publisher. Authors do their own typesetting,
readers do their own printing, the university that houses a journal
does its own distribution cheaply on the Web, and expensive marketing
was only necessary to persuade librarians to pay for everything else.

One journal editor told me that he still wants to charge for his
journal to pay for administrative support and to send the editors to
conferences, both as a reward for hard work and to make sure that the
editors meet face-to-face occasionally. Well, journals will require
less administrative support once we have decent Web-based tools to
manage a journal through the whole life cycle of article submission,
refereeing, revision, acceptance, publication, archiving, and so on.
And the perks for the editors can be paid for by licensing a paper
publisher to print and sell an annual bound volume of the journal to
those who want it, while the online version stays free. We'll need
more complicated measures in the interim, but that is where we are
headed -- assuming, that is, that we have the backbone to stand up to
the copyright interests.

My essay on journal publishing was intended as a humorous polemic,
not as serious analysis. For serious analysis, I highly recommend
the bracing (if not uncontroversial) work of Andrew Odlyzko, which
(long-timers will remember) first appeared on this list in July 1994;
see .
Particularly relevant here is his "The slow evolution of electronic
publishing" ,
which starts with an entertaining discussion of the adoption rates
of various technologies. He argues that "[a] decade does seem to be
the time scale on which new technologies are fully adopted", and that
"Internet time" is more or less of a myth. True, the Web did drive
the growth in Internet traffic on a very fast curve in the mid to late
1990s, but that is not the norm. (In fact, some people argue that the
explosive growth of the Internet starting in the mid 1990s was really
an artefact of pent-up demand whose satisfaction had been delayed by
the government's "acceptable use policy", which in turn was driven
by the great and prolonged difficulty that the government encountered
in persuading private firms to take over the Internet.) More typical,
he observes, are the slow adoption curves of IPv6 or HTTP1.1. Keep
this all in mind the next time an Internet enthusiast predicts giant
technology-driven social transformations on a three-year time frame.

I asked who first said something like "people tend to overestimate how
much will change in two years and underestimate how much will change
in ten years". One outstanding precedent, it turns out, is J.C.R.
Licklider's celebrated "Libraries of the Future" (1965), in which a
footnote on page 17 (quoted in Odlyzko's "slow evolution" paper) says:

  A modern maxim says: "People tend to overestimate what can be done in
  one year and underestimate what can be done in five or ten years".

He evidently regards it as a commonplace. So I assume that someone
else said it earlier.

After I wrote my little piece about Wal-Mart and the potential
role of wireless computing in the collective lives of recreational
vehicle enthusiasts, RRE readers kindly started educating me about
RV culture. In doing so, they reconfirmed for me a law of nature that
I teach in my classes: if you pick anything that someone cares about
and define the community of everybody in the world who cares about
that thing, then analysis will demonstrate 100% of the time that that
community has much more sophisticated forms of collective cognition
then you had imagined, even if you already knew all about it. I've
been informed that Europe is actually full of RV's (I had assumedthat
Europeans mostly travel by train), that Wal-Mart publishes a US road
atlas with all of their stores marked out on it, and that the best RV
club is the SKP's .  (The Good Sam Club, I
am told, is basically just a marketing thing.)  These clubs, together
with various grassroots groups, "have a network that forms and
re-forms constantly across US highways and into Canada and Mexico.
Some popular wintering spots, like the Salton Sea (old US military
base) become little towns every year with streets, sanitary
arrangements, etc". So my point is not that RV culture does not
exist, since X culture exists for nearly every X you can possibly
think of, but rather that wireless computing could help amplify
the culture-forming processes that are already at work. The point,
obviously, generalizes. What do you care about? What would it be like
for the culture of people who care about that thing to become more
intensively organized?

In response to Starhawk's essay on "How We Really Shut down the WTO",
some military people said that Starhawk obviously does not understand
military control structures. She had argued that a centralized, top-
down command system could not have organized the civil disobedience
actions in Seattle. But, the military people said, the military is
very used to decentralized operations, which make all kinds of sense
in the chaotic combat environment where communications are poor and
rational action requires deep knowledge of the local situation. As
a result, the protesters' command system does resemble that of the
military, except that each small military unit has a hierarchy.

You may recall that I asked for a device the size of a ham sandwich
that serves recordings of Grateful Dead shows, and that works with
other ham sandwiches to connect each user automatically to whichever
server will be most reliable. It turns out that Akamai does something
similar, though not with the self-organizing feature that I wanted.
It's called FreeFlow .

Recommended: Mary Poovey, Accommodating merchants: Accounting,
civility, and the natural laws of gender, Differences 8(3), 1996,
pages 1-20. This is an article about the role of gender ideology
in the emergence of a market economy in England. Merchants had to
persuade the king that something called the market even existed, and
that creating the institutional framework for the market's efficient
functioning would be in the king's advantage. Their main weapon
in this effort was double-entry bookkeeping, which created the
statistical basis for measuring the economy and portraying it as
something lawlike in the same fashion as Newton's heavens. The real
day-to-day life of business, however, involves all kinds of ambiguity,
complexity, contingency, and other messy stuff that accounting systems
do not capture. In order for "the economy" to be presented as a thing
of crystalline beauty, therefore, this stuff, which had always been
central to everyone's understanding of business, had to be hidden.
Poovey's argument is that the businessmen mapped the distinction
between the lawlike economy and the hidden messiness onto invidious
gender distinctions, rendering the messiness invisible by defining it
as women's work. The messy stuff was messy because women were messy,
unruly because women were unruly.  The argument is actually a lot more
complicated about this, and it's a really elegant argument, with all
sorts of compelling internal logic.

The main problem with Poovey's paper is that you mostly just have to
believe her. Her argument is intended to apply to a moderately large
number of people over a certain number of decades, and it only works
if the processes she describes really were general. She does provide
several compelling documents to support her argument, and if these
documents are representative then the case is closed. This is a
problem that confronts nearly all narrative history: one must assert
generalizations that one can reasonably believe in, having read the
whole mass of archives, but that one cannot adequately demonstrate for
the reader within the manageable scope of a paper or a book. I had
hoped that Poovey would expand on her argument in her recent book, "A
History of the Modern Fact: Problems of Knowledge in the Sciences of
Wealth and Society" (University of Chicago Press, 1998), but in that
book she is after a different target: the social construction of
value-neutrality in early modern science. This is an important topic,
but not one that I am deeply interested in. Still, it is right next
door: both are concerned with the hidden agendas in institutions
that claim to be objective and neutral. I have nothing much against
objectivity and neutrality, but I have plenty against institutions
that pretend to be objective and neutral when they really are not.
The world is full of that sort of thing, and it doesn't have to be.

Recommended: Metropolis. Metropolis is my favorite magazine, period.
It's about "design", by which they mean the more artistically inclined
varieties of design, everything from furniture to cities. What's so
good about it is its emphasis on context. A lot of design magazines
are focused entirely on the object, but Metropolis shows things in
real use, in history, as part of culture, and in the intersection
between the aesthetic and technical sides of design work. Although it
certainly observes that certain designs have gotten tired, it is not
obsessed with fashion -- it will not make you hip, much less edgy.
Metropolis has been around for years; I first encountered it in the
1980s when it was, in best 1980s style, the world's most gigantic
magazine -- at least two by three feet, though presumably it has grown
in my memory. Although I don't have any sense of how it has changed
since then editorially, it has shrunk to a more conservative and
mailbox-friendly size. It costs $29.95 for 10 issues. The Metropolis
Web site  has a batch of past articles,
although the webmasters make little attempt to reproduce the layout of
the pages, the pictures, etc.

Not recommended: Brill's Content. I bought the first issue of Brill's
Content at Union Station in Washington the day it came out. It was
the issue that had Steven Brill's epic article about press leaks from
Kenneth Starr's special prosecutor office, and I was so pleased to be
walking around Washington with this thing under my arm that I actually
subscribed to it. At first Brill's Content seemed like a meritorious
if quixotic project: an attempt at truth-telling about the media
without the one-sided "liberal media bias" type agendas that depend so
heavily on vagueness, fancy paraphrase, selective use of evidence, and
outright falsehoods. And at first that's how it seemed. But then it
changed, or else perhaps my perception of it caught up with reality.

That reality was not nice. The first thing I noticed was their need to
create a compelling headline by imposing a clear-cut interpretation on
situations that have two sides to them. Okay, I said, it's a magazine;
they need to pay the rent. But then I started seeing things that I
really didn't like: tendentious articles that are obviously driven by
a party that doesn't like its press coverage. There was a piece about
Consumer Reports, for example, that consisted of nothing but verbatim
complaints about Consumer Reports by the public relations departments
of companies whose products Consumer Reports has flunked. I knew this
because I taught a class about public relations and read articles by
the PR people. Then there was a cover story about the JonBenet Ramsay
case that was written totally from the perspective of the murdered
child's parents. Now, some people have argued that the police fouled
up a serious situation, or that elements of the press sensationalized
it. But this article argued that there was no story at all, and that
an "industry" of reporters were cynically promoting their careers by
pretending that there was. This will not do.

Worst of all, Brill's Content has been all too willing to go along
with antimedia bandwagons such as CNN's disgraceful failure to stand
behind the reporters who presented evidence of American soldiers using
poison gas against defectors in Vietnam. I don't know whether that
story was true or not, but I do know that CNN's stated reasons for
discrediting the report and firing the reporters were superficial
and unpersuasive. As with the San Jose Mercury-News' exile of Gary
Webb for his "Dark Alliance" articles about the CIA's toleration of
the Contra crack trade, the central theses of which were ultimately
vindicted by the CIA's own report, the grounds that CNN gave for
firing its reporters would put the vast majority of investigative
reporters on the street. A serious article on the case would have
evaluated carefully the possibility that CNN had caved in to another
right-wing campaign to suppress a news story it didn't like, but
Brill's Content took CNN's and the campaigners' objections at face
value. They did provide the fired reporters with a little space
to present their side, but not nearly enough to make a legitimate
debate of it. This stuff has become way too much of a pattern, I'm
afraid, and I will not be unhappy if Steven Brill's quixotic project
fails. Brill himself has recently announced his departure from the
magazine for an Internet startup, however, so we can at least hope
that the new management will turn things around.

Recommended: Noam Chomsky, The New Military Humanism: Lessons From
Kosovo, Common Courage Press, 1999. Noam Chomsky has an astounding
command of facts and an incredibly sharp eye for double standards,
and these attributes alone make all of his political writing worth
reading, whether one agrees with it or not. His book about the war
in Yugoslavia is no exception. He opposed the war, of course, and
regards it as part of a thoroughgoing pattern of American bullying and
doubletalk throughout the world. And only the most obdurate supporters
of the war will not have to rethink their reasons after reading
Chomsky's case against it.

His method is simple enough. (1) Ask whether the publicly stated
justifications for the war are factually true. Many of them simply
were not, such as the arguments that bombing was required to stop
ethnic cleansing that had not yet started on a significant scale
before the bombing began. This category also includes the remarkable
diplomatic history, which includes several episodes in which the
United States unambiguously flouted international law and its own
agreements. (2) Ask whether those justifications would also require
the United States and its allies to take other actions that they have
never contemplated taking. Many of them certainly do, especially in
the case of Turkey, whose treatment of its Kurdish minority is highly
analogous to the Serbian government's treatment of the Kosovars, with
the exception that the Turkish government's policies, implemented with
American hardware, are much more violent. NATO is hardly in a position
to get righteous about Serbia when a NATO member in good standing is
doing the same things only worse.

Except in some of his fast-forward discussions of the war in Bosnia,
I found Chomsky's logic pretty much ironclad. That does not mean that
one must necessarily reach his conclusions, but if one wants to reach
different conclusions one must reach them for more complicated reasons
than were the norm at the time. Notwithstanding the force of Chomsky's
logic, however, those who are unacquainted with his writing style
will need to consciously prepare themselves for the foot-thick layer
of sarcasm with which the entire book is written. His basic rhetorical
technique is to quote a random sample of op-ed slobbering over
America's righteous goodness, and then to recycle those quotes over
and over as the atrocities and nonsense accumulate.  It's a fair
technique, though, and I come away persuaded that the op-ed page is
even more of an ideological free-fire zone than it ordinarily seems.

I find it helps if you understand that Chomsky is an anarchist. His
problem is with government as such, and with the power elites that he
believes run it. Most serious academics find his arguments simplistic
-- the technical term is reductionistic -- because he does not leave
analytical room for the kind of contestation over government that
one sees in real life. Chomsky views this kind of complexity as a
pious hope, a tertiary effect that simply draws attention from the
primary effects that somehow never get past the filters of acceptable
debate. You will have to decide for yourself, of course. Just make
sure that you are not simply filtering out the arguments on the basis
of some automatic reflex, such as labeling him "anti-American" or
swallowing whole the ad hominem of his critics. One of my teachers at
MIT said that "Chomsky wins arguments even when he's wrong", and I've
seen that effect myself. But facts are facts and logic is logic, and
if you're going to disagree with Chomsky's arguments then you need
factual and logical reasons. That's all.

http://www.commoncouragepress.com/chomsky_humanism.html

Not recommended: Rage Against the Machine, The Battle of Los Angeles
(Sony). When Time Magazine declared this its record of the year, it
was 1999's equivalent of Metallica winning a Grammy. Having ignored
RatM as long as I could, and being a resident of their designated
battleground, I decided I had to break down and buy it. One's first
impression, of course, is of the sheer power that is somehow pouring
out of one's speakers. These guys are very talented; they have not
only invented a highly effective genre of rap lyrics that is a cross
between Public Enemy and Bob Avakian, but to my amazement they have
also discovered entirely new things to do with an electric guitar. I
didn't think I would survive my first listening to the record, but
then after my third listening I couldn't put it away.

Having focused my mind on what the innovative lyrics were saying,
however, I've gotten over it. It's too bad that the right-wing fringe
candidates have made such a joke of themselves with their complaints
about this record, since it really is disturbing. Time credits RatM
with a "social conscience", and while a social conscience is certainly
praiseworthy, I wonder if we really need the kind of conscience that
RatM's lyrics represent. Sony will come after me if I quote them at
any length, so suffice it say that they clearly advocate rioting (in
several places), violence ("Violence is in all hands / Embrace it if
need be"), and murder ("So long as tha rope / Is tight around Mumia's
neck / Let there be no rich white life / We bound to respect").

I agree that many of RatM's lyrics are entirely arguable, but still
I have to ask some questions. Easy ones first: we know that Mumia Abu
Jamal did not get a fair trial, and that unfair trials are epidemic
both in Philadelphia and in Los Angeles, but do we know that Mumia
Abu Jamal is innocent? We really don't. Get him a fair trial, make
him a symbol of unfair trials, make him a symbol of unfair trials for
political radicals, but don't make a hero of him. Next question: what
do the royalty checks from this record look like? You can campaign for
justice even after you get rich, but you can't get rich calling for
rich people to be killed.

I look at the RatM promo picture on the back of their CD's lyric
book and I ask, "who are these guys, and who is their constituency?".
I mean, I do support a lot of the causes whose URL's they provide
at the end of their liner notes -- the textile workers' union, for
example -- but do those causes support them? How can they claim to
speak for the oppressed people of Los Angeles when you say things like
"Jesus stripped bare / And raped the soul he was supposed to nurture",
when in reality the great majority of oppressed people in Los Angeles
regard Jesus as the Son of God who came to earth to redeem their sins
and provide them with their principal source of strength and hope in
life? I can understand anticlericalism, especially when the church
sets up a false opposition between straightening out one's soul and
organizing for dignity on earth, but this I can't understand. These
guys didn't get where they are by rousing the oppressed masses, so
who does listen to them? Is anyone really listening to them? And if
so then what are they thinking?  People certainly are oppressed in the
world, and in Los Angeles. But is this kind of hyperbole going to help
them? Is rage ever a useful emotion, or does it simply make you into
part of the problem?

My liberal friends talk around this sort of thing by saying that the
rappers are reporting violence, not encouraging it. I could sort of
buy this for some of the rap lyrics a decade ago that told fictional
stories about urban warfare, but that's not what this is. RatM do
report things, but they don't tell stories. The particular lyrics
I've quoted are clearly presented in the author's own voice. They are
declamations -- not reports, not depictions. They fall just about dead
center in the First Amendment's speech protections, so there can be no
question of censoring them. Disapproving of them, though, is another
matter.

Recommended: Tom Standage, The Victorian Internet: The Remarkable
Story of the Telegraph and the Nineteenth Century's On-Line Pioneers,
New York: Walker, 1998. This is a highly entertaining account of
the cultural history of the telegraph, written so to make evident
the parallels to the cyberspace craze. It's very funny in that way.
It's not intended as serious historiography, but you can read it in
a couple of hours.

Recommended: James C. Scott, Seeing Like a State: How Certain Schemes
to Improve the Human Condition Have Failed, New Haven: Yale University
Press, 1998. The 20th century is a closed book now, and even though
the numbers are arbitrary, they still retain a psychological kick.
When with enough time and distance the history of the 20th century
is written, I think that a central theme will be the rise and fall of
rationalism. Rationalism is not rationality; it is, rather, a false
and superfical imitation of rationality elevated to an ideological
excuse for social control. It comes in both right-wing and left-wing
varietes, as do critiques of it. It originated in the 19th century,
but only during the 20th century did the tools became available to
really put it into practice. And having been put into practice in a
thousand ways worldwide, it was responsible for many of the century's
accomplishments, and for most of its disasters.

Scott's book makes the case for rationalism as the main organizing
theme of the 20th-century state, and indirectly it makes the case
for the critique of antirationalism as the main organizing theme of
20th-century intellectual life. A great deal has thus been written
against rationalism before, and Scott's book, which is based heavily
on secondary sources as well as his own fieldwork, ultimately does
not expand the critique beyond the outer horizon of this substantial
body of work. Along the way, though, it proceeds by the sheer force
of clear writing to make that critique more vivid than it has ever
been. He organizes his story around a single observation: the need
of the rationalist state to make the world legible, that is, visible
to practices of accounting and management that can be coordinated in
administrative centers far from the localities where policies happen
to people's lives. In particular, he observes the recurring pattern
whereby rationalists impose a rectilinear order on the world, partly
to make the world literally visible to the visiting inspectors but
also as a sheer symbol of rational order. For example, his discussion
of Le Corbusier's philosophy of urban planning is devastating, and
it starts with the guy's drawings, which always portray a beautiful
geometric order that would only ever be visible to someone riding in
an airplane. The planned villages of the Soviet Union and Tanzania
were arranged likewise, with little regard for the terrain they rested
on or the practicalities of social life or agriculture within them.

These examples represent the mature and baroque form of rationalism.
But Scott also tells an even more compelling story about the origins
of rationalism in the necessity of tax extraction in the absolutist
states of 18th century Europe. This period of ceaselessly Darwinian
tribal warfare was been exactingly described by Perry Anderson in his
outstanding "Lineages of the Absolutist State" (Verso, 1974), but for
Scott it is a tale not of huge structures but of the small things of
local knowledge and practice that were flattened out by the war-fueled
drive to collect taxes from them. A traditional agricultural system
might divide plots of land into numerous strips that are cultivated
by different people in different seasons, but the administrative
systems of the 18th century were incapable of collecting taxes
unless good-sized hunks of land are assigned to particular people in
a stable way. The resulting rearrangement of land into neat parcels
may have been nonsense in agricultural terms, but they made sense on
paper. Scott tells a similar and especially fascinating story about
surnames, which despite their seeming antiquity were (he argues)
actually invented and assigned by modern-day administrative
convenience and not by venerable local custom. In each case the logic
is the same: those absolutist regimes which rendered their realms
legible succeeded, and those that did not failed.

The rise of the absolutist state, then, was in many ways a vindication
of rationalism. Agriculture may have suffered, but the relative
weakness of the state's powers of representation and coercion
meant that crops got grown even as taxes got collected and wars got
fought. No wonder, then, that the nouveau absolutist regimes of the
20th century should have sought to follow the pattern. They failed
because they succeeded in their aims: the more administratively
legible their societies became, the more they fell apart. Nor were
the methods of rationalism confined to the totalitarian world; Lenin,
after all, got his rationalism from the United States, and Scott
tells remarkable stories of American and Soviet agricultural planners
happily communing in hotel rooms as they planned the communes of the
rationalist future.

For Scott, the story ends with the collapse of rationalism and the
vindication of local knowledge and local practices over the assaults
of the hubristic planners. But for me, Scott's story does not reckon
with the very real successes of rationalism, which he notes along
the way but cannot digest. I think that Scott's story can be usefully
complicated by combining it further with Anderson's. For Anderson,
absolutism was a necessary waystation on the path from feudalism
to capitalism, and he concludes his book with a striking analysis of
the differences between the Japanese and European forms of capitalism
in terms of their different forms of feudalism and of Japan's failure
to consolidate an absolutist state before moving along to capitalism.
Older social forms, he argues, persist in the new.

We can look at Scott's book as supplying a missing piece of this
story.  Absolutism was not just the apotheosis of the state; it also
consolidated enough centralized power to impose a uniform regime
of representation on the whole society, and then this in turn was
a prerequisite of a functioning market. The metric system is a good
example: only an absolutist state would be capable of imposing it,
only an ideologically rationalist state would think of imposing it,
and only once it was imposed could it reduce transaction costs enough
to generate a critical mass of market activity. Once we get beyond
the simplistic opposition between "centralized" and "decentralized"
that structures both Scott's quasi-anarchism and the ideologies of
the market, we can see that markets in fact represent a complicated
compromise between the two. Properly functioning markets honor the
locality of rational choice, but they only function properly if enough
of an institutional grid has been laid down to make trade practicable
among an unbounded number of parties who are not ritually bound to
one another. The pattern continues to the present day: the government
pioneers new forms of representation and interconnection, and then it
privatizes them. Markets want transparency and uniformity -- "perfect
information" -- and in this imperative they are the natural allies of
government, not its opponents.

Some URL's.

Linux and DeCSS: What the MPAA is Really After
http://www2.linuxjournal.com/articles/currents/016.html

valuing the AOL / Time Warner merger
http://www.pathfinder.com/fortune/2000/02/07/loo.html

opting out of Doubleclick cookies
http://www.doubleclick.com/privacy_policy/privacy.htm

Scientology opponents set up shop in Clearwater
http://www.sptimes.com/News/020600/TampaBay/How_much_oddity_can_o.shtml

Scientology critics' extensive online video gallery
http://www.xenutv.com/

alt.religion.scientology Web Page Summary
http://members.home.net/jmwood1/arsweb.html

National Geographic's Map Machine
http://plasma.nationalgeographic.com/mapmachine/

GPS implants
http://www.newscientist.com/ns/20000108/newsstory8.html

the record companies are freaking about this
http://www.napster.com/
http://www.salon.com/tech/col/rose/2000/02/04/napster_swap/

IETF Policy on Wiretapping
http://www.ietf.org/internet-drafts/draft-ietf-iab-raven-00.txt
http://www.wired.com/news/politics/0,1283,34055,00.html

new magazine of political journalism
http://www.americandispatches.com/

Digital Arts and Culture conference, Norway, August 2000
http://cmc.uib.no/dac/

environmental networking conference, San Francisco, May 2000
http://www.planetworkers.org/planet.html

end
```