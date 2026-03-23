---
id: netscape-syntax-checking-and-market-position
title: Netscape syntax checking and market position
type: writing
writing_type: rre-post
date: 1996-03-11
url: http://commons.somewhere.com:80/rre/1996/Netscape.syntax.checking.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - commerce
  - forwarded-content
  - technology-policy
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1996/Netscape.syntax.checking.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991023093329/http://www.somewhere.com/)

  

# Netscape syntax checking and market position

```
[Concern is growing around the Internet about various policies of Netscape
that tend to reinforce its market position through violation of standards
and other nonstandard features.  The enclosed messages from Risks detail
the latest chapter in this instructive story.  The bottom line is that
Netscape is the market leader in an industry whose products are highly
standardized.  This is a recipe for disaster unless it can find some way
to differentiate its offerings.  It has two basic options: emphasizing
service and trying to break the standards.  It is clearly pursuing the
first of these options, but many people feel that it is pursuing the
second as well.  If so then it gets away with this in large part because
everybody is focused on preventing Microsoft from attaining a dominant
position on the Internet.  But it's worth keeping in mind that Netscape's
putative strategy here is precisely analogous to the strategy by which
Microsoft obtained its dominant position in PC software: an architecture
of proprietary standards (its own operating system) that help organize
a critical mass of mutually enabling customers (in economic terms, a
network) on top of a platform whose open standards are maintained by
others (the IBM PC spec).  It seems likely that the market will now
slow down momentarily for some rethinking in the light of the discovery
of serious security problems in Netscape 2.0, largely associated with
basic architectural decisions in Java.  That rethinking should include a
recommitment to functioning standards.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Subject: RISKS DIGEST 17.88

RISKS-LIST: Risks-Forum Digest  Monday 11 March 1996  Volume 17 : Issue 88

---

Date: Sat, 9 Mar 1996 07:51:22 -0800 (PST)
From: hbaker@netcom.com (Henry G. Baker)
Subject: Netscape's too-lenient syntax checking

> From:	[webmaster @ affected site]
> RE:	Re: [site name deleted] Web Link

> From [frustrated web site visitor]
> > The main link to [site name deleted] doesn't
> > work through 'lynx' because the html is not
> > correct.  The '<a href...' for the [...]
> > link is never terminated with '</a>', so that
> > the [site name deleted] link won't work.
> > Could you please look at this problem, and
> > send me a message when it is fixed.
> > Thanks very much.
> 
> Thanks for the input. The mistake was never noticed before because the 
> Netscape browsers are smart enough to detect the error and deal with it.
> Lynx, however, is not. The problem is fixed, although I don't recommend 
> looking at the site with anything but Netscape 1.1N and higher. We 
> incorporate too many of Netscape's features to make viewing these pages 
> without it useful.

I have nothing against Netscape trying to be smart, but the very
sloppiness that makes it behave reasonably for unreasonable input
leads web page designers to believe that their web pages have been
debugged if they work correctly on Netscape.  Perhaps Netscape should
have a `careful' mode for helping web page maintainers to provide
`squeaky clean' pages.

I have found numerous web page problems with Lynx in this way, and
when informed of these problems, some web page maintainers have been
downright snotty in their responses.  Their attitude seems to be `it
serves you right for not using a graphical browser like Netscape'.

Perhaps the web site designers should wake up to the fact that most of
the sophisticated web surfers that I know either use an ascii browser
like Lynx, or turn off image loading when surfing, because they actually
want to visit more than one web site per day.  All those pretty 4-color
buttons (??) that they use look good for one visit, and thereafter
become the source of a lot of irritation due to slow page loading.

Henry Baker  www/ftp directory: ftp.netcom.com:/pub/hb/hbaker/home.html

---

End of RISKS-FORUM Digest 17.88 

---

Date: Tue, 12 Mar 96 19:46:10 PST
From: RISKS List Owner <risko@csl.sri.com>
Subject: RISKS DIGEST 17.89

RISKS-LIST: Risks-Forum Digest  Tuesday 12 March 1996  Volume 17 : Issue 89

---

Date: Tue, 12 Mar 1996 06:26:30 GMT
From: Jonathan Kamens <jik@annex-1-slip-jik.cam.ov.com>
Subject: Re: Netscape's too-lenient syntax checking (Baker, RISKS-17.88)

 >  I have nothing against Netscape trying to be smart,

What Netscape does isn't merely "smart"; it's also a violation of the HTML
specification.

That specification defines what is or is not legal in an HTML document.
Programs which purport to be HTML viewers are supposed to confirm that the
document being viewed conforms to the HTML specification (e.g., not missing
"</A>" markers after "<A>" markers) and complain if it doesn't.

Unfortunately, Netscape decided, "Why should we write something which checks
the HTML for validity, which we can just write a smart interpreter which
figures out what the author of a document wanted to do, even if they
didn't actually say that?"

Henry Baker has already pointed out one problem with this -- it allows
webmasters who use Netscape to test their HTML to be lazy about ensuring its
correctness.  Since Netscape is the most popular browser, and therefore more
webmasters use it than any other browser to check HTML, users who don't use
Netscape are often "shut out" of sites.

Worse, Netscape has intentionally implemented numerous features that are not
conformant with the HTML specification, that their browser supports but
others do not.  Instead of working through the process recognized by the
HTML-design community for adding functionality to HTML, they just added the
functionality they thought was needed.  Since many sites take advantage of
this additional functionality (it is pretty neat, after all), once again,
users who do not use Netscape are "shut out".

Rectifying the latter problem isn't simply a matter of adding Netscape's
functionality to the HTML specification, because they've added functionality
which is difficult, if not impossible, to implement in SGML (the Standard
Generalized Markup Language, which is the meta-language in which HTML is
defined).  That doesn't matter to Netscape, since (as I mentioned above)
their browser interprets the HTML in a do-what-I-mean fashion, rather than
in a "Is this valid HTML?" fashion, but it matters to the rest of the Web
community, since browsers which are trying to remain true to what HTML is
supposed to be simply may not be able to implement the features which more
and more sites are using.

{Begin politics.}

I find what Netscape has done totally reprehensible.  There was a recognized
body of people defining the HTML standard, a recognized procedure for
implementing changes to that standard, and a recognized "proper" way to
parse and display HTML code.  Netscape threw that all away, and I believe
that they were fully conscious when they did so that they were breaking the
standard and causing lots of grief for the other HTML developers in the
world.  What they're doing is nothing more than an attempt to make Netscape,
a commercial product, the only browser that can be used to access the full
potential of the Web, which is supposed to be free.  The sad thing is that
they may very well end up succeeding.

{End politics.}

(Thanks to Andrew Greene for teaching me most of this and proofreading
this message.)

---

Date: Tue, 12 Mar 96 09:13:27 -0500
From: padgett@tccslr.dnet.mmc.com (A. Padgett Peterson)
Subject: Re: Netscape too lenient syntax checking? (Baker, RISKS-17.88)

> ...  The problem is fixed, although I don't recommend 
> looking at the site with anything but Netscape 1.1N and higher. 

That won't always work either. After putting 2.0 on a machine I noticed
large chunks of text on one site disappearing. Seens That with Netscape 1.x
if it encountered a syntactical mistake such as <A HREF="foo.gif> instead of
<A HREF="foo.gif"> it would realize that a double quote was missing on the
end and, having reached the end of the anchor, "assume" one.

Not 2.0. If the double quote is missing, things go wonky. So the real risk
is to assume that "smarts" will propagate along with versions instead of
correcting errors.

Padgett

---

Date: Tue, 12 Mar 96 20:28:38 EST
From: tilt+@UX3.SP.CS.CMU.EDU (Eric Tilton)
Subject: Re: Netscape's too lenient error checking (Baker, RISKS-17.88)

> ... Perhaps Netscape should have a `careful' mode for helping web page
> maintainers to provide `squeaky clean' pages.

It is for this very reason that I put together "Composing Good HTML," a few
years ago (http://www.cs.cmu.edu/~tilt/cgh/). Netscape pays at least token
attention to the problem, since they do have a reference to CGH in their own
documentation. Also, several HTML syntax checkers exist. The real RISK seems
to be that there is a popularly perceived "standard" -- HTML -- which is in
reality incredibly balkanized, with each browser choosing to interpret
different subsets and supersets of it in slightly (or not so slightly)
different ways. And that people's perceptions of that standard are largely
influenced by a WYSIWYG mentality that HTML only somewhat incidentally
supports.

---

Date: Tue, 12 Mar 96 20:37:26 -0500
From: Torrey McMahon <tm8025a@mailhost.soc.american.edu>
Subject: Re: Netscape's too-lenient syntax checking (Baker, RISKS-17.88)

I recently was involved in a lengthy discussion in
comp.infosystems.authoring.html about this very subject. Someone posted to
an other mailing list I subscribe to that Netscape allows such sloppy
behavior, in this case it was allowing a <b> to be closed by a </i>. The
argument given to me in the USENET group was "Netscape is a HTML browser,
not a validator. You can't fault it for correcting an author's bad HTML!" Of
course most people don't use a validator they just fire up Netscape, load
the page, and if it "works" they put it on their server. The compromise we
seemed to settle on was the browsers should correct HTML to some extent but
should also state that fact in a dialog box similar to the Arena browser.

I was also taken back by their "Netscape bigotry". My favorite message was
one person stating that since I don't use Netscape I shouldn't be
complaining because I'm not using the Internet standard browser!!! (I'm
using Omniweb 2.0 on a NeXT machine in case you're wondering.

The risks? Taking one person's, or company's, HTML parser as the correct
one.  Netscape bigotry in use of tags, poor HTML, and attitude is an obvious
other.

Torrey McMahon  American University School of Communication

---

End of RISKS-FORUM Digest 17.89 

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991023093329/http://www.somewhere.com/)