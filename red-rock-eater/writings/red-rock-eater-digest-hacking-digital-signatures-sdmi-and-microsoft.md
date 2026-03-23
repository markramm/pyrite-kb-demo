---
id: red-rock-eater-digest-hacking-digital-signatures-sdmi-and-microsoft
title: Red Rock Eater Digest - hacking digital signatures, SDMI, and Microsoft
type: writing
writing_type: rre-post
date: 2000-11-15
url: http://commons.somewhere.com:80/rre/2000/RRE.hacking.digital.sign.html
key_concepts:
  - capture-model
importance: 6
research_status: partial
tags:
  - ai
  - civil-liberties
  - commerce
  - cryptography
  - government-info
  - international
  - internet-policy
  - labor
  - law
  - media
  - military
  - privacy
  - religion
  - surveillance
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/2000/RRE.hacking.digital.sign.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20010501031819/http://commons.somewhere.com/rre/) | **Most Recent Article: Mon, 30 Apr 2001** |

```
[Abridged and reformatted to 70 columns.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
You are welcome to send the message along to others but please do not use
the "redirect" option.  For information about RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html

---

Date: Wednesday, November 15, 2000 4:58 PM
From: Bruce Schneier <schneier@counterpane.com>
To: crypto-gram@chaparraltree.com
Subject: CRYPTO-GRAM, November 15, 2000

                  CRYPTO-GRAM

               November 15, 2000

               by Bruce Schneier
                Founder and CTO
       Counterpane Internet Security, Inc.
            schneier@counterpane.com
          <http://www.counterpane.com>

A free monthly newsletter providing summaries, analyses, insights, and
commentaries on computer security and cryptography.

Back issues are available at <http://www.counterpane.com>.  To subscribe
or unsubscribe, see below.

Copyright (c) 2000 by Counterpane Internet Security, Inc.

** *** ***** ******* *********** *************

In this issue:
      Why Digital Signatures Are Not Signatures
      Crypto-Gram Reprints
      News
      Counterpane Internet Security News
      Secrets and Lies News
      SDMI Hacking Challenge
      Microsoft Hack (the Company, not a Product)
      Comments from Readers

** *** ***** ******* *********** *************

    Why Digital Signatures Are Not Signatures

When first invented in the 1970s, digital signatures made an amazing
promise: better than a handwritten signature -- unforgeable and
uncopyable -- on a document.  Today, they are a fundamental component
of business in cyberspace.  And numerous laws, state and now federal,
have codified digital signatures into law.

These laws are a mistake.  Digital signatures are not signatures,
and they can't fulfill their promise.  Understanding why requires
understanding how they work.

The math is complex, but the mechanics are simple.  Alice knows a
secret, called a private key.  When she wants to "sign" a document
(or a message, or any bucket of bits), she performs a mathematical
calculation using the document and her private key; then she appends
the results of that calculation -- called the "signature" -- to the
document.  Anyone can "verify" the signature by performing a different
calculation with the message and Alice's public key, which is publicly
available.  If the verification calculation checks out then Alice must
have signed the document, because only she knows her own private key.

Mathematically, it works beautifully.  Semantically, it fails
miserably.  There's nothing in the description above that constitutes
signing.  In fact, calling whatever Alice creates a "digital
signature" was probably the most unfortunate nomenclature mistake in
the history of cryptography.

In law, a signature serves to indicate agreement to, or at least
acknowledgment of, the document signed.  When a judge sees a paper
document signed by Alice, he knows that Alice held the document in
her hands, and has reason to believe that Alice read and agreed to
the words on the document.  The signature provides evidence of Alice's
intentions.  (This is a simplification.  With a few exceptions,
you can't take a signed document into court and argue that Alice
signed it.  You have to get Alice to testify that she signed it, or
bring handwriting experts in and then it's your word against hers.
That's why notarized signatures are used in many circumstances.)

When the same judge sees a digital signature, he doesn't know anything
about Alice's intentions.  He doesn't know if Alice agreed to the
document, or even if she ever saw it.

The problem is that while a digital signature authenticates the
document up to the point of the signing computer, it doesn't
authenticate the link between that computer and Alice.  This is a
subtle point.  For years, I would explain the mathematics of digital
signatures with sentences like: "The signer computes a digital
signature of message m by computing m^e mod n."  This is complete
nonsense.  I have digitally signed thousands of electronic documents,
and I have never computed m^e mod n in my entire life.  My computer
makes that calculation.  I am not signing anything; my computer is.

PGP is a good example.  This e-mail security program lets me digitally
sign my messages.  The user interface is simple: when I want to sign a
message I select the appropriate menu item, enter my passphrase into a
dialog box, and click "OK."  The program decrypts the private key with
the passphrase, and then calculates the digital signature and appends
it to my e-mail.  Whether I like it or not, it is a complete article
of faith on my part that PGP calculates a valid digital signature.
It is an article of faith that PGP signs the message I intend it to.
It is an article of faith that PGP doesn't ship a copy of my private
key to someone else, who can then sign whatever he wants in my name.

I don't mean to malign PGP.  It's a good program, and if it is working
properly it will indeed sign what I intended to sign.  But someone
could easily write a rogue version of the program that displays
one message on the screen and signs another.  Someone could write a
Back Orifice plug-in that captures my private key and signs documents
without my consent or knowledge.  We've already seen one computer
virus that attempts to steal PGP private keys; nastier variants are
certainly possible.

The mathematics of cryptography, no matter how strong, cannot bridge
the gap between me and my computer.  Because the computer is not
trusted, I cannot rely on it to show me what it is doing or do what
I tell it to.  Checking the calculation afterwards doesn't help;
the untrusted computer can't be relied upon to check the calculations
properly.  It wouldn't help to verify the code, because the untrusted
computer is running the code (and probably doing the verification).
It wouldn't even help to store the digital signature key in a secure
module: the module still has to rely on the untrusted computer for
input and output.

None of this bodes well for digital signatures.  Imagine Alice in
court, answering questions about a document she signed.  "I never
saw it," she says.  "Yes, the mathematics does prove that my private
key signed the document, but I never saw it."  And then an expert
witness like myself is called to the stand, who explains to the judge
that it is possible that Alice never saw the document, that programs
can be written to sign documents without Alice's knowledge, and that
Alice's digital signature doesn't really mean anything about Alice's
intentions.

Solving this problem requires a trusted signing computer.  If Alice
had a small hand-held computer, with its own screen and keyboard, she
could view documents on that screen and sign them with that keyboard.
As long as the signing computer is trusted, her signatures are
trusted.  (But problems remain.  Viewing a Microsoft Word document,
for example, generally involves the very software most responsible for
welcoming a virus into the computer.)  In this case we're no longer
relying on the mathematics for security, but instead the hardware and
software security of that trusted computer.

This is not to say that digital signatures are useless.  There
are many instances where the insecurities discussed here are not
relevant, or where the dollar value of the signatures is small enough
not to warrant worrying about them.  There are also instances where
authenticating to the signing computer is good enough, and where no
further authentication is required.  And there are instances where
real-world relationships can obviate the legal requirements that
digital signatures have been asked to satisfy.

Digital signatures prove, mathematically, that a secret value known
as the private key was present in a computer at the time Alice's
signature was calculated.  It is a small step from that to assume
that Alice entered that key into the computer at the time of signing.
But it is a much larger step to assume that Alice intended a particular
document to be signed.  And without a tamperproof computer trusted by
Alice, you can expect "digital signature experts" to show up in court
contesting a lot of digital signatures.

Comments on the new federal digital signature law:
<http://www4.zdnet.com:80/intweek/stories/news/0,4164,2635346,00.html>
(multipage, don't miss the others)
<http://www4.zdnet.com:80/intweek/stories/news/0,4164,2634368,00.html>
<http://www.infoworld.com:80/articles/hn/xml/00/10/02/001002hnesign.xml>
<http://www.pioneerplanet.com/tech/tcv_docs/028992.htm>

A survey of laws in various states and countries:
<http://rechten.kub.nl/simone/DS-LAWSU.HTM>

** *** ***** ******* *********** *************

              Crypto-Gram Reprints

Programming Satan's Computer:  Why Computers are Insecure
<http://www.counterpane.com/crypto-gram-9911.html#WhyComputersareInsecure>

Elliptic-Curve Public-Key Cryptography
<http://www.counterpane.com/crypto-gram-9911.html#EllipticCurvePublic-KeyCry
ptography>

The Future of Fraud: Three reasons why electronic commerce is
different
<http://www.counterpane.com/crypto-gram-9811.html#commerce>

Why copy protection does not work:
<http://www.counterpane.com/crypto-gram-9811.html#copy>

** *** ***** ******* *********** *************

                      News

A cyber Underwriters Laboratory?  Don't hold your breath.
<http://www.zdnet.com/enterprise/stories/main/0,10228,2640597,00.html>

The government of France concludes that Echelon is a threat to
privacy.  (Their report identifies two Echelon sites in Australia.)
<http://cgi.zdnet.com/slink?59369:8469234>
<http://www.it.fairfax.com.au/breaking/20001020/A62985-2000Oct20.html>

The stolen Enigma machine has been returned:
<http://news.bbc.co.uk/hi/english/uk/newsid_977000/977127.stm>

People are worried about security in cyberspace:
<http://dailynews.yahoo.com/h/nm/20001016/ts/tech_security_dc_1.html>
And yet again, industry analysts predict security problems.
<http://www.nwfusion.com/news/2000/1011attack50.html>

Good essay on hackers and the hacker ethic:
<http://www.feedmag.com/essay/es405_master.html>

About a year ago Carl Ellison and I wrote "10 Risks of PKI":
<http://www.counterpane.com/pki-risks.html>
Here is a rebuttal:
<http://members.nbci.com/aram_perez/ResponseTenRisks.html>

Remote-controlled robot spy:
<http://www.newscientist.com/nlf/1021/follow.html>
Military version of the same idea:
<http://www.newscientist.com/news/news.jsp?id=3Dns226113>

Two NSA documents about their own culture and disorganization:
<http://www.nsa.gov/releases/nsa_external_team_report.pdf>
<http://www.nsa.gov/releases/nsa_new_enterprise_team_recommendations.pdf>
Both reports are available as HTML:
<http://cryptome.org/nsa-reorg-et.htm>
<http://cryptome.org/nsa-reorg-net.htm>
And an article on the reports:
<http://www.theregister.co.uk/content/1/14170.html>

Putting tracking chips in people:
<http://www.digitalangel.net/>

Two useful publications from the Electronic Privacy Information Center.
The 2000 Privacy Law Sourcebook:
<http://www.epic.org/pls>
The 2000 edition of the Privacy and Human Rights survey:
<http://www.epic.org/bookstore/phr/>
Both are worth buying, and EPIC is worth supporting.

Software and hardware vendors treat security problems as public-relations
problems.  No surprise; I've been saying this for years.
<http://www.zdnet.com/sp/stories/column/0,4712,2642537,00.html>

Interesting article on the threats to business information:
<http://www.cnn.com/2000/TECH/computing/10/18/business.spy.threat.idg/index.
html>

The European Cybercrime Treaty threatens human rights.
<http://www.zdnet.co.uk/news/2000/41/ns-18546.html>

The AES algorithm as been chosen, but it's still a long and complicated
road towards standardization.
<http://www.nwfusion.com/news/2000/1016apps.html>
A good summary article on the AES process:
<http://www.javaworld.com/javaworld/jw-10-2000/jw-1027-aes.html>
An article on a talk I gave on AES:
<http://www.theregister.co.uk/content/1/14435.html>

An article that challenges the assumption that no two fingerprints are
exactly alike.  This kind of thing has interesting implications for
biometrics:
<http://www.linguafranca.com/print/0011/feature_fingerprints.html>

Cheating is rampant on multi-player computer games.  This excellent
summary article discusses the general classes of cheats, and tries to
offer some  ways to mitigate the problem.  The lessons apply equally
well to other Internet based systems: commerce, community, etc.  Well
worth reading.
<http://www.gamasutra.com/features/20000724/pritchard_pfv.htm>

Despite a White House prohibition, 13 U.S. government agencies are
secretly using technology that tracks the Internet habits of people
visiting their Web sites, and in at least one case provides the
information to a private company.
<http://abcnews.go.com/sections/tech/DailyNews/tracking001021.html>

FBI agent Marcus C. Thomas (who is mentioned in the EPIC FOIA
documents)  discussed Carnivore at a presentation at NANOG 20.
<http://cryptome.org/carnivore-demo.htm>

Publius: anonymous posting of files on the Internet.  How it works:
<http://www.sciam.com/2000/1000issue/1000techbus2.html>

The U.S. has implemented new, and more lenient, encryption export
regulations.  On October 19, the U.S. Department of Commerce's Bureau
of Export Administration (BXA) published an amendment to its export
regulations on encryption products.  The new rule amends the Export
Administration Requirements (EAR) and liberalizes exports and
re-exports of encryption products to the fifteen European Union
member states plus Australia, the Czech Republic, Hungary, Japan,
New Zealand, Norway, Poland and Switzerland.  The text of the revised
rules are available at:
<http://www.bxa.doc.gov/Encryption/pdfs/EncryptionRuleOct2K.pdf>
News reports:
<http://www.cnn.com/2000/TECH/computing/10/19/encryption.exports.ap/>
<http://www.usatoday.com/life/cyber/tech/cti691.htm>

SANS Security Alert, including security predictions for 2001 (mine are
in there, too):
<http://www.sans.org/SANSSecAlert2_102000.pdf>

Mideast cyberwar: Israeli and Palestinian hackers are attacking each
other's networks:
<http://www.zdnet.com/zdnn/stories/news/0,4586,2647934,00.html>
And this cyberwar is spreading to the U.S.
<http://www.wired.com/news/business/0,1367,39913,00.html>

Ross Anderson reports an example of a semantic attack, this one a
glitch: "British newspapers today reported that a baby was born at
Eastbourne General Hospital by Caesarian section, the operation being
performed under torchlight following a power cut caused by a storm.
On one account, the standby generators couldn't be started as the
computer that controlled them believed they were already on; and
when power was restored after twenty minutes it could not be switched
through to the operating theatre as the computer believed that the
generators were still running. On another account, the computer
refused to believe that the power had gone off in the first place."
Attacks of this type will similarly target the inability of computers
to collect corroborating information before making decisions.
<http://www.guardian.co.uk/uk_news/story/0,3604,381054,00.html>

Another commentary on semantic attacks:
<http://www.securityfocus.com/commentary/104>

Incident-response database:
<https://cassandra.cerias.purdue.edu/main/index.html>

** *** ***** ******* *********** *************

       Counterpane Internet Security News

The Smithsonian is sponsoring a lecture and book signing at the
International Monetary Fund Center:
720 19th Street, N.W., Washington, DC, on 29 November at 6:30 - 8:00
p.m.  Everyone is invited.

Bruce Schneier is chosen as one of the 20 executives to watch by CRN magazine:
<http://www.crn.com/Components/Search/Article.asp?ArticleID=3D21187>
<http://www.crn.com/Components/Search/Article.asp?ArticleID=3D21207>

Managed Security Monitoring:
<http://www.techrepublic.com/article.jhtml?id=3Dr00620001011cav01.htm&page=3D1>

Decent article on Schneier's BlackHat talk:
<http://www.techtv.com/cybercrime/hackingandsecurity/story/0,9955,2058,00.html>

** *** ***** ******* *********** *************

           Secrets and Lies News

Worldwide sales stand at 45,000; the book is in its fourth printing.
(About two dozen typos are corrected in this latest printing, none
serious.)  The book tour has been a success; thanks to all who
attended one of the events.

Book Web site:
<http://www.counterpane.com/sandl.html>

Upside magazine has excerpted Chapter 2:
<http://www.upside.com/Ebiz/39ac19eb0.html>

More book reviews:
<http://www.latimes.com/business/columns/innovation/20001030/t000103702.html>
<http://www.byte.com/column/BYT20001018S0001>
<http://www.matrix.net/publications/mn/mn1010_secrets_and_lies.html>
All reviews:
<http://www.counterpane.com/sandlrev.html>

Buy the book here:
<http://www.amazon.com/exec/obidos/ASIN/0471253111/counterpane/>
Through Amazon's affiliates program, sales of this book have raised over 
$6000 for the Electronic Privacy Information Center.

** *** ***** ******* *********** *************

             SDMI Hacking Challenge

The Secure Digital Music Initiative issued a hacking challenge in
an attempt to prove its content-protection system safe.  Despite a
widespread boycott of the challenge, a team of researchers claims to
have broken all the SDMI security technologies.

These are all points I've discussed before, but let's review.

1.  Hacking contests are meaningless; they do not show security.
Just because a technology survives a contest does not mean that it
is secure.  (Remember, hackers don't play fair.)  Near as I can tell,
the SDMI break does not conform to the challenge rules, and the music
industry might claim that the SDMI schemes survived the technology.

2.  Even if the contest was meaningful and the technology survived
it, watermarking does not work.  It is impossible to design a music
watermarking technology that cannot be removed.  Here's a brute-force
attack: play the music and re-record it.  Do it multiple times and use
DSP technology to combine the recordings and eliminate noise.  Almost
always there is a shortcut technique to neutralize the watermark, but
the brute-force attack always works.

3.  Even if watermarking works, it does not solve the content-
protection problem.  If a media player only plays watermarked files,
then copies of a file will play.  If a media player refuses to play
watermarked files, then analog-to-digital copies will still work.  If
a watermark is designed to identify the legitimate owner of the file,
it still doesn't prove who copied the file or provide the copyright
owner with a party worth suing.

Digital files intrinsically undermine the scarcity model of business:
replicate many copies and sell each one.  Companies that find
alternate ways to do business, whether they be advertising funded,
or patronage funded, or membership funded, or whatever, are likely
to survive the digital economy.  The media companies figured this out
quickly when radio was invented -- and then television -- so why are
they so slow to realize it this time around?

The challenge:
<http://www.hacksdmi.org/>
<http://www.salon.com/tech/log/2000/09/14/hack_sdmi/index.html>

The boycott:
<http://slashdot.org/articles/00/09/15/1244236.shtml>
<http://www2.linuxjournal.com/articles/misc/0022.html>

The break:
<http://biz.yahoo.com/prnews/001108/dc_sdmi_ex.html>
<http://www.zdnet.co.uk/news/2000/44/ns-18963.html>
<http://www.wired.com/news/technology/0,1282,40054,00.html>
<http://www.salon.com/tech/log/2000/11/08/sdmi_tests/index.html>
<http://www.washingtonpost.com/wp-dyn/articles/A49514-2000Nov8.html>

SDMI's denial:
<http://www.theregister.co.uk/content/1/14608.html>
<http://www.salon.com/tech/log/2000/11/08/sdmi_tests/index.html>

A nice analysis:
<http://www.eet.com/story/OEG20001031S0037>

Article about DMCA provisions becoming active:
<http://www.securityfocus.com/templates/article.html?id=3D107>

URL of an interesting (for its reasoning and justification) but lengthy
"rule-making process" under DMCA, which came into effect on 28 Oct 2000:
<http://cryptome.org/dmca102700.txt>

I wrote about the futility of hacking contests in Crypto-Gram two years
ago, and in Secrets and Lies.
<http://www.counterpane.com/crypto-gram-9812.html#contests>

I also wrote about the futility of digital content protection:
<http://www.counterpane.com/crypto-gram-9811.html#copy>

The most ironic part of this story: this kind of testing is not legal
under the Digital Millennium Copyright Act, unless SDMI specifically
agrees to it.

** *** ***** ******* *********** *************

   Microsoft Hack (the Company, not a Product)

First the attack lasted three months.  Then it was six weeks and the
attackers had access to major source code.  Then, it was only five or
six days.  Now it's 12 days but they didn't see anything interesting.
Soon, the whole thing will have been a penetration test by a Microsoft
tiger team.  And when Bill Gates finally takes over the world, he'll
have Winston Smith consign all copies of the story to a memory hole,
since it will never have happened.

I don't buy Microsoft's rewriting of history.  If the attacker didn't
get anything interesting, why was the FBI called in?  The FBI has
better things to do than trace every two-bit cracker that knocks on
Microsoft's door.  If the Trojan only got onto a home computer of a
Microsoft employee or contractor, why did Microsoft block access to
its corporate network for all of its employees, globally, over the
weekend?  Why did they make everyone change their passwords afterward?

Near as I can tell, this is how Microsoft was hacked:

1) An unknown employee received an e-mail carrying the QAZ Trojan,
and inadvertently installed it, possibly on a machine at home he used
to connect to the Microsoft network.  (QAZ first appeared in China
around July.)  This virus-like software disguises itself as Notepad,
a Windows program used for reading text messages.

2) QAZ then sent a remote signal to a computer in Asia with the
location on the Internet of the newly infected computer.  QAZ also may
have automatically downloaded and installed hacker tools from a Web
site in the South Pacific, but I don't know that for sure.  There may
be other malicious code involved, but I am not sure about that either.
QAZ then gave the intruder some control over the victim's computer,
and it automatically tried to spread to any computers it found in that
section of Microsoft's network.

3) The hackers used another program to collect employee passwords,
which were automatically sent to a Russian e-mail address.

4) Posing as Microsoft employees working off-campus, the hackers used
the pilfered passwords to enter sensitive areas of the network and
downloaded files.

Others have done an admirable job reporting on the events, but some
points still need to be made:

1) This isn't a professional job; it's an opportunistic one.
The attacker got in via a Trojan, stole some passwords, wandered
around the network for a while, and was eventually tossed out.
A professional would have gotten in, gotten the goods, and left.
Microsoft would never have known anyone was there.

2) I doubt the attacker modified any source code.  Modifying source
code in ways that don't break it is hard, even for the authors.  And
Microsoft probably has good version control on its code; changes would
get noticed.

3) Some reports have wondered why so many Microsoft employees have
access to the source code.  It's because Microsoft is a software
company, and giving employees access to the software is a good thing.
Sure, Microsoft could limit access to only the people who obviously
need access, but that would encourage myopia, reduce collaboration,
and limit synergy.  The U.S.  military works this way: people need
a security clearance to view information of a certain classification,
and also need to demonstrate "need to know" for any given piece
of information.  In doing this, the military deliberately chooses
security over effectiveness.  Microsoft is not the military; in
choosing to share information they made the smarter choice.

4) Some reports have claimed "poetic justice": Microsoft hacked by
flaws in its own products.  While technically true, this is unfair.
Any network of this size and complexity will have dozens, if not
hundreds, of security vulnerabilities.  The attackers got in through
a vulnerability in a Microsoft product, but they could have just as
easily chosen another route.  If the network were entirely SunOS or
Linux or whatever, there would be different vulnerabilities.  The
moral is not that Microsoft products are insecure, it's that complex
systems are insecure.

5) The only way to defend against this sort of thing is real-time
network monitoring.  Given that vulnerabilities exist, and always
will, detection and response are the only countermeasures that work.
I know this sounds self-serving, but in all honesty this is exactly
the kind of attack I built Counterpane Internet Security to defend
against.  If we were watching Microsoft, we would have seen this
immediately.

6) This kind of thing happens all the time, to everyone.  Microsoft
may be this month's poster child for bad security, but don't think
they're unique.  The amazing thing isn't that Microsoft noticed after
three months (or six weeks), it's that they noticed at all.

7) Networks that are "political" are more vulnerable: Microsoft,
cigarette companies, drug companies, governments, political parties.
These networks are more likely to be targeted than random corporate
networks.

8) The most damage was to Microsoft's image.  This is what they spent
the most effort repairing: spinning the story, limiting the press
damage, and so forth.  These secondary risks -- bad publicity, loss
of good name, potential shareholder liability -- are often far more
dangerous than direct losses.

9) Microsoft's spin-control hurt.  Many were not fooled.  Lots of
hackers became incensed at Microsoft's boasting.  There has already
been two additional public -- and successful -- attacks against
Microsoft in the days following this story.  I believe that the
attacker wanted to prove Microsoft wrong.  And I believe there will
be others.

Morals: Always keep your antivirus software up to date, monitor your
network in real time, and don't believe that you are invulnerable.
Static passwords are not sufficient to protect your major corporate
assets.  And please don't rewrite history; others can't learn from
your mistakes that way, and I'm sure the FBI will lose patience with
you pretty quickly.

The Associated Press coverage:
<http://www.courierpress.com/cgi-bin/view.cgi?200010/27+micro102700_latestne
ws.html+20001027>

Microsoft changes its story:
<http://www.zdnet.com/zdnn/stories/news/0,4586,2646430,00.html>
<http://www.zdnet.com/zdnn/stories/comment/0,5859,2646049,00.html>

Skepticism about the new story:
<http://www.theregister.co.uk/content/1/14306.html>
<http://www.theregister.co.uk/content/1/14327.html>

Top 10 Things Bill Gates said when he heard Microsoft was hacked:
<http://www.zdnet.com/zdnn/stories/comment/0,5859,2646523,00.html>

Commentary on the attackers' motivations:
<http://www.securityfocus.com/commentary/112>

Legal ramifications of seeing the stolen source code:
<http://www2.linuxjournal.com/cgi-bin/frames.pl/articles/currents/0024.html>

Lessons of the attack:
<http://www.zdnet.com/eweek/stories/general/0,11011,2646167,00.html>
<http://www.zdnet.com/zdnn/stories/news/0,4586,2646315,00.html>
<http://securityportal.com/articles/mshacked20001029.html>
<http://www.zdnet.com/zdnn/stories/comment/0,5859,2646203,00.html>
<http://dailynews.yahoo.com/h/nm/20001029/tc/microsoft_hackers_dc_12.html>

Other attacks against Microsoft:
<http://www.infoworld.com/articles/hn/xml/00/11/03/001103hnhacker.xml>
<http://thestandard.com/article/display/0,1151,20065,00.html>

** *** ***** ******* *********** *************

              Comments from Readers

[....]

** *** ***** ******* *********** *************

CRYPTO-GRAM is a free monthly newsletter providing summaries,
analyses, insights, and commentaries on computer security and
cryptography.

To subscribe, visit <http://www.counterpane.com/crypto-gram.html>
or send a blank message to crypto-gram-subscribe@chaparraltree.com.
To unsubscribe, visit <http://www.counterpane.com/unsubform.html>.
Back issues are available on <http://www.counterpane.com>.

Please feel free to forward CRYPTO-GRAM to colleagues and friends who
will find it valuable.  Permission is granted to reprint CRYPTO-GRAM,
as long as it is reprinted in its entirety.

CRYPTO-GRAM is written by Bruce Schneier.  Schneier is founder and
CTO of Counterpane Internet Security Inc., the author of "Applied
Cryptography," and an inventor of the Blowfish, Twofish, and Yarrow
algorithms.  He served on the board of the International Association
for Cryptologic Research, EPIC, and VTW.  He is a frequent writer and
lecturer on computer security and cryptography.

Counterpane Internet Security, Inc. is a venture-funded company
bringing innovative managed security solutions to the enterprise.

<http://www.counterpane.com/>

Copyright (c) 2000 by Counterpane Internet Security, Inc.
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20010501031819/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20010501031819/mailto:webmaster@somewhere.com). |