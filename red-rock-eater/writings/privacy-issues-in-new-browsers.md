---
id: privacy-issues-in-new-browsers
title: privacy issues in new browsers
type: writing
writing_type: rre-post
date: 1994-11-06
url: http://commons.somewhere.com:80/rre/1994/privacy.issues.in.new.br.html
coauthors: []
key_concepts:
  - privacy
  - surveillance
importance: 4
research_status: partial
tags:
  - auto-imported
  - internet-culture
  - privacy
  - rre
  - rre-post
  - surveillance
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1994/privacy.issues.in.new.br.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991013011953/http://www.somewhere.com/)

  

# privacy issues in new browsers

```
This is a somewhat out-of-context message about privacy issues involved in 
new network browsing programs such as Netscape.  The issue is whether (and
when) those programs record information about who is using them (and how).

Date:    Sun, 6 Nov 1994 23:33:55 -0800
From:    march@europa.com (Marc H.)
Subject: Re: HTTP, New Browsers, & Privacy

Ed Kubaitis <ejk@uiuc.edu> wrote, in V03 #21, about HTTP_FROM, an
environment variable passed by some web browsers to HTTP servers.  The
variable contains the user's email address as entered in their
"Preferences," and Ed expressed concern over possible logging of email
addresses by marketers or other web sites.  I'm glad to see this issue
raised again; I brought it up some months ago when AT&T opened their
"youwill.com" contest, for which they asked users to submit a web
form-based survey.  (Adam Curry, who was apparantly involved in the project
and who was surprised to hear address-gathering from forms was even
possible, assured several posters that no logging was taking place at
AT&T's site.)

First off, a list of the browsers supporting this variable (with version
numbers known to be inclusive; earlier versions may also belong here, and
later versions almost certainly do):
        MacMosaic 2.0.0a6
        Lynx/2.3 BETA
        Emacs-W3/2.1.54
        OmniWeb 0.7.4.1
        AIR_Mosaic(16bit)(demo)/v3.06.05.03
        MidasWWW/2.1
        Mozilla 0.9b (Netscape) [all platforms]
I collected this information during September of this year (with the
exception of Netscape); this list will hopefully prevent some duplication
of work, but it is not intended as a blacklist.  NCSA Mosaic for X and
Windows, MacWeb, Global Wide Help & Information System (GWHIS), Chimera,
and Spry's Enhanced Mosaic all do not send HTTP_FROM.

As a CGI (Common Gateway Interface -- a protocol for running scripts on web
servers) programmer, I am very much in favor of browsers supporting
HTTP_FROM.  Good use of the variable can allow automation of repetitive
tasks, which is the whole point.  I've used it several times to offer a
default return-address for mailing scripts, which both alerts the user to
the capability, and allows him or her to alter the address if they choose.
I see HTTP_FROM as similar to ftpd's familiar "Guest login ok, send your
complete e-mail address as password" prompt: any program or server that
asks users for their email addresses is completely open to receiving a
false address, or none at all, from those users.

On the other hand, Ed's reaction -- and Adam Curry's, and that of other
people to whom I've mentioned HTTP_FROM -- indicates that plenty of web
users don't know this capability exists.  I found out myself only by
running a script similar to Ed's (http://www.uiuc.edu/cgi-bin/printenv) to
list all environment varibles sent -- after having been assured by several
people that the web was completely anonymous, what I was seeking didn't
exist, etc.  To use my example above, ftpd is quite explicit about its
logging, but more recent ftp clients (such as ncftp) -- and the browsers
listed above -- are not.  I see this as the real problem.

Explicit warnings and documentation seem to be the best solutons. I'm not
sure what Lauren meant when he noted, "future versions of the Netscape
browser will probably be distributed with the name/address feature
defaulting to off."  It seems to me that this is already the case -- the
user has to enter his or her email address for the variable to work.  What
I would like to see is a much more explicit preferences dialog, one that
warns the user about possible logging by web sites.  I would disagree with
any assertion that particular browsers should be avoided because of
HTTP_FROM.  At worst, particular preferences dialogs should be avoided.  At
best, all browsers could provide a menu option -- similar to "Auto-load
images" -- that would allow the user to turn "Privacy" on or off.

This is not a web-specific issue.  Interested readers are referred to RFC
1413, "Identification Protocol,"
<URL:http://www.cis.ohio-state.edu/htbin/rfc/rfc1413.html>, which details a
more-reliable, transparent, and generalized implementation of TCP
connection logging.  I think it only prudent to assume that any site you
visit on the net could keep a log of your visit; and that as time passes,
more and more sites -- particularly commercial sites -- will do just that.
Browse carefully; the junk mail "you will" receive may be at stake.

I support Lauren's call for regulation of the use of such information.

M. Hedlund <march@europa.com>
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991013011953/http://www.somewhere.com/)