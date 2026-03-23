---
id: rre-surveillance-crypto-etc
title: "[RRE]surveillance, crypto, etc"
type: writing
writing_type: rre-post
date: 1999-05-08
url: http://commons.somewhere.com:80/rre/1999/RRE.surveillance.crypto..html
importance: 6
research_status: partial
tags:
  - activism
  - civil-liberties
  - cognitive-science
  - commerce
  - cryptography
  - education
  - government-info
  - health
  - international
  - internet-policy
  - labor
  - law
  - media
  - military
  - privacy
  - surveillance
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1999/RRE.surveillance.crypto..html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009054022/http://www.somewhere.com/)

  

# [RRE]surveillance, crypto, etc

```
[In case you don't know about this publication, here is a useful recent
issue.  By the way, in case you haven't heard ... in a little-noticed
provision of the recent Microsoft-AT&T-MediaOne-Comcast deal, Microsoft
has bought a 30% stake in RRE for a price estimated at $127M.  The list
will henceforth be known as MSRRE.  I know it probably seems like I'm
selling out, but it's the only way that I could guarantee distribution
to the fast-growing cable market.  In fact, MS would have bought another
10% of the list, except that the thicket of deals is so complicated
that nobody can figure out whether AT&T owns @Home.  (This last bit is
actually true.)  Stay tuned for more information on MSRRE merchandise,
and for RRE's new, more sophisticated understanding of antitrust law.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html
or send a message to requests@lists.gseis.ucla.edu with Subject: info rre

---

Date: Sat, 8 May 1999 15:56:58 -0500
From: dawson@world.std.com (Keith Dawson)
To: tbtf@tbtf.com
Subject: TBTF for 1999-05-08: Netopath

-----BEGIN PGP SIGNED MESSAGE-----

TBTF for 1999-05-08: Netopath

    T a s t y   B i t s   f r o m   t h e   T e c h n o l o g y   F r o n t

    Timely news of the bellwethers in computer and communications
    technology that will affect electronic commerce -- since 1994

    Your Host: Keith Dawson

    This issue: < http://tbtf.com/archive/1999-05-08.html >
    ________________________________________________________________________

C o n t e n t s

    Intercepting communications worldwide
    An advance in factoring: Shamir's TWINKLE
    Bernstein wins appeal
    Stunning Australian censorship proposal could become law
    Talk of US-mandated disabled access to Web pages is premature
    Electronic ink debuts
    Siliconia: the e-Coast
    Snailmail for the Internet age
    Web logs
    The world through an eBay lens
        eBayla
        Car dealer accused of libeling a competitor
        Auctioning an ISP team
        13-year-old bids $3M, thinking it's a game
    Jargon Scout: Netopath
    ________________________________________________________________________

..Intercepting communications worldwide

  Secret group founded by the FBI pushes international data monitoring

    The CALEA law in the US, an Australian regulation requiring tapping
    of telecomms, and a secret EU policy position are all traceable dir-
    ectly to the efforts of a secret international group of law enforce-
    ment officers -- called ILETS -- convened by the FBI and meeting
    since 1993 to push building universal wiretap-ability into worldwide
    communications. Duncan Campbell reports for the Guardian and Observer
    [1] (cookies required).

    The existence and operation of the ILETS group is but one subject
    covered in the report "Interception Capabilities 2000," which Camp-
    bell authored for the European Parliament's Science and Technology
    Options Assessment Panel. IC2000 was approved as a working document
    at the STOA meeting in Strasbourg on 1999-05-06. It is available
    here [2]. (The text downloads 332K. Turn off graphics to avoid an-
    other 761K; the graphics add little to the article.)

    Today your email, Web browsing, online chat, telex, phone calls,
    cell calls, and faxes are almost certainly being swept up in one
    or more national or international interception dragnets. Unless you
    routinely use PGP, or communicate over a robust encrypted VPN link,
    these communications can be read by unaccountable agencies in any
    one of a growing number of countries.

    Does this fact make you angry? Then encrypt.

    [1]  http://www.newsunlimited.co.uk/The_Paper/Weekly/Story/0,3605,45981,00.html
    [2]  http://www.gn.apc.org/duncan/ic2000.htm
    ____________

..An advance in factoring: Shamir's TWINKLE

  Opto-electronic sieving challenges 512-bit PGP keys

    Adi Shamir, one of the inventors of RSA, has made a major advance in
    the factoring of large numbers [3] (free registration and cookies
    required for this NY Times story). The new work describes hardware
    that, if constructed, might put the routine factoring of 150-digit
    numbers more easily within reach. This would mean that 512-bit RSA
    keys (for example) would be vulnerable to cracking with modest re-
    sources.

    Details of Shamir's approach have been posted on the RSA Labs site
    [4]. Shamir's paper is also available in PostScript (370K) [5] or
    Zip (79K) [6] form.

    Shamir proposes a fast piece of sieving hardware dubbed TWINKLE that
    could be built for about $5000 in volume. He roughly specs a photo-
    electric sieving device 100 to 1000 times faster than a typical PC
    for this task. Such devices are not new -- D.H. Lehmer built a mech-
    anical-optical sieve in the 1930's. The RSA site claims that Sha-
    mir's device would requires some sophisticated optical/electrical
    engineering to implement, but that it does appear feasible.

    [3]  http://www.nytimes.com/library/tech/99/05/biztech/articles/02encr.html
    [4]  http://www.rsa.com/rsalabs/html/twinkle_qa.html
    [5]  http://jya.com/twinkle.eps
    [6]  http://jya.com/twinkle.zip
    ____________

..Bernstein wins appeal

  Court decides, 3-2, that US encryption export laws are unconstitu-
  tional when applied to source code

    A three-judge panel for the US 9th Circuit of Appeals has ruled that
    the source code for Daniel Bernstein's crypto program "Snuffle" is
    speech protected under the First Amendment. The ruling affirms a
    lower-court decision issued a year and a half ago [7], before the
    control of crypto exports was moved from the State Department to
    Commerce. The ruling did not provide Bernstein with injunctive re-
    lief to publish his code pending the expected appeal by the Justice
    Department to the Supreme Court.

    Here is the ruling itself [8], authored by Judge Betty Fletcher;
    below are some excerpts.

      > Cryptographers use source code to express their scientific
      > ideas in much the same way that mathematicians use equations
      > or economists use graphs

      > We find that the export administration regulations operate
      > as a prepublication licensing scheme that burdens scientific
      > expression, vest boundless discretion in government offi-
      > cials, and lack adequate procedural safeguards.

      > We emphasize the narrowness of our First Amendment holding.
      > We do not hold that all software is expressive. Much of it
      > surely is not... We hold merely that because the prepubli-
      > cation licensing regime challenged here applies directly to
      > scientific expression, vests boundless discretion in govern-
      > ment officials, and lacks adequate procedural safeguards,
      > it constitutes an impermissible prior restraint on speech.

      > Whether we are surveiled by our government, by criminals,
      > or by our neighbors, it is fair to say that never has our
      > ability to shield our affairs from prying eyes been at such
      > a low ebb. The availability and use of secure encryption may
      > offer an opportunity to reclaim some portion of the privacy
      > we have lost. Government efforts to control encryption thus
      > may well implicate not only the First Amendment rights of
      > cryptographers intent on pushing the boundaries of their
      > science, but also the constitutional rights of each of us as
      > potential recipients of encryption's bounty. Viewed from
      > this perspective, the government's efforts to retard pro-
      > gress in cryptography may implicate the Fourth Amendment, as
      > well as the right to speak anonymously..., the right against
      > compelled speech..., and the right to informational privacy...

      > The government's argument suggests that even one drop of
      > "direct functionality" overwhelms any constitutional protec-
      > tions that expression might otherwise enjoy. This cannot be
      > so. If it were, we would have expected the Supreme Court to
      > start and end its analysis of David Paul O'Brien's burning
      > of his draft card with an inquiry into whether he was kept
      > warm by the ensuing flames.

    In light of the ruling some in the crypto community are calling for
    the immediate posting of cryptographically sensitive materials from
    US shores. Some examples are the interrnational Cryptography Freedom
    page [9] and the original source code for Snuffle itself [10]. But
    Cindy Cohn, one of the victorious lawyers, strikes a note of caution
    [11]: it would be wiser to wait 52 days before setting up a crypto
    redistribution repository in the US, even from the 6-state area
    under the purview of the 9th Circuit Court.

    Thanks to the TBTF Irregular David Black for his usual astute reading
    of legal prose.

    [7]  http://tbtf.com/archive/1996-12-24.html#s01
    [8]  http://jya.com/bernstein-9th.htm
    [9]  http://jya.com/crypto-free.htm
    [10] http://www.shmoo.com/~pablos/Snuffle/snuffle.shar
    [11] http://www.ljx.com/mailinglists/cyberia-l/20266.html
    ____________

..Stunning Australian censorship proposal could become law

  Advice of technical experts and government panels is ignored

    TBTF Irregular [12] Eric Scheid <eric at ironclad dot net dot au>
    has been feeding me material on a drastic swing to the right
    being played out now in Australia. Proposed legislation would out-
    law any Net content in that country down to an "R" rating and would
    compel ISPs to block all such material worldwide from Australian
    viewers. The SJ Mercury News's Dan Gillmor says [13]:

      > As Australia's government races headlong toward a regime of
      > Internet censorship, a visitor from the United States is
      > tempted to ridicule the notion and the politicians who are
      > responsible. But I find myself more saddened than smug as I
      > look at the proposed bill.

    Here are some salient points from the proposed legislation that
    sounds more suitable to a brutal dictatorship than to an en-
    lightened Western society, from a posting by Kimberley Heitman,
    Chair of Electronic Frontier Australia:

      > First new feature is the licencing of ISPs, and compulsory
      > trade unionism ... Daily penalties of $27,500 should be
      > enough to bring small ISPs into line, if the threat of being
      > shut down by the Federal Court doesn't.

      > Second, the ABA will... tell ISPs what hardware and software
      > to use. Oh, and from now on ISPs work weekends, as takedown
      > orders issued by email or fax will have to be complied-with
      > within 24 hours. Same penalties natch -- $27,500 daily for
      > merely allowing "adult themes" material.

      > Third, people can complain about ISPs as well as sites, for
      > permitting access to "adult themes" material anywhere in the
      > world... Is there any doubt that proxy filters are to be
      > compulsory?

      > Fourth, less censorious State and Territory laws are over-
      > ridden, and no-one under 18 is allowed to own an account.
      > Free speech is dead coast to coast...

      > And finally, everything archiveable is covered, not just web
      > sites. As technology improves, the industry and the public
      > will pay for smaller and smaller sieves down to the RAM
      > caches, IRC, and newsgroups.

      > There's no pretence in this Bill that self-regulation means
      > anything other than outsourcing censorship.

    This extremely disturbing story is still developing; you can fol-
    low the news on the Link mailing list [14] (search for Alston, Har-
    radine, censorship). Here are some links to resources provided by
    Eric Scheid.

* - The government proposals [15]* - EFA's response [16]* - A large law firm's take on the proposed legislation [17]* - Senator Alston's latest media release [18]* - Links to discussion and analysis of the bill [19]

[12] http://tbtf.com/the-irregulars.html
    [13] http://www.mercurycenter.com/svtech/columns/gillmor/docs/dg050499.htm
    [14] http://www.anu.edu.au/mail-archives/link/
    [15] http://www.dcita.gov.au/nsapi-text/?MIval=dca_dispdoc&pathid=3648
    [16] http://www.efa.org.au/Publish/PR990319.html
    [17] http://www.gtlaw.com.au/pubs/newdarkage.html
    [18] http://www.dcita.gov.au/nsapi-text/?MIval=dca_dispdoc&pathid=3756
    [19] http://www.efa.org.au/Campaigns/99.html
     ____________

..Talk of US-mandated disabled access to Web pages is premature

  Freedom Forum story is much reported and overblown

    A little-noted law passed last year requires the Web sites of gov-
    ernment agencies, and of anyone who supplies Web deliverables to
    the government, to meet criteria for accessibility for people with
    disabilities. Adam Clayton Powell III has touched off a broad de-
    bate with a story [20] that projects dire consequences from this
    simple and sensible law. The accessibility provision is contained
    in Section 508 [21] of the Workforce Investment Act, passed last
    year by Congress. While the law is mandatory only for government
    sites and for contractors that provide Web content to the govern-
    ment, Powell quotes some members of the committee responsible for
    writing the rules as they speculate on the (to them presumably
    desirable) possibility that all US-based Web sites may some day
    come under the force of such rules. In a Ziff Davis interview [22],
    Jenifer Simpson, a member of the rules committee, justified such
    unprecedented government intervention in a publishing medium this
    way:

      > The Internet is subject to market forces, but it didn't start
      > through market forces, it was started by the federal government.

    She was certainly speaking out of school. The Supreme Court has
    ruled, in striking down parts of the Communications Decency Act,
    that the Internet is a medium deserving of the strongest First
    Amendment protections.

    A poster to the fight-censorship mailing list summarized thus the
    universal government tendency to give us a fat 3-ring binder when
    what we need is a paragraph:

      > Given the reasonably sane goal of assuring that all taxpaying
      > citizens, regardless of their physical condition, have access to

      > what they've paid for, one might (if one were not a government
      > employee) expect something like:

      > "All data posted to the web by the government shall include
      > 'alt' tags in any graphics. The government shall design web
      > pages to conform with the capabilities of leading tools for
      > the handicapped, save where such conformance defeats the pur-
      > pose of the site."

      > Of course, that's not what we got.

    Thanks to the TBTF Irregulars, in particular Jamie McCarthy and
    David Black, for perspective and editorial balance on this story.
    McCarthy has written an analysis [23] concluding that the Freedom
    Forum story is irresponsible journalism and calling for a retrac-
    tion. Powell is sticking by his viewpoint.

    [20] http://www.freedomforum.org/technology/1999/4/30handicapaccess.asp
    [21] http://www.usdoj.gov/crt/508/508law.html
    [22] http://www.msnbc.com/news/260652.asp
    [23] http://truman.fac.org/forum/messagedetail.asp?msgID=16678
    ____________

..Electronic ink debuts

  "Immedia" technology promises real electronic books, someday

    E Ink [24], a Cambridge company, promises flat-panel displays that
    can be printed on any surface, moving us one step closer to the ad-
    vertising-saturated world of Neal Stephenson's Snow Crash [25]. The
    first commercial installation of its Immedia technology in an ad-
    vertising panel [26] has been unveiled in the sports department of a
    J.C.Penney store in a Boston exurb (photo [27], 61K). Area geeks have
    been making the pilgrimage to the Solomon Pond Mall in Marlboro,
    Massachusetts to marvel at a 4-by-6-foot (1.3-by-2 meter) display,
    3mm thick, featuring a miniature wireless device by which store em-
    ployees can update it every 10 seconds. The display uses less than
    100 watts of energy.

    [24] http://www.electronic-ink.com/
    [25] http://www.amazon.com/exec/obidos/ASIN/0553562614/tbtf
    [26] http://www.electronic-ink.com/releases/pr7.html
    [27] http://www.electronic-ink.com/images/jcp_1.jpg
    ____________

..Siliconia: the e-Coast

  Portsmouth, NH is the latest soon-to-be-hot tech area

    Portsmouth, New Hampshire is the latest region to hold a naming con-
    test and launch a branding program to boost its recognition as a
    technology center. The resulting Siliconium [28] is "e-Coast," des-
    ignating the 18-mile NH seacoast and adjacent areas of Massachusetts
    and Maine. It's too bad the Boston Globe headline writer chose to
    title its story [29] "Silicon Seacoast." Anchoring Portsmouth's
    vibrant and growing high-tech scene is venture-backed Bow Street
    Software, with killer office space on the Piscataqua River where the
    famous tugboats tie up [30]. Unfortunately I can't tell you what Bow
    Street does: their Web site [31] is too high-tech for my Communica-
    tor 4.51 browser. It presents a black-on-black window with a few
    rollovers; the link to a text-only version leads back to the same
    inaccessible site.
    
    Thanks to Aaron Smith <a dot smith at rscs dot net> of the Greater
    Portsmouth Chamber of Commerce for word on the e-Coast.

    [28] http://tbtf.com/siliconia.html
    [29] http://www.boston.com/dailyglobe2/125/business/Silicon_seacoast%2b.shtml
    [30] http://www.tugboatalley.com/index1.htm
    [31] http://bowstreet.com/
    ____________

..Snailmail for the Internet age

  Bridging email to a more venerable medium

    A new company [32] formed by an Irish e-commerce expert promises to
    turn Net surfers into letter writers. Letterpost is the brainchild
    of Dr. Donal O'Mahony of Trinity College in Dublin. While on sab-
    batical at Stanford he decided to partake of the local customs and
    create his own Internet startup. Here's how it works. You buy post-
    age at [32], 99 cents per letter, and type the recipient's address
    and your message. The letter is printed out, put in an envelope,
    and mailed from one of Letterpost.com's automated mail centers. The
    first such center is operational in San Francisco; Ireland will
    open in May and India in June. The company will be targeting US
    immigrant groups such as Irish-Americans and first- and second-
    generation Indians, helping them to keep in touch with unwired rel-
    atives back home.

    TBTF Irregular John R. LoVerso <loverso at sitaranetworks dot com>
    writes:

      > What's old is new again. Back in '82, the US Postal Service had
      > an (ummm, forgot the correct term) "electronic telegram" ser-
      > vice. This was when they were asking Congress to allow them to
      > control electronic mail delivery. Anyway, one enterprising soul
      > made a UUCP-to-egram gateway. You had to UUCP mail (foo!bar!-
      > another!there) the letter in an exacting format, but it ended
      > up getting printed and mailed. I used it several times. Like
      > all things in "the good old days" of the net, it was free.

    Reader Prasenjeet Dutta <pd at cse dot vec dot ac dot in> notes:

      > A company called Multinet Infosys [33] has been offering a free
      > letterpost service in India at for quite some time now. They'll
      > send letters to anywhere in India for free, although they do ask
      > you to register.

    [32] http://www.letterpost.com/
    [33] http://www.homeindia.com/post/main.htm
    ____________

..Web logs

  Going public with your filtered browsing

    If you've missed the Web log phenomenon, allow me to introduce you.
    For some years Web adepts have been posting daily commentary on and
    links to sites they find compelling; the first Web log may have been
    NCSA's What's New page [34]. Suddenly Web logs are legion. Leslie Har-
    pold comments on the phenomenon in Smug [35]:

      > I love riffing through a good log, it's kind of the vicar-
      > ious voyeuristic thrill picking through someone else's purse
      > or junk drawer, but I'm fairly certain there's more than
      > enough dull stuff on the web, so no need to add to the pile.
      > If Web Logs become as ubiquitous as the cargo pant, the
      > stylishness and cache will be wholly depleted and it will be
      > gone faster than the wrap sandwich.

    Here are some of the Web logs I find most useful to the topics TBTF
    covers:

* - Rafe Colburn -- Outraged Daily Edition [36]* - Wesley Felter -- Hack the Planet [37]* - Raphael Carter -- Honeyguide [38] (his Sonnets on Science [39]
      aren't bad either)* - Jesse James Garrett -- Infosift [40]* - Lawrence Lee -- Tomalak's Realm [41]

Some consider TBTF's Tasty Bit of the Day feature a Web log, but
    that's a stretch. The TBoDay is considerably more cooked than the
    items in most Web logs; it's a first draft for a regular TBTF item.
    But a growing acquaintance with Web logs has moved me to make TBTF
    available in "push" form to Dave Winer's Userland [42], a sort of
    toolkit for constructing your own personal meta-log.

    [34] http://www.ncsa.uiuc.edu/SDG/Software/Mosaic/Docs/old-whats-new/whats-new-0693.html
    [35] http://www.smug.com/current/net.html
    [36] http://rc3.org/">rafe
    [37] http://hack-the-planet.felter.org/
    [38] http://www.chaparraltree.com/honeyguide/
    [39] http://www.chaparraltree.com/scison/
    [40] http://www.jjg.net/infosift/
    [41] http://tr.pair.com/
    [42] http://my.userland.com/
   ____________

..The world through an eBay lens

    The eBay auction site is now about the size of the 1994 Internet and
    I would wager it is growing as fast. Auction is one of the killer
    apps of the Net today. eBay presents us with various analogies to
    the early Net: it's large, shambling, nearly unmanageable; it's
    fast-moving, rough-and-tumble, and very American. For weeks now Web
    watchers have been passing around eBay URLs, pointing to auctions in
    progress or completed, as bellwethers of coming trends. Here are a
    few.
    ____________

    ..eBayla

    Canadian security enthusiast Tom Cervenka, who goes by the handle
    Blue Adept, has invented a new flavor of virus: he has created an
    infected eBay auction item [43] that he calls eBayla. The exploit
    works because eBay allows JavaScript in the member-authored pages
    describing an item offered for sale. When an eBay member bids on
    an infected item, his/her username and password are emailed to
    Cervenka. EBay's response [44] to the exploit sets a new low for
    bone-headedness. Not only does eBay downplay the seriousness of
    the security hole; not only do they get the technical details of
    the exploit's workings wrong; but they also make vague threats in
    Cervenka's direction, because he brought this vulnerability to
    their attention. EBay deserves to get slapped, hard, by its mem-
    bers -- nothing else will make them rethink their cluelessness.
    Thanks to Michael Sanders <msanders at confusion dot net> for the
    prod on this story.

    [43] http://www.because-we-can.com/ebayla/default.htm
    [44] http://www.news.com/News/Item/Textonly/0,25,35321,00.html
    ____________

    ..Car dealer accused of libeling a competitor

    A popular feature of the eBay site allows users to rate their en-
    counters with other site users. This forum provides some reputation
    accountability: both bidders and sellers can check out others' ex-
    periences with eBay users and choose whether to do business with
    them. eBay doesn't monitor, adjudicate, or characterize the posted
    comments. Recently a vendor of automobiles, new to eBay, watched
    several bidders withdraw their bids after someone posted negative
    comments about the dealer [45], [46]. With little difficulty the
    dealer traced the negative postings to employees of a rival firm
    operating on eBay.

    [45] http://www.washingtonpost.com/wp-srv/business/feed/biztop925293980763.htm
    [46] http://abcnews.go.com/sections/tech/DailyNews/ebay990408.html
    ____________

    ..Auctioning an ISP team

    Sixteen system administrators, developers, and managers from a "major
    ISP" tried to auction themselves off on eBay [47]. The minimum bid was
    set above $3.1M, which would give the purchaser use of the team for
    one year -- and provide the team members with healthy raises. It is
    unclear if anyone actually bid for this "item" on eBay, but team
    members said in an interview that [48] several companies had con-
    tacted them. Thanks to TBTF Irregular Eric Scheid <eric at ironclad
    dot net dot au> for the tip.

	[47] http://cgi.ebay.com/aw-cgi/eBayISAPI.dll?ViewItem&item=96369441
    [48] http://www.washingtonpost.com/wp-srv/business/daily/april99/ebay30.htm
    ____________

    ..13-year-old bids $3M, thinking it's a game

    13-year-old Andrew Tyler's parents were surprised when an eBay rep-
    resentative contacted them and asked how Andrew intended to pay
    $900,000 for a Van Gogh painting he had won at auction [49]. The
    teenager had also bid on a 1955 Ford convertible, an antique bed,
    a Viking ship replica, and a Superman comic book.

    [49] http://www.usatoday.com/life/cyber/tech/ctf027.htm
    ____________

..Jargon Scout: Netopath

  What to call a pathological Net abuser

    Jargon Scout [50] is an irregular TBTF feature that aims to give you
    advance warning -- preferably before Wired Magazine picks it up --
    of jargon that is just about ready to hatch into the Net's language.
    Spam fighter JoWazzoo <jowazzoo at whiteice dot com> takes credit
    for coining the term "netopath," which is applied to the most ex-
    treme and deranged form of Net abuser. The Usenet posting in which
    JoWazzoo coined the term (7952fe$ggl@chronicle.concentric.net) has
    expired from the archives of both Deja News and Alta Vista, but this
    immediate followup post [51], which references and quotes it, ce-
    ments JoWazzoo's claim to the invention.

    [50] http://tbtf.com/jargon-scout.html
    [51] http://ww2.altavista.com/cgi-bin/news?msg@266119@news%2eadmin%2enet%2dabuse%2eemail%267952fe+ggl+chronicle+concentric+net
    ________________________________________________________________________

N o t e s

> TBTF has been slashdotted [52]. The link [53] to the eBayla story
    above resulted in 6667 visitors on 1999-04-21 (1000 would have been
    normal) and 126K hits (vs. a normal 15K). The bandwidth bill has
    come due and it is not pretty, not that I'm complaining.

    [52] http://www.tuxedo.org/~esr/jargon/frames/slashdoteffect.html
    [53] http://slashdot.org/articles/99/04/22/1816245.shtml

> Some readers took exception to my use of the Jive dialect in the pre-
    vious issue's title story. Upon reflection I should have chosen
    another example. Apologies and no offense intended.
    ________________________________________________________________________

S o u r c e s

> For a complete list of TBTF's (mostly email) sources, see
    http://tbtf.com/sources.html .
    ________________________________________________________________________

    TBTF home and archive at http://tbtf.com/ . To (un)subscribe send
    the message "(un)subscribe" to tbtf-request@tbtf.com. TBTF is Copy-
    right 1994-1999 by Keith Dawson, <dawson@world.std.com>. Commercial
    use prohibited. For non-commercial purposes please forward, post,
    and link as you see fit.
    _______________________________________________
    Keith Dawson               dawson@world.std.com
    Layer of ash separates morning and evening milk.

-----BEGIN PGP SIGNATURE-----
Version: PGP for Personal Privacy 5.5

iQCVAwUBNzSfBGAMawgf2iXRAQFQdwQAvI1HDmYZCV3kCIV/loMH7V1G0mD/SVGy
jF2UlhPu6vPBaYpxXnciSoW4zcFdTOjua6EhrZr+uD4IWMMrk2GUAQEOD4NlyOHh
Jy7AEKvfAMmE0fVcb/woGPYkgIVbbiEbuCzrTFevMiJuRQ7gKR/qqlZodJqgzkko
aITtPqAMJ7o=
=mepb
-----END PGP SIGNATURE-----
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009054022/http://www.somewhere.com/)