---
id: bobby-inman-on-clipper-and-the-x9-triple-des-proposal
title: Bobby Inman on Clipper and the X9 Triple-DES proposal
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1994/Bobby.Inman.on.Clipper.a.html
coauthors: []
key_concepts: []
importance: 6
research_status: partial
tags:
  - cryptography
  - digital-rights
  - privacy
  - rre
  - surveillance
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1994/Bobby.Inman.on.Clipper.a.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991003181052/http://www.somewhere.com/)

  

# Bobby Inman on Clipper and the X9 Triple-DES proposal

```
Date: Wed, 23 Nov 94 09:54:12 EST
From: lethin@ai.mit.edu (Rich Lethin)
Subject: Admiral Inman visits MIT

-----BEGIN PGP SIGNED MESSAGE-----

Phil, below is something that I forwarded to cypherpunks a few days ago, a
rough transcription of class notes.  The note you sent yesterday mentioned
that the NSA objected to the Triple-DES proposal on the X9 committee.
Admiral Inman's comments below might reflect on a motivation for this.

Rich

- ---

11/21/94

Admiral Bobby Inman, the former director of the NSA, Deputy directory of
the CIA, and Director of Naval Intelligence spoke at Hal Abelson's MIT
class today about Clipper, export regulations and cryptography.  He was
impressive with respect to the clarity of his points, his even-handedness,
and the precision with which he addressed questions from the class.

He began his talk with the beginnings of the export control debate as
arising with mid-80's. Intelligence from the French disclosed a Soviet
"shopping list" of technologies to acquire from the West, starting with
overt purchases, and moving to covert purchases and theft if necessary.
The US government was particularly alarmed at the size of the figure for
the number of Rubles that the Soviets saved.  The resulting internal
government reaction started by working to reclassify technologies that were
previously public, and then moved restructure the ground rules for business
in order to prevent sensitive technologies from being exported in the
future.  

One of those technologies was cryptograpy. Inman said there was a myth in
the press about the value of technical intelligence as not providing
information about intentions, instead providing only information about
configurations and positions.  That's true for imaging technologies, but
communications intelligence (COMINT) does provide information about
intentions.  He said that while he can't provide specific cases, in the
last 20-30 years COMINT has provided significant information about
intentions, including cases where the military was employed.  There were
some cases where they were able to gain access to the transmissions, but
unable to go further because the adversary employed cryptography.

He mentioned that as head of the NSA, he was involved in the decision to
declassify the work related to Magic and it's successes against the
Japanese during WWII.  Even though much of the material was 40 years old
there was govt. resistance to declassification because in many instances
adversaries have employed extremely dated encryption technology, which the
NSA was easily able to crack.  It was felt that in all cases, the less said
about cryptography publicly, the better.

He touched on the mid-70's debate about public cryptography which led to
the establishment of voluntary peer review with a 30-day response from the
NSA.  He felt that this system worked for about 10 years, and finally broke
down when commercial opportunities for cryptography started to arise so
that economic incentives instead of publishing incentives framed the
debate.  (He said something about the extensive, nonpublic, dialogues
between commercial cryptographic companies and the government which
eventually became public.  I didn't quite follow this; he seemed to be
censoring himself as he said it.  Something about both parties or one party
regretting this becomming public.)  

The other side of this polarization between public cryptography and
government cryptography was an "evolution of concern" within the
government, driven by public perceptions, about white-collar crime, which
he said was a recent (since Watergate) phenomenon.  Public cryptography
threatens white-collar enforcement, because the FBI has become "totally
dependent" on wiretaps.  When asked later about the proportion of concern
within the government between the various white-collar crimes, such as
drugs, organized crime, terrorism, etc., he replied that the governmental
concern about wiretaps was and is primarily and unambiguously about
narcotics.

The driving concern about public cryptography changed from export to
domestic concerns.  This led to the technological solution, Clipper, which
he termed a mini-disaster.

He said that people inside the government miscalculated the depth of
distrust of government which led to the anti-clipper groundswell.  He felt
that this was simply a "blind spot" in those people; it's not that they
have bad motives, it's just that they can't comprehend why someone wouldn't
trust the government.  By proposing clipper (which is technologically
sound) with it's government-entity escrow, he said that they fed the
spectre of Big Brother, when it would have been better to deal with it from
the start.

One of the ways that they could have dealt with it was via commercial or
nongovernmental escrow, specifically citing the companies in Boston and NY
which deal with stock certificate transactions.  However, he was skeptical
whether nongovernmental escrow had any political future since the initial
blunder.

- From a public policy standpoint, he felt that given the single-issue voting
in the recent election, regarding crime, the public's equivalence of crime
with drugs, and the essential nature of the wiretaps as the sole source of
leads in combatting narcotics, that arguments *to the public* about privacy
would be ineffective.  Most of the public do not see wiretaps as
threatening them.  He felt that if one wanted to fight for privacy in the
public domain, the only chance was to link it with another issue that the
voting public feels strongly about: namely, Big Government, Bureaucracy.

Throughout his talk, this theme was reiterated several times: the public
does makes governmental policy by the way they vote.  The public cares
about crime.  Crime and Drugs are the same thing (in the public eye).
Arguments about privacy will not fly.  The argument must be PACKAGED in
terms that links it to an issue that the public cares about, and the public
cares about and opposes Big Government. 

He suggested that the alternatives to government wiretap abilities to
combat drugs might be random uranalysis of the public, specifically to
combat the demand side of the drug trade since enforcement against the
supply side is so terribly unsuccessful.  Note: he wasn't advocating this
action by the government, just pointing out that there are implications to
extreme positions on any issue, largely related to the public's current 
concerns.

Back to Narcotics.  He gave the statistic that 90% of the narcotics leads
related to money laundering come from domestic wiretaps.  He claimed that
international wiretaps are less valuable, because of the trail of the money
which generally travels this route:

Small US Bank <1> Large US Bank <2> Canadian Bank <3> Cayman Island <4> Columbia

He claimed that the only valuable link for enforcement is link <1> because
this identifies the individuals subject to law enforcement, while scanning
links <2> and <3> is illegal due to treaty clauses which preclude
surveilance of companies located in friendly-nation intelligence allies
(e.g. Canada) while scanning link <4> is not worthwhile because it's too
far removed and difficult to identify with specific individuals in the US.

When asked about the often rumored "you spy on my citizens, I'll spy on
yours and we'll exchange what we get" cooperation that would allow the US
to subvert restrictions on unauthorized wiretapping of citizens by having,
say Great Britain do it for them, he said that that would be illegal
because of those treaty clauses preventing such spying and it doesn't
happen; he claimed that the intelligence sharing that goes on is motiviated
by cost considerations, rather than trying to subvert laws in the form that
this rumor alleges.

He suggested that most companies are not willing to spend money on strong
cryptography and that in order to get companies more interested in strong
cryptography, there must be one or two well-publicized cases where
companies experience actual losses due to some sort of ether-sniffing.

Inman made the point that when governments are faced with problems that are
too big, they often just throw up their hands and don't deal with it.
Someone else in the class followed on this by pointing out that the logical
implication of that argument is that redoubling efforts for the adoption of
PGP or the like would effectively make the problem a big one for the
government.  

Inman was surprised by the looming introduction of VoicePGP, and said that
that would be a big problem, particularly with the advent of mobile
computers that supported VoicePGP, since much of the dealer-level narcotics
enfocement relies on such surveilance.  He pointed out, though, that
current cellular phones are difficult to monitor because "there's no
technology that can sweep up and sort out phone conversations" despite very
large investments in this.  He drew an analogy to a case where he had to
inform President Carter that an insecure dedicated private land-line to the
British Prime Minister had been compromised. Inman told Carter that the
nature of the public phone system, with its huge volume and unpredictable
switching, would have made using a pay phone more secure.

Inman, when asked about foreign export restrictions felt that the best way
to remain ahead technologically was not to restrict export, but speed the
pace at which you advance domestically.  The current global economic system
is very different from the days when export constraints were first
proposed, and that they're probably not applicable.

Many of you might remember the controversial hearings regarding Clinton's
nomination of Inman for DCI about a year ago; it was rumored in the press
that William Saffire of the New York Times and Senator Dole had worked out
a pact, whereby Dole would sink Inman if Saffire would sink Clinton.  This
rumor was never substantiated, but Saffire's scathing editorial about Inman
stemming from an incident in which he felt that Inman has lied to him
helped scuttle Inman's nomination. 

Today, Inman mentioned that his privacy had been invaded during the
nomination process; when asked for elaboration, he cited cases of the press
going around asking questions about his wife and sons.  So Inman seems
sensitive to issues of privacy, but in this case, they seem to be primarily
associated with invasions of privacy by the media rather than by the
government.

In all, Inman gave a balanced talk, concerned primarily with clarifying the
motives of the different players (the govt and the public) to make some
sense of complicated issues.

-----BEGIN PGP SIGNATURE-----
Version: 2.6.1

iQCVAwUBLtNXcd2yvmfs/TJFAQFWGgP/eao60HTSIkIxHpNQH0SDhUwLWkc8e6Ez
mFOF425xMfypvQWSM19OOFfqNFwUxb/3NAMPapedPXgoolZn1jNzswLbdduNTxkS
WXWRzMb3/u2CyW9bYYWE2wq3xdT1QAsSjWhPRG04k6G6g7dy9ne4aqeUkEtbn+sX
M3cmDCKphOE=
=rBX4
-----END PGP SIGNATURE-----
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991003181052/http://www.somewhere.com/)