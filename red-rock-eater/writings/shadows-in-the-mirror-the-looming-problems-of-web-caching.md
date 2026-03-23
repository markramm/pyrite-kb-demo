---
id: shadows-in-the-mirror-the-looming-problems-of-web-caching
title: "Shadows in the Mirror: The Looming Problems of Web Caching"
type: writing
writing_type: rre-post
date: 1997-10-05
url: "http://commons.somewhere.com:80/rre/1997/Shadows.in.the.Mirror.Th.html"
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

Automatically imported from: http://commons.somewhere.com:80/rre/1997/Shadows.in.the.Mirror.Th.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991005220810/http://www.somewhere.com/)

  

# Shadows in the Mirror: The Looming Problems of Web Caching

```
[Lauren Weinstein's periodic reports in his Privacy Forum on emerging
technological privacy issues are very good.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Sun, 5 Oct 97 19:40 PDT
From: privacy@vortex.com (PRIVACY Forum)
Subject: PRIVACY Forum Digest V06 #14

PRIVACY Forum Digest      Sunday, 5 October 1997      Volume 06 : Issue 14

---

Date:    Sun, 5 Oct 97 10:58 PDT
From:    lauren@vortex.com (Lauren Weinstein; PRIVACY Forum Moderator)
Subject: Shadows in the Mirror: The Looming Problems of Web Caching

Greetings.  As the World Wide Web has continued its explosive growth,
it seems as if new potential areas of concern pop up almost every day.
Often these worries revolve around the use of technologies for
purposes, or in ways, for which they were not originally intended.

Such seems to be the emerging situation regarding "caching" of web pages.
Considered a mundane technical issue by most net users who have even heard
of it, caching carries an array of promises and problems, with some of the
latter impacting areas ranging from reliability to hacking, from freedom
of information to censorship, from security to privacy.

Caching refers to the growing practice of some Information Service Providers
(ISPs) of maintaining local copies of web pages for their subscribers, and
using technical means to encourage (or require) that their users access
those pages only from the local "cache", and not from the actual remote
sites from which the web pages originated.

The ostensible reasons for caching are valid and important ones.  In some
environments, security/firewall requirements have dictated a level of
control where "proxy servers", using local caching, have been deemed the
most practical procedure for allowing user access to the Web.  Caching also
can impart significant bandwidth savings, to the extent that users (for
example, in a cable TV, cable modem environment) can be forced to retrieve
"popular" pages from the local ISP's server, rather than having all accesses
going out over limited bandwidth facilities to the Internet proper.
This reduces load on both the outside network and on the remote web servers
themselves.

But as usual with our technological marvels, there are a number of serious
potential problems surrounding caching, about which we should all be
concerned.  Some of these problems are technical, some are the result of the
vacuum of laws relating to these areas, and some are even more directly
political and could impact basic expectations relating to freedom of speech
and privacy.

Research regarding these impacts is pretty much in the early stages, and so
are studies and surveys of these issues relating to caching.  I'm not going
to present a detailed analysis in this message, but let's very briefly
explore a list of items to be thinking about:

-- How recent are the pages in local caches?  How often do caches
   refresh their data from the original sources?  Where caching
   interval requests are present on the original pages, what guarantee
   is there that caches will honor those requests?

-- What happens to pages that are frequently updated or that display
   "dynamically created" content (that is, content that varies with each
   access)?  Will cache users be presented with old, static versions of
   these pages?  Will some caches attempt to "penalize" such pages with less
   frequent caching (this is apparently already a significant issue). 

-- To what degree do centralized caches of web pages present a centralized
   target for hacking?  What recourse do sites have against caches who leave
   copies of the original sites' pages vulnerable to outside alteration, or
   caches that even subtly or overtly alter, modify, or add to the content
   of the original pages without the original sites' permission?  How will
   typical users know if they're looking at the original, "accurate" pages
   or a modified, corrupt, or stale copy?  Cryptographic signing techniques
   seem likely to be of only limited assistance for a variety of reasons.

-- To what extent do centralized caches simplify surveillance of user web
   browsing activity, censorship, and other controls over what users may
   access?  Efforts to create a worldwide hierarchy of caches (the so-called
   "global mesh") may potentially introduce a range of risks, especially in
   those countries where government authorities already exercise a large
   degree of control over access to the net by their citizens.  Caches,
   without appropriate safeguards, could greatly exacerbate these problems.  

-- What about the copyright rights of the original sites whose pages are
   being cached?  Can sites effectively choose not to be cached?  If so,
   will they suffer "access limitation" retaliation by some caches, making
   it difficult or impossible for users behind those caches to access those
   pages?

-- Will Web search engines begin returning references to cached versions of
   web pages rather than the "real" pages under the originating sites'
   control?  To what extent could this further confuse the question of where
   the pages are really coming from or how accurate they are?

-- What happens to the web access statistics collected by centralized
   caches?  Caches prevent the originating sites from accurately judging the
   viewerships of their pages, since cached hits are never known to the
   originating site.  In fact, the more popular the site, the more likely it
   may be to be heavily cached, and for their statistics to be even more
   dramatically skewed downward due to cached "diversion" of their hits and
   other page view statistics.  Many sites depend on these statistics to
   help them in determining their page update schedules and allocation of
   page design resources.  Advertising decisions and rates are often made
   based on the assumption of the accurate local availability of these
   statistics.
 
   Of even greater concern may be the possible misuse of cached statistical
   data.  The information privacy policies of the originating web sites mean
   nothing if the hit data collected by a cache regarding cached pages is
   under the control solely of that caching entity.  This can include
   sensitive information about sites and users viewing those pages and
   selecting particular links.  Is the caching organization free to do
   whatever they like with that information?  Sell it for marketing lists?
   Provide it for investigative purposes as they see fit?  Sell it to
   commercial databases?  A given originating site may have very strict
   policies regarding any information collected regarding sites or
   users who visit their web server.  But a cache may have a completely 
   different policy, or no policy at all.  The privacy implications
   are vast.

		       	    -------

I think that's enough to provide the flavor of the issues involved.
Yes friends, another can of worms, indeed.  Without a doubt caching
technologies are a powerful tool that will be crucial to the
continued growth and development of the Internet and the World Wide Web.
Properly designed, they can bring significant benefits that clearly
need to be explored.  But their potential downside appears very real
as well, and could impact fundamental issues of privacy, freedom
of speech, and other cherished beliefs that many people consider
to be their rights.  Before caching becomes entrenched in the
Internet infrastructure, it would do us well to consider these
impacts, and what we want to do about them--technically, legislatively,
and politically.  The window of opportunity to do this is now.

--Lauren--
Moderator, PRIVACY Forum 
http://www.vortex.com

---

The Internet PRIVACY Forum is a moderated digest for the discussion and
analysis of issues relating to the general topic of privacy (both personal
and collective) in the "information age" of the 1990's and beyond.  The
moderator will choose submissions for inclusion based on their relevance and
content.  Submissions will not be routinely acknowledged.

All submissions should be addressed to "privacy@vortex.com" and must have
RELEVANT "Subject:" lines; submissions without appropriate and relevant
"Subject:" lines may be ignored.  Excessive "signatures" on submissions are
subject to editing.  Subscriptions are by an automatic list handling system;
for subscription information, please send a message consisting of the word
"help" (quotes not included) in the BODY of a message to:
"privacy-request@vortex.com".  Mailing list problems should be reported to
"list-maint@vortex.com". 

All messages included in this digest represent the views of their
individual authors and all messages submitted must be appropriate to be
distributable without limitations. 

The PRIVACY Forum archive, including all issues of the digest and all
related materials, is available via anonymous FTP from site "ftp.vortex.com",
in the "/privacy" directory.  Use the FTP login "ftp" or "anonymous", and
enter your e-mail address as the password.  The typical "README" and "INDEX"
files are available to guide you through the files available for FTP
access.  PRIVACY Forum materials may also be obtained automatically via
e-mail through the list handling system.  Please follow the instructions above
for getting the "help" information, which includes details regarding the 
"index" and "get" commands, which are used to access the PRIVACY Forum 
archive via the list handling system.

All PRIVACY Forum materials are available through the Internet Gopher system
via a gopher server on site "gopher.vortex.com".  Access to PRIVACY Forum
materials is also available through the Internet World Wide Web (WWW) via
the Vortex Technology WWW server at the URL:  "http://www.vortex.com"; full
keyword searching of all PRIVACY Forum files is available via WWW access.

---

End of PRIVACY Forum Digest 06.14

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991005220810/http://www.somewhere.com/)
