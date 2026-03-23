---
id: self-help-ip
title: "Self-Help IP"
type: concept
tags:
- intellectual-property
- digital-rights
- drm
- platform-power
- legal-critique
links:
- target: security-theater
  relation: related_to
  note: 'DRM is security theater: it imposes costs on legitimate users while failing to stop determined adversaries, with its stated purpose as performative cover'
  kb: schneier
importance: 6
metadata:
  first_appeared: "Developed across EFF advocacy and pluralistic-blog; most clearly articulated in discussions of DRM and the DMCA"
  key_writings: &id001
  - pluralistic-blog
  - information-doesnt-want-to-be-free
  - the-internet-con
  related_concepts: &id002
  - digital-rights-management-critique
  - right-to-repair
  - adversarial-interoperability
  - switching-costs
  - chokepoint-capitalism
  coined_by: "Legal scholars have used related terminology; Doctorow popularizes the concept in this specific form"
first_appeared: "Developed across EFF advocacy and pluralistic-blog; most clearly articulated in discussions of DRM and the DMCA"
key_writings: *id001
related_concepts: *id002
coined_by: "Legal scholars have used related terminology; Doctorow popularizes the concept in this specific form"
---

Self-help IP refers to the practice by which corporations use technical measures — particularly digital rights management and software locks — to enforce intellectual property claims unilaterally and continuously, without resorting to courts, against users who have not necessarily violated any law. Cory Doctorow uses the concept to critique a fundamental shift in how intellectual property is enforced: from occasional, contested litigation to ambient, automated technical control embedded in products.

## The Traditional IP Model

Traditional intellectual property law is enforced through litigation: a rights holder who believes their copyright, patent, or trademark has been infringed brings a legal action, a court adjudicates the claim with procedural safeguards, and a remedy is ordered. The process is slow, expensive, and uncertain for both parties. Users have due process protections. Overbroad claims can be contested.

## The Self-Help Alternative

Self-help IP replaces the legal process with a technical one. Rather than suing users who copy, modify, or resell, rights holders embed technical restrictions in products that physically prevent the disfavored action. DRM on an ebook prevents copying without any court involvement. Serialized parts on a smartphone physically prevent unauthorized repair. Software locks prevent a purchased tractor from running with third-party parts.

The critical feature is that these restrictions are enforced **preemptively and unconditionally**: they apply to all users, including those whose actions would be entirely legal. A user who purchases a DRM-protected ebook and then loses the service that authenticates their access loses their book — not because a court found them guilty of infringement but because a technical system operated unilaterally by the rights holder withdrew access. See [[digital-rights-management-critique]].

## Legal Enablement

Self-help IP is not merely a technical choice — it is legally enabled by statutes that make circumventing technical protection measures illegal. In the US, Section 1201 of the DMCA makes it illegal to "circumvent a technological measure that effectively controls access to a copyrighted work," regardless of whether the underlying use is infringing. This means that:

- A user who bypasses DRM to make a legitimate personal backup commits a federal offense
- A researcher who circumvents software locks to study security vulnerabilities may be liable
- An independent repair technician who bypasses a parts-pairing lock to install a genuine replacement part may violate the law

The DMCA thus converts technical self-help measures into legally-backed enforcement tools. The rights holder does not need to prove infringement — circumventing the lock is itself the offense.

## Doctorow's Critique

Doctorow's argument, developed extensively on [[pluralistic-blog]] and in the context of [[right-to-repair]] advocacy, is that self-help IP has fundamentally changed the relationship between manufacturers and owners. When you buy a device, you have received a physical object but the manufacturer retains ongoing control through the software — and has made that ongoing control legally enforceable.

This produces what he calls a "feudal" property relationship: the nominal owner of the device does not have the full bundle of rights historically associated with ownership (use, repair, modify, resell) because the manufacturer has used self-help IP mechanisms to retain effective control over those rights.

The concept connects to [[chokepoint-capitalism]]: self-help IP is one of the tools by which manufacturers install themselves as unavoidable intermediaries even after the sale transaction is complete. A tractor that only runs with manufacturer-authorized parts creates a captive aftermarket not through contractual obligation but through technical compulsion.

## Relationship to [[free-software-foundation]]

The [[free-software-foundation]]'s critique of proprietary software overlaps significantly with the self-help IP analysis. Richard Stallman's argument that proprietary software gives manufacturers "unjust power" over users is a precursor to Doctorow's more legal-systemic framing. Doctorow bridges the free software tradition and the digital rights / antitrust tradition, situating self-help IP as both a technical and a political-economic problem.

## Countermeasures

Doctorow's preferred remedies for self-help IP include [[right-to-repair]] legislation, DMCA Section 1201 reform, and [[interoperability-mandates]] — measures that collectively strip away the legal protection that converts technical locks into enforceable restrictions.
