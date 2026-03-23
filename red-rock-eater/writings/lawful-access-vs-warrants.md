---
id: lawful-access-vs-warrants
title: "\"Lawful access\" vs warrants"
type: writing
writing_type: rre-post
url: "http://commons.somewhere.com:80/rre/1998/Lawful.access.vs.warrant.html"
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - civil-liberties
  - cryptography
  - democracy
  - education
  - forwarded-content
  - government-info
  - law
  - libraries
  - media
  - military
  - privacy
  - rre
  - rre-post
  - surveillance
  - telecommunications
---



## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1998/Lawful.access.vs.warrant.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991012142339/http://www.somewhere.com/)

  

# "Lawful access" vs warrants

```
[Forwarded with permission and reformatted to 70 columns.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Sun, 19 Apr 1998 13:43:21 -0700
From: John Gilmore <gnu@toad.com>
X-List: cypherpunks@cyberpass.net
Subject: "Lawful access" vs warrants:  I found the difference today!

Remember how in the Clipper debate, the government insisted on using
the term "lawful access" when talking about what the government had
to do to get keys out?  They implied it meant a warrant issued by a
judge, but actually the proposed rules said any "lawful access" would
do.  That phrase kept reappearing in government proposals.

I've been looking for years in the laws to find what secret loophole
they've been trying to protect.  Today I ran across it!

It's Executive Order 12333, signed by our favorite senile president,
Ronald Reagan, in 1981.  It says:

    2.5 Attorney General Approval.  The Attorney General hereby is
    delegated the power to approve the use for intelligence purposes,
    within the United States or against a United States person abroad,
    of any technique for which a warrant would be required if
    undertaken for law enforcement purposes, provided that such
    techniques shall not be undertaken unless the Attorney General has
    determined in each case that there is probable cause to believe
    that the technique is directed against a foreign power or an agent
    of a foreign power. Electronic surveillance, as defined in the
    Foreign Intelligence Surveillance Act of 1978, shall be conducted
    in accordance with that Act, as well as this Order.

In other words, if the Attorney General claims that someone is an
agent of a foreign power, no warrants are needed; the target has no
Constitutional rights any more:

    Fourth Amendment

    The right of the people to be secure in their persons, houses,
    papers, and effects, against unreasonable searches and seizures,
    shall not be violated, and no warrants shall issue, but upon
    probable cause, supported by oath or affirmation, and particularly
    describing the place to be searched, and the persons or things to
    be seized.

You will recall that the Attorney General made exactly this claim
about Martin Luther King (that he was an agent of a foreign power),
to justify the years of FBI surveillance.  For all we know, they have
been claiming that anyone who advocates crypto legalization must be an
agent of a foreign power.  It really wouldn't surprise me.

We shouldn't stop looking for more loopholes -- they may have several --
but I think this is the big one.

       John

Date: Sun, 19 Apr 1998 22:00:51 -0400
From: "Stewart Baker" <sbaker@steptoe.com>
To: <farber@cis.upenn.edu>
Subject: John Gilmore gets one wrong

John Gilmore claims that the government's references to "lawful
access" mean that the government will be using EO 12333 to perform
warrantless key seizures on anyone the Attorney General decides to
classify as a foreign agent.  He says Martin Luther King qualified as
a foreign agent and that perhaps so will opponents of key recovery.

John is wrong.

The Foreign Intelligence Surveillance Act governs electronic
intercepts of foreign agents with a connection to the US (located
here, communicating into or out of the US, US nationals, etc.).  The
Act requires a warrant (from a special court that is set up to handle
very secret data) and it has been tested in court many times without
being held in violation of the fourth amendment.

Under the law, "foreign agent" is a defined term; MLK would not have
qualified, nor would somebody who takes money to lobby for foreign
governments even if he is registered as an official foreign agent for
registration purposes.  Basically, it covers spies and employees of
foreign governments, agents of terrorist organizations, etc.

There is an exception to the warrant requirement.  In a declared
emergency the Attorney General can waive the obtaining of a warrant.
For about 48 hours, at which point the case has to go to court.
Not exactly a civil liberties scandal, but it probably explains the
reluctance of government representatives to use the phrase "warrant"
instead of "lawful access."

Stewart Baker

Date: Mon, 20 Apr 1998 09:58:51 -0700
From: John Gilmore <gnu@toad.com>

Stewart is distracting you into wiretap law.  EO 12333 is much more
broad.  It claims to allow the Attorney General the use of any
activity that would normally require a warrant -- such as a physical
search -- if he merely claims probable cause to believe

    that the technique is directed against a foreign power or an agent
    of a foreign power.

Stewart is correct that wiretaps under EO 12333 must also follow the
FISA.  But non-wiretap activities under EO 12333 aren't covered by
FISA.

The FISA was written before key escrow was even contemplated.  It
doesn't cover or control the obtaining of keys from third parties.  It
covers electronic intercepts of the communications of people suspected
of being foreign agents.  (I like how Stewart says it "governs
electronic intercepts of foreign agents".  If we're investigating
them, they must be guilty!)

The proponents of Clipper knew this was a hot button for us -- if
their intentions were innocent, why didn't they defuse it by replacing
the phrase "lawful access" with "court order"?

Stewart was undoubtedly in on the drafting of the Clipper proposals.
If he thinks my theory that EO 12333 is part of "lawful access" is
full of holes, have him propose his own.  I challenge him to give an
exact legal definition of "lawful access", naming the complete set of
statutes, regulations, Executive Orders, and other circumstances under
which he believes the phrase would authorize the release of escrowed
encryption keys to anyone.

	John

Date: Mon, 20 Apr 1998 10:54:05 -0400 (EDT)
From: "Michael Froomkin - U.Miami School of Law" <froomkin@law.miami.edu>
To: Dave Farber <farber@cis.upenn.edu>
Subject: Re: IP: "Lawful access" vs warrants:  I found the difference today!

I'm afraid this is really, really old news.  Congress passed the law
authorizing this some time ago, and it was widely reported and written
up.

E.g.:

[from http://www.law.miami.edu/~froomkin/artticles/clipper.htm
in footnote 492.]

492.  Warrantless wiretaps are authorized by the Foreign Intelligence
Surveillance Act (FISA), 50 U.S.C. =A7 1802(a) (1988). The President,
acting through the Attorney General, may authorize electronic
surveillance for up to one year if the surveillance is directed solely
at communications between or among foreign powers, there is no
substantial likelihood of acquiring communication of U.S. citizens,
and minimization procedures have been followed. See id. Title 18 of
the U.S. Code also permits warrantless surveillance in emergency
situations involving immediate danger, death, or serious physical
injury to any persons; conspiratorial activities threatening the
national interest; or conspiratorial activities characteristic of
organized crime. See 18 U.S.C. =A7 2518(7) (1988).

[and from note 493:]

Congress recently authorized the FISA court to issue warrants for
national security break-ins and inspections of the interior of
buildings by "technical means."  Intelligence Authorization Act for
Fiscal Year 1995, Pub. L. No. 103-359, tit. VIII, =A7 807(a), =A7
301(5), 108 Stat. 3423, 3444 (1994) (to be codified at 50 U.S.C. =A7
1821). This authority can be used against American citizens if the
Justice Department persuades the FISA court that the suspects are
agents of a foreign power.  See id. =A7 301(b), 108 Stat.  3423,
3445; see also United States v. Humphrey, 629 F.2d 908, 912-14 (2d
Cir. 1980) (holding that a warrantless search did not violate the
Fourth Amendment because it was related to national security); In re
Application of the United States for an Order Authorizing the Physical
Search of Nonresidential Premises and Personal Property (F.I.S.C.
1981) (holding that a FISA order was not required, and was at any rate
unavailable due to lack of jurisdiction, for A warrantless national
security break-in), reprinted in S. Rep. No. 280, 97th Cong., 1st
Sess. 16 (1981).

[and from the text around there:]

The law says the government may paw through a citizen's garbage
without a warrant,{484} and that she lacks a reasonable expectation of
privacy in relation to telephone numbers dialed.{485} The police may
fly over her house in A helicopter at four hundred feet{486} and use
special cameras to photograph everything below.{487} The government
may [Page 824]use satellites to spy in her windows;{488} it may use
heat- detection gear to monitor heat emanations from her home;{489}
it may use dogs to sniff her luggage and her person.{490} Once the
government has arranged for an informant to plant a beeper on A
citizen, the government may use the signal to track the citizen's
movements.{491} When national security is at risk, many procedural
[Page 825]protections that are required in the ordinary course of
an investigation are suspended. For example, the government may,
for reasons of national security, break into some premises without
a warrant to plant a bug, whereas the same action in an ordinary
criminal investigation would require a warrant.{492} National security
wiretap requests go to a secret court that meets in camera and never
issues opinions.{493}

A. Michael Froomkin        | +1 (305) 284-4285; +1 (305) 284-6506 (fax)
Associate Professor of Law |=20
U. Miami School of Law     | froomkin@law.tm          http://www.law.tm=20
P.O. Box 248087            |  =20
Coral Gables, FL 33124 USA | It's warm here.

Date: Mon, 20 Apr 1998 10:21:55 -0700
From: John Gilmore <gnu@toad.com>
To: "Michael Froomkin - U.Miami School of Law" <froomkin@law.miami.edu>
Subject: Re: IP: "Lawful access" vs warrants: I found the difference today! 

Michael, thanks for your response.  I think you, like Stewart, focused
on FISA and wiretap law, while EO 12333 appears much more broad.

I did notice when they expanded the FISA court to let it approve
break-ins too -- though apparently under the EO they can just do
break-ins, physical searches, and black bag jobs (burglary) WITHOUT
the approval of any court as well.

Thanks for the pointers to court cases which are claimed to say that
no warrants are needed under the Fourth Amendment if some government
geek claims a classified reason that national security is at stake.
I'll get them and read them.

I heard a rumor that the Attorney General's authority to authorize
searches without a warrant, under EO 12333, has since 1981 been
delegated several levels down in the Justice Department.  Know
anything about that?

	John

Date: Mon, 20 Apr 1998 13:29:27 -0400 (EDT)
From: "Michael Froomkin - U.Miami School of Law" <froomkin@law.miami.edu>
To: John Gilmore <gnu@toad.com>
Subject: Re: IP: "Lawful access" vs warrants: I found the difference today! 
cc: Dave Farber <farber@cis.upenn.edu>, Ken Bass <Ken@bassandco.com>,
        Shirley and Ken Bass <bassanco@access.digex.net>

I vaguely recall that it got delegated down a few levels.  Ken Bass
would know -- he would have worked for the person who signed them, or
done it himself! But that's still a small number of people - one level
down is the #2, the next is small, and then you have assistant AGs who
are not that numerous either.  But I could be wrong about this.

The thing to understand in parsing the EO vs. statute stuff is this:
the executive branch has never agreed that it needs congressional
approval for national security work, claiming it's an inherent
executive function.  But they are quite happy to avoid testing this in
court if possible.

National security regulations are exempt for the APA, so an EO is an
appropriate way to do implementing regulations; you don't mention the
statute so you don't create a precedent of admitting you rely on the
statute.

I've cc'd Ken since he's far more expert than I on this.  ...

A. Michael Froomkin        | +1 (305) 284-4285; +1 (305) 284-6506 (fax)
Associate Professor of Law | 
U. Miami School of Law     | froomkin@law.tm          http://www.law.tm 
P.O. Box 248087            |   
Coral Gables, FL 33124 USA | It's warm here.

Date: Mon, 20 Apr 1998 10:44:24 -0700
From: John Gilmore <gnu@toad.com>
To: "Michael Froomkin - U.Miami School of Law" <froomkin@law.miami.edu>
cc: John Gilmore <gnu@toad.com>, Dave Farber <farber@cis.upenn.edu>,
        Ken Bass <Ken@bassandco.com>,
        Shirley and Ken Bass <bassanco@access.digex.net>, gnu

> The thing to understand in parsing the EO vs. statute stuff is this:
> the executive branch has never agreed that it needs congressional
> approval for national security work, claiming it's an inherent
> executive function.

That's a great theory, but where do Constitutional rights fit into it?
Is the theory that the Fourth Amendment doesn't require warrants
for unreasonable searches, that it only says, "If you get a warrant,
it must only issue based on ..."?  Or is the idea that anything
the Executive Branch is scared of (i.e. the national security is in
danger!) must provoke a reasonable search instead of an unreasonable
one?

This starts to sound a lot like the USSR Constitution -- high sounding
phrases, completely vitiated in actual administration.

	John

Date: Tue, 21 Apr 1998 10:26:55 -0400
From: Ken Bass <kcbass@venable.com>
To: John Gilmore <gnu@toad.com>
Subject: Re: IP: "Lawful access" vs warrants: I found the difference today!
CC: "Michael Froomkin - U.Miami School of Law" <froomkin@law.miami.edu>,
        Dave Farber <farber@cis.upenn.edu>

John, Michael, et al.

I have always understood the "lawful authority" reference to be a
codeword for "court order where required, AG approval where not
required."

There are several categories of AG-only approvals.  Under FISA the
AG alone approves surveillances of "purely foreign establishment"
targets, e.g., dedicated channels within a foreign power's facilities,
in certain circumstances.  As to physical searches, when we were "in
power" AG Civiletti decided as a matter of policy to seek orders from
the FISA court for physical searches as well as ELSURs, retaining the
option to use the "inherent executive power" argument that the courts
have come close to holding unconstitutional --but never actually done
so.  Each administration has claimed that power, similar to a line of
assertions of Executive power in a variety of national
security/foreign power areas.

Suffice it to say that during the Cart Administration we were
sufficiently unsure of the legitimacy of the claim that we decided, as
a matter of policy, to always try to get a court order.

The FISA court accepted and granted our physical search applications.
When the new administration assumed office, they held a different
view and managed to persuade the FISA court that it did not have
jurisdiction to issue physical search orders.  Finally Congress got
around to amending FISA to add such authority and DOJ is, I assume,
obeying the law.

As to the level of authority, when I was there it was at the Deputy
AG level (#2) or higher.  That may have changed, but I have not kept
current on any internal delegations.  If you wish, I can easily check
and get back to any of you.

Not knowing exactly what Stewart has said, I hesitate to comment
on his views, but I would be surprised if he did not also view the
"lawful order" phrase as encompassing those non-warrant instances that
have been encountered over the years where the Pres. has relied on
"inherent executive power."

Ken

Date: Wed, 22 Apr 1998 15:46:37 -0500
From: Jim Dempsey <jdempsey@cdt.org>
To: John Gilmore <gnu@toad.com>
Subject: IP: "Lawful access" vs warrants

John,

Your above captioned comment on IP was forwarded to me.

>Remember how in the Clipper debate, the government insisted on using
>the term "lawful access" when talking about what the government had
>to do to get keys out?  They implied it meant a warrant issued by a
>judge, but actually the proposed rules said any "lawful access" would
>do.  That phrase kept reappearing in government proposals.
>
>I've been looking for years in the laws to find what secret loophole
>they've been trying to protect.  Today I ran across it!
>
>It's Executive Order 12333, signed by our favorite senile president,
>Ronald Reagan, in 1981.  It says:

>We shouldn't stop looking for more loopholes -- they may have several --
>but I think this is the big one.

There are many other forms of "lawful access" not requiring a judicial
warrant.  For example, the Fourth Amendment does not apply at the
border: the government can seize your laptop and inspect and probabaly
copy its contents without a court order, without probable cause,
without even the showing of some degree of suspicion that is required
for even simple encounters with police on the street within the
borders.  See United States v. Ramsey, 431 U.S. 606 (1977), where the
Supreme Court stated, "That searches made at the border, pursuant to
the longstanding right of the sovereign to protect itself by stopping
and examining persons and property crossing into this country, are
reasonable simply by virtue of the fact that they occur at the border,
should, by now, require no extended demonstration."

Also, of course, no court order is required for the government to
corrupt your employee or your lover, who may then copy those things
to which you have given him or her access and provide them to the
government.  These people are called informants or "cooperating
witnesses" and they are not subject to the Fourth Amendment because
you have consented to their presence in your life.  Ditto for your
employee or lover who gets pissed off at you and walks out with a copy
of everything on your hard drive and turns it over to the government
(assuming, again, that the employee or lover was somewhere you had
allowed them to be).  Dumpster-diving is also a form of "lawful
access."

And of course, "lawful access" often means by subpoena.  Grand jury
subpoenas are issued in the name of a grand jury, which is technically
subject to the supervision of a judge, but in fact they are forms
signed by the assistant prosecutor and never seen or approved by
members of the grand jury, let alone by a judge.

On top of that, many administrative agencies are authorized to issue
"administrative subpoenas."  At the federal level alone, we identified
200 grants of subpoena authority to federal agencies, including to
the FBI and DEA in drug cases.  Typically, these statutes authorize
an executive branch official or agency to issue subpoenas "for any
papers, correspondence, memoranda or other records that the Secretary
[or Board or Commisssion] deems relevant and material."  The Supreme
Court has held that an administrative agency can investigate "merely
on suspicison that the law is being violated, or even just because it
wants assurance that it is not."  US v. Morton Salt Co., 338 US 632
(1950).

It is precisely because there are some many means of "lawful access"
to plaintext, ciphertext and decryption keys not requiring judicial
approval that we have called for legislation creating specific
statutory court order requirements. Some have criticized our support
for court order requirments as paving the way for key recovery, but to
do nothing is to accept the many forms of "lawful access" that do not
require court approval.

>PS: It isn't clear that the President has the authority to do this.
>The claimed authority is "the National Security Act of 1947, as
>amended".  I doubt it delegates to the President the right to approve
>warrantless searches of US citizens.  Even if it did, I doubt whether
>such a provision would be Constitutional.  I'd be very interested in
>knowing if any court has ever looked at whether this Executive Order
>has any effect at all on the civil rights of US persons.

In United Presbyterian Church v. Reagan, the validity of E.O. 12333,
particualrly sec. 2.5, was challenged by political and religious
organizations, journalists, academics and a member of Congress.  The
suit was dismissed on the ground that no plaintiff could demonstrate
injury in fact.  Plaintiffs, of course, had been prevented from
conducting discovery that might have revealed injuries.  In 1984, the
federal court of appeals for the District of Columbia affirmed the
dismissal.

The courts have never conclusively ruled on the constitutionality of
warrantless physical searches.  In the John Ehrlichman case, Judge
Gesell held that warrantless search of the office of Daniel Ellsberg's
psychiatrist, undertaken in the name of national security, was clearly
illegal under the Fourth Amendment.  But in a 1978 case involving two
alleged spies for North Vietnam, one of them a US citizen, the courts
upheld warrantless searches approved by Pres. Carter and Attorney
General Bell under the predecessor to E.0. 12333.

In any case, section 2.5 of E.O. 12333 was superseded by legislation,
adopted, I think, in 1994.  50 USC 1821 - 1829.  Now the Attorney
General can authorize physical searches on her own only of premises,
property or material "used exclusively by, or under the open and
exclusive control of, a foreign power."  Searches directed at agents
of foreign powers must be approved by the Foreign Intelligence
Surveillance Court.  My boss at the time, Cong. Don Edwards was one of
the few who objected, arguing, that these "black bag jobs" should be
abolished altogether, not given to the FISA court.

Glad you asked?

Best regards,

Jim Dempsey

Center for Democracy and Technology
1634 Eye Street, NW Suite 1100
Washington DC, 20006
voice: 202.637.9800 x112     fax: 202.637.0968

                * WORKING FOR DEMOCRATIC VALUES IN A DIGITAL AGE *
                Protecting Free Speech and Privacy on the Internet
			      http://www.cdt.org/

Date: Wed, 22 Apr 1998 16:05:37 -0700
From: John Gilmore <gnu@toad.com>
To: Jim Dempsey <jdempsey@cdt.org>

Thanks for your note.  It helps to talk with people who have seen this
from the other side.

> warrant.  For example, the Fourth Amendment does not apply at
> the border: the government can seize your laptop and inspect and
> probabaly copy its contents without a court order, without probable
> cause, without even the showing of some degree of suspicion that is
> required for even simple encounters with police on the street within
> the borders.

So the gov't proposal under Clipper was that in a border search, they
be able to access the key repository to unlock any encrypted stuff you
have on your hard drive?

> Also, of course, no court order is required for the government to
> corrupt your employee or your lover, who may then copy those things
> to which you have given him or her access and provide them to the
> government.

This would not qualify for a key access though -- just because they
were given a hard-drive full of encrypted stuff, they'd still need
some form of due process to get the keys out.  Or were they really
claiming, "If we have possession of some encrypted data, that IN
ITSELF is enough reason that the key escrow center has to give us the
key"?

> And of course, "lawful access" often means by subpoena.  Grand
> jury subpoenas are issued in the name of a grand jury, which is
> technically subject to the supervision of a judge, but in fact
> they are forms signed by the assistant prosecutor and never seen
> or approved by members of the grand jury, let alone by a judge.

I have never had the pleasure of serving on a grand jury.  What an
amazing fishing expedition.  If I ever do get to serve, is there
anything I can do as a grand juror to object to this sort of conduct?
To at least see what subpoenas are going out under my name?

> DEA in drug cases.  Typically, these statutes authorize an executive
> branch official or agency to issue subpoenas "for any papers,
> correspondence, memoranda or other records that the Secretary [or
> Board or Commisssion] deems relevant and material."

Normally the target of the subpoena would be required to decrypt any
encrypted materials that fall within the subpoena, just as they are
required to get them from dead storage if they're offsite, or to
unlock the safe if they're in one.  That's what I have been assuming.
Are you assuming that today a company could encrypt all its records
and then respond to a subpoena with, "Here you go, all the relevant
encrypted records..."?

> It is precisely because there are some many means of "lawful access"
> to plaintext, ciphertext and decryption keys not requiring judicial
> approval that we have called for legislation creating specific
> statutory court order requirements. Some have criticized our support
> for court order requirments as paving the way for key recovery, but
> to do nothing is to accept the many forms of "lawful access" that do
> not require court approval.

This isn't clear from the above.  The only examples you gave that
seems to be an issue is the border search.  What's the state of the
law today with respect to grand juries?  Do they or don't they have
the power to demand translation, decryption, interpretation, etc?
Or can they merely demand that any physical records be turned over
to them?

> Glad you asked?

Very much so; thanks!

	John
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991012142339/http://www.somewhere.com/)