---
id: red-rock-eater-digest-design-for-a-web-filtering-service
title: Red Rock Eater Digest - Design for a Web Filtering Service
type: writing
writing_type: rre-post
date: 2001-11-04
url: http://commons.somewhere.com:80/rre/2001/RRE.Design.for.a.Web.Fil.html
importance: 6
research_status: partial
tags:
  - activism
  - cryptography
  - democracy
  - media
  - military
  - privacy
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/2001/RRE.Design.for.a.Web.Fil.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20011105023846/http://commons.somewhere.com/rre/) | **Most Recent Article: Sun, 4 Nov 2001** |

```
  Design for a Web Filtering Service

  Phil Agre
  http://dlis.gseis.ucla.edu/pagre/

  Version of 4 November 2001.
  2600 words.

For a few years now I've been using this mailing list to filter the
Web.  I ask people to send me URL's on certain topics.  Then I look
at the pages, keep the good ones, and assemble packages of URL's with
titles and short commentaries.  The results are sent to the mailing
list, kept in a Web-based archive of the list, and included in a
single big Web page of all the URL's I've sent out -- the latter
mostly to help me avoid duplicates.  I have sent out many thousands
of URL's under this system: about 1500 on the recent US elections,
about 4000 about the current war, and perhaps 6000 on other topics.
Complete lists of the URL's can be found through the RRE home page:

  http://dlis.gseis.ucla.edu/people/pagre/rre.html

These 10,000+ URL's have been submitted by hundreds of people, and
the great strength of Web filtering is that it draws on the diversity
of the participants.  I would never have heard of most of those URL's
on my own.

Community Web filtering seems like a good idea, and it's time to
explore automated tools to support it.  In this article I will suggest
a design for a Web-based filtering tool.  I cannot participate in
building such a tool, but I would be happy to try out any prototypes
that others might construct.  I have established a discussion list for
people who might be interested in working on a tool:

  http://groups.yahoo.com/group/webfilter

This list is open and unmoderated.  If something more sophisticated
is needed, I am hoping that people who join the list can self-organize.
I believe that such a tool would be an excellent public service, not
just for this list but for many others as well, and I hope that some
public-spirited subscribers will be interested in taking initiative
to build it.  I would be happy to publicize their contributions, or
else help them preserve their anonymity, whichever they would prefer.

Here, then, is my proposed design.  I am sure that people who design
Web-based services for a living can do better, but I also hope that
any designers will listen to my rationales, which are based on years
of experience running a community Web filtering service by hand.

The "webfilter", as I'll call it, is a cross between a discussion
list, a weblog, and a bookmark file.  It is not just a weblog, since
it includes numerous functionalities to deal with long lists of URL's.
Nor is it just a discussion list, since the goal is to produce a
reasonably clean and orderly presentation of the URL's.  Nor is it
just a bookmark file, because of its community nature.

The webfilter lives on the Web.  The key idea is to require people who
submit URL's to impose a minimal degree of order on their submissions.
Right now, I get free-form text messages from submitters, and I have
to fish through these messages by hand to recover a useable URL.  Even
though most submitters are well-intentioned, it takes a lot of work
to process these text messages.  The messages are so diverse that it
would be impossible to write an automated tool to parse them.  That's
why we need a more structured tool on the Web.  The tool should be
friendly, simple, and efficient, but I don't think that will be hard.

The webfilter code should be open-source -- I'm not interested in a
proprietary system.  Each site that runs the webfilter code will be
called a "webfilter" (by analogy with "weblog").  Each webfilter will
provide one or more "services".  For example, on my own list I have
effectively been providing three services: the election, the war,
and miscellaneous (mostly politics and social aspects of technology).
Lots of people would like me to separate the political service from
the non-political services, and the webfilter could support many
such divisions.

Services come in two types: edited and unedited (by analogy with
moderated and unmoderated mailing lists).  Each service has an owner,
and some services have editors.  The owner and editor need not be the
same person.  Each will have a password.

Each webfilter service on a given site has five modes: Submit, Edit,
Revise, Configure, and View.  I'll explain mode each in turn, stopping
to explain the reasons for each design choice.

(1) Submit mode

The owner creates the service using the Configure mode and then
advertises a Web page where people can submit URL's to it.  No login
is required.  The Submit page is very simple.  It has three boxes, a
menu, and a button:

* * URL - The box should be large enough to handle the cumbersome,
  multiline URL's generated by some online publications, such as
  the Globe and Mail.  Required.* * Title - We should encourage people to extract the real title of
    the material on the page and insert it in this box.  The title
    of the Web page itself may not be useful.  Optional.* * Commentary - Space for several lines of commentary.  I typically
      provide one line of commentary at most, but many people prefer
      to include several lines, and many readers prefer more clues about
      whether they should click on a link.  Optional.* * Category - Large lists of URL's are overwhelming unless they are
        broken down into categories.  Imposing the categories takes work,
        and we should shift most of this work onto the submitting users.
        The list owner should establish the categories, and should have
        an interface for editing them.  The categories should then appear
        to submitters as a (potentially two-level) pop-up menu.  This
        is optional, simply because the default category will be "other".
        Still, submitters should be politely encouraged to provide a more
        specific category.* * A button called "submit".

The "submit" button should rapidly bring up a confirmation page.
The confirmation page will include the submitted page (i.e., the page
whose URL has been entered) in a frame, and above the frame the URL,
title, and commentary should be neatly presented.  If the same URL has
already been published in the same service, then an appropriate notice
should apepar, together with a link to the archive entry for that
issue.  (Users should not be prevented from resubmitting URL's that
have already been published on the service, but the editor should
have a configuration option to automatically throw such submissions in
the trash.)  The confirmation page should have two buttons: "confirm"
and "edit".  The "confirm" button sends the page to the input queue,
says "thank you", and gives the user a blank Submit page.  The "edit"
button returns to the Submit page with the user's URL, title, and
comment.

We need a confirmation page because people often accidentally submit
URL's that don't work.  The counterargument is that the confirmation
protocol imposes overhead on the majority of users that outweighs the
hassle of badly formed submissions.

When a page is sent to the input queue for a service, the webfilter
should check for duplications.  If several people have submitted the
same URL with different commentaries then the webfilter needs to do
something reasonable, which I'll discuss under Edit mode.

(2) Edit mode

Webfilter services, as I say, can be either edited or unedited.
Once it has been set up, an unedited service is entirely automated.
An edited service has an editor, who is a user with a login name
and a password.  (In principle it could have several editors, but
I will keep it simple.)  Each service has a separate URL for the
editor; this URL is presumably not advertised, though no harm would
result if it was.  (This is better than having a single login page
for everyone, which makes the editor enter the name of the service
every time and clutters the interface for non-editors.  Both types
of users need to be able to bookmark the page for their respective
mode for a given service.)

Having logged in, the editor is offered a link to Configure mode,
explained in a moment.  But in most cases the goal is editing, and it
is crucial for the Edit interface to be efficient.  The editor's job
is to rake through the URL's that have been submitted by subscribers
to the service.  The editor should presumably be shown a list of
these URL's, perhaps just the titles with hyperlinks, together with
statistics about how many URL's are in the queue, when the last batch
of URL's was released, the total number of URL's published to date,
and so on.  (The latter item is purely for the editor's curiosity.)

The editor's goal is to assemble an "issue" of the webfilter service.
Each issue consists of a title (i.e., the Subject: line of an email),
a prefatory text, lists of URL's under successive categories with
titles and commentaries, and perhaps a concluding text.  The editor
can work on an issue incrementally, and need not publish it until it
is ready.  So the service will always have a partially assembled issue
stored in its database.  The editor can only work on a single issue
of a given service at a time.  If the editor wants to fork off several
issues, that probably means it's time to break the service into
several services with distinct identities.

The crucial part comes when the editor settles down to filtering the
submitted pages.  Having clicked a button in the Edit mode called
"filter", the editor should be presented with a series of framed
pages.  One frame (at the bottom) will have the submitted page,
and the other (at the top) will have the URL, title, and commentary
(all in their own boxes) and the categorization (with the same pop-up
menu that the submitters see).  Four buttons are also provided on
the top frame: "accept" (include this page in the issue), "reject"
(throw this page in the trash), "postpone" (hold this page back for
potential inclusion later on, either in this issue or the next), or
"stop" (make no decision on this page, and instead return to the main
Edit mode page).

The general idea is that the editor can change any of the entries
that the submitting user has made.  The editor can change the URL
(for example, removing the junk after the "?"), the title (for example,
substituting a paraphrase or a descriptive rant for a title that
may not be self-explanatory), the commentary (for example, deleting
the commentary altogether or editing it down to something simpler),
and the categorization (for example, supplying a category when the
submitting user has kept the default).  A particular problem arises,
as I mentioned, when several users have submitted the same URL with
different commentaries (or different titles, for that matter).  I
don't know what the right answer is here.  Perhaps the editor should
simply get all of the commentaries (or titles) in the single box, and
should delete or edit the whole lot of them at will.

Once the editor hits an "accept", "reject", or "postpone" button, it
is crucial that a new framed page appear as quickly as possible.  It
should be possible for an editor to crank through dozens of submitted
pages every day, making rapid decisions on each one.  Once the queue
has been exhausted or the editor has hit the "stop" button, the Edit
mode page should come back.  In addition to the features that I've
mentioned, that page should also have tools for publishing an issue
consisting of the URL's that have already been accepted.  I would
suggest that the editor be able to supply (in the Configure mode) a
"boilerplate" text that goes at the top of each issue, and then before
publishing should have a chance to edit that boilerplate text, for
example by adding extra comments.  (Perhaps the interface for editing
the boilerplace text should go in the Revise mode.)

The Edit mode page should have, inter alia, a "revise" button and
a "publish" button.  I'll explain the Revise mode in a moment.

When an issue is published, several things should happen.  An email
version of the issue should be sent to everyone who has subscribed
to the service, the URL's in the issue should be included in one giant
historical file for the service (for quick reference as to what has
already been published), and the URL's should also be entered into a
database, indexed by the category that they have been published under.
This database is what the View mode looks at.  Finally, the editor
should be returned to the Edit page, which should clearly reflect
the successful publishing of the new issue, along with whatever URL's
still remain in the queue.

(3) Revise

When "revise" is pressed in Edit mode, the editor is taken to a page
that resembles in spirit a Web browser's bookmark editor.  This is
probably the most difficult mode to program.  A mock-up of the issue
should appear, and the editor should have point-and-click commands
to rearrange the links, delete them, edit the titles and commentaries
again, and so on.  The mock-up should gather the URL's under each
category in the order they were submitted, and the categories
themselves should appear in the same order as they do in the pop-up
menu.  The order of the URL's within each category of the issue
is quite important, and the editor's tools for moving URL's around
within a category (or, I suppose, between categories) should afford
rapid wholesale rearrangement.  It is possible to make this interface
infinitely complex, for example by providing features to break
categories down into new subcategories or whatever, but this sort
of thing is not crucial.  In running webfilter services by hand, I
have sometimes used standardized categories and sometimes allowed
categories to emerge spontaneously within each issue.  But it is not
crucial to be able to improvise new categories, so long as it is easy
to edit the category menu in the Configure mode.

Incremental changes in the Revise page should be permanently stored
in the mocked-up issue.  The Revise page should have a "return" button
that returns to the Edit mode page without publishing the issue, as
well as a "publish" button.

(4) Configure mode

Along the way, I have listed some of the configuration options that
the editor should have.  It is easy to multiply such options, and you
can probably imagine them as well as I can.  It would be nice for each
service to have its own visual identity, selected from some options.
The Configure mode should presumably be used when a webfilter service
is first established, but it should hopefully not be needed very
often afterward.  I would guess that the most commonly used Configure
function will be adding new categories to the category menu.

(5) View mode

The owner also publicizes a URL for the service's View mode.  (For the
sake of cleanliness this should be a different page from the service's
Submit mode, though obviously the two pages should be linked to each
other.)  If you wanted to get fancy then you could offer users the
option of logging in and configuring the way they view a service.
But for most purposes a simple interface should suffice: links to
the recent issues in reverse chronological order.  It would also be
nice to offer links to reverse chronological lists of the links under
particular categories: the user would select these lists using the
same pop-up menu that they use to submit links.  Each list within a
given category would, of course, consist of sequential entries: title,
commentary, and URL.  The URL should be hyperlinked to the page it
names.  It would be nice if the server could periodically check all of
the pages to make sure they still exist, labeling links that have gone
bad so as to save users the trouble of trying to follow them.

The View mode page should also have a simple interface for subscribing
to the service by e-mail.  Just type in your address and hit the
"subscribe" button.  The server should obtain a confirmation by return
e-mail before adding the address to the list.

That's it.
```