---
id: switching-costs
title: "Switching Costs"
type: concept
tags:
- platform-economics
- monopoly
- lock-in
- antitrust
- digital-rights
importance: 7
metadata:
  first_appeared: "Economics terminology predating Doctorow; he uses and extends it extensively from the late 2010s onward"
  key_writings: &id001
  - the-internet-con
  - pluralistic-blog
  - enshittification-talk-defcon
  - chokepoint-capitalism-book
  related_concepts: &id002
  - enshittification
  - adversarial-interoperability
  - platform-decay-cycle
  - competitive-compatibility
  - interoperability-mandates
  - digital-rights-management-critique
  coined_by: "Economics literature (Klemperer and others); Doctorow popularizes and extends the concept in platform contexts"
first_appeared: "Economics terminology predating Doctorow; he uses and extends it extensively from the late 2010s onward"
key_writings: *id001
related_concepts: *id002
coined_by: "Economics literature (Klemperer and others); Doctorow popularizes and extends the concept in platform contexts"
---

Switching costs are the costs — financial, social, technical, and psychological — that a user incurs when moving from one product, service, or platform to another. In standard economic usage, switching costs include things like contract termination fees, time spent learning a new system, and lost functionality from incompatible data formats. Cory Doctorow's use of the concept extends this to encompass the deliberately engineered lock-in that characterizes dominant digital platforms.

## Standard Economic Definition

In industrial organization economics, switching costs explain why competitive markets may not efficiently discipline incumbent firms: even if a competitor offers a better product, users may not switch if the cost of switching exceeds the benefit of the superior product. High switching costs give incumbents pricing power — they can raise prices or reduce quality up to the level of the switching cost without losing users.

This analysis predates Doctorow significantly; economists like Paul Klemperer developed formal models of switching costs in the 1980s and 1990s. The concept is also central to network effects analysis: in a network with high switching costs, the dominant platform's advantage compounds over time.

## Doctorow's Extension: Engineered Lock-In

Doctorow's contribution is to emphasize that switching costs on digital platforms are not merely a natural feature of network effects but are **actively engineered** by incumbents using legal and technical tools. This is the crucial political-economic move: it converts switching costs from a structural inevitability into a policy choice that can be reversed.

The engineered switching costs he identifies include:

- **Social graph lock-in**: Your friends and professional contacts are on the platform, and you cannot port that relationship data to a competitor. This is not technically inevitable — it is a consequence of the platform refusing to implement [[adversarial-interoperability]] for social connections.

- **Content and history lock-in**: Messages, posts, photos, documents accumulated on the platform are in proprietary formats or inaccessible through export tools. Data portability, while required in some jurisdictions under laws like GDPR, is often implemented in ways that are technically useless (you can download your data but cannot import it to a competing service in a usable form).

- **DRM-induced lock-in**: Ebooks, music, and video purchased from platform stores are locked to that store through [[digital-rights-management-critique|DRM]], meaning switching platforms means abandoning purchased content. This is legally enforced self-help IP, not a natural feature of digital goods.

- **Complementary investments**: Users have learned the platform's interface, workflows, and idiosyncrasies. This is natural switching cost, but platforms actively increase it by avoiding standard interfaces and making their UX deliberately non-transferable.

- **Ecosystem lock-in**: Hardware, software, and services within a platform ecosystem are designed to work better together and to work worse with alternatives (Apple/Google ecosystems are canonical examples).

## The Role of [[adversarial-interoperability]]

Doctorow's core argument is that historically, switching costs were much lower because [[adversarial-interoperability]] and [[competitive-compatibility]] were possible. A competitor could build a tool that read your data from the incumbent, imported your social connections, and let you switch without losing your accumulated investment. This is how many historical technology transitions worked — email clients compete on the same mailbox; office suites compete on the same file formats.

The suppression of adversarial interoperability by incumbents — through DMCA, CFAA, terms of service, API closures, and technical barriers — is the mechanism by which switching costs have been artificially inflated to their current levels.

## Policy Implications

If switching costs are engineered rather than natural, they can be unengineered through policy:

- **[[interoperability-mandates]]** force incumbents to expose interfaces that allow users to take their data and connections to competitors
- **Data portability requirements** ensure users can export their data in formats that competing services can actually use (not just technically download)
- **Anti-blocking rules** prevent incumbents from technically interfering with third-party interoperability tools

These interventions do not require breaking up platforms — they change the structural incentives by making exit credible, which in turn disciplines incumbent behavior. Doctorow argues this is preferable to behavioral regulation (which tells platforms what to do) because it empowers market discipline rather than regulatory micromanagement.

## In Doctorow's Broader Framework

Switching costs are the fulcrum of [[enshittification]]: the subsidy-then-extraction sequence only works if users are locked in by the time the extraction phase begins. Without high switching costs, the degraded platform simply loses users to competitors. With high switching costs, degradation can proceed well past the point that would cause exit in a competitive market.

[[chokepoint-capitalism-book]] applies the same logic to creators: publishers, streaming services, and ticketing monopolies extract from creators precisely because switching costs for those creators (losing their audience, their contracts, their distribution channels) are engineered to be prohibitive.
