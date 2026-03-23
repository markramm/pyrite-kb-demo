---
id: how-to-complain-about-spam
title: How to Complain About Spam
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1997/How.to.Complain.About.Sp.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - commerce
  - education
  - forwarded-content
  - government-info
  - internet-policy
  - law
  - libraries
  - rre
  - rre-post
  - telecommunications
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/How.to.Complain.About.Sp.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991023134115/http://www.somewhere.com/)

  

# How to Complain About Spam

```
Please do not forward this message.  It is a draft of a short article that
explains how to report suspicious spam to appropriate legal authorities
and Internet service providers.  I have tried to keep it as simple as
possible.  In particular, I have not tried to explain the legal issues in
detail, since it is the authorities' job to investigate whether a given
suspicious or offensive spam message violates any laws.  Likewise, it is
an ISP's own decision whether to initiate legal action against a spammer
who abuses its facilities.  

I'm hoping that you can read this draft.  Let me know about any factual
errors or any other specific information such as addresses or high-quality
URL's that might be good to include.  I think many people are despairing
about spam right now, and I'd like to help erase that despair by providing
simple actions that people can take to bring justice in those cases where
it is most required.

Thanks a lot

Phil

Encl:

  DRAFT FOR COMMENT -- DO NOT CIRCULATE

  How to Complain About Spam, or, Put a Spammer in the Slammer

  Phil Agre
  http://communication.ucsd.edu/pagre/

  November 1997

  DRAFT FOR COMMENT -- DO NOT CIRCULATE

  DRAFT FOR COMMENT -- DO NOT CIRCULATE

Unsolicited commercial bulk e-mail, commonly called "spam", has become an
extraordinary nuisance.  Spam as such is not illegal.  A large proportion
of the actual spam messages, however, do violate some state or federal
law.  Many others violate the spammer's contract with his or her Internet
Service Provider, or else cause enough harm to a third party to warrant a
civil lawsuit.  No legal action will be taken against a spammer, however,
unless someone reports the problem.  This article does not provide legal
advice.  It does, however, provide instructions for reporting messages
that may, in your judgement, deserve further investigation by appropriate
authorities.  Reporting spam does take a little effort at first, but once
you get a little practice, it can easily become a routine part of reading
e-mail.

The contact information I provide here is incomplete, and at present
includes only the United States.  Those with contact information for other
jurisdictions are encouraged to send it along for including in future
editions.

(1) Potential fraud and related issues

Many spam messages make offers that seem too good to be true, for example
money-making pyramid schemes, impossibly lucrative work-at-home deals,
suspiciously low prices, disingenuously described goods, and so forth.
You needn't judge for yourself which messages are legal.  If you find a
messages suspicious then you have a right, and perhaps even a moral duty
to others less sophisticated than yourself, to report the possible fraud
or misrepresentation to the Federal Trade Commission.  Simply print the
message out, add a simple cover letter expressing your concerns, and mail
it to:

  Federal Trade Commission
  6th Street and Pennsylvania Ave NW
  Washington, DC  20580

The FTC doesn't settle particular disputes, but it is very interested in
patterns, and a massive, fraudulent spam is nothing if not a pattern.

(2) Issues relating to paper mail

Schemes that employ the US mail may interest postal inspectors.  If a
suspicious spam message includes a US mail address, you might send a copy
of the message to the postmaster for the city and zip code in the address.
Again, simply print it out, add a simple cover letter expressing your
concerns, and mail it to:

  Postmaster
  Anytown, XX  12345

(3) Complaining to the police

Messages that are obviously illegal can also be reported to the FBI, to
the attorney general of any state that the message claims as its origin,
and to the local police.  In each case, once again, simply print out the
message and include a brief cover letter expressing your concerns.

To find the address of the nearest FBI field office, consult the following
web page:

  http://www.fbi.gov/fo/fo.htm

You can get the address for a given state's attorney general's office
by calling them on the phone; you can get their phone number by calling
directory information for the state capital (1 + the state capital's area
code + 555 1212).  If you send me the addresses for the attorneys general
of some of the larger states then I will include them in future editions
of this article.

If the message includes a postal address then you can get the address for
the spammer's local police department similarly.

(4) Complaining to your legislator

If you receive a particularly outrageous item of spam, you can use it
to help educate your elected representatives on the need for appropriate
legislative action.  You might focus particularly on state legislators,
because action is most likely at the state level.  At least one state,
Nevada, has passed very bad legislation in this area because legislators
were not well-enough educated.  You can easily identify your legislators
and obtain their addresses by calling your state's capitol building.

(5) Complaining to the service provider

Most Internet Service Providers require all of their subscribers to sign
contracts that forbid spam.  It is appropriate, therefore, to complain to
any ISP whose users originate spam.  The ISP usually isn't responsible for
the spam, so be polite.  But do encourage the ISP to take action against
the offender, and to strengthen its contractual language so that future
offenders face stronger penalties for spamming.  

The hard question is how to identify the spammer's ISP.  The most obvious
approach is to look in the From: field of the spam message's header.  If
you see a field like:

  From: yourfriend@flowers.net

you can be confident that the header was forged and that the message did
not originate at flowers.net.  Likewise, any header field such as:

  Comment: Authenticated sender is otherguy@aol.com

is probably bogus as well.  Another part of the header, however, is much
less likely to be forged.  It looks like this:

  Received: from networld.com ([194.177.96.7])
	by weber.ucsd.edu (8.8.6/8.8.6) with ESMTP id QAA23180
	for <pagre@weber.ucsd.edu>; Wed, 12 Nov 1997 16:01:42 -0800 (PST)

If you don't see any "Received:" fields in the header, that's because your
mail-reading program isn't displaying the complete header.  Consult the
program's documentation, or your ISP or system administrator, to find out
how to see the complete headers.  (It may be simple as using an alternate
command to write the message to a file.)  You will usually see several
"Received:" fields, which are supposed to trace which machines the message
has passed through.  Many spam messages include bogus "Received:" fields
to throw you off track.  But if you look at a header closely, you will
usually find that one or more of the fields mentions your own site; the
one you want is the one that records the message's first arrival within
your site.  This field was generated by the mailer at your site, so it
is probably reliable.  In the case of (fictional) the "Received:" field
that I quoted above, the message came from networld.com.  To report the
message, therefore, you should forward a copy of it like so:

  To: postmaster@networld.com
  Subject: spam from your site

  here is a spam message sent from your site ...

  [include a copy of the message, including the full header]

It is very important to include the full header of the message because
that's the site maintainer's major source of clues about the message's
actual origins.  In fact, the site to which you are complaining was most
likely "hijacked" against its will to produce spam.  This is very common,
and it generally results in torrents of "bouncemail" for the messages
that the spammer sent to bad addresses -- potential cause for a lawsuit.
Even if no lawsuit is filed, the site's maintainers need to upgrade
their software to prevent this sort of hijacking in the future, and your
complaint will help motivate them to do so.

You can also write to the postmaster of any site that is mentioned
in a URL that might be included in a spam message.  Enclose a copy of
the message, again with complete headers, and explain that the site in
question is being used by a spammer.

(6) Other resources

Here are the URL's for some other sources of information about spam:

http://server.Berkeley.EDU/BTLJ/articles/11-2/carroll.html
[more URL's for quality information sources are welcome]

(7) Conclusion

If we despair about spam then the spammers win.  Many thousands of people
are working against spam, each in their own way.  If you simply pick the
one method that you find most convenient then you can be confident that
these antisocial people will eventually be compelled to find better ways
of making a living.

Copyright 1997 by the author.  You may forward this article electronically
to anyone for any noncommercial purpose.  However, you must forward it
in its entirety, without modification.  This article is the responsibility
solely of its author.  It does not represent the views of the University
of California or any other organization.
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991023134115/http://www.somewhere.com/)