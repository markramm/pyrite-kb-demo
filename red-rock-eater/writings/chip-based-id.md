---
id: chip-based-id
title: chip-based ID
type: writing
writing_type: rre-post
date: 1997-09-06
url: http://commons.somewhere.com:80/rre/1997/chip-based.ID.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - forwarded-content
  - government-info
  - privacy
  - surveillance
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/chip-based.ID.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009062605/http://www.somewhere.com/)

  

# chip-based ID

```
[A web version of this paper with hyperlinks to numerous resources can
be found at http://www.anu.edu.au/people/Roger.Clarke/DV/IDCards97.html
My apologies for the garbled bits toward the end of this ASCII version.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Sat, 6 Sep 1997 12:46:18 +1000
From: Roger Clarke <Roger.Clarke@anu.edu.au>

Chip-Based ID:  Promise and Peril

Roger Clarke 
Roger.Clarke@anu.edu.au
Principal, http://www.ozemail.com.au/~ecommrce/Roger.Clarke/Xamax
Consultancy Pty Ltd, Canberra
Visiting Fellow, http://cs.anu.edu.au/Department of Computer Science,
http://www.anu.edu.auAustralian National University

Version of 6 September 1997
=A9  Xamax Consultancy Pty Ltd, 1997

Invited Address to a Workshop on 'Identity cards, with or without
microprocessors:  Efficiency versus confidentiality', at the
http://www.confpriv.qc.caInternational Conference on Privacy, Montreal,
23-26 September 1997

This paper is at http://www.anu.edu.au/people/Roger.Clarke/DV/IDCards97.html

Abstract

Multi-purpose identification schemes in general, and national identification
schemes in particular, represent the most substantial of information
technologies' threats to individual liberties.

This is because they concentrate information, and hence power; and because
it is simply inevitable that, at some stage, even in the most apparently
stable and free nations, power will be exercised against the interests of
individuals, and of the public generally.

Miniaturised computer processors (chips), mounted in such carriers as
'credit-cards', coins, rings and watches, are an important tool.  They are
now entering widespread use as a means for identifying inert objects such as
goods on a production-line and in a logistics-chain, and living things such
as valuable animals.

Chips are being proposed as a means of identifying people as well. 
They present an opportunity to devise and implement highly repressive
identification schemes; and many corporations and countries are in the
process of harnessing those potentials.

Chips also offer great scope for designing schemes that are
privacy-sensitive, and that balance privacy interests against other social
and economic interests and law and order concerns.  Unfortunately, that
scope has to date been almost entirely overlooked or ignored.  This paper
argues that the simplistic approaches being adopted by the proponents of
identification schemes are in the process of destroying public confidence,
and hence of undermining the intended return on investment.  This paper
builds on the author's substantial prior research and publications in the
area.  It reviews the social and political risks involved in identification
schemes.  It then identifies ways in which chip-cards may be applied
to address those risks, and achieve balance between the interests of
individuals, on the one hand, and of the society and State, on the other.

Privacy-sensitive design options include:
-	'electronic signature cards' rather than 'id cards';
-	no central storage of biometrics;
-	two-way device authentication;
-	less identity authentication, and more eligibility authentication;
-	fewer identified transaction trails, and more anonymity and
pseudonymity;
-	multiple single-purpose ids, rather than multi-purpose ids;
-	separation between zones within multi-function chips;  and
-	role-ids as well as person-ids.

Public concerns about privacy-invasive and repressive applications of
information technology must be reflected not only in the designs implemented
by scheme operators, but also in policies implemented by governments.  It is
argued that the focus on 'data protection' that has been adopted during the
period 1970-1995 needs to be rapidly matured into a new orientation towards
protection of the interests of people.

Insensitive application of intrusive information technologies (including
consumer and citizen profiling, matching and linkage among personal
databases, video-surveillance, intelligent highways, as well as chip-based
identification) is resulting in heightened public concern about the exercise
of control over individuals by governments and corporations.

Failure to appreciate the intensity of public concerns, to adapt to it,
and to apply chip technologies in privacy-enhancing ways, will result in
further cleavage between people and their institutions.  This will result in
decreased compliance by people with schemes about which they are justifiably
suspicious, and failure of chip-based and related technologies to deliver on
their potential.

Contents

Introduction
Human Identification
Identification, Anonymity and Pseudonymity
The Assault on Anonymity
Dataveillance Risks
Threats in Chip-Based Schemes
Threats in Multi-Purpose Identification Schemes
Threats in Chip-Based Multi-Purpose Identification Schemes
Public Policy Options for Chip-Based ID Schemes
Design Options for Chip-Based ID Schemes
Conclusions
References to Other People's Works
References to the Author's Own Works

 Introduction

This paper is concerned with:
-	the technology of miniaturised integrated circuits (chips);
-	the identification of humans in information systems;  and
-	the use of chips to support human identification.

Chip technology has been improving for a quarter-century, and can now support
moderate storage-capacity and processing power.  Chips are now capable of
being hosted in plastic cards, coin-sized tokens and watches, and in goods,
and the cartons and pallets whereby goods are delivered.  Chip-cards are now
being issued in considerable numbers, particularly in public transport and
stored-value applications.  For a positive perspective on such schemes, see
Clarke (1997c).  In many circumstances, it is useful, and even necessary, to
identify people.

Many different identification techniques are used, including appearance,
social behaviour, names, codes, knowledge, tokens, bio-dynamics, natural
physiography and imposed physical characteristics.

Chips are capable of being used as a form of enhanced token.  They may be
embedded in a carrier such as a plastic card, a watch, a ring, a bracelet,
or an anklet.  ID chips are already being directly implanted in animals,
commonly in the ear or the neck of valuable ones like pets and breeding
stock.  It is unlikely to be long before embedded chips are seriously
proposed as a means of identifying humans.

This section firstly provides some examples of the application of chip-based
ID to humans, and then explains the purpose and structure of the paper.- South Korea

  Building on the present national photo-id card, the Korean ID Card Project
  involves a chip-based ID card for every adult member of the population.  It
  is to include scanned fingerprints, and is intended to support the functions
  of a multi-purpose identifier, proof of residence, a driver's licence, and
  the national pension card.  Its impact is reviewed in Kim (1997).- Malaysia

    Malaysia's Multimedia Super Corridor (MSC) initiative features a number of
    'flagship' applications.  One of these is a 'National MultiPurpose Card'
    (MPC), which is to be a chip-based multi-purpose identification card, with
    specific support for driving licence, immigration status, and health data.
    It is expected that its uses will be extended to other electronic government
    projects.  Of particular significance for other countries is the voluntary
    and gratis participation in the initial phases of the MPC project of most of
    the world's major smart card technology developers.  They would appear to
    perceive great advantages to themselves in being involved in the first of
    what they hope will be a wave of such implementations, throughout at least
    Asia.- Thailand

      Chip-based technology is bound to be attractive to government agencies that
      already have substantial databases, in countries whose population is already
      subject to id schemes.  Thailand is an example of a market ripe for the
      plucking.

      "The Thai Ministry of Interior maintains the second-largest relational
      database in the world ...  In conjunction with the Central Population
      Database project, the Ministry of Interior introduced a new identity
      card issuing project in early 1994 ...  An image of the person's right
      thumbprint is scanned and stored in the national database at the time of
      card creation. The card contains printed biographical information and an
      identification photograph on the front side, and a magnetic strip containing
      biographical information and a reference to the person's thumbprint on the
      back side" (technology-provider LSC Inc.'s promotional material).- Warm Water and the Frog

        It is conventional for intrusive, dehumanising technologies (such as genetic
        testing, genetic manipulation and eugenics) to be first harnessed in contexts
        that are economically beneficial, and difficult to resist.  The popular
        metaphors for this process are 'the thin end of the wedge', and the frog
        placed in warm water that is gradually heated to boiling point.

        The initial applications of chip-based ID in Anglo-American and European
        countries appear likely to be to institutionalised people, who are expensive
        to administer, and whose human rights are in any case subject to greater than
        usual qualifications.  The most obvious examples are:

        -	prisoners, particularly those who are being granted a degree of
        freedom, such as relatively open 'prison farms', and day-release schemes; and
        -	senile dementia patients, whose movements within a retirement home
        can be tracked, and whose non-movement in an unusual location can be reported
        to carers.

        People afflicted by the slow processes of other institutions may be readily
        attracted to voluntarily participate in such schemes.  Since 1995, the
        Immigration and Naturalisation Service Passenger Accelerated Service System
        (INSPASS), based on a card bearing a measure of the holder's hand-geometry,
        has been in use at New York's International Airports as a means of expediting
        the clearance of frequent travellers.

        The official information available on INSPASS does not appear to even mention
        privacy matters.  Indeed, the challenge is seen as merely "How then do we
        balance the needs of enforcement; the prompt identification and denial of
        entry to persons we, as a nation, do not want to allow into our country,
        with the needs of facilitation; the prompt admission of those we want to
        welcome?".  The scheme is justified with the hilariously incorrect statement
        that "In the past, the right of travel was only paid lip service in most
        countries.  Only recently, with the convergence of democratic trends around
        the world and the advent of relatively cheap international air travel, have
        people been able to exercise the right to travel" (Ronald J. Hays, 4 January
        1996).

        Immigration officials in other countries, many of them with the same
        cavalier, even imperious, attitude of their U.S. equivalents, are understood
        to be trialling similar technologies.- The (Suspended?) British Project

          Comprehensive chip-based ID schemes are not restricted to Asian countries.
          The United Kingdom differs significantly from its Continental European
          partners in that it does not have a general-purpose ID card.  The
          Conservative Government spent some years developing a proposal for a
          chip-based scheme, but this was abandoned by the recently-elected Labour
          Government.  The primary impulse for the scheme came from within the ranks
          of the civil service; so it will doubtless re-appear as a Labour initiative,
          once the new Government becomes tired and begins to depend on civil servants
          for ideas.- The (Emergent?) U.S. Project

            Driver licensing authorities can generally see little benefit in upgrading
            their existing cards to chip-based technology.  On the other hand, such
            a development can be readily harnessed to multiple purposes.  According
            to The Winds (1997), the U.S. Illegal Immigration Reform and Immigration
            Responsibility Act of 1996 contained an obscure passage amending Title IV,
            section 656(b) in order to convert state drivers' licences into a national ID
            card.  Comprehensive information on this matter is to befound in the National
            ID Archives of the Electronic Privacy Information Centre.- The Plan of This Paper

              To what extent does a chip-based ID scheme represent merely a confirmatory
              identification method, with limited privacy-invasiveness, and to what extent
              is it a basis for comprehensive surveillance, and for authoritarian rather
              than democratic society?

              This paper first reviews the notions of identification, anonymity and
              pseudonymity, and the threats that identified data and transactions
              represent to individuals and to societies.  This leads into an assessment
              of multi-purpose identification and inhabitant registration schemes.

              Chips are shown to create opportunities for designers, such that
              chip-based ID schemes can deny privacy outright, or can be implemented
              in a privacy-sensitive and even privacy-protective manner.  An assessment
              is undertaken of the likelihood of public concern forcing governments and
              designers to be extremely careful with this society-threatening technology.
              Specific proposals are provided, in relation to both public policy and
              technical design.

              Human Identification

              Human identification is the association of data with a particular human being
              (Clarke 1994c).  It is used in relation to historical data held on files, and
              to new transaction data that captures aspects of real-world events.

              A number of bases are available to assist in formal identification.  None of
              them satisfies all of the desirable characteristics.  Organisations therefore
              combine identification techniques in order to achieve an appropriate balance
              between the harm arising from false-inclusions (i.e. associating data with
              the wrong person), and from false-exclusions (i.e. failing to associate data
              with the right person).

              An approach that is commonly adopted when an organisation first establishes
              a relationship with a person, is to seek a variety of information about
              them, from a variety of sources.  In the absence of inconsistencies or 'bad'
              references, the person is accepted as being identified by that loose set of
              data.

              To facilitate identification during subsequent interactions between the
              organisation and the individual, a token (typically a card) is issued to the
              individual.  To engender sufficient confidence in the person's identity, an
              organisation may seek not only production of the token, but also of knowledge
              that only the individual would be expected to have, such as a password or
              'personal identification number' (PIN).

              Dependence on documents, tokens and knowledge produce a system of at best
              moderate reliability.  With developments in technology, some organisations
              are increasingly attracted to biometrics.  This is the identification of an
              individual through a measure of some part of their person, or of something
              that the person does.

              Identification, Anonymity and Pseudonymity

              There are some kinds of transactions that cannot reasonably be performed
              without the disclosure, verification and recording of the parties'
              identities.  This is usefully referred to as 'identity authentication'.
              An important class of circumstances in which identity authentication is
              needed is where an undertaking is given by a person to perform some action
              in the future, e.g. repaying a loan; or appearing in court, in return for
              the granting of bail.

              There are further kinds of transactions in which one party wishes to satisfy
              themselves as to the appropriateness of the other party participating in that
              particular class of interaction (e.g. by virtue of their age, affiliation,
              authority to represent a particular organisation, or qualification for a
              concession).  One convenient way to perform such 'eligibility authentication'
              is for one party to provide evidence of identity, but for the other to
              record no more than that satisfactory evidence was provided (e.g. recording
              'driver's licence sighted', rather than the licence-number).  A special case
              of this is where a person collects a privacy-sensitive document (such as
              medical information), or a token intended to serve as evidence of identity
              (such as a passport).

              Anonymous data is data that cannot be associated with a particular person.
              There is a vast range of transactions for which identification is not a
              logical prerequisite.  These include cash payments of all kinds, barter
              transactions, telephone and counter enquiries, and inspection of publications
              on library premises.

              Depending on the context, identification may assist in protecting the
              interests of one or both of the parties, or of third parties, or of society
              as a whole.  It also threatens the identified party, for reasons summarised
              in the following section.  Anonymity satisfies the interests of individuals
              in avoiding the accumulation of data-holdings by others about them; but may
              compromise interests of other parties.

              An alternative exists, that represents a compromise between the extremes
              of identification and anonymity.  A pseudonym is an identifier for a party
              to a transaction, which is not, in the normal course of events, sufficient
              to associate the transaction with a particular human being.  The data may,
              however, be indirectly associated with the person, if particular procedures
              are followed.

              The simplest (although by no means the only) way to implement a pseudonymous
              scheme is to maintain an index that correlates the pseudo-identifier
              with a reliable identifer for the person, and to subject it to technical,
              organisational and legal protections.  Hence individuals may be, in practical
              terms, anonymous, except where circumstances justify access to the index,
              e.g. where a search warrant is issued to a law enforcement agency.

              The principles of pseudonymity are reasonably well-known, yet they have
              been remarkably under-applied.  Clarke 1995c examines the technique and its
              importance as a means of achieving balance between conflicting interests.

              The Assault on Anonymity

              There already exist large numbers of data trails that individuals leave
              behind them; and new technologies are resulting in new trails being created
              (Clarke 1995d).

              During much of the current century, organisations have been seeking to
              reduce the costs involved in the administration of their relationships
              with individuals, by replacing the human touch with automation.  This has
              resulted in an incentive for greater 'data intensity' in those relationships
              (Rule 1974).

              Organisations are seeking to exploit the ongoing technological revolutions,
              and are trying to convert hitherto anonymous transactions into identified
              ones.  Examples include:
              -	the conversion of anonymous cash into identified credit-card,
              debit-card and stored-value-card transactions;
              -	the application of Calling Number Display (CND) / Calling-Line
              Identification (CLI) in telephony, in order to identify (initially) the
              area and even location from which a call is made, and (progressively) the
              identity of the individual making the call;
              -	loyalty schemes to identify all transactions each individual has
              with a particular organisation;  and
              -	extended 'loyalty' schemes, to identify the intensive stream of
              transactions each individual has with a range of organisations.

              Government agencies are frequently in a position to legally impose on
              individuals the condition that they identify themselves when performing
              particular kinds of transactions.  Corporations may use a combination of
              inducements and market power to achieve the same end.

              Dataveillance Risks

              Dataveillance is the systematic use of personal data systems in the
              investigation or monitoring of the actions or communications of one or more
              persons.  Personal surveillance is the surveillance of an identified person.
              Mass surveillance is the surveillance of groups of people, usually large
              groups, generally so as to identify individuals who belong to some particular
              class of interest to the surveillance organization, or perhaps to repress
              their behaviour.

              Organisations acquire power over individuals through the accumulation of
              data about them.  They can enhance that power by drawing data from multiple
              sources.  Individuals are generally incapable of withstanding the pressure,
              and of enforcing correction of erroneous data, mistaken judgements and
              unreasonable decisions.

              At the level of society as a whole, further serious problems arise, as
              a climate of suspicion prevails, and individual self-determination and
              diversity are strangled by the 'chilling effect' of omnipresent monitoring.
              The threats of dataveillance to privacy are well-documented (e.g. Clarke
              1988), and are not further examined here.

              Threats in Chip-Based Schemes

              Chip-cards are capable of being applied to a great many purposes.  This
              section provides a brief scan of the privacy implications of several of them.
              Additional analyses are to be found in the N.S.W. Privacy Committee's 'Smart
              Cards: Big Brother's Little Helpers' (1995); and in Privacy International's
              archives on Identity Cards.

              An assessment of the privacy issues in the retail financial sector Clarke
              (1996d) identified the following major concerns:- greatly increased intensity of transaction trails ('whereas your
                credit-card and debit-card generated a trail of 5-10 transactions per
                month, or perhaps per week, your smart card can enable the recording of
                where you are and what you are doing 5-10 times per day');- exploitation of the transaction trails:
                  -	by government agencies, which represents oppressive use of the
                  State's power over individuals;  and
                  -	by consumer marketing corporations to better target prospects for
                  their goods and services;- the risk of 'function creep', i.e. extension to additional
                    functions;  and- 'proof of identity' concerns, particularly:
                      -	the need for 'proof of identity' in relation to the acquisition or
                      use of a card;  and
                      -	the use of a smart card as multi-purpose 'proof of identity'.

                      Beyond their applications in financial services, cards and their associated
                      databases can provide evidence of identity and of affiliation.  The risks
                      have been dramatised, although not unduly exaggerated, using the catchcry
                      "Is your Jew-bit set?", and "Let your card 'out' your homosexuality for you!".
                      Beyond the well-known examples such as the fate of Jews in The Netherlands
                      at the time of the Nazi invasion, recent press reports suggested that racial
                      information associated with the national id card was used in distingushing
                      people's tribal association during the Ruanda massacres.

                      Two further applications of chips are of great significance.  The first of
                      these is as a means of carrying the cryptographic keys that are very likely
                      to be used by people in the near future to encrypt messages, and to digitally
                      sign electronic documents.  There is a serious risk that one maverick nation,
                      the United States, may continue its unrealistic, Cold War-era stance, and
                      seek the ability to intrude into individuals' private keys.

                      In any case, digital signatures, and the key certification authority
                      mechanism to support them, generate a range of privacy implications.  These
                      are examined in Greenleaf & Clarke (1997).

                      Another application of a chip is to carry a biometric, i.e. a measure of some
                      part of a person such as a fingerprint, or the geometry of a hand, finger,
                      or thumb; or of some pattern of the person's behaviour, such as the dynamics
                      of signature-writing or password-typing.  The bio metric can then be used to
                      test whether the person presenting the card is likely to be the same as the
                      person to whom it was issued.  It could also be used as a means of unlocking
                      the encryption keys stored on the same chip.  Biometrics are for many people
                      highly intrusive and threatening.  Depending on how they are applied, they
                      could not just seem that way, but be that way.

                      Threats in Multi-Purpose Identification Schemes

                      Many identification schemes are used by a single organisation, for a single
                      purpose;  but there are obvious attractions in sharing the costs across
                      multiple organisations and business functions.

                      A special case of a multi-purpose id scheme is what is usefully described
                      as an inhabitant registration scheme'.  This provides everyone in a country
                      with a unique code, and a token (generally a card) containing the code.  It
                      is typically used for the administration of taxation, national superannuation
                      and health insurance.  In some countries, is is used for additional purposes,
                      such as the administration of social welfare and banking, and to ensure that
                      particular rights are exercised only by people entitled to them, such as the
                      exercise of voting rights, the right of residence, the right to work, the
                      right of movement across the country's borders, and the right of movement
                      within the country.

                      Inhabitant registration schemes are endured, and perhaps even welcomed, by
                      the inhabitants of some countries;  but are disliked, actively opposed, and
                      undermined in many others.

                      Privacy-related protections vary from very little to moderately strong; but
                      the very existence of such a scheme represents a threat against which mere
                      'data protection' or 'fair information practices' arrangements are almost
                      an irrelevance.  The public policy aspects of schemes of this nature are
                      discussed in (Clarke 1992), and at Clarke (1994c).
                      To create a surveillance society, three conditions need to be fulfilled:
                      1.	there needs to be a range of personal data systems, each processing
                      data for specific purposes;
                      2.	personal data systems must be connected via one or more
                      telecommunications networks;  and
                      3.	the data must be identified consistently.

                      The first two have been satisfied during the last two decades, as a result
                      of the application of information technology.  The third is accordingly
                      the critical technical factor inhibiting the achievement of a surveillance
                      society.  Inhabitant registration schemes overcome that hurdle (Clarke 1988).

                      Threats in Chip-Based Multi-Purpose Identification Schemes

                      It can be no surprise that the application of chips to comprehensive,
                      multi-purpose ID schemes results in a compounding of the privacy threats
                      that arise from each of them.

                      An assessment is to be found in Davies (1996), especially at pp. 75-133,
                      161-175.  The book is reviewed at Clarke (1996e).

                      In Clarke (1994c), the conclusion was reached that:

                      Any high-integrity identifier represents a threat to civil liberties, because
                      it represents the basis for a ubiquitous identification scheme, and such a
                      scheme provides enormous power over the populace. All human behaviour would
                      become transparent to the State, and the scope for non-conformism and dissent
                      would be muted to the point envisaged by the anti-utopian novellists.

                      The highest-integrity schemes combine physically intrusive data-collection
                      with a potentially ubiquitous instrument of power. As a result, the kinds
                      of multi-purpose identification schemes, or inhabitant registration systems,
                      which would appear capable of exciting the greatest degree of concern are
                      those based on DNA-printing and implanted chips.

                      Jeremy Bentham's 1791 conception of the 'panopticon' depended on line
                      of sight, visual surveillance, by prison warders, from a high tower.
                      Foucault's twentieth century image of modern society as prison is associated
                      with dataveillance rather than visual surveillance methods (Foucault 1977).
                      The creator of the chip-card recognised at the time, in 1974, that the
                      most central element of the 'virtual panopticon' is the enforced, computer-
                      readable, real-time monitorable identifying chip.

                      Public Policy Options for Chip-Based ID Schemes

                      General policy considerations are addressed in Clarke (1996d).
                      These encompass:
                      -	awareness and education;
                      -	public participation, through impact statements, consultation, and
                      direct involvement in the design;
                      -	access to anonymous or pseudonymous schemes;
                      -	measures to encourage pseudonymous schemes;
                      -	justification for personal data collection and retention;
                      -	equitable terms and conditions of usage;  and
                      -	comprehensive privacy laws, going beyond mere 'data protection'
                      and 'fair information practices' legislation.  Relevant documents include
                      the EU Directive, and the Australian Privacy Charter.  Inadequacies in
                      one country's protective regime are examined in detail in Clarke (1997b).

                      It is readily argued that governments are captives of business interests,
                      and that social interests will therefore necessarily capitulate to economic
                      interests.  On the other hand, public concerns in many countries are a
                      considerable political force.  A substantial example of community impact on
                      policy in Australia is documented in Clarke (1987).

                      Overviews of community attitudes in that country are provided at Clarke
                      (1996b), and in Clarke (1997a).  Similarly high levels of concern exist
                      in many other countries.  In Clarke (1996b), it is argued that the public's
                      increasing wariness of the power that IT offers organisations is resulting in
                      increasingly clear demands for greatly enhanced privacy protections.  There
                      are many signs of imminent change.  Organisations that are slow to appreciate
                      these new realities risk suffering the consequences; whereas those that move
                      proactively to gain a competitive or strategic advantage from their privacy
                      stance, will reap the benefits.

                      Design Options for Chip-Based ID Schemes

                      From the analysis conducted in this paper, it would seem inevitable that
                      chip-based ID schemes threaten privacy, and that a direct conflict exists
                      between the deployment of chips in ID cards and the survival of the kinds
                      of relatively free and democratic society that advanced nations aspire to.

                      Because of their programmability, however, chips are very flexible
                      instruments.  They offer such a wide scope to the scheme designer that they
                      can in fact be applied with several alternative effects:
                      -	to destroy privacy, at one extreme;
                      -	to protect privacy, at the other;  or
                      -	to achieve balance between the privacy interest, and other
                      interests of individuals, of groups, of corporations and government
                      agencies, and of societies as a whole.

                      The following are particular design features that need to be adopted by the
                      sponsors of schemes that apply chip technology to identification-related
                      purposes:
                      -	private keys used for both encryption and for digital signatures
                      may be stored on a personal card, but never in a central store.  This is
                      sometimes referred to as an 'electronic signature card' rather than an 'id
                      card';
                      -	the control of individuals' biometrics must be in the hands of the
                      individuals, not the State.  Hence biometrics may be stored on the relevant
                      person's card, and in backup arrangements under the individual's control,
                      but no central storage of biometrics must be permitted to develop;
                      -	schemes must feature two-way device authentication, i.e. personal
                      chips must verify the authenticity of devices that seek to transact with
                      it, and must not merely respond to challenges by devices;
                      -	identity authentication must be restricted to circumstances in
                      which it is justified by the impossibility of alternatives.  Much greater
                      application must be made of eligibility authentication;
                      -	identified transaction trails must be restricted to circumstances
                      in which they is justified by the impossibility of alternatives.  Anonymity
                      must be sustained except where it is demonstrably inadequate.  Much greater
                      application must be made of pseudonymity through protected indexes;
                      -	the myth of people having only a singular identification must be
                      demolished, and multiple single-purpose ids implemented rather than a few
                      multi-purpose ids;
                      -	a particular application of the 'multiple ids' principle that is of
                      great importance is the maintenance of separation between zones within
                      multi-function chips, in order to assure the integrity of each application,
                      and protect against unauthorised sharing of data and ids;
                      -	another important application of the 'multiple ids' principle is
                      the implementation of role-ids as well as person-ids, to enable multiple
                      individuals to perform particular organisational functions, over a period
                      of time, and even at the same time.

                      Conclusions

                      Chip-based ID embodies the most serious perils for free and democratic
                      societies.  One scenario is direct conflict between the power of governments
                      and government agencies, supported by corporations, on the one hand, and, on
                      the other, a populace that is unprepared to go meekly to the slaughter.

                      But the technology also holds promise.  As a result, an alternative scenario
                      exists, in which chips are applied in a manner that balances the interests
                      of the State and of corporations against those of individuals.  This will
                      fail to achieve the nirvana of a controlled and efficiently-run society, with
                      individuals treated as goods, and behaving in a manner no less predictable
                      than livestock; but in return it will sustain humanity.

                      The time for choice between those two scenarios is not remote.  It is now.

                      References to Other People's Works
                      Bentham J. (1791) 'Panopticon; or, the Inspection House', London, 1791
                      Davies S. (1992) 'Big Brother: Australia's Growing Web of Surveillance'
                      Simon & Schuster, Sydney, 1992
                      Davies S. (1996)  'Monitor:  Extinguishing Privacy on the Information
                      Superhighway', Pan Macmillan Australia, 1996
                      EPIC (1995-)  'National ID Cards', Electronic Privacy Information Center,
                      Washington DC, at
                      http://www.epic.org/privacy/idcards/default.htmlhttp://www.epic.org/privacy/id
                      cards/default.html
                      Foucault M. (1977) 'Discipline and Punish: The Birth of the Prison'
                      Peregrine, London, 1975, trans. 1977
                      Kim J. (1997)  'Digitized Personal Information and the Crisis of Privacy:
                      The Problems of Electronic National Identification Card Project and Land
                      Registry Project in South Korea', at
                      http://kpd.sing-kr.org/idcard/joohoan2.htmlhttp://kpd.sing-kr.org/idcard/joohoan
                      2.html
                      NSWPC (1995)  'Smart Cards:  Big Brother's Little Helpers', The Privacy
                      Committee of New South Wales, No.66, August 1995, at
                      http://www.austlii.edu.au/au/other/privacy/smart/http://www.austlii.edu.au/au/ot
                      her/privacy/smart/
                      Privacy International (1996)  'Privacy International's FAQ on Identity
                      Cards'', at
                      http://www.privacy.org/pi/activities/idcard/http://www.privacy.org/pi/activities
                      /idcard/
                      Rule J.B. (1974) 'Private Lives and Public Surveillance: Social Control in
                      the Computer Age' Schocken Books, 1974
                      The Winds (1997)  'The future has arrived'  (June 1997), at
                      http://www.thewinds.org/archive/government/idcard6-97.htmlhttp://www.thewinds.or
                      g/archive/government/idcard6-97.html

                      References to the Author's Own Works
                      Clarke R. (1987)  'Just Another Piece of Plastic for Your Wallet:  The
                      Australia Card'  Prometheus  5,1  June 1987  Republished in Computers &
                      Society  18,1  (January 1988), with an Addendum in Computers & Society
                      18,3  (July 1988).  At http://www.anu.edu.au/people/Roger.Clarke/DV/OzCard.htmlhttp://www.anu.edu.au/people/Roger.Clarke/DV/OzCard.html
                      Clarke
                      R. (1988) 'Information Technology and Dataveillance', Commun. ACM 31,5 (May
                      1988). Republished in C. Dunlop and R. Kling (Eds.), 'Controversies in
                      Computing', Academic Press, 1991, at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/CACM88.htmlhttp://www.anu.edu.au/pe
                      ople/Roger.Clarke/DV/CACM88.html
                      Clarke R. (1992)  'The Resistible Rise of the National Personal Data
                      System'  Software Law Journal 5,1 (January 1992) , at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/SLJ.htmlhttp://www.anu.edu.au/peopl
                      e/Roger.Clarke/DV/SLJ.html
                      Clarke R. (1993a)  'Why the Public Is Scared of the Public Sector', IIR
                      Conference paper February 1993.  Abstract at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/AbstractPubSector.htmlhttp://www.an
                      u.edu.au/people/Roger.Clarke/DV/AbstractPubSector.html
                      Clarke R. (1993b)  'Profiling:  A Hidden Challenge to the Regulation of
                      Data Surveillance', Journal of Law and Information Science 4,2 (December
                      1993), at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/PaperProfiling.htmlhttp://www.anu.e
                      du.au/people/Roger.Clarke/DV/PaperProfiling.html.  . A shorter version was
                      published as 'Profiling and Its Privacy Implications' Australasian Privacy
                      Law & Policy Reporter 1,6 (November 1994), at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/AbstractProfiling.htmlhttp://www.an
                      u.edu.au/people/Roger.Clarke/DV/AbstractProfiling.html
                      Clarke R.A. (1994a) 'The Digital Persona and Its Application to Data
                      Surveillance' The Information Society 10,2 (June 1994), at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/DigPersona.htmlhttp://www.anu.edu.a
                      u/people/Roger.Clarke/DV/DigPersona.html
                      Clarke R. (1994b)  'Information Technology:  Weapon of Authoritarianism or
                      Tool of Democracy?'  Proc. World Congress, Int'l Fed. of Info. Processing,
                      Hamburg, September 1994.  At
                      http://www.anu.edu.au/people/Roger.Clarke/DV/PaperAuthism.htmlhttp://www.anu=2Eedu
                      =2Eau/people/Roger.Clarke/DV/PaperAuthism.html
                      Clarke R. (1994c)  'Human Identification in Information Systems:
                      Management Challenges and Public Policy Issues'  Information Technology &
                      People 7,4 (December 1994) 6-37, at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/HumanID.htmlhttp://www.anu.edu.au/p
                      eople/Roger.Clarke/DV/HumanID.html
                      Clarke R. (1994d)  'Dataveillance by Governments:  The Technique of
                      Computer Matching'  Information Technology & People  7,2  (December 1994).
                      Abstract at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/AbstractMatchIntro.htmlhttp://www.a
                      nu.edu.au/people/Roger.Clarke/DV/AbstractMatchIntro.html
                      Clarke R. (1995a)  'Computer Matching by Government Agencies:  The Failure
                      of Cost/Benefit Analysis as a Control Mechanism'  Informatization and the
                      Public Sector  (March 1995).  At
                      http://www.anu.edu.au/people/Roger.Clarke/DV/MatchCBA.htmlhttp://www.anu.edu=2Eau/
                      people/Roger.Clarke/DV/MatchCBA.html
                      Clarke R. (1995b)  'A Normative Regulatory Framework for Computer Matching'
                      Journal of Computer and Information Law XIII,4 (Summer 1995) 585-633.
                      Abstract at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/AbstractMatchReg.htmlhttp://www=2Eanu
                      =2Eedu.au/people/Roger.Clarke/DV/AbstractMatchReg.html
                      Clarke R. (1995c)  'When Do They Need to Know 'Whodunnit?':  The
                      Justification for Transaction Identification;  The Scope for Transaction
                      Anonymity and Pseudonymity'  Proc. Conf. Computers, Freedom & Privacy, San
                      Francisco, 31 March 1995.  At
                      http://www.anu.edu.au/people/Roger.Clarke/DV/PaperCFP95.htmlhttp://www.anu.edu.a
                      u/people/Roger.Clarke/DV/PaperCFP95.html.  Revised version published as
                      'Transaction Anonymity and Pseudonymity' Privacy Law & Policy Reporter 2, 5
                      (June/July 1995) 88-90.  Condensed paper published as 'Identification,
                      Anonymity and Pseudonymity in Consumer Transactions:  A Vital Systems
                      Design and Public Policy Issue', October 1996, at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/AnonPsPol.htmlhttp://www.anu.edu.au
                      /people/Roger.Clarke/DV/AnonPsPol.html
                      Clarke R. (1995d) 'Trails in the Sand', at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/Trails.htmlhttp://www.anu.edu.au/pe
                      ople/Roger.Clarke/DV/Trails.html
                      Clarke R. (1996a)  'Smart move by the smart card industry:  The Smart Card
                      Industry's Code of Conduct'
                      http://lexsun.law.uts.edu.au/~graham/PLPR_guide.htmlPrivacy Law & Policy
                      Reporter  2, 10  (January 1996)  189-191, 195.  At
                      http://www.anu.edu.au/people/Roger.Clarke/DV/SMSC.htmlhttp://www.anu.edu.au/peop
                      le/Roger.Clarke/DV/SMSC.html
                      Clarke R. (1996b) 'Privacy and Dataveillance, and Organisational Strategy',
                      EDPAC Conference Paper (May 1996), at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/PStrat.htmlhttp://www.anu.edu.au/pe
                      ople/Roger.Clarke/DV/PStrat.html
                      Clarke R. (1996c)  'Data Transmission Security, or Cryptography in Plain
                      Text'Privacy Law & Policy Reporter 3, 2 (May 1996), pp. 24-27 , at
                      http://www.anu.edu.au/people/Roger.Clarke/II/CryptoSecy.htmlhttp://www.anu.edu.a
                      u/people/Roger.Clarke/II/CryptoSecy.html
                      Clarke R. (1996d)  'Privacy Issues in Smart Card Applications in the Retail
                      Financial Sector', in http://acff.com.au/sm_cards.html'Smart Cards and the
                      Future of Your Money', Australian Commission for the Future, June 1996,
                      pp.157-184.  At
                      http://www.anu.edu.au/people/Roger.Clarke/DV/ACFF.htmlhttp://www.anu.edu.au/peop
                      le/Roger.Clarke/DV/ACFF.html
                      Clarke R. (1996e)  'The Information Infrastructure is a Super Eye-Way:
                      Book Review of Simon Davies' 'Monitor'' Privacy Law & Policy Reporter 3, 5
                      (August 1996), at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/Monitor.htmlhttp://www.anu.edu.au/p
                      eople/Roger.Clarke/DV/Monitor.html
                      Clarke R. (1997a)  'What Do People Really Think?  MasterCard's Survey of
                      the Australian Public's Attitudes to Privacy', Privacy Law & Policy Report
                      3,9 (January 1997), at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/MCardSurvey.htmlhttp://www.anu.edu.
                      au/people/Roger.Clarke/DV/MCardSurvey.html
                      Clarke R. (1997b)  'Flaws in the Glass; Gashes in the Fabric:  Deficiencies
                      in the Australian Privacy-Protective Regime', Invited Address to Symposium
                      on 'The New Privacy Laws', Sydney, 19 February 1997 , at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/Flaws.htmlhttp://www.anu.edu.au/peo
                      ple/Roger.Clarke/DV/Flaws.html
                      Clarke R. (1997c)  'Smart Cards in Banking and Finance'  The Australian
                      Banker 111,2 (April 1997), at
                      http://www.anu.edu.au/people/Roger.Clarke/EC/SCBF.htmlhttp://www.anu.edu.au/peop
                      le/Roger.Clarke/EC/SCBF.html
                      Clarke R. (1997d)  'Privacy and 'Public Registers'', Proc. IIR Conference
                      on Data Protection and Privacy, Sydney, 12-13 May 1997, at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/PublicRegisters.htmlhttp://www.anu.
                      edu.au/people/Roger.Clarke/DV/PublicRegisters.html
                      Greenleaf G.W. & Clarke R. (1997)  'Privacy Implications of Digital
                      Signatures', IBC Conference on Digital Signatures, Sydney, 12 March 1997,
                      at
                      http://www.anu.edu.au/people/Roger.Clarke/DV/DigSig.htmlhttp://www.anu.edu.au/pe
                      ople/Roger.Clarke/DV/DigSig.html
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009062605/http://www.somewhere.com/)