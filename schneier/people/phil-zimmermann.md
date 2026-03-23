---
id: phil-zimmermann
title: "Phil Zimmermann"
type: person
tags:
- cypherpunk
- cryptography
- crypto-wars
- digital-rights
- pgp
importance: 8
role: "Creator of PGP (Pretty Good Privacy), cryptographer, digital rights activist"
affiliations:
- electronic-frontier-foundation
research_status: draft
---

Phil Zimmermann (b. 1954) is the creator of PGP (Pretty Good Privacy), the email encryption software whose 1991 release made strong public-key cryptography available to ordinary people for the first time. His subsequent criminal investigation by the US government — for allegedly "exporting munitions" by posting PGP on the internet — became the defining legal drama of the [[crypto-wars-export-controls]] and the human face of the policy debates that Schneier engaged throughout the 1990s.

## PGP and the Democratization of Encryption

Zimmermann built PGP in 1991 specifically as a civil liberties tool: he feared that legislation requiring government access to communications was imminent, and he wanted to get strong encryption into public hands before the window closed. PGP combined RSA public-key cryptography (developed by Rivest, Shamir, and Adleman) with symmetric encryption in a hybrid system that was practical for ordinary users. It also used a "web of trust" model rather than centralized certificate authorities — a design choice that reflected deep distrust of institutional key management.

This was the same distrust that animated the cypherpunk movement Zimmermann was part of, alongside [[tim-may]], [[eric-hughes]], and [[john-gilmore]]. Where Schneier approached cryptography primarily as a technical discipline, Zimmermann approached it as direct political action. The two framings were complementary: Schneier provided the technical depth and analytical frameworks in [[applied-cryptography]]; Zimmermann demonstrated what was at stake by becoming a defendant.

## The Criminal Investigation

After PGP spread globally via the internet, US Customs opened a criminal investigation into Zimmermann for unlicensed export of munitions — cryptographic software was classified as a weapon under ITAR (International Traffic in Arms Regulations). The investigation ran from 1993 to 1996, when the government dropped it without explanation. During those years Zimmermann became the most visible symbol of the absurdity of the [[crypto-wars-export-controls]]: the source code had been physically published as a book (which was protected speech under the First Amendment), and anyone with a scanner could have reconstructed the "munition."

The [[electronic-frontier-foundation]] and the broader civil liberties community rallied around Zimmermann, and the case gave concrete human stakes to arguments that otherwise risked seeming abstract. Schneier's writing during this period — particularly the technical arguments in [[applied-cryptography]] — provided the substrate that advocates like Zimmermann needed: if export controls on cryptography were purely performative (since any determined adversary could implement the algorithms themselves), then the restrictions only burdened innocent users.

## Relationship to Schneier's Intellectual Project

Zimmermann and Schneier occupy adjacent but distinct positions in the crypto community. Zimmermann is a builder and activist; Schneier is an analyst and writer. Where Zimmermann's contribution was creating and deploying a technology, Schneier's was explaining the landscape in which such technologies operated — the threat models, the policy tradeoffs, the sociology of security. [[secrets-and-lies]] represents Schneier's pivot away from the purely technical frame that PGP exemplifies: cryptography is a tool, but security is a system, and tools alone don't make systems secure.

Zimmermann's career after PGP — including work on ZRTP (encrypted voice over IP) and his role at Silent Circle — continued the pattern of building practical cryptographic tools for ordinary users, a mission aligned with the access-to-security values that Schneier has championed in his [[schneier-on-security-blog]] and policy advocacy. Both figures represent the position that strong civilian cryptography is a public good, not a national security threat — a position that proved correct when the [[snowden-revelations]] confirmed that mass surveillance had proceeded exactly as the Crypto Wars critics feared.
