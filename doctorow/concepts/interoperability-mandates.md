---
id: interoperability-mandates
title: "Interoperability Mandates"
type: concept
tags:
- platform-regulation
- antitrust
- digital-rights
- policy
- interoperability
importance: 8
metadata:
  first_appeared: "Developed in EFF advocacy and pluralistic-blog; central argument of The Internet Con (2023)"
  key_writings: &id001
  - the-internet-con
  - pluralistic-blog
  - enshittification-talk-defcon
  related_concepts: &id002
  - adversarial-interoperability
  - competitive-compatibility
  - enshittification
  - switching-costs
  - digital-rights-management-critique
  - end-to-end-principle
  coined_by: "Policy terminology predating Doctorow; he is a leading proponent and has shaped the advocacy framing"
first_appeared: "Developed in EFF advocacy and pluralistic-blog; central argument of The Internet Con (2023)"
key_writings: *id001
related_concepts: *id002
coined_by: "Policy terminology predating Doctorow; he is a leading proponent and has shaped the advocacy framing"
---

Interoperability mandates are regulatory requirements that dominant platforms or technology providers expose interfaces, protocols, or data portability mechanisms that allow competing services and users' own tools to interoperate with the incumbent's platform — without requiring the incumbent's permission and on terms the incumbent cannot unilaterally control. Cory Doctorow's 2023 book [[the-internet-con]] is structured as an extended argument for interoperability mandates as the primary policy lever for breaking up platform monopolies.

## The Core Argument

Doctorow's case for interoperability mandates rests on several linked claims:

1. **Platform lock-in is engineered, not natural.** The high [[switching-costs]] on platforms like Facebook, Google, and Amazon are not an inherent feature of network effects but a deliberate policy achievement — incumbents have used legal and technical tools to suppress [[adversarial-interoperability]] and [[competitive-compatibility]] that would otherwise allow users to leave.

2. **Structural remedies outperform behavioral ones.** Breaking up platforms (structural separation) is politically difficult and may simply recreate the problem in smaller units. Content moderation rules and privacy regulations tell platforms what they must do but leave underlying monopoly power intact. Interoperability mandates change the structural incentives: if users can always leave, platforms must compete on quality rather than lock-in.

3. **Interoperability enables market competition to discipline platforms.** If a user dissatisfied with Facebook can move to Mastodon while still messaging their Facebook-using friends, Facebook faces competitive pressure it currently does not face. If an Audible customer can take their audiobook library to a competing service, Audible must offer good terms. Mandated interoperability restores the disciplining force of exit.

## Forms of Interoperability Mandates

Doctorow and related advocates distinguish several types:

- **Data portability mandates**: Users can export their data in machine-readable formats (already partially implemented in GDPR's Article 20 and some state laws)
- **API access mandates**: Third-party services can query the platform's data with user permission, enabling bridge tools and alternative clients
- **Protocol mandates**: Platforms must implement open protocols (like ActivityPub for social media, or email protocols) that allow federated competition
- **No-blocking rules**: Platforms cannot technically block interoperation by third parties who are not themselves causing harm

## The Internet Con's Argument

[[the-internet-con]] is Doctorow's most sustained treatment of interoperability mandates. The book explicitly argues against the view that the internet's current dysfunction is primarily a story of bad people making bad decisions at tech companies. Instead, Doctorow attributes platform decay ([[enshittification]]) to the structural conditions created by monopoly power and the suppression of interoperability. The remedies must therefore be structural.

The book is also notable for engaging with counterarguments: critics argue that interoperability mandates could harm privacy (forcing platforms to expose user data to third parties), security (creating new attack surfaces), or children's safety (allowing tools that bypass parental controls). Doctorow takes these concerns seriously but argues they can be addressed through design — interoperability can be conditioned on user consent, third parties can be held to conduct standards, and safety rules can apply to interoperating services.

## Legislative Context

The EU's Digital Markets Act (2022) includes interoperability requirements for "gatekeeper" platforms, requiring them to open messaging services (relevant to WhatsApp, iMessage). The proposed ACCESS Act in the US Congress was an earlier attempt at a broader interoperability mandate. [[lina-khan]]'s FTC and [[tim-wu]]'s White House role under Biden both engaged with interoperability as a competition tool. Doctorow's advocacy has contributed to placing interoperability on the policy agenda in both jurisdictions.

## Relationship to [[electronic-frontier-foundation]]

The EFF has been a consistent advocate for interoperability, and Doctorow's tenure there shaped the organization's emphasis on this issue. The EFF's technical and legal staff have contributed analysis of how specific legal barriers — the DMCA, CFAA, trade secret law — would need to change to enable robust adversarial interoperability even absent formal mandates.
