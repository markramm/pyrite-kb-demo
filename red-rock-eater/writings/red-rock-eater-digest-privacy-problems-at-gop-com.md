---
id: red-rock-eater-digest-privacy-problems-at-gop-com
title: Red Rock Eater Digest - Privacy Problems at GOP.COM
type: writing
writing_type: rre-post
date: 2000-06-22
url: http://commons.somewhere.com:80/rre/2000/RRE.Privacy.Problems.at..html
importance: 6
research_status: partial
tags:
  - civil-liberties
  - cryptography
  - environment
  - government-info
  - international
  - military
  - privacy
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/2000/RRE.Privacy.Problems.at..html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20000816232108/http://commons.somewhere.com/rre/) | **Most Recent Article: Tue, 15 Aug 2000** |

```
[Reformatted to 70 columns.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
You are welcome to send the message along to others but please do not use
the "redirect" option.  For information about RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html

---

Date: Thu, 22 Jun 2000 18:07:29 -0700 (PDT)
From: PRIVACY Forum <privacy@vortex.com>
To: PRIVACY-Forum-List@vortex.com
Subject: PRIVACY Forum Bulletin: Privacy Problems at GOP.COM

			PRIVACY Forum Bulletin
			----------------------
			    June 22, 2000

	
	 House Majority Leader Criticizes Federal Government
     Web Sites' Privacy, but Apparently Failed to Check GOP.COM!
	
		    -----------------------------

Greetings.  Republican House Majority Leader Dick Armey today issued
a statement (http://freedom.gov/library/technology/lostprivacy.asp)
strongly condemning federal government Web site privacy practices,
particularly relating to the revelation regarding the use of cookies
and outside banner ad servers, and related information collection,
by companies working with the Office of National Drug Control Policy.
While that office contends that no privacy violations took place,
it is certainly true that if nothing else the appearance of privacy
problems caused by mixing cookies and banner ads with such agencies
would best be avoided.

The Majority Leader ended his statement with the words:

   "People with glass websites shouldn't throw stones."

I agree.  That's why it was with some surprise that I discovered that
the Republican National Committees' own Web site,

   http://www.gop.com

has a major privacy problem of its own.  While it turns out that
their site uses cookies, that's not necessarily a problem in and of
itself.  Much more serious is the situation on their linked GOPnet.com
("MyGOP") page:

   http://www.gopnet.com/MemberLogin.asp?Call=/mygop/mygop.asp

This page includes both a member login form and further down a form
for new members to register, where it collects personal information
such as names, e-mail addresses, credit card numbers, card expiration
dates, billing addresses, phone numbers, and so forth.

The page displays the VeriSign banner and claims that it is secure.
It is not.  At the time of this writing, the page security status
shows that the page is entirely unencrypted and that all data that
users provide via that page are subject to potential interception and
abuse at any point along their travels through the Internet.

At least one other page that collects credit card data at the GOP
site does have proper (Secure Sockets Layer) security enabled, and
it certainly seems reasonable to assume that the insecure page is the
result of a configuration error, not purposeful intent.

However, this points out most vividly the complexity of these systems,
and how easily they can be misconfigured in ways that negatively
impact security and privacy, even including such sensitive financial
information as credit card numbers and related data.  This also
highlights the dangers in rushing towards the implementation of broad
electronic signature and document systems, as described in:

   http://www.pfir.org/statements/2000-06-17

when it's so easy to have such serious problems with relatively
well-known credit card security systems.

As the House Leader stated, it's certainly true that "People with
glass websites shouldn't throw stones."

That of course should apply regardless of whose sites are involved.

--Lauren--
Lauren Weinstein
lauren@pfir.org or lauren@vortex.com
Co-Founder, PFIR: People for Internet Responsibility - http://www.pfir.org
Moderator, PRIVACY Forum - http://www.vortex.com
Member, ACM Committee on Computers and Public Policy

Date: Fri, 23 Jun 2000 09:36:16 -0700 (PDT)
From: PRIVACY Forum <privacy@vortex.com>
To: PRIVACY-Forum-List@vortex.com
Subject: PRIVACY Forum Update: More on GOP.COM and Security

			 PRIVACY Forum Update
			 --------------------
			    June 23, 2000

	
	  More on GOP.COM and Complexity in Security Systems
	
		    -----------------------------

Greetings.  In yesterday's (22 Jun 2000) PRIVACY Forum Bulletin, I
reported on a credit card submission Web page:

   http://www.gopnet.com/MemberLogin.asp?Call=/mygop/mygop.asp

whose security status showed "insecure" (no "lock" icon in Internet
Explorer, an open "lock" icon from Netscape browsers).  Most Web
users are now familiar with these icons, which provide the status
information that can be used (in conjunction with the additional
data available through the browsers at that point) to verify the
identity of a site and to determine the security status of pages
and the information that may be submitted via forms on those pages.
Due to a continuing series of security bugs in popular Web browsers,
it has become a standard security recommendation for users to review
that security information (which includes viewing the Secure Sockets
Layer certificate for detailed security data and identity) before
submitting information on such forms.

The main point of yesterday's bulletin was that these systems are
complex and easy to misconfigure, and that this demonstrates the risks
inherent in rushing towards the implementation of broader electronic
signature and document systems.

Upon continuing investigation, it turns out that this case is an
even better example of this complexity than I originally realized.
Analysis of the raw source code of the page referred to above reveals
that the form in question was indeed apparently sent to a secure
server (and so would presumably have its data protected with some
level of security), but this fact would not be apparent without such
source code analysis, and verification of site identity and security
levels could not be conducted in any normal way by users prior to
their submitting data via the form.

This appears to be an unusual and confusing configuration, since
the security status of the forms themselves as received by users
are typically the only information users have to make these important
security decisions before submitting their personal information.
In fact (as I mentioned yesterday) at the same site there are other
pages which are secured in the typical manner which allows users to
fully interrogate their security status prior to sending their personal
data.  It's critical that sites handling such data not only be secure,
but that they be configured in ways that clearly indicate to users
their actual, verifiable security status, and that allow ordinary
users to completely authenticate sites' identity and page security
levels prior to submitting any personal information via those pages.
Anything less can foster poor security practices by users in general,
which leaves them vulnerable to all manner of potential security and
privacy problems as they travel around the Web.

The complexity of these systems, and the various ways in which they
can be misconfigured in incorrect or confusing manners, should act as
a clear warning that we may be too rapidly moving to deploy mission-
critical applications in what is still a very new environment!

--Lauren--
Lauren Weinstein
lauren@pfir.org or lauren@vortex.com
Co-Founder, PFIR: People for Internet Responsibility - http://www.pfir.org
Moderator, PRIVACY Forum - http://www.vortex.com
Member, ACM Committee on Computers and Public Policy
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20000816232108/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20000816232108/mailto:webmaster@somewhere.com). |