---
id: rre-governing-cyberspace
title: "[RRE]Governing Cyberspace"
type: writing
writing_type: rre-post
date: 1998-06-05
url: http://commons.somewhere.com:80/rre/1999/RRE.Governing.Cyberspace.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - rre
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1999/RRE.Governing.Cyberspace.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20000523043143/http://commons.somewhere.com/rre/) | **Most Recent Article: Mon, 22 May 2000** |

# [RRE]Governing Cyberspace

```
[Forwarded by permission and reformatted.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html
or send a message to requests@lists.gseis.ucla.edu with Subject: info rre

---

[http://www.temple.edu/lawschool/dpost/icann/comment1.html]

			Governing Cyberspace,
				 or
	      Where is James Madison When We Need Him?

	     David G. Post -- Plugging in -- June 1999

In a column last Fall I suggested that the pending reorganization of
the Internet's domain name system (DNS) had the potential to become
cyberspace's own 'constitutional moment', a profound and thorough
transformation of the institutions and processes responsible
for law-making and regulation on the global electronic network.
Over the last several months, the shadowy outlines of a new kind of
constitutional structure for cyberspace have indeed begun to emerge.
The consequences of these developments for the Internet's future could
not be more profound, and the picture that is emerging is not always
a pretty one.  Not many people are paying close attention to these
developments; they should.  Not to be an alarmist, but to boil a
frog alive, the parable tells us, you need just to turn up the heat
by increments so small that the frog never notices -- never pays
attention to -- the rising temperature until it is too late to do
anything about it (like jump out of the pot).  Well, the temperature
on the Internet is starting to rise.

1. (A bit of) Background

[Those of you who already know how the DNS works, and what a "root
server" is, might want to skip ahead to (2) . . . ]

For the Internet to exist as a single coherent network, there must be
a way to be sure that a message sent from any point on the network to
janedoe@xyz.com, or a request to view the webpage at www.school.edu,
is routed to the "right" machine; that is, each of those addresses
(xyz.com or www.school.edu) must be associated unambiguously with a
particular machine if message traffic is to move in a predictable way.

To make an extremely long story short, the global network we call "the
Internet" manages this by, first, requiring that each machine on the
network have a unique numerical address [e.g., 123.45.67.89]; indeed,
to be "on the Internet" means to have (or to be connected to) a
machine to which such an address has been assigned.  For your message
to www.school.edu to be routed correctly, your computer must somehow
be able to find the numerical address corresponding to the machine
named www.school.edu.  This is accomplished, on the Internet, by means
of what Tony Rutkowski calls a "magical mystery tour".

When you send off a message requesting a copy of the www.school.edu
home page ("http://www.school.edu"), the message first stops off at a
machine known as a "DNS [Domain Name System] server".  It is the job
of the DNS server, which is usually operated by your Internet Service
Provider, to find the correct numerical address for your message.
The DNS server reads, in effect, from right to left; seeing that this
is a message destined for some machine in the EDU domain, it needs to
find out where addresses in the EDU domain are stored.  It does this
by asking a different machine (known as the "root server") that very
question: "Who is responsible for the EDU domain?".  The root server
replies with the numerical address of a different machine (known as
the "EDU domain server").  Your DNS server then asks the EDU domain
server the question: "Who is responsible for school.edu?".  The EDU
domain server replies with another numerical address [or with "Not
Found" if it cannot find an entry for "school.edu" in its database of
names and addresses].  Your DNS server then asks this machine: "Who
is responsible for www.school.edu?".  School.edu replies with yet
another numerical address, and now your DNS server has completed its
task; once it receives the address for www.school.edu, it places that
address into your message and sends it on its way(1).

How does this all work as smoothly as it does?  Who is in charge of
the root server?  How does the operator of the root server decide
which machines are the "authorized" domain servers for EDU, or COM,
or ORG, or any of the other top-level domains?  Who controls those
machines (and the database of names and addresses contained in them)?
And how is this whole scheme enforced?  That is, what makes the root
server "the" root server?  Why do the many thousands of Internet
Service Providers, operating the many thousands of DNS servers
worldwide, all use the same root server?

In the early days of the Internet, of course -- through, say, the
early 90s -- no one outside the small cadre of engineers that was
putting the system together cared very much about the answers to these
questions.  There were, of course, answers to them all.  The United
States government had long operated the root server (a holdover from
the days that the Internet was a Defense Department project), and
had worked with something known as the Internet Assigned Numbering
Authority (IANA) -- a group of engineers led by the late Jon Postel
-- to organize the necessary data and to see that the various domain
servers were being properly managed.

As long as it all seemed to be working smoothly enough; who cared
what was going on behind the Wizard's curtain?  And who noticed when,
in 1992, as the extraordinary growth of the network began to outstrip
the management capacity of this (largely volunteer) operation,
the U.S. government engaged a private firm, Network Solutions, Inc.
(NSI), to manage and maintain the databases and domain servers for the
COM, ORG, and NET domains?

But slowly, as more and more people began to realize that the Internet
was a Really Big Deal (and that these funny "domain name" things
might actually be of real value), more and more people started to pay
attention to all of this, and this arrangement began to come under
increasing fire from many quarters.  The government and NSI found
themselves increasingly under attack from within and without the Net
community-- by those challenging NSI's apparent monopoly control over
these increasingly valuable top-level domains, by trademark owners
concerned about domain names that appeared to infringe upon their
valuable trademark rights, and others.

As the expiration date of the government's contract with NSI
approached last June, the Commerce Department announced that the
government wanted to get out of the DNS management business entirely.
Citing "widespread dissatisfaction about the absence of competition
in domain name registration", and the need for a "more formal and
robust management structure", the government proposed transferring
responsibility for management and operation of the DNS to a
private non-profit corporation.  This new corporation, to be formed
by "Internet stakeholders" on a global basis, would take over
responsibility for overseeing the operation of the authoritative
Internet root server.(2)

2. Um, What Does This Have To Do With "Internet Governance"?

This new corporation -- ICANN, the Internet Corporation for Assigned
Names and Numbers -- has, over the past several months, set up shop
and gotten to work.  It's been a busy time.  It has begun to establish
"Supporting Organizations", new coalitions comprising various Internet
constituencies (e.,g., domain name registrars, trademark owners) who
will be responsible for electing certain members of the ICANN Board of
Directors and for formulating aspects of domain name policy.  It has
accredited five companies (America Online, CORE (Internet Council of
Registrars), France Telecom/Oleane, Melbourne IT, and register.com) to
begin issuing registrations in the COM, ORG, and NET, domains during
a two-month test period (along with twenty-nine other entities who can
begin accepting registrations in these domains once the test phase is
completed).  It commissioned, and recently adopted (in part), a report
from the World Intellectual Property Organization (WIPO) outlining
the procedures to be used in cases involving "cybersquatting"
(the intentional "warehousing" of domain names for later sale).
[Information about all of the above can be found at the ICANN home
page.]

My goal here is not to discuss any of these specific actions; there
is much here to digest and debate, pro and con, and I will have a
great deal more to say about the specifics of ICANN's activities over
the next several months.  [As, I hope, will others; I particularly
recommend Michael Froomkin's commentary on the WIPO Report referenced
in the preceding paragraph]

Rather, my goal here is just to suggest that notwithstanding the
government's (and ICANN's) protestations to the contrary, this is
about nothing less than Internet governance writ large.  The Commerce
Department took pains to characterize it in other terms; this new
corporation would be responsible only for "technical management
of the DNS", the "narrow issues of management and administration of
Internet names and numbers on an ongoing basis" -- sort of what the
International Telecommunications Union does with respect to managing
interconnections on the international telephone network.  This new
framework for managing the DNS

  ". . . does not set out a system of Internet 'governance'.  Existing
  human rights and free speech protections will not be disturbed and,
  therefore, need not be specifically included in the core principles
  for DNS management.  In addition, this policy is not intended to
  displace other legal regimes (international law, competition law,
  tax law and principles of international taxation, intellectual
  property law, etc.) that may already apply.  The continued
  applicability of these systems as well as the principle of
  representation should ensure that DNS management proceeds in the
  interest of the Internet community as a whole."(3)

It is all well and good to say that this new institution will not
be engaged in Internet governance -- but words will not make it so.
Any entity exercising control over the DNS will be subject to immense
pressure to do more than mere "technical management", because, bizarre
as it may seem at first glance, the root server, and the various
domain servers to which it points, constitute the very heart of the
Internet, the Archimedean point on which this vast global network
balances.

To appreciate that, imagine for the moment that you had control over
operation of the root server.  You alone get to decide which machines
are "authoritative" domain servers for the COM, NET, ORG, EDU, and
the other top-level domains, the machines to which all Internet users
worldwide will be directed when they try to send any message to any
address in those domains.  You have the power, therefore, to determine
who gets an address in those domains -- who gets a passport without
which passage across the border into cyberspace is impossible.
You can say "From now on, we will use the data in machine X as the
authoritative list of COM names and addresses, but only so long as the
operator of that machine complies with the following conditions", and
then you can list -- well, just about anything you'd like, I suppose.
It's your root server, after all.  You can require that all domain
server operators pay you a certain fee, or provide you with particular
kinds of information about the people to whom they have handed out
specific names and addresses, or only allow transmission of files
is a specified format, or abide by a particular set of laws or rules
or regulations.  And you can demand that they "flow through" these
conditions (or others) to anyone whom they list in their authoritative
databases, that they revoke any name given to anyone who does not
pay the required fee, or provide the required information, or use
the specified file format, or comply with the specified rules and
regulations.

This is quite literally a kind of life-or-death power over the global
network itself, because presence in (or absence from) this chain of
interlocking servers and databases is a matter of [network] life or
death: If your name and address cannot be found on the "authoritative"
server, you simply do not exist -- at least, not on the Internet.
Eliminate the entry for xyz.com from the COM domain server and xyz.com
vanishes entirely from cyberspace; designate as the new COM domain
server a machine that does not have an entry for xyz.com in its
database, and you have imposed the electronic equivalent of the death
penalty on xyz.com.

Anyone interested in controlling the rules under which activities
on the Internet take place -- and many commercial interests, who now
realize the huge economic stake they have in this medium, and many
governments, who have spent the last few years worrying about how
they would ever get back their taxing and regulatory authority over
Internet transactions, find that they are indeed quite interested in
that now -- is likely to find the existing of a single controlling
point awfully tempting.  Anyone with a vision of how the Internet can
be made a "better" place -- by making it safer for the exploitation
of intellectual property rights, say, or by eliminating the capability
to engage in anonymous transactions, or by making it more difficult
for children to get access to indecent material -- is likely to view
control over the root server as the means to impose its particular
vision on Internet users worldwide.  After all the talk over the past
few years about how difficult it will be to regulate conduct on the
Internet, the domain name system looks like the Holy Grail, the one
place where enforceable Internet policy can be promulgated without
any of the messy enforcement and jurisdictional problems that bedevil
ordinary law-making exercises on the Net.

And that is why these are governance questions, why any reorganization
of this system, far from being an arcane technical detail of Internet
engineering, is inherently of constitutional significance.  Power
corrupts, absolute power corrupts absolutely -- on the Internet as
elsewhere.  Questions about constraining any form of absolute power
are constitutional questions of the highest order, and "governance"
means nothing more (and nothing less) than the search for mechanisms
to insure that absolute power is not exercised in an unjust or
oppressive manner.  How can we be assured that ICANN will be able
to resist pressures to stray beyond this limited "technical" mandate?
Where are the checks on the new corporation's exercise of its powers?

You think, perhaps, that I exaggerate the significance of these
developments, and perhaps I do.  But let me point to a few dark clouds
on the horizon that make me very, very nervous about what ICANN is
up to.  Remember all those things you could do if you were in control
of the root?  Like "require that domain server operators pay you
a certain fee"?  Well, ICANN has imposed the requirement that each
accredited registrar pay ICANN a fee of $1 for each new domain name
they hand out -- can anyone say "taxation without representation"?
Or "provide you with particular kinds of information about the people
to whom they have handed out specific names and addresses"?  ICANN,
having now endorsed the WIPO Report referenced earlier, is about
to impose a requirement on all domain name registrars that they
collect and make available "accurate and reliable contact details
of domain name holders", and that they agree to "cancel the domain
name registrations" wherever those contact details are shown to be
"inaccurate and unreliable" -- a move with grave consequences for the
continued viability of anonymous communications on the Internet.  Or
"abide by a particular set of laws or rules or regulations"?  The WIPO
Report, again, envisions that all claims by trademark holders that a
domain name registrant registered an infringing name "in bad faith" be
submitted to a single, uniform, worldwide dispute resolution process
for adjudication.

Now, some, or even all, of these may be good ideas.  But this is
already way beyond the realm of technical "standards-setting", and
we really must ask whether we really want or need this kind of global
Internet policy and whether this is the way it should be put together.
When did the affected constituency -- all Internet users worldwide --
decide that they want a global policy-making organ of this kind?  Who
decided that the bottom-up, decentralized, consensus-based governance
structures under which the Internet grew and flourished are
incompatible with its continued growth and development?  When are we
going to get a chance to ratify these new arrangements?

There are hard questions here, but one thing is clear; we need
to disabuse ourselves of the notion that this is somehow not about
Internet governance if we are going to make any serious headway
on them.  We know something about how institutions that possess
life and death power can be constrained, about constitutions and
constitutionalism, about the fragmentation of power and the need for
checks on the exercise of power, and we better start thinking about
this problem in these terms before too much more time elapses.

Oh -- and about James Madison?  Madison not only thought more clearly
and more insightfully about these questions than anyone before or
since, he understood the necessity for public discussion and debate
about issues of this kind; the Federalist Papers, in which he and
Alexander Hamilton (and a somewhat recalcitrant John Jay) laid out the
arguments for (and against) the constitutional structure put together
in Philadelphia in 1787, began life, let us not forget, as newspaper
columns appearing weekly in the New York press.  We could do worse
than to start thinking about updating that for the new cyber world we
are building now.

---

---

1. (Of course, the engineers have designed any number of tricks to
speed up this process -- each DNS server, for example, stores the
answers it receives to these various queries for a period of time,
cutting down on the need to ask the same questions over and over again
-- but that need not concern us here).

2. It would be guided, in the government's view, by four basic
principles: first, inasmuch as the "stability of the Internet should
be the first priority of any DNS management system", the new system
"should not disrupt current operations or create competing root
systems"; second, "decentralized market mechanisms" should drive DNS
management; third, the private process should "reflect the bottom-up
governance that has characterized development of the Internet to
date"; and fourth, the management of the new corporation should
"reflect the functional and geographic diversity of the Internet and
its users".

3. These quotes all come from the Department of Commerce's "White
Paper", entitled "The Management of Internet Names and Addresses"
(June 5, 1998), available here.

end
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20000523043143/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20000523043143/mailto:webmaster@somewhere.com). |