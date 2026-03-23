---
id: certificate-authorities-and-digital-signatures
title: certificate authorities and digital signatures
type: writing
writing_type: rre-post
date: 1997-07-16
url: http://commons.somewhere.com:80/rre/1997/certificate.authorities..html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - commerce
  - community-networking
  - cryptography
  - education
  - environment
  - forwarded-content
  - government-info
  - health
  - international
  - labor
  - law
  - privacy
  - technology-policy
---



## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/certificate.authorities..html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009035854/http://www.somewhere.com/)

  

# certificate authorities and digital signatures

```
[Relevant Web sites include http://csrc.nist.gov/events/Pubfrm-agn.html
http://csrc.nist.gov/events/pfcadsegec.html and http://www.acm.org/usacm/]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Fri, 18 Jul 1997 16:09:42 -0500
From: Marc Rotenberg <rotenberg@EPIC.ORG>

                       ASSOCIATION FOR COMPUTING
                           Washington Office
                   666 Pennsylvania Ave., SE Suite
                         Washington, DC 20003
                             202/544-4859
                       http://www.acm.org/usacm/

July 16, 1997

Director, Information Technology Laboratory
ATTN: "Public Forum on Certificate Authorities and Digital Signatures"
Technology Building, Room A231
National Institute of Standards and Technology
Gaithersburg, MD 20899.

The United States Public Policy Committee for the Association for Computing
(USACM) welcomes this opportunity to participate in the "Public Forum on
Certificate Authorities and Digital Signatures: Enhancing Global Electronic
Commerce".  Safety, confidentiality, integrity and authenticity of
electronic transactions and communications should be protected, and
encryption is the backbone of the solution that will secure sensitive
electronic transmissions over insecure channels. In the context of policy
development for digital signatures, it is particularly not to confuse the
roles of certificate authorities and key recovery infrastructure. Any such
blurring of functions will seriously curtail the growth of electronic
commerce and the trust of users in this technology.

USACM believes that the best way to promote rapid development of superior
and reliable technology is by ensuring open and collaborative efforts
between government agencies and private industry.  We commend the Commerce
Department's present initiative to invite the participation of the private
business and academic sectors in this forum.

Introduction

The present initiative to call the "Public Forum on Certificate Authorities
and Digital Signatures: Enhancing Global Electronic Commerce" is timely and
necessary.  There is much work to be done in formulating a policy on the
use of digital signatures and certificate authorities, a policy that the
Commerce Department realizes has wide-reaching, fundamental implications,
as evidenced by the broad themes sketched in the call for comments.  To
begin with, it is important to have a clear understanding of the
terminology involved in discussing a public key infrastructure.  In
particular, for the purposes of this forum, it is important to define
clearly the role of "digital signatures" and "certificate authorities" in a
public key infrastructure, and we will begin our comments by doing so.
Beyond defining these terms, we will focus our comments on the
technological challenges of certificate authorities and digital signatures,
and on user expectations and requirements.  These are issues 3 and 4 in the
call for comments, which, for reference, may be found at:
http://csrc.nist.gov/events/pfcadsegec.html.

We begin our comments by defining the functional role of digital
signatures and certificate authorities in a public key infrastructure.
Next, we discuss a technological concern about the performance of an
infrastructure that would couple the implementations of certificate
authorities and a key recovery system.  We then discuss our concerns about
user expectations in this area.  Also, we briefly discuss the recent
significant international interest in the field.  Finally, we present a
summary of our recommendations.

It is our conclusion that private signature keys should not be
deposited with a key recovery agent not under the direct control of the
key owner.  For this reason, we recommend that the public key
infrastructure should decouple any implementation of a key recovery system
from the role conventionally associated with CAs.  We also recommend that
the Department explore means to protect consumers from the fraudulent use
of keys.  We also
believe that the Department should look specifically at the question of how
to apply the OECD privacy guidelines to the development of digital
signature and certification authority services.

The Role of Digital Signatures and Certificate Authorities

In a public key infrastructure, digital signature technology is used to
ensure sender authentication and message integrity in electronic
communications, and certificate authorities are an essential supporting
feature in the infrastructure.  In the following discussion, an "owner" of
a key is defined to be the individual or organization that wishes to create
a digital signature that can withstand legal challenge, and to whom the key
belongs.

A public key infrastructure implementing digital signatures uses two keys:
one (called the private key) known only to the owner and the other (the
public key) which is disclosed to the public. For the system to be secure,
the private key must be computationally impossible to deduce from the
public key.  Therefore, only one party knows the private key, and knowledge
of the public key by a third party does not compromise the legal standing
of a signature created with the private key.  It is important to emphasize
that in a world of electronic commerce with transactions depending upon
legally valid digital signatures, it is crucial that only the signing party
know and have access to the private key.

The protocol for the transmission of "signed" electronic document, D, from
Alice to Bob would work as follows.  Alice creates a hash (a message digest
uniquely associated with a particular documents), H, of her document including
its signature (using, for example, something like NIST's SHA).  She then runs H
through the digital signature process (digitally signs the hash with her
private key), and sends both the output from the process, O, and the document
with its signature to Bob. Bob establishes sender authentication and message
integrity by creating H for himself (the same way Alice did, by hashing the
signed document) and then compares H with the result of unwrapping O with
Alice's
public key.  The result of the unwrapping, if all is well, is identical to H.
Because only a person with access to Alice's secret private key could have
created the signature, and only Alice's public key can verify its
authenticity,
Bob is convinced that the signature is authentic and also that the content of
the letter has not been altered.

To trust such a protocol, and in particular, to give it strength against
potential legal challenges, users need to be assured that the public key
published by Alice is indeed her own.  This certification is provided by
CAs.  CAs provide this service in the following way.  Alice submits
documents to a CA establishing her legal identity.  Alice also submits a
public key to the CA.  Once the CA is satisfied that Alice is who she
purports to be, it links her public key with her identity in the CA's
database.  When called upon by Bob to provide a certificate binding Alice's
identity and her public key, the CA sends the certificate electronically,
signing its electronic transmission with its (the CA's) private key.  Bob
can then verify the source of the certificate with the CA's public key, and
hence have confidence in its authenticity.  CAs, then, perform the role of
a notary public combined with a directory, providing certified copies of
certificates which contain and assure an identity-key binding. The
recipient of the certificates, Bob in our example, can thus establish with
high confidence that the public key he receives is truly Alice's.

Technological Challenges

An implementation of a public key infrastructure must be technologically
reliable, and to be acceptable to a broad user base, must also be
cost-effective.  At the same time, when an implementation creates
significant privacy risks, it must be built in a way that addresses and
resolves, or at least minimizes these risks.  We discuss in this section
how these reliability, risk and cost variables must be juggled with some
care in the context of a possible role envisaged for CAs by a recent FBI
suggestion.

In his testimony before the Senate Judiciary Committee on July 9, FBI
director Louis Freeh suggested, in a move that would combine the role
conventionally associated with CAs with that of key recovery agents, that
certificate authorities should be required to keep copies of their
customers' private keys.  USACM believes that this would be problematic
both because it creates risks that are unsupportable in a public key
infrastructure, and because it would handicap the growth and efficiency of
the infrastructure.

Discussions on key recovery often blur the distinction between recovery of
signature keys, and recovery of encryption keys.  USACM believes that this
distinction is important and should be emphasized in all key recovery
discussions.  Encryption keys are used to keep conversations and documents
confidential;  a stolen encryption key allows eavesdropping and the reading
of confidential documents.  Signature keys are used for sender
authentication;  stolen signature keys enable impersonation of the key
owners.  If private signature keys were stolen, this would compromise the
legal standing of the digital signature process.  There is, therefore,
every legal justification against depositing private signature keys with a
key recovery agent not under the direct control of the key owner.  If a
copy of the private key database fell into the wrong hands, impersonators
would be able to assume any cyber-identity, forge signatures, and
compromise the legal standing of the infrastructure.  This could be
catastrophic.  USACM suggests that the world of electronic commerce and an
electronic transactions environment cannot withstand such risks: CA's must
not be allowed to store private signature keys.  Private signature keys
must be in the sole custody and responsibility of the individual or
organization that generated them.

Quite apart from this fundamental concern, under a suggestion such as
Freeh's, to prevent a catastrophe CAs would be forced to assume an enormous
responsibility, since they would be the safekeepers of all private keys.
USACM is concerned that this responsibility could handicap the growth of
the public key infrastructure.  CAs are too crucial a component of the
public key infrastructure to be slowed down with extra cost and regulation
forcing them to adopt key recovery.  Even if an argument can be made that
key recovery is good, forcing CAs to be key recovery agents has very clear
economic downsides.  Under the FBI suggestion, all certificate authorities
would be required to be licensed.  Consumers would be free to use whatever
encryption they wanted, but if they wanted to patronize the CA they would
be forced to turn over a copy of their private key.  Consumers would thus
be required to choose between the risks of giving their keys to their CA,
and living without the security of a certificate.  Since CA's are the
backbone of a public key infrastructure supporting electronic commerce,
consumers would consider it an indispensable service.  Forcing the extra
security precautions associated with a key recovery implementation onto CAs
would unnecessarily handicap their traditional and crucial role, and hence
adversely affect the growth of the public key infrastructure.

User Expectations

This section focusses on the expectations of the users of a public key
infrastructure.  We focus our comments on the role of policy makers in
protecting the consumers of digital signature technology and CAs from
fraudulent, unauthorized use of keys.  We also discuss the need for the
creation of safeguards to protect users' privacy needs.

(1) Consumer Protection

Besides the need for a government policy that respects the need for
confidentiality, integrity, and authenticity of transactions, USACM
recognizes the need for an infrastructure that would protect consumers from
fraudulent transactions.  There is one issue in particular that we would
like to flag in this connection:  limiting individual consumers' exposure
to fraudulent loss through the use of digital signatures for consumer
transactions.  As we move into the world of electronic commerce, we might
want to relearn (or rather, preempt relearning) a lesson we learnt with
credit cards.  The credit card system was set up so that a consumer would
be held liable for any transactions made with her card, even in cases of
fraudulent, unauthorized use.  Many a person suffered grievously under that
set-up, until it was changed by legislation.  Under a public key
infrastructure, provisions must be made to protect individual consumers
from such fraud.  If a key owner loses a key, that consumer must not remain
liable for unauthorized transactions made by the person fraudulently
holding the key.  Note that in this regard, if private signature keys
are compromised when in the possession of any third party, there should
be no personal liability. Further, centralized private signature key
repositories would raise the possibility of mass fraud.  The larger a
signature key database that is compromised, the broader the potential for
its fraudulent use.

(2) Privacy

Quite aside from the central intent of a public key infrastructure (i.e., to
establish and certify relationships among keys and the identities of
individuals or organizations), the very existence and operation of the PKI
raises very troublesome privacy issues.  Of specific concern is that of
unauthorized uses of personal-certificate and transaction-generated
information, and in particular, the sale of aggregate personal profiles.
USACM believes that strong privacy protections must be reflected in a
government policy regarding the development of a public key infrastructure.

In the process of establishing identity of an individual with the strong
confidence essential for a certificate process, personal information such
as addresses, dates-of-birth, social security numbers, etc, will likely
have been provided to CAs.  Such a collection of data will automatically
become an attractive target of opportunity for exploitation in unrelated
(to PKI) ways.  In fact, such secondary use for other purposes (such as
sales of profiles to direct marketing organizations) might even compromise
the integrity of the central purpose of a CA organization or its
certificates.  This problem would be particularly severe, even magnified, if
there were to be only a small number of centralized key databases.

In any CA, the database is bound to contain personal information on
individuals and it will therefore also become a target for subversion and
penetration by crackers, internal employees, and other malicious attackers.
In the event that such databases were to be compromised, vast amounts of
personal data could well be put up for sale, or used to the disadvantage of
individuals or class of individuals. Such potential events would be a
serious infringement of personal privacy.

We note that CAs for valid operational reasons (including fiduciary
responsibilities levied by law) will probably keep audit data indicating to
whom each individual certificate will have been provided.  Hence, the
database will also acquire a trail of activity coupled to an individual or
organization.  The depth of detail in such records will be even more
complete if every consumer is required to have a single key for all
electronic transactions.

We point out that one does not have a single physical key for all physical
locks; similarly, one should not require there be a single electronic key
for all electronic affairs.  Having multiple keys would act to minimize,
but not completely eliminate, the risk that derivative personal information
that has been aggregated from multiple transactions would lead to an even
more comprehensive personal profile.  If there allowed to happen because
the government policy permitted or were silent on the point, the database
would become an ever more attractive opportunity for subversion and/or
exploitation for profit-oriented sales and/or access by federal, state or
local agencies (for example, law enforcement authorities, tax authorities,
judicial authorities, other enforcement authorities) and/or access by
private organizations (e.g., trial attorneys, insurance companies,
healthcare providers).  Such latent risks are especially threatening if
transactions are not anonymous.

The USACM stresses that such collateral considerations, such as the privacy
risks that we have just identified, must be considering in setting the
permissible boundary of operations and legally established protections
of CA organizations.

An International Perspective

We note that the Organization for Economic Cooperation and Development
(OECD) recently completed a proposed framework for cryptography policy
which addressed several issues now under consideration by the Department of
Commerce.  In considering whether countries should promote lawful access to
encryption keys, the OECD said that it was important to consider "the risks
of misuse, the additional expense of any supporting infrastructure, the
prospects of technical failure, and other costs." We believe that this is a
sensible warning.  As Dr. Peter Neumann noted before the Senate Judiciary
committee on July 9, 1997: "The real costs that must underlie any extensive
key-retrieval mechanisms and recovery infrastructures are a serious source
of concern. To date, those costs have not been adequately considered by
proponents of key-recovery, key-escrow, and key-management mechanisms and
their supporting computer- communication environments. The costs in the
large necessarily involve the entire key-recovery infrastructure itself,
including its operational procedures, management, oversight, enforcement
costs, legal liabilities, and costs of litigating misuse."

The OECD further recommended that privacy safeguards be established for
cryptographic products and services.  As the OECD noted: "Cryptographic
methods can be a valuable tool for the protection of privacy, including
both the confidentiality of data and communications and the protection of
the identity of individuals.  Cryptographic methods also offer new
opportunities to minimize the collection of personal data, by enabling
secure but anonymous payments, transactions and interactions.  At the same
time, cryptographic methods to ensure the integrity of data in electronic
transactions raise privacy implications.  These implications, which include
the collection of personal data and the creation of systems for personal
identification, should be considered and explained, and, where appropriate,
privacy safeguards should be established."

Recommendations

We suggest to the Department that it is important to have a clear
understanding of the terminology involved in discussing a public key
infrastructure;  in particular, it is important to define clearly the role
of "digital signatures" and "certificate authorities" in the world of
electronic commerce.  It is also important to recognize the different
implications of implementing key recovery for signature keys versus
encryption keys.  We believe that there is every legal justification
against depositing private signature keys with a key recovery agent not
under the direct control of the key owner.  We recommend that the public
key infrastructure should decouple any implementation of a key recovery
system from the role conventionally associated with CAs.  We also recommend
that the Department consider initiatives to protect consumers from the
fraudulent use of keys, and to prevent infringements of individual privacy
through the aggregation and sale of private information.  In particular, we
believe that the Department should look specifically at the question of how
to apply the OECD privacy guidelines to the development of digital
signature and certification authority services.

Sincerely,

Dr. Barbara Simons, Chair
USACM

---

The Association for Computing is an international professional society
whose 76,000 members (60,000 in the U.S.) represent a critical mass of
computer scientists in education, industry, and government. USACM was
created by ACM to provide a means for promoting dialogue on technology
policy issues with U.S. policy makers and the general public. USACM
responds to requests for information and technical expertise from U.S.
government agencies and departments, seeks to influence relevant U.S.
government policies on behalf of the computing community and the public,
and provides information to ACM on relevant U.S. government activities.
USACM also identifies significant technical and public policy issues and
brings them to the attention of the general public.  We provide a
World-Wide-Web site located at http://www.acm.org/usacm/ to educate our
members and the public on information technology issues. At the site, we
make available government documents, reports, policy statements, and links
to other science policy resources. The site includes information on
encryption policy.

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009035854/http://www.somewhere.com/)