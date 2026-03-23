---
id: privacy
title: privacy
type: writing
writing_type: rre-post
date: 1997-10-22
url: http://commons.somewhere.com:80/rre/1997/privacy.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - administrative
  - auto-imported
  - civil-liberties
  - commerce
  - cryptography
  - democracy
  - education
  - forwarded-content
  - government-info
  - international
  - internet-policy
  - labor
  - law
  - libraries
  - media
  - military
  - privacy
  - rre
  - rre-post
  - surveillance
  - telecommunications
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/privacy.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20001219033400/http://commons.somewhere.com/rre/) | **Most Recent Article: Fri, 15 Dec 2000** |

# privacy

```
[There's so much good stuff in this issue of Privacy Forum that I've simply
enclosed the entire issue.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Sat, 1 Nov 97 15:06 PST
From: privacy@vortex.com (PRIVACY Forum)
Subject: PRIVACY Forum Digest V06 #15

PRIVACY Forum Digest      Saturday, 1 November 1997      Volume 06 : Issue 15

            Moderated by Lauren Weinstein (lauren@vortex.com)         
              Vortex Technology, Woodland Hills, CA, U.S.A.
	                 http://www.vortex.com 

                       ===== PRIVACY FORUM =====              

    -------------------------------------------------------------------
                 The PRIVACY Forum is supported in part by
                    the ACM (Association for Computing)     
	         Committee on Computers and Public Policy,      
          "internetMCI" (a service of the Data Services Division         
                  of MCI Telecommunications Corporation), 
	  	  Cisco Systems, Inc., and Telos Systems.

* - - -

These organizations do not operate or control the     
          PRIVACY Forum in any manner, and their support does not
           imply agreement on their part with nor responsibility   
        for any materials posted on or related to the PRIVACY Forum.
    -------------------------------------------------------------------

CONTENTS 
	Update on the SPAM Battle (Lauren Weinstein; PRIVACY Forum Moderator)
	Information "Potatoes" (Lauren Weinstein; PRIVACY Forum Moderator)
	Prisoners with access to personal information (Jonathan G. Stotzer)
	Privacy in patients records (Charles MacLean)
	IE 4.0: bright spots and shadows (Peter Langston)
	S/MIME Crack?  Beware press bearing incomplete stories (Bruce Schneier)
	New Privacy Book by Beth Givens (Robert Gellman)
	Press Release: Junger v. Daley (Peter D. Junger)
	Monitoring of e-mail unlawful (Keith Parkins)
	Towards A European Framework for Digital Signatures And Encryption
	   (Keith Parkins)
	House Panel Questions FBI Implementation of Wiretap Law (Monty Solomon)
	Clinton Medical Privacy Recommendations Undercut State Protections,
           ACLU Says (Monty Solomon)
	The Electronic Privacy Papers: A new book by Schneier/Banisar
	   (Bruce Schneier)
	Europe spikes spooks' e-mail eavesdrop bid [by Duncan Campbell]
           (Dave Farber)

 *** Please include a RELEVANT "Subject:" line on all submissions! ***
            *** Submissions without them may be ignored! ***

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

VOLUME 06, ISSUE 15

   Quote for the day:

	"Would you like to know more?"

		-- "Federal Network" promotional slogan
		   "Starship Troopers" (TriStar/Touchstone; 1997)

---

Date:    Sat, 1 Nov 97 11:38 PST
From:    lauren@vortex.com (Lauren Weinstein; PRIVACY Forum Moderator)
Subject: Update on the SPAM Battle

Greetings.  This is a brief update on the battle against SPAM here at the
PRIVACY Forum.  I'm sorry to report that the problem appears to be growing
by leaps and bounds, and the block filter tables here against spam-oriented
sites, domains, and networks expand at a rapid pace.

I have a standard, polite message that I send out to postmasters in response
to spam, to which I always append the entire received original spam, complete
with all its headers to aid in tracing.  I also point out the problems of
third-party SMTP abuse and the need to control such activities.  At least
half the time, I usually get polite responses back, sometimes with requests
for more info about means for blocking spam at their sites.

But an unfortunate development is the distressingly ignorant attitude of an
increasing number of postmasters when it is pointed out that their sites are
being abused for third-party spamming.  I have this image of kindergarten
children with laptops, operating out of sandboxes, when I see the infantile
responses that sometimes arrive.  These are often rude, threatening, and in
general remarkable for persons dealing with the public about such important
matters.

Interestingly, the most offensive messages sometimes come from large
organizations--one of the worst I've received recently was from the
postmaster of a major nationally-known food company.  Do the public
relations representatives for these firms have any idea how much damage such
an attitude can cause?  Apparently not--but I suspect they'll learn the hard
way eventually.

In any case, I've become increasingly willing to add entries to the already
lengthy block lists here, and the amount of time spent dealing with this
garbage is rising very rapidly.  

The existence of what might be termed some "low-life" postmasters must bring
joy to the hearts of the spammers, and is yet another point calling into
question the feasibility of controlling this mess without legislation and
technical measures that might end up bordering on the draconian.  Not a
pretty picture.

--Lauren--
Moderator, PRIVACY Forum
http://www.vortex.com

---

Date:    Mon, 27 Oct 97 18:51 PST
From:    lauren@vortex.com (Lauren Weinstein; PRIVACY Forum Moderator)
Subject: Information "Potatoes"

Greetings.  A recurring theme here in the PRIVACY Forum is that many of the
privacy-related problems we see are basically artifacts of the legal vacuum
that exists when it comes to individuals having rights over their personal
information once it is in the hands of other entities.  In essence, personal
data is usually considered to be just another commodity to be bought, sold,
and in many cases handled haphazardly at best, just like sacks of potatoes.

In the absence of significant national policies and legislation, the
"free-for-all" when it comes to personal data can only be expected to
continue.  

The following two messages point out particular aspects of the general
problem.  The first deals with personal data collected by the "captive"
worker force of prison labor.  The second concerns personal medical data in
the hands of private transcription and processing persons and firms. 

"Happy" reading.

--Lauren--
Moderator, PRIVACY Forum
http://www.vortex.com

---

Date:    Fri, 24 Oct 1997 15:09:54 -0700
From:    "Jonathan G. Stotzer" <JON@FRIENDLYNET.COM>
Subject: Prisoners with access to personal information

On October 22, 1997 the ABC News Magazine "Primetime Live" featured a 
piece on the use of prison inmates by government agencies and private 
businesses to contact private citizens by mail and phone solicitations, 
and to gather and handle personal information of citizens, all without 
identifying the solicitors as prisoners, in prisons; and/or without 
advising the citizens that the information they provide to the government 
agency or private business would be handled and processed by prison 
inmates. 

The "Primetime Live" report indicated that at least 33 of our 50 states use
these convicted rapists, sexual offenders, murderers, and thieves, among all
others in the prison population, in this fashion. The contacts that these
prisoners have are nationwide. The obvious risks of this procedure were
shown in the report by several private citizens' whose information was
coopted by prisoners and used by the prisoners to send disturbingly graphic,
personally detailed, and sexually explicit letters to the citizens using
their personal information, and in other instances to charge items to their
credit cards. The rational for the use of these prisoners is that they are a
stable, reliable, and cheap workforce.

The forms of contacts made by these criminals with the public and the kinds
of personal information available to these criminals is astonishing.
consumer product questionnaires, telephone flight reservation Agents, state
boards of tourism telephone information operators, tax return handling and
processing, and telephone sales solicitations by charitable and for profit
organizations are all now being handled by criminals in prison.

Consumer product questionnaires people filled out by citizen for private 
companies with the persons name and address information, items of value 
they own, products they use, and income amounts they are processed by 
prison inmates. 

State tourism boards use prisoners as phone handlers, who obtain names, 
addresses and dates of travel.

Individual tax returns, showing names addresses, social security numbers, 
employer names and addresses, bank names, addresses, and account interest 
information, investment names and dividend income information are handled 
by criminals. 

Travel information, which gives the prisoners knowledge of credit card 
numbers, and the dates when you would be away from home is available, 
since some airlines use prisoners as phone reservation people. 

Phone sale solicitations by both for profit, and not for profit, businesses
use criminals as phone sales solicitors and sales representatives. One
example shown in the report was a "family-oriented" video sales company that
used criminals to make calls soliciting purchases by phone of their videos
and asking for referral names and numbers of other persons who might be
interested in the products.  Credit card information frequently is
transmitted by the private citizen.

I do not feel that it is appropriate for the government to allow any 
access to personal information that we as private citizens disclose to 
them, or am required to disclose to them by law should be in any fashion 
accessible to criminals in prisons.  Further, I do not believe that it is 
fair or appropriate for any business to be allowed to utilize prison 
labor to contact the public in general, or to handle personal information 
of private citizens without their specific prior knowledge and consent.

---

Date:    Sat, 25 Oct 1997 10:15:19 -0400
From:    "Charles MacLean" <chasmx@ix.netcom.com>
Subject: Privacy in patients records

I'm very concerned about the current trend by health care providers to
release confidential medical records into private homes for transcription
directly to their own employees, or through a service that has work at home
employees.  

The potential for intentional abuse or accidental disclosure is extremely
high.  No where else in the entire medical records system is one person
allowed to take that record off site without a court order. The medical
transcriptionist has total control over the confidential patient record in
an unsupervised environment (her home).

Once the doctor's dictation is transcribed into a medical report the
resulting disk file becomes along with many others becomes virtual mini
medical records.  The potential for abuse or accidental disclosure is
immense.

Now with the advent of the internet confidential patient records go zooming
around the globe as far away as Bombay India to get transcribed.  All this
without the knowledge of the patient.  Something has to be done to stop
this practice.

What are your feelings?

G. Charles MacLean
MTS, Inc.

---

Date:    Wed,  8 Oct 97 17:35:56 -0700
From:    Peter Langston <psl@langston.com>
Subject: IE 4.0: bright spots and shadows

Excerpted-from: TBTF for 10/6/97: Can you dig it?

IE 4.0: bright spots and shadows

  Microsoft broke records for downloads of its eagerly awaited new
  browser, but a couple of troubling questions have arisen

In the first two days after Microsoft made Internet Explorer 4.0 available,
users downloaded 1.2 million copies [5]. At 20 MB a pop, this represents a
copy every 6 seconds, or an average download band- width equivalent to three
T3s. Many more copies were distributed by 20+ mirror sites -- no central
figures exist. An additional two hun- dred thousand left Redmond on CD-ROM,
and Microsoft announced a deal with Sony to bundle IE4 on Sony music CDs.
(I wonder if, when I buy the latest Fiona Apple CD, Microsoft counts me as
a customer on the way to its stated goal of 50% of the browser market?)

In the midst of the enormous popularity of this software a couple of warning
flags have appeared (in addition to the questions raised by IE4's swift but
deviant Java implementation -- see above). First, IE4 provides a powerful
new way for content providers to log user actions. Second, an early survey
questions the inherent wisdom of Microsoft's strategy of unifying Net and
desktop.

1. Channel Definition Format. When you subscribe to push information using
IE4's built-in facilities, providers can log your access to their content
even if you went through an anonymizing proxy server, and even if your
access came from your local cache and not over the Net. IE4's channel
definition format [6] includes a feature, LOG- TARGET, that allows a
Web-site provider to command IE4 to deliver logs of your usage via an HTTP
POST or PUT directive. It's not clear whether the provider could include
other sites in its channel defin- ition to obtain, for example, logs of your
usage of competing ser- vices. Below is an extract from Microsoft's site
[7] where the LOGTARGET directive is defined.

      > Logging Declarations

      > Specifies where to upload a client's page-hit log file in Ex-
      > tended Log File Format.

      > HREF="url"
      >     Required. Specifies the URL of where the log file should
      >     be sent.
      > METHOD="POST" | "PUT"
      >     Required. Specifies the HTTP method to be used for sending
      >     the data. [RFC 1945]
      > SCOPE="ALL" | "OFFLINE" | "ONLINE"
      >     Specifies which type of page hits should be logged. Page
      >     hits can be logged for offline (read from local cache)
      >     or online (read from URL) browsing. The default for this
      >     attribute is "ALL", which logs both types of hits.
      > PURGETIME
      >     When the log file is being uploaded, any page hits older
      >     than PURGETIME will not be reported.

      > Example:

      > <LOGTARGET HREF="http://www.foosports.com/logging"
      >     Method="POST" SCOPE="OFFLINE">
      >     <PURGETIME HOUR="12"/>
      > </LOGTARGET>

Thanks to Jamie McCarthy <jamie@voyager.net> for the first forward of
information on this troubling feature.

---

Date: Fri, 26 Sep 1997 16:08:17 -0500
From: Bruce Schneier <schneier@counterpane.com>
Subject: S/MIME Crack?  Beware press bearing incomplete stories

What I did:  write a Windows 95 screen saver that automatically brute
forces 40-bit RC2 keys.  The screen saver is has an easy interface, and
parallizes nicely.

What I didn't do:  break S/MIME.  I did not find any flaw in the S/MIME
security specification.  I did not find any flaw in any of the cryptographic
algorithms used.  I did not find any flaw in any software implementation
of S/MIME.  There is nothing wrong with the S/MIME standard.

What I find, though, is that many S/MIME implementations don't interporate
at anything stronger than 40-bit RC2.  I find that the default encryption
is 40-bit RC2, and the user isn't given any indication that the encryption
level should be changed.

40-bit RC2 is weak.  This is nothing new to anyone who reads the S/MIME
specifications. In fact, the S/MIME specification is very forthcoming in
discussing security of 40-bit RC2.

> 2.6 ContentEncryptionAlgorithmIdentifier
>
> Receiving agents MUST support decryption and encryption using the RC2
> algorithm [RC2] at a key size of 40 bits, hereinafter called "RC2/40".
> Receiving agents SHOULD support decryption using DES EDE3 CBC,
> hereinafter called "tripleDES".
>
> Sending agents SHOULD support encryption with RC2/40 and tripleDES.

Later in the spec, the following appears:

> Before sending a message, the sending agent MUST decide whether it is
> willing to use weak encryption for the particular data in the message.
> If the sending agent decides that weak encryption is unacceptable for
> this data, then the sending agent MUST NOT use a weak algorithm such
> as RC2/40. The decision to use or not use weak encryption overrides
> any other decision in this section about which encryption algorithm to
> use.

And even later:

> 2.6.2.3 Rule 3: Unknown Capabilities, Risk of Failed Decryption
>
> If:
>  - the sending agent has no knowledge of the encryption capabilities
>    of the recipient,
>  - and the sending agent is willing to risk that the recipient may
>    not be able to decrypt the message,
> then the sending agent SHOULD use tripleDES.
>
> 2.6.2.4 Rule 4: Unknown Capabilities, No Risk of Failed Decryption
>
> If:
>  - the sending agent has no knowledge of the encryption capabilities
>    of the recipient,
>  - and the sending agent is not willing to risk that the recipient
>    may not be able to decrypt the message,
> then the sending agent MUST use RC2/40.

And:

> 2.6.3 Choosing Weak Encryption
>
> Like all algorithms that use 40 bit keys, RC2/40 is considered by many
> to be weak encryption. A sending agent that is controlled by a human
> SHOULD allow a human sender to determine the risks of sending data
> using RC2/40 or a similarly weak encryption algorithm before sending
> the data, and possibly allow the human to use a stronger encryption
> method such as tripleDES.

I wrote this screen saver not to trash S/MIME (even though the announcement
was used by another company), but to 1) illustrate that 40-bit RC2 really
is insecure, and 2) try to force companies who implement S/MIME to get
DES and triple-DES to interoperate.  I heard recently that RSADSI has said
there is a triple-DES message on their website that can be understood by
both Microsoft Internet Explorer and Netscape Communicator.  I don't know
about the message, but when I tried to get DES and triple-DES to interoperate
a few months ago I couldn't.

Bruce

---

Bruce Schneier, President, Counterpane Systems     Phone: 612-823-1098
101 E Minnehaha Parkway, Minneapolis,MN  55419       Fax: 612-823-1590
                                            http://www.counterpane.com

---

Date:    Sun, 21 Sep 1997 21:17:24 -0400 (EDT)
From:    Robert Gellman <rgellman@cais3.cais.com>
Subject: New Privacy Book by Beth Givens

There is a new privacy book that should be of interest to people
on this list.  It is "The Privacy Rights Handbook:  How to Take
Control of Your Personal Information" by Beth Givens.  Some of
you will recognize Beth as the founder of the Privacy Rights
Clearinghouse in San Diego, CA <www.privacyrights.org>.

The Privacy Rights Clearinghouse is just about the only privacy
organization that deals directly with consumers.  As a result,
the book is expressly geared to consumers and is filled with
practical advice on what can be done to control personal
information and enhance privacy.  Chapters contain FAQ and
addresses and phone numbers of dozens of companies and
organizations.  

The book addresses commercial and governmental activities, both
on and off the Internet.  It has advice on workplace privacy and
on personal safety (i.e., stalking).

I've read most of the privacy books that have come out in the
last decade, and this is the most practical book for a long time. 

The publisher is Avon Books.  It is a paperback with a US price
of $12.50 and a Canadian price of $16.50.  ISBN 0-380-78684-2.

Robert Gellman          rgellman@cais.com   
Privacy and Information Policy Consultant   
431 Fifth Street S.E.                       
Washington, DC 20003                        
202-543-7923 (phone)   202-547-8287 (fax)   

---

Date: Thu, 16 Oct 1997 15:59:56 -0400
From: "Peter D. Junger" <junger@samsara.LAW.CWRU.Edu>
Subject: Press Release: Junger v. Daley

			    Press Release

	   Summary Judgment Motion Filed in Suit Attacking
	      Restrictions on the ``Export'' of Software

	    Brief Claims Publication of Computer Software
		   Is Protected by First Amendment

 Export Regulations Restrict Only Publication of Encryption Software,
			     Not Its Use

   ----------------------------------------------------------------

	     Cleveland, Ohio, Tuesday, October 16, 1997
			For Immediate Release

		    For More Information Contact:
 

		    Peter D. Junger (216) 368-2535
		    <junger@samsara.law.cwru.edu>

		    Gino Scarselli (216) 291-8601
		    <gscarsel@mail.multiverse.com>

		    Raymond Vasvari (216) 622-1780
		   <freespeech@mail.multiverse.com>

	Or see URL: http://samsara.law.cwru.edu/comp_law/jvc/
 

To be added to, or removed from, the list of those who were sent this
 press release, please send e-mail to <lawsuit@upaya.multiverse.com>.

     _________________________________________________________________
   

Cleveland, Ohio, October, 16. -- 

Pointing out that no law forbids or restricts the use of encryption
software, attorneys for Professor Peter D. Junger have moved for
summary judgment on first amendment grounds in his suit to strike down
export regulations that forbid the publication of ``encryption
software'' on the Internet or in other electronic form.

The government justifies the restrictions on publication, which are
part of the Export Administration Regulations administered by the
U.S. Department of Commerce, by arguing that computer software is
functional and that the use that encryption software might be put to
could endanger national security.  But, as Junger's lawyers point out
in their brief in support of the motion, ``[a]lthough the reasons the
government has given for controlling the export of encryption software
have to do with the software's potential use, the regulations do not
prohibit its use.''

``This is not a complicated case involving complex issues of computer
science or engineering,'' says Gino J. Scarselli, Professor Junger's
lead attorney.  ``Once you recognize that computer programs are
written and published just like any other text---like mathematical
proofs and musical scores, for example---it becomes clear that the
regulatory scheme, which requires a would-be publisher to apply for
and obtain a license before he can publish, is a classic example of a
prior restraint and it's unconstitutional.''

``I am convinced,'' Scarselli adds, ``that a law prohibiting the use
of encryption software would be unconstitutional, for the same reason
that a law forbidding the manufacture and sale of printing presses or
word processors would be unconstitutional.  But that's not the issue
in Junger's case.  There is no law against the use of encryption
software; there are only regulations forbidding its publication.  And
the fact that it is only publication on the Internet and in other
electronic form that is restricted does not help the government,
because the Supreme Court held this year that the Internet is entitled
to the full protection of the First Amendment.''

Junger's case is similar to one brought by Professor Daniel Bernstein
in which Judge Patel of the Federal District Court for the Northern
District of California recently declared that the challenged
regulations ``are in violation of the First Amendment on the grounds
of prior restraint and are, therefore, unconstitutional''.  That
decision is now being appealed by the government.

Recently there has also been extensive debate in Congress over the
issue of whether the import and the domestic distribution of
cryptographic software should be restricted, as has been proposed by
the FBI and other law enforcement agencies who are unhappy with the
idea that they may not be able to read everyone's electronic mail.
But Professor Junger contends that his case and the Bernstein case
involve issues of much greater importance than the availability of
electronic envelopes.  ``If the government's functionality argument
were to be upheld, it would mean that the government could suppress
the writing and publication of any software which might be used in
ways the government does not like.  And not just software.  Any
writing that delights or instructs or persuades has functionality.
The government's functionality argument could justify requiring you to
get a license before you publish a legal form book or a political
pamphlet or a book of sermons.  And it is exactly that type of
censorship that led the adoption of the first amendment.''

Copies of the brief and motion will shortly be available at
<http://www.jya.com/> and <http://samsara.law.cwru.edu/comp_law/jvd/>.
Copies of earlier pleadings and other documents in the case of Junger
v. Daley can be found at <http://samsara.LAW.CWRU.Edu/comp_law/jvd/>.

				 -30-

---

Peter D. Junger--Case Western Reserve University Law School--Cleveland, OH
 EMAIL: junger@samsara.law.cwru.edu    URL:  http://samsara.law.cwru.edu   
     NOTE: junger@pdj2-ra.f-remote.cwru.edu no longer exists

---

Date:    Tue, 28 Oct 1997 07:55:06 PST
From:    "Keith Parkins" <keithpp@hotmail.com>
Subject: Monitoring of e-mail unlawful

According to an article by Duncan Campbell, in The Guardian, it
is unlawful for companies in Europe to monitor their employees
private communications (this would incl e-mail).

This issue was settled in the European Court of Human Rights about six
months ago, when former Mersyside Asst Chief Constable Alison Halford was
awarded damages against her former employers, who conceded that they had
tapped her office telephone.

ref

Duncan Campbell, Europe spikes spooks' e-mail eavesdrop bid, 
Online, The Guardian, 16 October 1997

        http://www.guardian.co.uk/online/

Keith

		[ Of course, don't necessarily assume the same outcome in
		  other situations or other locales!  Laws regarding
		  employer monitoring vary widely around the world.

					-- MODERATOR ]

---

Date:    Tue, 28 Oct 1997 07:56:03 PST
From:    "Keith Parkins" <keithpp@hotmail.com>
Subject: Towards A European Framework for Digital Signatures And 
	 Encryption

The EC has published a paper, that if adopted as an EU directive,
would make proposals such as those contained in SAFE unlawful in
any member state. 

I am pleased to say that what I have read as a summary of this
paper it appears to have taken heed of my submissions to the UK
DTI on the regulation of encryption.

I may have more to say once I have read the EC paper and had time
to digest the detail.

        http://www.ispo.cec.be/eif/policy/97503.html

        http://www.i-way.co.uk/~reality/sunrise/ukdtittp.htm

        http://www.i-way.co.uk/~reality/sunrise/spooks.htm

Note  There is currently problems with access to my pages.  This
problem may or may not have been solved by the time this appears.

Keith

---

Date:    Tue, 28 Oct 1997 13:08:05 -0500
From:    Monty Solomon <monty@roscom.COM>
Subject: House Panel Questions FBI Implementation of Wiretap Law

Excerpt from ACLU News 10-26-97

House Panel Questions
FBI Implementation of Wiretap Law

FOR IMMEDIATE RELEASE
Thursday, October 23, 1997

WASHINGTON -- Amid growing concerns about privacy implications and
costs, a House subcommittee today questioned FBI implementation of a
controversial 1994 law that forced telephone companies help law
enforcement agencies gain access to digital phone lines for surveillance
operations.

During the four-hour hearing before the Crime Subcommittee of the House
Judiciary Committee, two Republicans -- Bob Barr of Georgia and Steve
Chabot of Ohio -- were harshly critical of the 1994 law, has implemented
it, saying it represents an enormous invasion of privacy and could lead
to a system of ongoing government surveillance.

Seconding those criticisms, the American Civil Liberties Union said that
safeguards originally implemented in the legislation have failed to
protect the American public. "The hearing today clearly revealed that
the FBI is embarked on a scheme to undermine the privacy of every
law-abiding American," said Donald Haines, a Legislative Counsel with
the ACLU's Washington National Office.

"From the very beginning, the FBI has flagrantly violated both the
process and the requirements set out in the legislation," Haines added.
"The FBI has repeatedly sought to coerce the telecommunications industry
into changing its technology so that law enforcement agencies could
increase their wiretapping."

The 1994 telecommunications act is far from the only effort by the FBI
to gain backdoor access to private communications. In another ongoing
Congressional debate, the FBI is trying to impose restrictions on the
use of privacy-protecting encryption technology. 

"Congress must squarely confront this persistent pattern of FBI and law
enforcement intrusions into our privacy," Haines said. "Congress should
act immediately to repeal the 1994 law, or, at an absolute minimum,
refuse to fund any implementation activities."

---

Date:    Wed, 29 Oct 1997 23:19:21 -0500
From:    Monty Solomon <monty@roscom.COM>
Subject: Clinton Medical Privacy Recommendations Undercut State Protections,
         ACLU Says

Excerpt from ACLU News 10-29-97

Clinton Medical Privacy Recommendations
Undercut State Protections, ACLU Says

FOR IMMEDIATE RELEASE
Tuesday, October 28, 1997

WASHINGTON -- As a Senate committee today continued its hearings on the
Clinton Administration's recommendations regarding medical privacy, the
American Civil Liberties Union said the government's proposal is even
more dangerous than originally believed because it would undermine some
state-level protections.

The ACLU said that it agreed with several privacy experts who told the
Senate Labor and Human Resources Committee that the Clinton
Administration proposal would limit states from offering more protection
to medical records than provided by the federal government.

"This is yet another of the Clinton Administration privacy dodges," said
Donald Haines, a Legislative Counsel for the ACLU's National Washington
Office.

"During her testimony last month, Health and Human Services Secretary
Shalala promised that individual states would be free to offer their
citizens more protection," Haines said. "But closer analysis of the
Clinton recommendations has shown that that is just not true."

Many state-level protections for medical information come from common
law rights (interpretations developed through the years by judges)
rather than statutes (laws passed by the legislature). But, buried at
the end of the Shalala recommendations -- far from her rhetoric praising
state laws -- is a provision that would override protections offered
medical privacy by state common laws.

Given this latest discovery about the Clinton recommendations, the ACLU
reiterated its request that Congress repeal so-called "Administrative
Simplification," a little-known amendment to the 1996 Health Insurance
and Portability Act. Under "Ad Simp" and related provisions, Congress
set in motion the creation of massive national databases of everyone's
cradle-to-grave personal medical information. 

The law also ordered Shalala to protect medical privacy, offering the
Administration the opportunity to safeguard medical records from being
forcibly included in the databases and widely disseminated. But the ACLU
said that by failing to stop the creation of the databases, the Shalala
recommendations actually harmed medical privacy more than they protected
it.

"Those of us who don't want to become a number in this Orwellian scheme
must call for a repeal of the legislation mandating these regulations,"
Haines said. "Congress should scrap Ad Simp and start over from
scratch."

Any medical privacy legislation, the ACLU said, must include protections
against the following:

-- Computerization. Patients must be given the option of a "paper only"
record -- thereby keeping confidential information out of computer
networks and databases -- without risking denial of insurance or loss of
benefits.

-- Lack of informed consent. Secretary Shalala and others have
said that privacy rights cannot be absolute, claiming that "it's not
always possible to ask for permission" to use a patient's record. But
Americans think differently. According to a Time/CNN poll, 87 percent of
Americans demand to be asked for permission every time medical
information about them is being used.

-- Establishment of a National I.D. Number. Any law must prohibit
establishment of a "unique health identifier" -- a de facto national
I.D. assigned by government or business and used to link all medical
records from cradle to grave.

The ACLU said it was particularly eager to review the new legislation
offered today by Senator Patrick Leahy, D-VT, to see if it meets all
those tests.

"Senator Leahy has already made significant contributions to this
ongoing debate about medical privacy by opposing some of the Shalala
recommendations," Haines said. "Unfortunately, we fear that the Leahy
proposal will fail in some important respects. Will it, for example,
live up to the American public's demand that no disclosure be made
without prior approval?" 

Other Senate offices and private groups are discussing legislation that
would impose compulsory disclosure of confidential medical information,
the ACLU warned. Prohibiting access by government agents to personally
identifiable medical information remains another important concern under
the Clinton recommendations, the Leahy bill and other legislative
proposals.

"We are eager to support legislation -- at both the state and federal
level -- that genuinely protects medical privacy," Haines said. "But we
will strongly oppose any proposals that merely pretend to protect
privacy or offer some protection while failing in other important ways." 

---

Date:    Wed, 1 Oct 1997 20:18:04 -0500
From:    Bruce Schneier <schneier@counterpane.com>
Subject: The Electronic Privacy Papers: A new book by Schneier/Banisar

The Electronic Privacy Papers: Documents on the Battle for Privacy
in the Age of Surveillance

by Bruce Schneier and David Banisar

John Wiley & Sons, 1997
ISBN: 0-471-12297-1; 747 pages
Retail: $60 hardcover

Trying to keep up with the advancements in cryptography and digital
telephony, the government has advocated controversial new tools that will
allow them to monitor electronic communications. On the other side of the
spectrum, privacy advocates are vehemently opposed to any government
monitoring whatsoever.

The Electronic Privacy Papers is a collection of previously unreleased
documents dealing with privacy in the Information Age.  Combining public
government pronouncement, public reactions, and previously classified
documents released under FOIA, this book paints a clear picture of
government policies towards encryption and privacy and how they will impact
individuals and companies involved with the Internet.

Issues covered include:

	The economic and political rationale for demanding digital
wiretapping and surveillance.

	The legal foundations, and limitations to, government
surveillance.

	Government strategies for soliciting cooperation from
telephone companies and equipment manufacturers.

	Which policies industries and individuals can expect the
government to pursue in the future.

The Electronic Privacy Papers retails for $60 in hardcover.  I am
offering it at the usual 15% discount.

---

                          ORDER FORM

The Electronic Privacy Papers (Hardcover): $60 * .85 = $51.00

          Shipping:
                    Air (U.S.):       $5 per book
                    Surface (U.S.):   $3 per book
                    Canada/Mexico:    $7 per book
                    Everywhere else:  $9 per book

Send to:

          Counterpane Systems, 101 E Minnehaha Parkway,
                    Minneapolis, MN  55419

I need payment by check, in U.S. funds drawn on a U.S. bank.  Or a
postal money order.  Sorry, no credit cards.

---

                     Table of Contents

PART 1: PRIVACY AND THE INFORMATION SNOOPERHIGHWAY
Introduction: Roadblocks on the Information Superhighway

PART 2: WIRETAPPING
Overview of Wiretapping

PART 3: LOBBYING FOR SURVEILLANCE: THE DIGITAL TELEPHONY PROPOSAL
Government Pronouncements: The Digital Telephony Proposal
Behind the Iron Curtain: Operation Root Canal
Digital Telephony: The Public Response

PART 4: CRYPTOGRAPHY
Cryptography - The Cure for the Common Bug

PART 5: THE BATTLE FOR CONTROL OF CRYPTOGRAPHY
The Field of Battle: An Overview
Early Skirmishes
The Clipper Chip Proposal
Unclassified: The Story Behind Clipper
Clipping the Clipper: Public Response to Desktop Surveillance

PART 6: PUTTING THE GENIE BACK IN THE BOTTLE: EXPORT CONTROLS ON
	CRYPTOGRAPHY
Atom Bombs, Fighter Planes, Machines Guns and Cryptography: Export
	Control
Untying the Gordian Knot: Efforts to Relax Export Controls

PART 7: BIG BROTHER AS THE KEEPER OF THE KEYS: WILL THE GOVERNMENT
	TAKE OVER CRYPTO?
Banning Cryptography
Software Key Escrow

EPILOGUE: THE FUTURE OF CRYPTOGRAPHY
Bibliography of Books on Wiretapping, Cryptography and Privacy
Index.

---

Date: Sun, 26 Oct 1997 13:49:07 -0500
From: Dave Farber <farber@cis.upenn.edu>
Subject: Europe spikes spooks' e-mail eavesdrop bid [by Duncan Campbell]

* - - - - -

Duncan Campbell
Europe spikes spooks' e-mail eavesdrop bid

US and British intelligence agencies received a major blow last week,
when the EC urged governments to introduce uniform and effective
encryption standards to protect communications on the Internet,
writes Duncan Campbell. In a landmark report, the EC asserted that
legal recognition and standards for digital signatures, which depend
on effective cryptography, should be put in place across the EU by
2000 "at the latest".

The EC report, Ensuring Security and Trust in Electronic
Communication [http://www.ispo.cec.bei/eif/policy/97503.html], is
set to receive enthusiastic IT industry backing, after years of
foot-dragging by the US National Security Agency (NSA) and the
last British government in an attempt to block effective international
encryption and keep Net communications accessible to their global
surveillance systems.

Since 1991, the Clinton administration has been trying to persuade
its citizens and allies to adopt a system for secret government access
to private code keys. A heated battle is now underway in the US
Congress, where five competing and opposing versions of an
encryption law have been passed in different committees.

But Europe is having no truck with this. The EC report maintains
that allowing third parties secretly to decode personal and business
communications will not merely fail to stop criminals, but will
create massive new security headaches. It would also threaten
personal data privacy, already protected by a European directive on
data protection. What's more, says the report, it would intolerably
damage European interests in electronic commerce and the
information society.

Although the EU concedes that individual governments can, in
principle, make their own national security arrangements, member
states are now being warned that restrictions on importing or
exporting cryptographic products may be unlawful under sections of
the European treaty, as well as contrary to existing community
directives.

"The European Union simply cannot afford a divided regulatory
landscape in a field so vital for the economy and society," the
Commission maintains. "Divergent and restrictive practices with
regard to cryptography can be detrimental to the free circulation of
goods and services within the internal market" and will "hinder the
development of electronic commerce".

To back this up, the EC has set a fast-paced timetable, which kicks
off before the end of the year with an Internet Forum and the
liberalisation of national and international restrictions on selling
cryptography products. The EC has already decided in principle that
member states should be required to guarantee "the free movement of
encryption technologies and products" within the EU.

The Commission plans to hold an international hearing at the
beginning of next year on this month's proposals, to be followed up
by a directive on digital signatures. By 2000, the goal is to have a
"common framework on cryptography in place throughout the
Union".

The Commission says it found no evidence that regulation could or
would stop criminals from using effective encryption. On the
contrary: "Restricting the use of encryption could well prevent
law-abiding companies and citizens from protecting themselves
against criminal attacks."

Even more dangerous, says the EC, is the current US plan to build
central depositories for private code keys. Such a system was also
proposed in the UK a few weeks before the general election. The EC
says this would give criminals "additional ways to break into a
cryptographic system" and that the central key stores themselves
would or could "become target for attacks" by organised crime or
hostile intelligence agencies.

Europe's determination to press ahead with genuinely secure privacy
and digital signature systems now threatens to put the US into third
place, after Europe and Asia, in the race to exploit electronic
commerce.

Opponents and advocates of effective cryptography agree that key
access systems will fail entirely if introduced only in one country, as
users will obtain secure cryptographic services from countries that do
not have such restrictions. Electronic isolationism is not an option
for an industrialised nation in the 21st century.

If US intelligence agencies continue to demand universal access to
keys, they will not merely imperil their own citizens' privacy and
constitutional rights, but gravely undermine the US lead in IT. Faced
with increasing industry, international and civil liberties opposition
from right and left, intelligence agency advocates have reached levels
of hysteria not seen since the peak of the cold war. Three months
ago, FBI director Louis Freeh told the US Senate Judiciary
Committee that "uncrackable encryption will allow drug lords, spies,
terrorists and even violent gangs to communicate about their crimes
and their conspiracies with impunity". The public safety of our
citizens was at stake, he insisted.

One official response to the EC report in Washington last week was
a claim that corporations wanted key access systems in order to check
on their employees' private e-mail messages. But this latest shift of
tack only emphasises how out of touch US policymakers are. It is
already clear in Europe that, whether or not companies might want
to, it is unlawful for them to spy on their employees' private
communications. That issue was settled six months ago in the
European Court of Human Rights, when former Merseyside assistant
chief constable Alison Halford was awarded damages against her
former employers, who tacitly conceded that they had tapped her
office telephone.

In Britain, advocates for restricting cryptography have spoken,
almost wishfully, of the possibility of "a backlash" which would
turn public opinion their way, "if there are serious crimes committed
and people killed and encryption is in use".

Such scenarios are lampooned by experts of the seniority of
Cambridge's Professor Roger Needham, now also Microsoft's
Director of Research, who last month described the US plans as:
"Like requiring men waving red flags to walk in front of horseless
carriages. Strong and effective encryption systems can't be stopped."

British policy on encryption is now "up for grabs", say insiders.
"There are only a limited number of moves that a government can
make in a democratic society," DTI information security specialist
Nigel Hickson told last month's Cambridge conference on economic
crime. "We are still thinking what they can be."

Meanwhile, Labour IT minister Barbara Roche has taken delivery of
an assessment of responses to the former government's proposals.
DTI officials are taking comfort from the support they received for
digital signature schemes, in contrast to the opposition and abuse
engendered by the proposal for government access to keys. Both of
these features have been intensified by last week's EC report.

The DTI now appears to be in favour of separate plans for digital
signatures from the "law enforcement" agenda to restrict
cryptography, and to press ahead with the former. It is confident of
political and industrial support for this approach. Until last week,
that left the question of a cryptography policy open, making British
as well as US policymakers' offices potentially the site of trench
warfare between clandestine agencies and the powerful IT lobby.

At an extremely timely moment, Europe has lifted the Government
off the horns of that dilemna. Its clear and fast timetable, coupled
with a firm warning that no European state may go it alone, the EC
has not only pushed the spooks away but given the Government the
chance next year to win substantial EC financial backing for
Britain's IT industry in pioneering the new cryptosystems Europe
should have in place for the millennium.

[Duncan Campbell is a freelance writer and broadcaster, and not the
Guardian's crime correspondent of the same name]  15 October 1997

---

End of PRIVACY Forum Digest 06.15

---
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20001219033400/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20001219033400/mailto:webmaster@somewhere.com). |