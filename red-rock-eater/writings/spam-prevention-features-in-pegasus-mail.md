---
id: spam-prevention-features-in-pegasus-mail
title: spam prevention features in Pegasus Mail
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1997/spam.prevention.features.html
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

Automatically imported from: http://commons.somewhere.com:80/rre/1997/spam.prevention.features.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991013201922/http://www.somewhere.com/)

  

# spam prevention features in Pegasus Mail

```
[A most excellent RRE subscriber was telling me about legal and technical
steps that David Harris, originator of Pegasus Mail, had taken to prevent
his program from being used for spam purposes.  Here are some relevant
messages.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Mon, 24 Nov 1997 08:14:18 -0600
From: "Scott Morizot" <tmorizot@ccsi.com>

[...]

The US Pegasus web site is:

http://www.pmail.com/

The Terms and Conditions are available at:

http://www.pmail.com/license.htm

I think you'll like them.  It's the only package I know currently that
explicitly includes provisions against spam in the license.  Although
they don't have extensive legal funds to pursue all the people who do
use it (and the laws vary extensively from country to country) anyone
who does use Pegasus in that manner is essentially using the software
illegally.  And that might help in a third-party lawsuit if needed.
2 relevant messages I retrieved from Dejanews are below.

---

From Dejanews, the message where David Harris announced the Anti-Spam
measures incorporated into Pegasus:

Subject:      Anti-spam measures incorporated into v2.5x.
From:         David Harris <David.Harris@PMAIL.GEN.NZ>
Date:         1997/04/02
Message-ID:   <182ED682034@urania.pmail.gen.nz>
Newsgroups:   bit.listserv.pmail
[More Headers]

The use or distribution of Pegasus Mail for the purposes of sending
bulk, unsolicited commercial e-mail is prohibited under its terms and
conditions of use. In order to support this prohibition, Starting with
version 2.50, Pegasus Mail for Windows incorporates measures that should
make it less useful to "spammers" (senders of unsolicited commercial
e-mail), and which should allow users of e-mail applications that can
filter mail to deal automatically with undesired "spam" messages sent
using Pegasus Mail.

Pegasus Mail now adds one of three new headers to messages it sends when
more than 50 recipients are present in the message. These headers can be
used as filtering triggers to delete such messages. The headers are based on
the number of recipients, and are as follows:

   0-50 recipients - no added header
   50-499 recipients - "X-Distribution: Moderate"
   500-4999 recipients - "X-Distribution: Bulk"
   5000+ recipients - "X-Distribution: Mass"

These headers have an internal CRC check applied to them and cannot be
changed or omitted by patching the binary. We have deferred announcing
the presence of these headers until now in order to give WinPMail v2.5x
a chance to propagate widely, and presumably into the hands of a large
number of spammers. While spammers using older versions of WinPMail will
escape the new headers, they will become progressively further and
further out of date and will be unable to take advantage of the newer
capabilities of the system without upgrading and thus exposing
themselves to automated detection.

As an example of how these headers may be useful in reducing spam levels, we
show below the steps necessary to create the Pegasus Mail filtering rules that
will delete such messages. Similar actions could presumably be taken in other
e-mail packages supporting automated processing of this kind.

We believe this addition to Pegasus Mail should be a significant step
towards reducing the prevalence of spam, or at least towards reducing the
abuse of Pegasus Mail for this purpose, yet it does not significantly impact
on legitimate users of the program.

Cheers!

-- David --

-------------------------- Cut here ----------------------------

Adding Pegasus Mail filtering rules to handle the new headers:

1: Open your "New mail filtering rules", "Rules applied when folder is
opened" rule set. In WinPMail v2.5x you  will find this on the "Tools"
menu under "Mail filtering rules".

2: Click the "End of list" entry to ensure the rule is added at the end
of the list of rules.

3: Click "Add Rule"

4: Click the radio button labelled "As an expression" and make sure the
radio button labelled "In message headers only" is also checked.

5: In the "Trigger text" field, type "X-Distribution:*Bulk"

6: Set the "Action to take" to "Delete" (or whatever else you feel is
appropriate).

Now repeat steps 2 to 6, but at step 5 type "X-Distribution:*Mass"

Save the rules, and you're done. These rules will automatically remove
any messages generated by a copy of Pegasus Mail v2.5x containing more
than 500 recipients. You could also add a rule that deleted all messages
containing more than 50 recipients, but doing this may occasionally
result in legitimate messages being deleted.

If you receive mail from a legitimate mailing list that could contain
these headers, you can prevent the message from being deleted by adding
a rule higher in the list than the spam-detection rule, that triggers on
some different characteristic of the message (like the sender's address)
and choose the "Exit this rule set" action, or else perhaps move the
"good" message to a folder.

------------------ David Harris -+- Pegasus Mail --------------------------
  Box 5451, Dunedin, New Zealand | e-mail: David.Harris@pmail.gen.nz
           Phone: +64 3 453-6880 | Fax: +64 3 453-6612

Sign in the room of an Italian hotel:
   "Visitors are requested not to throw coffee or other matter
    in the basin. Why else it stuffs the place inconvenient for
    the other world."

---

Also from Dejanews, the announcement of the supply for spam provision.
(The use for spam provision was always there.)

 Subject:      IMPORTANT: Enough is enough!
 From:         David Harris <David.Harris@PMAIL.GEN.NZ>
 Date:         1996/11/14
 Message-ID:   <29B8EBA3B81@urania.pmail.gen.nz>
 Newsgroups:   bit.listserv.pmail

Effective immediately, the terms and conditions of use for Pegasus Mail
are amended to include the following paragraph:

   The supply or promotion of Pegasus Mail for the purpose of sending
   bulk, unsolicited e-mail is incompatible with the basic aims of the
   program, which revolve around the free provision of a service that
   enhances the quality of peoples' communication. Pegasus Mail may not
   be included in any package designed for this purpose, whether free or
   otherwise, nor may vendors of such packages use the "Pegasus Mail"
   trademark or other related material in the promotion of their package.

Vendors or suppliers currently including Pegasus Mail in their bulk e-
mail products are hereby required to remove copies of and all references
to the Pegasus Mail software from their products. Failure to comply with
this requirement will lead to legal action.

The assistance of all members of the PMAIL and PM-NEWS mailing lists in
getting this message to vendors of mass-mail products would be gratefully
appreciated: in many cases, these people do not have functional e-mail
addresses and only have fax numbers. If you receive an obvious "spam", we
would be appreciative if you would fax this message to the perpetrator.

Pegasus Mail is a tool for quality communication, and we regard
indiscriminate mass-mailing as an antisocial, irresponsible abuse of
what we believe is our generosity in providing a service to the broader
Internet community.

David Harris
Author and owner, Pegasus Mail System.
14th November 1996.

------------------ David Harris -+- Pegasus Mail --------------------------
  Box 5451, Dunedin, New Zealand | e-mail: David.Harris@pmail.gen.nz
           Phone: +64 3 453-6880 | Fax: +64 3 453-6612

On the box of a clockwork toy from Hong Kong:
   "Guaranteed to work throughout its useful life."

---

---

Scott Morizot
tmorizot@ccsi.com
http://www.ccsi.com/~tmorizot/

Date: Mon, 24 Nov 1997 10:30:30 -0600
From: "Scott Morizot" <tmorizot@ccsi.com>
To: Phil Agre <pagre@weber.ucsd.edu>
Subject: Re: How to Complain About Spam

[About the Comment: field...]

This may be in the FAQ on the Web site somewhere, but following is the
segment from the Help file about the Comment: field with the Authenticated
sender message.

---

 From field:  WinPMail allows you to specify your own from field in outgoing
messages. This facility is provided only to allow you to conform with local
addressing schemes or requirements and should not be used capriciously. In
order to prevent message forgery using this feature, WinPMail will only send
mail if you have entered a valid username and password in the POP3 section of
the configuration dialog, and will check the validity of these details when
sending. The valid POP3 address is written into a field in the message for
security reasons.

---

The field in the message is the Comment: header with the authenticated sender
information.  It could be bogus, but it would require that someone had the
collusion of a provider (as in one of the spam providers) or had altered
Pegasus.  Of course, it the mail agent isn't Pegasus, then it's almost
certainly bogus as I don't think any other client actually does the above.

Again,  hope this helps.

Scott
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991013201922/http://www.somewhere.com/)
