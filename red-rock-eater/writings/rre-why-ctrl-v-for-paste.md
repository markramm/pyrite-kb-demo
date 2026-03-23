---
id: rre-why-ctrl-v-for-paste
title: "[RRE]Why Ctrl-v for Paste?!"
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1999/RRE.Why.Ctrl-v.for.Paste.html
importance: 6
research_status: partial
tags:
  - commerce
  - cryptography
  - education
  - environment
  - international
  - media
  - military
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1999/RRE.Why.Ctrl-v.for.Paste.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/20000226130902/http://www.somewhere.com/)

  

# [RRE]Why Ctrl-v for Paste?!

```
[This gets a little dense, but stick with it.  If you want to write to
Dan, note that his message header uses ".twx" rather than ".tw" to defeat
programs that automatically sniff newsgroup messages for spam addresses.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html
or send a message to requests@lists.gseis.ucla.edu with Subject: info rre

---

Date: 9 Jan 1999 09:16:31 GMT
From: Dan Strychalski <dski@cameonet.cameo.com.twx>
Newsgroups: alt.folklore.computers
Subject: Re: Why Ctrl-v for Paste?!

Interesting that knowledgeable folks can't figure out why some programs
use Ctrl-V for Paste. It's supposed to be "intuitive," dontcha know.

Wherever the assignment of modifier-Z/X/C/V to Undo/Cut/Copy/Paste
originally came from, it was introduced to the computing public through
the first Macs, in 1984. The Mac used Command-X/C/V for Cut/Copy/Paste
(and maybe Command-Z for Undo) from the beginning. "X out" is another
way of saying "cross out," i.e., remove; C is for Copy; and V (1) points
down and (2) makes for a neat row. Z can be thought of as "zap," which
isn't too far from "reverse the last action." Having the keys all in a
row is an old idea; witness vi.

It had nothing to do with WordStar, Word, or the ASCII assignment of
CAN(cel) to 18h. (For non-computerists, that's 18 hex, i.e., 24 decimal,
meaning Ctrl-X at the keyboard, X being the 24th letter of the alphabet.
Ctrl+letter-key combinations produce ASCII control codes, and those
codes do not print. They are command codes. This is part of the
same standard that makes this text readable on just about every computer
system in the world.)

(By the way, what system uses Ctrl-X to delete a line? I've been at this
stuff since 1982, and I've never seen it.)

One of the design goals of the Mac's creators was to make programs such
as WordStar impossible. They were not about to copy anything from
WordStar. While WordStar lets you do everything through the Ctrl key,
the Mac in its first three years had no Ctrl key; it had a single
Command key, and that key was in the worst possible place for
comfortable use with all but a few character keys. The OS and the first
model apps simply did not allow keyboard-only operation. At the time,
CP/M was still going strong; lots of new IBM-type and non-IBM-type
machines were coming out; and WordStar held near-absolute sway in the
word processing world. Steve Jobs did not want Mac users learning a
method of operation that would be transferrable to other systems.

(Yo, Ralph -- it was indeed WordStar that jumped from zero to at least
seventy-five percent of the x86 word processing market in the second
half of 1982, creaming some twenty competitors. Sorry I didn't respond
to your question about this earlier; things have been gnarly here.)

Remember that every serious general-purpose system must have a Ctrl
key (even the Mac eventually got it), and that before 1986 Ctrl was
almost universally in the home row, immediately to the left of the A
key, the position preferred by most (most, I said) people who know a
thing or two about computers and must use the keyboard a great deal.

Since Z, X, and C are all in the bottom row (in QWERTY), Ctrl-Z, Ctrl-X,
and Ctrl-C, when used without a prefix keystroke in WordStar, move the
viewframe or the cursor down (all motion control is on the left hand).
Ctrl-V, being in the relatively awkward area between a touch typist's
hands, is assigned to the little-used insert/overtype toggle (and V can
be taken to represent "oVertype"). In blocK operations (which all have
Ctrl-K as a lead-in, and which include so-called cut-and-paste
functions), there is indeed a superficial similarity to the Mac
conventions: Ctrl-Kc copies, and Ctrl-Kv moVes, a marked block to the
current cursor position. Ctrl-Kx, however, is "save and exit with no
questions asked" (I have no trouble thinking of a file as a block; your
mileage may vary), and Ctrl-Kz at the time was not used.

Microsoft Word for MS/PC DOS did not use Alt-Z/X/C/V for Undo/Cut/Copy/
Paste, and Gates had a standing rule that programs must not use any
main-block Ctrl-key combinations (MS/PC DOS utilities responded to the
few recognized by the CP/M 2.2 command interpreter -- Ctrl-C, Ctrl-H,
Ctrl-I, Ctrl-M, Ctrl-P, and Ctrl-S -- but that was it for ten years,
until DR-DOS came along with a WordStar-like editor and WordStar-style
command-line recall and editing). Check out any big-name eighties-era
word processor other than WordStar. It is incredible the hoops
developers jumped through, both at Microsoft and at companies ostensibly
competing with Microsoft, to avoid assigning command functions to Ctrl-A
through Ctrl-Z.

Like Jobs, Gates wanted his customers conditioned to using keystrokes
available only on systems he profited from. Ctrl being common to all
machines, he didn't want people using it. His job was harder than
Jobs's: he didn't have direct, absolute control over hardware and
application design. With the cash and the clout afforded by his control
of the operating system, however, he could reward or punish other
companies according to whether or not they toed the line. And that's
exactly what he did. You can't deny the possibility out of hand. First
check out the command keystrokes of big-name eighties-era word
processors. Thoroughly. Please. The keystrokes tell all.

(This had the added benefit of ensuring that people would detest using
the keyboard and be ripe for Windows. I know a whole lotta people who
love, and I mean l-o-v-e LOVE WordStar, vi, or Emacs keystrokes and can
use them for everything all day every day. When was the last time you
heard anyone rave about WordPerfect, Word for MS/PC DOS, or MultiMate
[or, for that matter, Macintosh, or Windows, or CUA] command keystrokes?
Considering how many more people have used these programs by now, isn't
that just a little bit strange?)

Ctrl-Z/X/C/V for Undo/Cut/Copy/Paste did not exist in the x86 world
until IBM moved Ctrl out of the home row and Microsoft started moving
its Mac applications to Windows. Through version 2.03, the applications
bundled with Windows used Del for Cut, Ins for Paste, and F2 for Copy.
Alt worked as it does today, and Ctrl sat there dead as a doornail.
Check out Windows, the "official guide to Microsoft's operating
environment," copyright 1986 by Nancy Andrews (Microsoft Press, ISBN
0-914845-70-5). It wasn't enough to have a (minimally) consistent
interface; just like Jobs's (minimally) consistent interface, it had to
be as inconsistent as possible with any other system folks might come
across.

By the end of the eighties, CP/M was out of contention, almost all
keyboards had Ctrl in the bottom corner, word processors that ignored
Ctrl had pretty much taken over through institutional sales, and Windows
was in shape to be passed off as usable even to halfway knowledgeable
folks. Gates felt he could safely use Ctrl, and Lord knows he needed
something to offset the inefficiency of his mouse-and-proprietary-keys
method of working. To say he stole the Z/X/C/V suite from Apple is
exactly right.

Dan Strychalski                dski at cameonet, cameo, com, tw (no x)
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/20000226130902/http://www.somewhere.com/)