---
id: messages-on-spam
title: messages on spam
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1996/messages.on.spam.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - forwarded-content
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1996/messages.on.spam.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991010032257/http://www.somewhere.com/)

  

# messages on spam

```
[I have enclosed two messages about resisting spam.  The first is from Stanton
McCandlish at EFF (but writing on his own, and not as an EFF representative).
The context is that he had written a little manual about tracing the route
by which a spam message travelled into your mailbox, and I asked him to add
some examples.  Another is from someone I don't know well.  I do not endorse
everything he says, but the message is full of useful information and seems
reasonable.  Please use your own judgement and check your facts before doing
anything serious.  And, of course, please don't do anything illegal.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Wed, 2 Oct 1996 14:16:47 -0700 (PDT)
From: Stanton McCandlish <mech@eff.org>
To: pagre@weber.ucsd.edu (Phil Agre)
Subject: Re: traceroute

These are genuine examples. I do not mean to imply that cyberpromo.com 
is a spammer and should be targeted, though others accuse them of being 
spammers on a grand scale.  I just picked them as an example more or less 
randomly.

> Date: Wed, 25 Sep 1996 20:32:40 -0700 (PDT)
> From: Stanton McCandlish <mech@eff.org>
> To: pagre@weber.ucsd.edu (Phil Agre)
> Subject: Re: spam service
> 
> Note apparent spammer's site name.
> 
> at Unix prompt (or with Mac or whatever traceroute util if not on unix):
> 
> % traceroute site.name
> 
> You get a list of all the intermediate hops to the site. Last one on list 
> is the site's net feed.

An example of the traceroute maneuver:

% traceroute www.cyberpromo.com

traceroute to cyberpromo.com (208.9.65.20), 30 hops max, 40 byte packets
 1  gw.eff.org (204.253.162.1)  3 ms  3 ms  3 ms
 2  Loopback0.GW1.SCL1.Alter.Net (137.39.2.71)  7 ms  6 ms  17 ms
 3  Fddi0-0.CR2.SCL1.Alter.Net (137.39.19.6)  8 ms  8 ms  8 ms
 4  107.Hssi4-0.BR1.NUQ1.Alter.Net (137.39.70.125)  12 ms  13 ms  10 ms
 5  sl-mae-w-F0/0.sprintlink.net (198.32.136.11)  25 ms  17 ms  20 ms
 6  sl-stk-6-H3/0-T3.sprintlink.net (144.228.10.45)  26 ms  88 ms  113 ms
 7  198.67.6.5 (198.67.6.5)  96 ms  245 ms  33 ms
 8  sl-dc-6-H1/0-T3.sprintlink.net (144.228.10.1)  111 ms  89 ms  92 ms
 9  sl-dc-15-F0/0.sprintlink.net (144.228.20.15)  89 ms *  131 ms
10  sl-cybrprom-2-S0-T1.sprintlink.net (144.228.125.66)  95 ms * *
11  cyberpromo.com (208.9.65.20)  91 ms  96 ms  85 ms

www.cyberpromo.com is obviously served by cyberpromo.com, which is the 
same folks, so the "last" hop on the list should be considered 
sprintlink.net. 
 

> Next email abuse@site.name and abuse@net.feed's.site.name, and note 
> politely that a user at site.name, which appears to be getting its feed 
> from net.feed's.site.name is spammin' the globe, sorry if you've already 
> been notified.  

It's generally important to send to the admins of the "master" host for 
a domain, since "sl-cybrprom-2-SO-T1.sprintlink.net" and the like may 
just be routers or something. You need, in this example, to talk to 
abuse@sprintlink.net. In this example, cyberpromo itself is accused of 
spamming, so no point in mailing them. If cyberpromo appeared to be an 
ISP serving a spamming user, perhaps joe@cyberpromo.com, you'd want to 
mail abuse@cyberpromo.com, too.

> If you get a bounce (not all ISPs have "abuse" aliases yet) resend the 
> message to postmaster@site.name (or postmaster@net.feed's.site.name - 
> whichever bounced.)
> 
> If you suspect the site.name is actually a one-man operation of the 
> spammer himself, do:
> 
> % whois site.name 
> 
> (or use a GUI whois application) and see if admin or tech contact is the 
> spammer (if they used real name). If in doubt call and ask what site.name 
> is (marketing biz? ISP?) At any rate, if you hit the site's net feed too, 
> no big deal.  

An example of the whois maneuver:

% whois cyberpromo.com
Cyber Promotions Inc (CYBERPROMO-DOM)
   8001 Castor Avenue, Suite 127
   Philadelphia, PA 19152
   USA

   Domain Name: CYBERPROMO.COM

   Administrative Contact, Technical Contact, Zone Contact, Billing Contact:
      Wallace, Sanford  (SW430)  cyberpr@ANSWERME.COM
      (215) 288-9230

   Record last updated on 22-Sep-96.
   Record created on 26-Apr-96.

   Domain servers in listed order:

   NS3.CYBERPROMO.COM           208.9.65.10
   NS4.CYBERPROMO.COM           208.9.65.11

The InterNIC Registration Services Host contains ONLY Internet Information
(Networks, ASN's, Domains, and POC's).
Please use the whois server at nic.ddn.mil for MILNET Information.
 
This should give you a tidbit or two on which to make a judgement call. 
If the Admin or Tech Contacts for the domain are the spammer, bingo. If 
not, you can't really tell what this site is, so you might as well mail 
abuse@cyberpromo.com too. If they are the spammers, they'll just ignore 
you in most cases. If they aren't, and are the spammer's ISP, you might 
get some action.

Disclaimer: This is just a personal message and does not represent 
official EFF statements or opinions.  EFF has no official position on 
spamming.

---

<HTML><A HREF="http://www.eff.org/~mech">     Stanton McCandlish
</A><HR><A HREF="mailto:mech@eff.org">        mech@eff.org
</A><P><A HREF="http://www.eff.org">          Electronic Frontier Foundation
</A><P><A HREF="http://www.eff.org/hot">      Program Director    </A></HTML>

Date: Mon, 30 Sep 1996 22:13:14 -0400 (EDT)
From: "George F. Nemeyer" <tigerwolf@tigerden.com>
To: antispam@shmooze.net
Subject: antispam: Urgent call to action - Protect your mailbox from junk mail

Cyber Promomotions, notorious for sending millions of unsolicited
commercial advertising e-mail (UCE) messages, has filed suit against AOL
which has been trying to respond to massive complaints from their own
members to end the floods of junk they receive.  The outcome of this court
case is likely to be a landmark in the unsolicited junk e-mail issue.  If
unsolicited junk e-mail is given any legal legitimacy, the floods will be
impossible to stem and your e-mailbox will be forever clogged.

Regardless of your attitude about AOL, they deserve your support in this
fight.  Hearings are coming up.  The first as soon as 8 October.

Send AOL a polite message voicing your opposition to UCE and ask that they
provide it to the judge.  Provide an explaination as to why you resent
having to pay for getting junk ads you didn't ask for, don't want, and
have to pay to receive.  Ask the judge to rule that unsolicited e-mail
advertising is a violation of your desire for privacy and that it
threatens to make an otherwise valuable personal communications tool
worthless if such practices continue.  YOUR VOICE CAN MAKE A DIFFERENCE!

If you have any evidence to show you've requested to be removed from Cyber
Promotions mailing lists, but have continued to receive from them, be
SURE to include that information.

Write to:

  America Online
Legal Department
Cyber Promo lawsuit
2200 AOL Way
Dulles, VA  20166
 
  Email: aollegal@aol.com

Help spread this word.  Time is short to prevent bad law from being made
which gives junk e-mail ad spammers a legal foothold.  Pass this message
to your friends.  Please *DO NOT* mass spam it to newsgroups, but do help
it propagate.

---

The message above is the *IMPORTANT PART*, but there's lots more info and
useful places you can lodge a complaint.  Act on these as well, of
course, but remember, the AOL lawsuit will be the first real legal test
of whether you have a right to an uncluttered, useful e-mail system on
the Internet.  Put your main energy there for now.

>>>>>>>>>>>>>>>>>>>>> Other Cyber Promo Info <<<<<<<<<<<<<<<<<<<<<<<<<<

Informative and complaint locations for Cyber Promotions and UCE

---

    The following sections contain websites where articles describing
    Cyber Promotions' operations, practices, and attitudes may be found.

    In addition, a section is provided that lists places you can contact
    where your voice can be heard directly by people who can make a
    difference.

    If you are sick of junk e-mail and want to end it, don't just ignore
    it, FIGHT BACK!

    This list will be revised as new information and locations are
    found.

>>>>>>>>>>>>>>>>>>>>>>>> Background Information <<<<<<<<<<<<<<<<<<<<<<<<<

New York Times - A series of articles dealing with Cyber Promo and the AOL
lawsuit.  MUST READING!  You have to fill out a form for a password, but
it's free.  There are buttons on the form to let them know if you will
accept mail from them and/or their advertisers.  CAUTION: These buttons
default to 'on', so if you DON'T want to get on mailing lists, be sure
to un-press them.

http://www.nytimes.com/library/cyber/week/0926aol.html
http://www.nytimes.com/library/cyber/week/0921junkmail.html
http://www.nytimes.com/library/cyber/week/0907aol.html
http://www.nytimes.com/library/cyber/week/0905aol.html
http://www.nytimes.com/library/cyber/week/0704promote.html

     -----------------------------------------------------------

Garbage In Garbage Out -  deals with many aspects of the spam situation.
Including an *entire section* devoted to Cyber Promo.  This section
includes quite a bit of past history, Wallace quotes, and horror stories
about just the sort of tactics Cyber/Wallace employ.  Good background
material.

                 (main page)
http://www.mindspring.com/~mdpas/gigo.html
                 ('Your Pals at Promo Enterprises' section )
http://www.mindspring.com/~mdpas/promo/pe_count.html

>>>>>>>>>>>>>>>>>>>>>>>> Places to Complain <<<<<<<<<<<<<<<<<<<<<<<<<<<<<

Better Business Bureau - Cyber Promotions touts their BBB membership.  The
BBB's mission is to promote accurate and responsible advertising, and can
be a valuable asset in the war against junk e-mail.  You can even file a
complaint on-line.  Be sure to urge them to come out strongly against the
invasive, cost-shifting, practice of unsolicited bulk e-mailing as an
advertising technique.

http://www.bbb.org/easternpa

Some actual names to write to:
Ms Stacy Scholl
Mr Aron Greberman

Better Business Bureau
Serving Eastern Pennsylvania
1930 Chestnut Street
Philadelphia PA 19103
Phone: (900) 225-5222 24 hours / 8:30-6:00 $.95/minute
Fax: (215) 561-5216

The address below if for the national council of BBBs.  The issue to
address when writing here is that the BBB should set national policy which
opposes unsolicited bulk e-mail as advertising practice.  No truly
responsible business should advertise in this manner.

Mr Allen Beatty
Sr Vice President
Council of Better Business Bureaus
4200 Wilson Blvd   Suite 800
Arlington, VA    22207

     -----------------------------------------------------------

SPRINT - Sprintlink is the latest in a series of network access providers
which have been infested by Cyber Promo.  They've been booted from at
least one area provider, and are now getting their connectivity to the net
through this major national backbone provider.  Unlike MCI, which will not
tolerate the kind of abuses that Cyber Promo engages in, Sprint's current
policies are more 'we don't care'.  This can change.  It must change.
It's not the kind of behavior a respected, national company should allow
on its facilities.  UCE is net abuse.  Period.

Generic complaint address:  abuse@sprintlink.net

InterNIC listed Administrative Contact:
      Kurt, Gastrock  (GK368)  gastrock@SPRINT.NET
      1-800-230-5108

Network Info & Support Center  -  (800) 669-8303
      noc@sprintlink.net

Executive Offices - (800) 347-8988

     -----------------------------------------------------------

An article in InfoWorld and a gripeline 800 number
http://www.infoworld.com/cgi-bin/displayArchives.pl?dt_iwe37-96_23.htm

     -----------------------------------------------------------

>>>>>>>>>>>>>>>>>>>>> Other anti-junk e-mail sites <<<<<<<<<<<<<<<<<<<<

Outlaw Junk E-mail Now - generic site with lots of info and links to yet
more sites and articles on the overall subject.

http://www.public.asu.edu/~dtopping/ojen.html

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>> End <<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<<

Help fight the scourge of unsolicited commmercial ads before it's too
late!

----- End of forwarded message from George F. Nemeyer -----
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991010032257/http://www.somewhere.com/)