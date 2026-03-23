---
id: trip-report-usps-advanced-technology-presentation
title: "\"Trip\" report: USPS Advanced Technology presentation"
type: writing
writing_type: rre-post
url: "http://commons.somewhere.com:80/rre/1995/Trip.report.USPS.Advance.html"
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - rre-post
  - auto-imported
  - rre
  - technology-policy
  - commerce
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1995/Trip.report.USPS.Advance.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991012032206/http://www.somewhere.com/)

  

# "Trip" report: USPS Advanced Technology presentation

```
Date: Fri, 7 Apr 1995 11:12:21 -0700
From: jyl@riesling (Jacob Levy)
Subject: "Trip" report: USPS Advanced Technology presentation
Reply-To: jyl@Eng

Please forward this message as widely as you see fit.

INTRO

---

This is a "trip report" of sorts. Thursday (4/6/95) evening I attended a
Smart Valley sponsored talk at Rickey's Hyatt by the VP of Advanced
Technology at the US Postal Service, Bob Reissler (sp?) and by the
technical architect, Richard Rothwell. The purpose of the talk was to give
USPS an opportunity to present their plans for "electronic mail and
electronic commerce for the general population".

I was the only one from Sun there as far as I could tell. There was a big
contingent of people from HP, Apple and some IBMers, many one-person
companies and startups, some trainers and educators and many unaffiliated
individuals - a total of about 150 people attended, standing room only.

OVERVIEW

---

Mr Rothwell's talk was the more substantive and interesting among the two.
He presented USPS's plans for offering electronic access to their email
delivery system to the 80 million US households and businesses that are
currently not reached by online service providers or the Internet. After
his talk, Mr Rothwell presented a short video on how they intend to educate
their customers on the new product, and another USPS employee demoed the
client side of their system online. Their client side system works under
Windows 3.1 with MS Mail and Lotus Notes.

Overall points to note: They are very concerned about privacy. They do not
want to be in the business of managing or issuing escrowed key-pairs. They
are very concerned about the new possibilities for abuse of privacy that
become available when public keys and identity certificates are widely used
(I didn't understand this part - what would these oppties be?). They are
interested in working with whoever cares to make the US Govt and
legislative branch relax the rules about using crypto and the export
controls. They are working on a system that works globally, and active
collaboration with other postal services is high on their agenda.  Canada
and European services were mentioned several times.

TECHNICAL POINTS

---

The system they are building is based on a transliteration of the basic
principles that make hardcopy mail work today, into the electronic world:

Stamp                   -> Digital Signature+digital money
Privace (envelope)      -> Encryption
Dating+location         -> Per-client digital time stamp (dts)
Identity (signature)    -> Digital signature (ds)

In regular hardcopy mail, the stamp proves that you paid and provides a
guarantee that the postal service will deliver your hardcopy. The envelope
provides privacy and is protected by privacy laws from tampering. The
dating is provided by the cancellation on the stamp. The location is
provided by each post office having its own cancellation label with its
name and serial number listed. The identity is provided by the signature of
the sender on the hardcopy stored within the sealed envelope carrying the
cancelled stamp.

The postal service will offer:

- An electronic mechanism for stamping a message and adding a dts so that
  it proves payment and dates the message
- Registered mail equivalent where the message gets signed by the USPS
  private key and the signature is returned to sender
- Mechanisms for managing public keys (see below - no escrow)
- Certificate mechanisms (see below - no escrow)
- Archival services for both messages, certificates and message signatures

In their new system, the "stamp" will be replaced by a digital signature on
a receipt returned to the sender and archived by the service. The receipt
will contain "enough bits to track the message through the system" (his
words). The service replaces the traditional envelope with encryption: it
accepts messages that are already encrypted and it will also offer RSA
public key encryption as a service. Dating is achieved by adding a dts plus
a digital signature identifying the client from which the message was
received (if desire) or a more generic signature. Finally the service
offers extensive mechanisms for corporate and individual public key
management and certification with various levels of identity checking, all
the way from biometrics based to a simple send-in-by-mail "under penalty of
perjury I hereby certify that I am Jacob Levy and this key is my public
key".  The service also offers a certificate and public key lookup service
based on an ISO 509 standard (?) without a publishing database, i.e.
modelled after the "Moscow city phonebook" (his words). The idea is you can
get anyone's public key if you know who they are but you cannot harvest the
phone book for, e.g., all postal employees living in San Mateo (apparently
they are concerned about e-mail bombs :).

Some new services that he talked about:

- Receipt notification through the equivalent of "sign here to receive
  your package" and delivery of the signed receipt back to the sender
- "Bonded mail" which as far as I could tell includes archival and
  delivery upon the occurrence of an event specified by the sender.
  He called this "Forever mail", i.e. you send something which is
  potentially never delivered, and he noted that this is already a
  service offered by the current USPS (many laughs..) and so it should
  be offered in the new system, in the interest of preserving their
  current product offerings (more laughs).
- Automatic tamper-proofing through the addition of a USPS generated
  signature that notarizes the text of your message.

--JYL
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991012032206/http://www.somewhere.com/)