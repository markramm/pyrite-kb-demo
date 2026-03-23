---
id: notes-and-recommendations-for-17-june-1997
title: "Notes and Recommendations for 17 June 1997"
type: writing
writing_type: paper
date: 1997-06-17
url: "https://pages.gseis.ucla.edu/faculty/agre/notes/97-6-17.html"
coauthors: []
key_concepts: []
importance: 5
research_status: stub
tags:
  - paper
  - auto-imported
---

## Source

Automatically imported from: https://pages.gseis.ucla.edu/faculty/agre/notes/97-6-17.html

## Content

```
Some notes.  This month I've been darned to heck for many small sins, to
which I shall confess below.  I need a vacation.

The FTC privacy hearings were useful enough, I suppose, but they also
pointed out the sorry state of public discourse on privacy policy in
the United States.  Polls and other media discussion tended to focus
on questions of whether businesses should be able to capture information
through their Web sites.  This is a highly tendentious way of phrasing the
question, since it's very extreme to say that business should be prevented
from capturing any information at all.  What's missing from the discussion
is the Fair Information Practices that are the basis of privacy policy
through virtually all of the industrial world, except of course for the
United States (the anemic public-sector Privacy Act aside).  The initial
question is not whether information should be captured, but what the
ground rules should be for such capture, e.g., notifying users of one's
privacy policies.

Once those basic rules have been established, it then becomes possible
to ask more sophisticated questions about how that information is defined,
and specifically the exact architecture of social identity in these
systems.  Is everyone anonymous?  Does everyone have a pseudonym that
cannot be linked to identifiers in other databases?  Under what conditions
can electronic payments be tracked back to a payer?  That sort of thing.

Some will say that these matters are highly technical and that the public
can never be expected to understand them.  I disagree.  In my opinion,
the root of the problem here is the client-server model.  This model began
life in institutional settings where the boundary between the client and
server had no legal or moral significance, either because nothing of any
great sensitivity passed across it or because both client and server were
wholly owned by the same power.  The reason we have all these wild rumors
about "cookies" is that the user interfaces for Web browsers do not make
the browser-server boundary visible.  That boundary is not even part of
the Web's organizing metaphors, and as a result some important legal and
moral transactions happen in an obscure space that has not been made at
all transparent to users.  This is a design and interface problem, not a
frailty in the minds of the users.

The misunderstandings about cookies are especially unfortunate given that
cookies -- as currently implemented -- actually embody a very good default
compromise on privacy.  Although the interface doesn't communicate this
very well, a Web site doesn't know who you are unless you tell it.  You
can navigate a Web site all day, and the Web site designer can trace your
path (for example, to help in redesigning the site for more efficient
navigation, or to see which advertisements lead to which hyperlinks
being clicked) without knowing who you are.  Even when you do establish
an account with a site, it is still very easy to enter false information.
A Web site designer who really wants to link your information with other
databases (for example, to authenticate actions that really require you
to be who you say you are) is obligated to put you through a cumbersome
procedure, such as e-mailing you a confirmation at your claimed e-mail
address.  This kind of protocol chases users away, and so site designers
are motivated to avoid such protocols unless they are really necessary.

Our fears about personal privacy on the Web, therefore, can be neatly
divided into two components.  On one level, it is a complete and total
no-brainer that the Fair Information Practices should apply to Web sites,
just as they should apply to all other significant and systematic captures
of personal information in society.  On another level, we should concern
ourselves with the model of identity that is embedded in Web browsers and
Web sites.  That model is currently quite good, actually, and we mostly
need to make that already good model more visible to users.  The most
serious concern pertains to the future.  Web browsers and sites need to
evolve toward architectures of identity whose demands for identification
are proportionate to real needs, and not just for purposes of targeting
that people have not explicitly consented to.  It is not enough to require
all users to identify themselves fully and then simply observe that use
of a site is "voluntary".  Instead, over and above the Fair Information
Practices, we need to understand the full spectrum of intermediate forms
of identification, and to make social judgements about which kinds of
demand for identification are appropriate in which settings.  It might
seem like an overly abstract discussion to be having, but the discussion
has already started in the rest of the industrial world.  It's only the
United States where such concepts are still strange.

We spend lots of time spinning futuristic technological scenarios.  These
scenarios, though, usually flout an important principle of technological
change: technological changes, if they have any significant consequences,
are always part and parcel of institutional changes.  The technologies and
institutions coevolve, and if we focus our attention wholly on machinery
then we will be twisting an inherently helical path of development into an
unnaturally straight line.  We've been doing way too much of this, and it
has fouled up our imaginations.  To redress the imbalance, we should spend
some time imagining new institutions.  That is, instead of starting with
the internal logic of technical develop and extrapolating it, let's start
sometimes with the internal logic of institutions.

Many people find it hard to imagine institutions, of course, because they
think of institutions solely in terms of phoniness and constraint; those
people often align themselves with what are essentially theological views
of technology and its supposed impact on society.  Maybe you're feeling
it now: the powerful sense that technology will surely sweep away all
institutions and replace them with completely new ones, or with none at
all.  A more mature and realistic approach is to comprehend the positive
aspects of institutional logic and ask how technology can help people to
reinforce those aspects and alleviate the others.

I'll start with an aspect of my own favorite institution: graduate school.
Graduate school is a good thing, and I think we should keep it regardless
of what all the fashionable think-tank anti-intellectualists say.  Going
through graduate school means getting a new identity: shifting from
the anonymous identity of undergraduate life to the unique professional
identity that one acquires by presenting one's research in public.
That's a painful transition, and good graduate schools try to smooth it.
One common part of this transition is making the students write a survey
paper: a paper that summarizes and interrelates "the literature" -- all
of the work that has previously been written on some topic.  It's a great
exercise because you're both contributing to scholarship and mapping out
the intellectual territory in which you're planning to locate yourself.

Some of these graduate student survey papers are very good.  Unforunately,
in the paper-based system we have now they mostly just get filed away.
I think we should put them all on the Internet.  Let's ask some librarians
to fashion a standard for these documents and their cataloguing, indexing,
and management.  At one level we'd want to evolve a genre for these survey
papers, with somewhat standardized kinds of language and notation.  Then
at the next level we'd want formatting templates so that the papers look
alike and afford the same kinds of automatic processing.  For example, we
could use SGML (assuming that SGML doesn't croak) to give each field its
own templates.  Or we could follow the technical fields and use LaTeX and
postscript, with automatic (and hopefully much improved) HTML generators
for online viewing.

Each survey paper would go through a formalized refereeing process.  For
example, the paper could be made available in draft form to the author's
local research group first, then to a specified broader circle of friends,
and then finally to public comment.  Each field would have its own editor
of surveys, just as journals have editors now, and this editor would ask
for anonymous referees' comments in addition to the public comments.  The
paper might be revised several times before being officially published,
and the publication date would mark a new graduate student's official
debut into the research community.

Once online, the survey papers would be searchable by automatic tools,
starting from the topic or authors, or working backwards from particular
citations.  They would be given their own catalog entries and included in
online library catalogs.  The catalog entries would be hyperlinked to the
papers themselves, and the papers' citations would be hyperlinked to the
catalog entries for the publications they represent.

Taken together, the technology and institution of the graduate student
survey papers would become a pivotal resource for the world of research.
The papers would be extremely numerous, and they would be easy to find.
Barriers to entry into a research community would be greatly lowered,
since someone wishing to conduct research in a new area would simply
be able to fetch the appropriate surveys from a well-known location.
The surveys themselves would be extremely numerous, given that thousands
of graduate students write these things every year, and students would
be challenged to define their survey areas in new ways.  No longer would
it be necessary for a hundred graduate students to write survey papers
on the sociology of organizations, although it wouldn't hurt to have ten
such papers, written from different conceptual or national perspectives.

Best of all, the graduate students themselves would acquire well-defined
identities fairly early in their graduate careers.  It would then be much
less painful to submit one's first conference paper, currently a source of
tremendous anxiety for many students.  Students would have a standardized
mechanism for getting feedback before their work was released to the whole
world, thus alleviating the equally extreme anxiety of publishing work
that -- surely, one always thinks -- will get brutally shot down in public
by some powerful researcher.  Of course, everyone will look back and wish
that their public survey paper was stronger.  But that's okay; once you've
started your career and obtained your unique professional identity you can
focus on the future, building professional relationships and presenting
new and better work to bigger and friendlier audiences.  Many people never
make it through that transition because it's just too daunting.  I want to
change that.

Several people wrote to argue that, contrary to what I wrote, amazon.com's
mailings to its customers shouldn't be regarded as spam because they fall
in such a clearly separate category from the forged-headered messages from
Joe's XXX Porn.  I don't think it's a useful exercise to try defining the
word spam, not least because it opens the door to the fog-creation devices
of spam's defenders.  What does matter is what definition gets written
into law.  Since the issue pertains to speech, any law should obviously be
written as narrowly as possible.  Both of the bills in Congress clearly do
not outlaw commercial e-mail within the bounds of an existing commercial
relationship, and this seems reasonable.  It's easy to imagine abuses when
the "commercial relationship" is very minimal, for example when all you've
done to initiate this "relationship" is ask for product literature.  Even
so, your capacity to exact revenge in such cases is clearly much greater
than with Joe's XXX Porn right now.

Other people complain that bills that outlaw unsolicited commercial e-mail
do not outlaw noncommercial e-mail nuisances, such as the recent spam of
passages from the Bible.  The fact is, however, that only commercial mail
has caused a major nuisance so far, and laws restricting speech should be
closely tailored to real and proven nuisances.

Another objection is that laws against unsolicited commercial e-mail could
be construed to apply to messages whose "commercial" content is marginal
or incidental, such as a newsgroup posting by Company X's employee that
adds further facts to some other posting's praises of Company X's product,
or an unsolicited personal message that includes a company affiliation and
slogan in a signature file.

It's good to accumulate these scenarios, but it's not okay to use them to
create fog.  The whole point of law is to consider all of these cases and
make a theory that defines the real offense, so that the laws regulate the
right things.  What we need now is serious legal theory about the issues
surrounding spam.

The US government wants to disburse federal benefits electronically.  For
details see  http://www.fms.treas.gov/ebt/ebt.html

Recommended: Mark Casson, Information and Organization: A New Perspective
on the Theory of the Firm, Oxford: Clarendon Press, 1997.  By assuming
that markets happened pretty much by magic, traditional economics ignored
information.  The fog is lifting, though, as the hard-bitten dogmas of
neoclassical economics have become increasing embarrassments in an economy
whose urgent questions swirl around information and its technology.  The
main alternative to neoclassical equilibrium analysis of the firm has been
transaction cost analysis, as developed by Coase and Williamson; despite
its many clearly demonstrated problems, many people (myself included) have
employed transaction cost analysis in their research on the institutional
dimensions of information technology for lack of anything better.

That situation is changing, fortunately, and Casson's "Information and
Organization" is the best synthesis so far of the emerging alternative.
Markets cannot function without producing and circulating vast amounts of
information, Casson points out, and so economics ought to engage in dual
analyses of both material flows and information flows.  Markets change
historically in their structure, and these changes can be explained
largely in terms of information costs; as information costs go down,
reality actually begins to resemble, however faintly, the neoclassical
idealization.  Consequently, everyone whose life is affected by electronic
commerce should read this book.

If Casson's book doesn't hit you squarely between the eyes, put it
down for a minute and prepare yourself by reading Lisa Bud-Frierman's
tremendous edited volume "Information Acumen: The Understanding and
Use of Knowledge in Modern Business" (Routledge, 1994).  Another helpful
reference is William H. Melody, Information: An emerging dimension of
institutional analysis, Journal of Economic Issues 21(3), 1987, pages
1313-1339.  Also Arthur L. Stinchcombe, Information and Organizations,
Berkeley: University of California Press, 1990.

Also recommended: Robin Mansell and Roger Silverstone, eds, Communication
by Design: The Politics of Information and Communication Technologies,
Oxford: Oxford University Press, 1996.  This is a dense and serious volume
on the institutional organization of technical design, with a special
focus on interaction between designers and users.  Most of the papers come
from the very strong research groups on technology and community at the
University of Sussex.  Many myths are exploded here, my favorite being the
really strange idea that open standards necessarily prevail in electronic
commerce, and that electronic commerce therefore necessarily levels market
playing fields.

Having presented a qualified argument in my last notes against usage-based
pricing of Internet router capacity, I should cite a brief, accessible
summary of the arguments in favor of such schemes: Jeffrey K. MacKie-Mason
and Hal R. Varian, Some FAQs about usage-based pricing, Computer Networks
and ISDN Systems 28, 1995, pages 257-265.  I do have one complaint about
this article: it does not distinguish consistently between pricing the
use of individual servers, a thoroughly decentralized mechanism which does
not affect the basic architecture of the Internet, and pricing of packet
routing, which has pervasive consequences for the architecture.  It seems
to me, as I pointed out in my notes, that congestion of particular servers
is a completely different issue from congestion of the packet-switching
network.

(I find it puzzling, by the way, that I have never heard anybody discuss
congestion of domain name servers in economic terms.  That seems like
easily the most remediable of the bottlenecks that disrupt my own use of
the Web, particularly given that -- like many people -- I avoid loading
images as much as possible.)

I would also emphasize that MacKie-Mason and Varian, who are serious
economists, only advocate usage-based pricing to support the variable
costs of running the Internet, not the fixed cost.  Moreover, as they
point out, almost all of the costs of running the Internet are fixed
costs.  At the same time, they suggest that the revenues from usage-based
pricing be used to create new capacity.  I do not understand the rationale
for that suggestion.  It seems like, by their own logic, new capacity
should be funded through the capital markets, with the investors getting
their money back once the new capacity is online and the new fixed-rate
fees start rolling in.

Recommended: Sharon Eisner Gillett and Mitchell Kapor, The self-governing
Internet: Coordination by design, in Brian Kahin and James Keller, eds,
Coordination of the Internet, Cambridge: MIT Press, 1997.  Available on
the Web at http://ccs.mit.edu/CCSWP197.html .  This is a good introduction
to the Internet's governance mechanisms, with a clear emphasis on keeping
those mechanisms as decentralized as possible.  While I certainly agree
that the Internet's culture of decentralization and interoperability etc
is a good thing and worth preserving, I would also argue that the kinds of
formal mechanisms and cultural values that Gillett and Kapor describe are
only one fairly weak force in favor of keeping the Internet decentralized.
If the Internet is a natural monopoly -- a concept that many people simply
dismiss out of hand with no substantive argument -- then that force will
be swept away sooner or later unless some other, greater force -- like big
bad government -- becomes aligned with it.

Bad news: Jeff Buckley, whose fabulous album "Grace" I recommended here
a while back, drowned in a swimming accident in Memphis the other day, a
couple weeks before he was scheduled to begin recording his second album.
Bummer.  Good news: Dick Gaughan, whose fabulous album "Handful of Earth"
I recommended the other day, is also (as one of RRE's fabulous readers
has pointed out to me) a computer geek.  His home page can be found at
http://www.dickalba.demon.co.uk/index.htm

It seems you're not a popular music critic until you've persuaded your
readers to listen to the British guitarist Richard Thompson.  Get thee
right out, therefore, and buy the eloquently sad "Pour Down Like Silver"
(Carthage, 1983), the best of the records that Thompson made with Linda
Thompson during their fouled-up marriage.  I tend to prefer Thompson's
acoustic songs to his more raucous and frivolous electric side, and
"Pour Down Like Silver" explains very carefully why the acoustic guitar
was invented.  The best passages, as in the closing instrumental piece,
"Dargai", somehow communicate whole worlds in single notes.

Of his other work, my favorite song is the very funny melodrama, "1952
Vincent Black Lightning", from 1991's amusing but not-quite-profound
"Rumour and Sigh".  I was living in England when it first came out, and
I remember John Peel and Andy Kershaw fighting over which of them would
get to play it first.  Music hasn't quite died out yet.

I keep trying to lay off Microsoft, but they won't let me.  For example,
the 6/9/97 issue of Fortune quotes Bill Gates as follows (page 136):

  "IBM has decided that this market [groupware for corporate intranets]
  is strategic, meaning that they are willing to take noneconomic returns,
  hoping it will help them imagewise or marginwise in other businesses.
  Microsoft has decided that Exchange is 'strategic'.  This means we are
  willing to take noneconomic returns.  So you'd call this space hyper-
  competitive between IBM and Microsoft.  It is kind of surprising to have
  somebody else [i.e., Netscape] come along and say, 'Oh, yeah, me too'."

"Noneconomic returns", of course, is a euphemism: Gates is saying that
Microsoft is willing to take a loss to ensure that its appalling Exchange
program is adopted as a de facto standard in the corporate groupware
market.  (Whether it's really Exchange that they keep pushing, or some
other Outlook-based mailer, doesn't much matter.  In fact, that just
restates the problem.)  This particular market is distinctive, of course,
in that Microsoft is competing against a company with a similar capacity
to take losses.  The point, though, is that the software market has
evolved to the point where it is impossible to compete without huge cash
reserves to use in undercutting competition.  Venture capitalists are
now said to evaluate new PC software start-ups purely in terms of the
likelihood that Microsoft will buy them.

In the old days when the most famous commodities in the marketplace were
oil or steel -- and even when they were memory chips made by Japanese
companies -- this practice of deliberately taking losses for competitive
purposes was regarded as the very definition of an anti-competitive
practice.  In this case, the purpose of a loss-taking strategy is clear
enough: once a de facto standard becomes entrenched in the marketplace,
its owner can then leverage it to extract monopoly rents, and to gain an
advantage in selling other kinds of software that benefit from integration
with the standard.

Now, my own analyses of Microsoft's rapidly expanding dominion have almost
entirely avoided this language of "anti-competitive practices", which has
been central to most other analyses.  Partly this is because the issues
run deeper than that: because software has such different properties from
oil and steel, and even from memory chips, it is quite possible in theory
to establish a monopoly without coming close to the classical definitions
of anti-competitive practices.  But more to the present point, even when
those definitions seem to apply, the whole theory of antitrust is so
tied to the properties of traditional commodities that it does not yield
many legally actionable consequences -- as the US government learned a
few years back to its embarrassment (see the article on this subject by
Francois Bar et al that I cited in TNO 3(2)).  You can't reduce market
shares in the PC operating system market, for example, just by breaking
Microsoft into several pieces, the way that Standard Oil was broken up a
hundred years ago.

On the general subject of opposition to Microsoft, the Boycott Microsoft
site, which I haven't investigated well enough to either endorse or not
endorse, is  http://www.vcnet.com/bms/

Just one more swipe at Microsoft.  You've probably seen their ads lately
promoting the idea of the personal computer.  Everyone assumes that they
are trying to ward off the threat of network computers -- at least the
ones that do not run Windows.  It's really interesting that a company is
spending huge sums of money simply to promote an abstract concept about
the relationship between human beings and computers.  The real shame is
that it's a lousy concept.  The whole idea of the personal computer was
fouled up from the start, because people do not work in isolation from one
another.  People are social animals; they think together and they share
things.  Personal computers, are Rob Kling pointed out long ago, are used
by people who are located within a whole web of relationships, not least
the relationship to their coworkers and system maintainers.  The whole
problem with viruses originated with the first personal computers' lack
of a coherent model of the social relationship between the user and the
software on her machine.

The bogus idea of the personal computer is responsible for the singularly
unilluminating flap between the ActiveX and Java models of security for
software downloaded from the Internet.  ActiveX carries insurmountable
security problems because it offers the user no defenses at all against
bad behavior by downloaded software, besides someone's vague promise that
such things wouldn't happen.  Java is famous for addressing this problem
by enclosing downloaded software in a "sandbox" that restricts its ability
to grab hold of the machine's innards.  As the Microsoft people gleefully
point out, however, this restricts the functionality of Java applets to
relatively trivial applications.  Microsoft owns the operating system, and
they will happily explain the advantages of close integration between the
operating system and the applications programs.  It follows that the Java
model will have to replicate many of the functions of an operating system,
or that it will have to create a more sophisticated platform-independent
interface between the applets and the operating system.  This is pretty
much of a contradiction in terms, of course.

It's important to understand how Microsoft benefits from the primitive
technology of its operating system.  I hope that I will not show my age
if I suggest that this new generation of Internet-centric computer people
might benefit from having a look at an ancient operating system called
MULTICS.  You've heard of MULTICS -- a timesharing operating system for
mainframes.  We all grew up being indoctrinated into the anti-mainframe
religion, of course, but now we've subjected the whole world to the evils
of the opposite extreme -- a model of computing which lacks the most basic
conception of how to permit multiple processes to operate simultaneously
inside a computer without trashing each other.  Yes, computer security
people know all about this stuff.  But they're just powerless to help
us, because we've all become locked in to antisocial technologies that
simply don't work.  Social creatures need protocols to safely negotiate
gradually increasing levels of interaction and intimacy with one another.
That's what normal social interactions are all about.  And yet, if I may
risk invoking a stereotype here, it is as if the whole personal computer
model was designed by people who never had any experience of such things.

Okay, here are my minor sins for the last month or two...

  * I used the term "attachment" inaccurately, it seems, in a
    complaint about the Microsoft Exchange program. The problem --
    spurious mail to me -- was, or so it was explained to me, caused
    by a new feature for creating hyperlinks to mail messages. I think
    that this feature is just as bad as the nonexistent one that I
    complained about, but I'll let it go.

  * When I sent out the press release on Internet naming issues by
    the Association for Interactive Multimedia, I took for granted
    that it was (as one person put it) unhinged ranting. I've now
    been thoroughly informed that not all Internet users found this
    self-evident. I sent it out primarily because I found it so
    interesting that an organization with such a large corporate
    membership was carrying on in such a fashion. When I said "I have
    no opinion about this", I meant something more like "I don't want
    to get involved in this". Fat chance. I've asked an IANA guru to
    write a formal rebuttal, and I'm hoping he'll deliver so we can
    get the record straight.

  * The long message on the FTC spam hearings by Keith Lynch suggested
    that some connection be drawn between the fatness of the major
    spammers and the evilness of their behavior. I have been duly
    chastised for having contributed to such stereotypes. People do
    seem to have a range of opinions about how responsible I am for
    the content of the messages I send to my list. I send things out
    because I find them interesting, and I do not endorse them unless
    I say so explicitly. Many people, however, believe I effectively
    endorse a message by the simple act of sending it to my list. I
    don't know if they have any philosophy behind this view, or if
    they're just mad.

  * I mentioned switching from amazon.com to www.altbookstore.com
    after the amazon.com people started sending me unsolicited
    commercial email. My recommendation of altbookstore was based on
    my students' positive experience with them. My own experience,
    however, was not so happy. That $100+ order I mentioned was
    a mess. They charged my credit card for the money in mid-May,
    and it was only in mid-June, after several phone calls and some
    increasingly strident legal threats, that I got anything back
    from them beyond vague excuses. What a nuisance.

  * In my note about the dramatic deterioration of domain name
    service, I spoke of the old days "when the government did it". Of
    course, the government never literally serve domain names itself;
    what I meant to say was "when the government controlled it". What
    we have now is the worst of possible worlds: an unaccountable
    monopoly that can charge whatever it likes without any incentive
    to run an efficient service.

  * While I'm confessing my minor sins here, in a book review in
    Wired a couple years ago, I mocked the idea that "IBM can be saved
    simply through a fanatical recommitment to its original vision".
    From what I can tell, though, that's pretty much what they did.
    Sometimes the hype is right.

Going back through my other recent RRE messages, I now recall that
several others have drawn flames from people who claim to be big
friends of RRE for all other purposes. Such friends.

As my book on the metaphors of artificial intelligence was going
to the printer, I noticed an awful editing error in the very first
paragraph. This is what happens when you're beating your brains out
trying to finish a book by a deadline. Or perhaps it's simply there to
keep me humble, in which case it worked. The subject was the history
of cybernetics, so while I waited to discover whether the printers
were going to be able to fix the problem in time (no), I resolved to
locate another round of scholarship on the subject. In doing so, I
came across two interesting and intellectually sophisticated analyses
of the subject that I wish I had encountered in time to cite them in
my book:

  Geof Bowker, How to be universal: Some cybernetic strategies,
  1943-70, Social Studies of Science 23, 1993, pages 107-127.

  Peter Galison, The ontology of the enemy: Norbert Wiener and the
  cybernetic vision, Critical Inquiry 21(1), 1994, pages 228-266.

Each article describes how cybernetics got generalized in very few
years from a (not very effective) technology of automatic antiaircraft
fire to a science of the entire universe.  Bowker argues that this
generalization was both rhetorical and political, inasmuch as it
provided the occasion for entirely new modes of research funding.
Galison argues that the original metaphors of Wiener's antiaircraft
work, which were predicated the moment-by-moment exchange of tactics
with a distant but intelligent enemy, were carried through in a coded
form to the whole vast range of later applications of cybernetics.

The two articles raise the question of how much of a technology's
original meaning gets generalized to other applications.  Conventional
computer system design, for example, is clearly derived from
traditional industrial automation methodologies. Does that mean that
personal computing in the home, or intelligent transportation systems
on the highway, necessarily incorporate or encourage the same kinds of
social relationships as in the early 20th century American factories?
It's a nontrivial question, and it takes heavy intellectual lifting to
draw the line between "yes" and "no".

Critical Inquiry, by the way, is pretty much the smartest of
intellectual publications in English. We hear a lot of propaganda
about the supposed decline of scholarship, all of it drawing on real
but marginal cases of excessive academic exuberance or politically
motivated caricatures and distortions of serious work. The fact is
that we're living in a golden age of scholarship right now, not least
because of cheap airplane tickets that permit scholars to travel
to archives and meetings, and Critical Inquiry is one journal
that maintains high standards of both erudition and rigor. Whereas
most journals serve the social function of archiving the necessary
increments within well-established disciplinary projects, every
article in Critical Inquiry actually has an interesting new idea.

My friends in AI were jubilant over Deep Blue's victory in its match
with Garry Kasparov. Although Kasparov is a pissy loser, I was sad
to see him lose anyway, largely because I was hoping to postpone the
bad philosophy we've had to suffer through lately. The AI people are
particularly jubilant because Hubert Dreyfus, in his much-reviled
anti-AI tract "What Computers Can't Do", effectively predicted that
computers cannot play good chess. If you read the whole book, and
then reread the passages that are specifically about chess, then it is
clear that he meant simply that computers cannot play chess the same
way that people do.  Unfortunately, Dreyfus clearly did not understand
heuristic search, the technical method which all serious chess
programs have used. This doesn't affect his real argument, since
heuristic search bears little relationship to human players' methods.
If he had understood heuristic search, then he could have sharpened
his claims and a whole very elaborate thirty-year farce of a
philosophical argument could have been avoided.

Normal people seem to be having difficulty understanding the
philosophical significance of Deep Blue's victory, and in my opinion
that's because there isn't any. Game 2 did give a sense of what
superhuman chess might be like, and I look forward to seeing how the
machine plays when they double the processing speed again. But we're
already well accustomed to machines that exhibit superhuman strength,
speed, and calculation; superhuman chess-search ability is just
another step along. The people who invented heuristic search thought
it was univerally applicable, and some of them still do, but the fact
is that heuristic search has only proven really useful in applications
that closely resemble chess.

Kasparov does have some valid points. He's right that they should have
played the machine in tournaments before challenging the champion.
That way he wouldn't have had to spend the first few games trying to
figure out how the machine played. That is an unfair advantage, and
he should have imposed such a restriction before he agreed to the
match. Even so, the bottom line in my view is that Kasparov defeated
himself, and that he did so in the way you would expect from Star
Trek. The guy is famous for the tornado of negative vibes that he
exudes during a match. This time, however, those vibes had nowhere to
go, so they bounced back on him and messed up his mind. He got what he
deserved.

Recommended: Chris Freeman, The economics of technical change,
Cambridge Journal of Economics 18, 1994, pages 463-514. A good survey
article on studies in the (very broadly and heterogeneously defined)
Schumpeterian tradition of economics. (You may recall that Schumpeter
is the patron saint of entrepreneurs.)

Public Citizen's Global Trade Watch has begun a Campaign of Inquiry
to remove the veil of secrecy from the very radical Multilateral
Agreement on Investments that has been negotiated within the OECD
since 1995 with virtually no citizen input. For details see
http://www.citizen.org/gtw

Some more resources on MAI are

  http://www.islandnet.com/plethora/
  http://www.geocities.com/athens/3565/nomai.html
  http://www.policyalternatives.ca/mai.html
  http://www.tao.ca/earth/lk97/

An OECD report entitled "Information Infrastructure Convergence and
Pricing: The Internet", published a year ago but still interesting,
can be found at http://www.oecd.org/dsti/gd_docs/s96_xxe.html

Someone sent me a list of e-mail addresses of accused spammers. I was
naturally tempted to broadcast it to the entire list, but the pitfalls
of that plan should be pretty obvious. It's probably a good thing that
vigilantism needs to be organized in a more decentralized way than
that.

I've noticed many subtle positive consequences of the Web. One of
them is that people interviewing for jobs are much better informed
than they used to be. When I interviewed for my current job at UCSD
in 1991, I was not able to obtain even a simple list of the faculty in
the department before I arrived for the interview. The last few people
who have interviewed for jobs in my department, by contrast, have
shown up in my office with an encyclopedic knowledge of my background,
which they got from my Web pages. This is good, even if it's a little
creepy to have someone actually know everything on my Web pages.

Check out this weird thing called InterGOV, which poses as a kind of
world government of the Internet -- http://www.intergov.org/ . It's
interesting the phenomena you get when anybody can make Web pages
overnight to present themselves as anything they want.

A few months ago, some RRE subscribers were kind enough to offer
comments on the latest round of my students' studies of current or
prospective Internet user communities. Some of their finished projects
are available online through the class pages:
http://weber.ucsd.edu/~pagre/111-home.html

The big news in personal computers these days is laptops for under
$1000. I think that's great. In fact, I have a laptop that I bought
for $900. I even wrote 200 pages of my book on it. I bought it in
1989. It's a Toshiba T-1000, and it has the best keyboard I've ever
used. It has no modem, just a serial port, but I could have gotten
a modem for $150 if I had wanted to read my e-mail even more than
I already do. It only has 512K of memory, but that has never been a
problem because the program I use 99% of the time is Emacs, a powerful
text editor that occupies such a small part of 512K that I have room
left over in memory for about 100 pages of text as well. What's my
point? My point is that laptops could have cost less than $1000 all
along if our software wasn't so grotesquely bloated and nonmodular.
It will be objected that my T-1000 doesn't have a hard drive. But
the only reason why personal computers need hard drives is that no
high-capacity floppy-drive format has become established yet, and
the main reasons for that are institutional and market dynamics, not
technical limits.

We are constantly told that technology is endlessly revolutionized
for the better, but that's not really true. Some aspects of the
technology do get steadily better -- hardware whose external behavior
is standardized and software whose functionality had not formerly
existed. But other aspects of the technology improve at glacial rates
or not at all -- operating systems, for example, or software that has
been standardized in such a way that its external behavior cannot
change without breaking everthing else. Multics was a better operating
system in many ways than what most people use today.  My point is not
that anyone is bad or stupid, but that we should ditch the big
generalizations about the progress of technology. Instead we should
analyze things case-by-case, keeping watch for cases of technological
lock-in that retard progress or create perverse incentives that make
things worse.

As a prime example of technological lock-in, I nominate the basic
Internet electronic mail protocol, SMTP.  SMTP is well over 100 in
dog years and close to prehistoric in Internet time. Its shortcomings
underlie many of the Internet's worst problems, for example the
ease of forging headers and the consequent difficulty of meaningful
screening of spam. It cannot change significantly without breaking a
thousand applications. By far the most significant change to Internet
e-mail is MIME. Nathaniel Borenstein and the other people who pushed
MIME through are heroes, not principally for their undoubted technical
genius but for their diplomatic skills -- building consensus around a
simple mechanism that permits complex data structures to be included
in e-mail messages. But MIME is the exception that proves the rule:
it is built on top of SMTP; its codes are included in SMTP messages,
and the many e-mail programs that do not recognize them, instead of
blowing up, simply display them in their raw form to the user.

This is why I'm happy about the various next generation Internet
projects. Instead of trying to extend the mess we have now, they're
starting over fresh. Once the academics develop and exercise the new
protocols in all of their shiny broadband glory, maybe we can imagine
transitioning all of the worthwhile activities from the crummy old
Internet to the new network.  I don't even know if that's anyone's
plan, but it would be a good plan. At the same time, if that is the
plan then everyone should be concerned with the philosophy that's
embedded in these next generation architectures. Are the Internet
principles of decentralization still in force? Will the systems lend
themselves to low-overhead operation, or will their economics or
architectural presuppositions (or both) tend to impose the overhead
and hassle of detailed accounting for every packet that goes by?
Etc.

Can I ask users of Pegasus Mail to conduct an experiment for me?
I have had two reports of this program's "forward" command generating
misleading headers that cause me to receive misdirected e-mail. The
problem seems analogous to the problem with the "redirect" command in
Eudora: if you use the command to pass a message along to someone else
who uses Pegasus Mail, and they reply to it, the reply unexpectedly
goes to the person who originated the message, not to the person who
sent it along. If anybody can validate this behavior and figure out
exactly why it happens (i.e., what bad header entries it creates) then
I would be most grateful. If this behavior doesn't happen with the
"forward" command, maybe it happens with some other command? Perhaps
the behavior depends on the (somewhat complicated) headers on RRE
messages? Documentation of any such problem, together with contact
information for whoever is supposed to maintain the program, would be
most helpful. Thanks a lot.

Worldwide radio stations on the Internet:
http://www.brsradio.com/webcasters/stationsinter.html
http://www.ontheair.com/

New Telecom Quarterly is a serious industry-oriented journal that
crosses the lines between traditional telecom thinking and digital
information infrastructure.  http://www.ntq.com

end
```