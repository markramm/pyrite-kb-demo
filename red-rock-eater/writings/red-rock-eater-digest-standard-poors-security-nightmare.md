---
id: red-rock-eater-digest-standard-poors-security-nightmare
title: Red Rock Eater Digest - Standard & Poors security nightmare
type: writing
writing_type: rre-post
date: 2001-05-12
url: http://commons.somewhere.com:80/rre/2000/RRE.Standard.Poors.secur.html
importance: 6
research_status: partial
tags:
  - cognitive-science
  - cryptography
  - law
  - media
  - military
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/2000/RRE.Standard.Poors.secur.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20010513001054/http://commons.somewhere.com/rre/) | **Most Recent Article: Sat, 12 May 2001** |

```
[This is just to give another idea of the kinds of security problems
one sees on the Internet.  This stuff is not rocket science.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
You are welcome to send the message along to others but please do not use
the "redirect" option.  For information about RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html

---

Date: Wed, 17 May 2000 12:44:01 -0700
From: Stephen Friedl <friedl@MTNDEW.COM>
To: BUGTRAQ@SECURITYFOCUS.COM
Subject: Standard & Poors security nightmare

Standard & Poor's ComStock division sells a MultiCSP system that
provides realtime stock quotes and news, and this was the subject of
a BugTraq posting in February 2000 by Kevin Kadow (this link a copy
posted in March):

http://www.securityfocus.com/templates/archive.pike?list=1&date=2000-03-22&msg=20000324230903.13640.qmail@msg.net

His review was fairly scathing, but he substantially UNDERstates the
risk of running one of these machines. He told me he didn't want to
give away everything (to allow people time to clean things up), but
I intend to do so here. These machines are an unmitigated disaster
for security, and it's not often I can use "unmitigated" so literally.

For starters, on the "outside" interface they provide an /etc/issue
file that kindly tells you nearly everything you need to know. Just
telnet to the box, and it greets you with:

	Red Hat Linux release 5.1 (Manhattan)
	Kernel 2.0.35 on an i686
	
	MCSP - Standard & Poor's ComStock - The McGraw-Hill Companies
	
	Multiuser CSP Login:
	<alt><F1> login: screen
	<alt><F#> login: showusers
	<alt><F#> login: showlog
	<alt><F#> login: netconfig
	<alt><F#> login: isdnconfig
	<alt><F#> login: helpmcsp
	<alt><F#> login: helpicl
	login:

The only thing missing is "Please Hack Me -- I'm easy". The last two
"help" accounts have no passwords, and they bring up "more" on some
text files. When paused at the first prompt, it's easy to type "v" to
bring up vi on the file, then type

	:set shell=/bin/bash <RETURN>
	:shell <RETURN>

and get a non-root shell. This takes about 12 seconds. The other
"config" accounts provide similarly easy interfaces via simple menus,
though I didn't spend any time on them. They helpfully keep passwords
in the "old" format in /etc/password: no /etc/shadow, no MD5, so Crack
gave me the root password of "c0mst0ck" (zero instead of oh -- aren't
they clever). Now you are root on a Linux box with a C compiler.

The machine has LOTS of security issues: programs with known holes,
/many/ unneeded services, world-writable directories, and the list
goes on. But in one respect this shouldn't matter much: if you have a
proper firewall in place, this machine won't allow the outside world
to get anywhere near it. Or so you thought.

These machines have a dedicated circuit on the second network
interface (T1, ISDN, etc.) that supports the feed from S&P, and it
seems to be on a 172.23.*.* private network run by Concentric. By
downloading and compiling a few tools (the compiler was thoughtfully
left behind), I was able to "scan" various 172.23.x.x address blocks
to discover numerous MultiCSP machines owned by entirely unrelated
customers. Since these machines are all configured to run Samba by
default, their "signature" is very easy to detect with a NETBIOS
nameservice scanner.

Once the machines were identified, it was a trivial matter to login
to these remote machines and get root via the same default password
or "vi" exploit. These machines were apparently located all over the
world (I think that two of them were in The Netherlands and Singapore),
and every single one had a "private" 10.x.x.x or 192.168.x.x address
on the "customer" side of the machine. I found dozens of them before I
decided that I'd seen enough.

This means that no matter how good your firewall and security is
on the "outside" of the network, I am able to show up as root on
a Linux box with compiler tools. On the inside of your network.
I had these visions of wandering around the underground sewer tunnels
in Washington DC and popping up in the middle of the State Department:
maybe that's where the laptops went.

The short answer is that if you have one of these machines unmodified,
you are only as secure as the least secure OTHER customer with these
machines. It doesn't get much more scary than this.

Recommendations

---

These are presented roughly in order of how easy they are to
implement.  Keep in mind that I know virtually nothing about
the actual MCSP application, so you have to adjust per your own
experience.

1) Scream *bloody murder* at your S&P representative. They have
   more or less completely ignored reports of this serious matter
   as far as I can tell.  The previous reporter of this (Kevin Kadow)
   tried every way he knows how to get them interested, and nothing
   happened, and even an indirect communiation to S&P's CTO got
   no response. Talk to your legal counsel if you are so inclined.
   S&P is just grossly negligent on this front.

2) Remove the /etc/issue file that reveals just how much stuff is
   here.  Though there are way too many services running on this
   machine, and it would probably take no time to break into via other
   means, the big /etc/issue file provided is just an open invitation
   to abuse by even a casual passer-by. It surely caught my attention.

3) Put good passwords on ALL the accounts, including the "helpful"
   ones.  If you really don't need the help accounts, disable them
   entirely.  These help files are very easy to find without special
   logins. I believe that S&P might login to these machines remotely,
   so you may need to coordinate this with them.

4) Find out from S&P just which services that they really need and
   drop the ones not needed. They are running Samba, portmapper,
   and SNMP, and it's not clear that any are really needed. Apache
   is running, and I am fairly sure it's /not/ needed. Shut down
   EVERYTHING you don't need.  I'm told that telnet is the only thing
   really needed.

5) Use TCP wrappers to limit who can login to your system from random
   IP addresses, and certainly disable all logins from the Concentric
   side of the world. If possible, disable the telnet daemon entirely
   and just do all your administration from the console. Use Secure
   Shell instead of telnet.

6) Install and use ipchains on both interfaces to drastically reduce
   what this machine can do. The Concentric side of the world seems to
   talk to just two machines that are mentioned in /etc/hosts:

	#Name of machine on far side (e.g big1 and big2)
	172.23.94.10 BIG1
	172.23.95.10 BIG2

   If you determine that this is the limit of your "outside" traffic,
   firewall everything else. I have the impression that S&P's BIG1 and
   BIG2 accept connections on port 25600, so you might be able to get
   away with denying all UDP and permit only established TCP traffic.

   You must also firewall the "outside" interface as well on the
   assumption that the machine is compromised from the "inside".
   Also use ipchains to limit virtually everything on this interface,
   allowing only that which you know to be required. I have the
   impression that the customer hits the quote/news server on TCP
   port 6010, so blocking everything else seems like a good idea.
   Also block outbound traffic from this machine so a compromised
   machine can't be used as a launchpad. I'm afraid I don't have
   enough experience with ipchains to get any more specific on these
   recommendations.

I am sure that these suggestions are incomplete, as I've not be the
one responsible for securing this machine (I was simply doing an
audit).  Standard & Poors is simply out of their minds for producing
a product like this and not responding when the issue was raised.

As Kevin said previously, "pray".

---

Stephen J Friedl|Software Consultant|Tustin, CA|  +1 714 544-6561
3B2-kind-of-guy |I speak for me only|  KA8CMY  |steve@unixwiz.net
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20010513001054/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20010513001054/mailto:webmaster@somewhere.com). |