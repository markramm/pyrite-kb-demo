---
id: nsa
title: "National Security Agency"
type: organization
importance: 9
tags:
- surveillance
- signals-intelligence
- crypto-wars
- Snowden
- government
- SIGINT
org_type: government-agency
founded: "1952"
location: "Fort Meade, Maryland"
url: "https://www.nsa.gov"
---

The National Security Agency (NSA) is the U.S. government's primary signals intelligence and cryptanalysis organization. It is simultaneously one of the world's most capable cryptographic institutions and Schneier's most important adversary in policy debates — the agency whose programs, capabilities, and institutional overreach have motivated much of his public policy work across the [[cryptography-era]], [[trust-and-surveillance-era]], and [[systems-subversion-era]].

## NSA and the Crypto Wars

During the [[crypto-wars-export-controls]] battles of the 1990s, NSA was the primary institutional force defending government control over civilian cryptography. Its preferred solution — the [[clipper-chip-announcement]] — was a hardware encryption system with built-in key escrow, designed to give law enforcement access to all encrypted communications. Schneier's opposition to Clipper was technical as well as political: key escrow is a cryptographic weakness, and NSA's track record in proposing standards designed for government access (the DES key length reduction, the later Dual EC DRBG case) demonstrated that its standardization interests were not aligned with civilian security interests.

NSA's relationship to open cryptographic standards has been consistently complicated. The agency employs more cryptographers than any other institution in the world, and its classified expertise is genuinely substantial. But its institutional interest in maintaining intelligence collection capabilities creates systematic incentives to weaken civilian cryptographic standards in ways that are not disclosed. Schneier's [[schneiers-law]] — that security requires open analysis, not trusted authority — applies directly to NSA's role in standards bodies.

## NSA and NIST

NSA participates in [[nist]]'s cryptographic standardization processes, and the relationship between the two agencies has been a source of concern throughout Schneier's career. The most egregious documented example was the Dual EC DRBG backdoor: NSA influenced NIST to standardize a random number generator containing a secret backdoor, then paid RSA Security to deploy it widely. The [[snowden-revelations]] confirmed what Schneier and colleagues had suspected in 2007 when they published their analysis of the algorithm's suspicious structure.

This episode confirmed Schneier's long-standing argument that security claims from NSA-adjacent processes cannot be trusted without independent analysis, and that the institutional structure of U.S. cryptographic standardization creates systematic vulnerabilities.

## Mass Surveillance Programs

The [[snowden-revelations]] revealed the full scope of NSA's surveillance programs: bulk collection of telephony metadata, direct access to data from major technology companies through PRISM, tapping of internet backbone cables through Upstream programs, and active subversion of encryption systems and commercial products through Tailored Access Operations. For Schneier, the most significant revelation was not any individual program but the strategic orientation: NSA had systematically weakened the cryptographic and security infrastructure of the internet in pursuit of surveillance access, making everyone's security weaker in order to make everyone's communications accessible.

This finding drove the [[trust-and-surveillance-era]] analysis of [[data-and-goliath]] and [[click-here-to-kill-everybody]], and it anchors the broader [[systems-subversion-era]] argument of [[a-hackers-mind]]: NSA's surveillance programs are an instance of [[hacking-as-systems-subversion]] at institutional scale — a powerful actor exploiting the rules and infrastructure of a shared system to serve its own interests at the expense of everyone who depends on that infrastructure's integrity.

## Policy Adversary

Schneier has testified before Congress, participated in policy forums, and written extensively about NSA oversight and reform. His position is not that NSA should not exist or that signals intelligence is illegitimate, but that NSA's programs as revealed operated with insufficient legal authority, democratic accountability, and respect for the civil liberties of both Americans and non-Americans. The oversight mechanisms — FISA courts, congressional intelligence committees — had failed to constrain NSA's most aggressive programs.

The relationship between Schneier and NSA is thus structural as much as personal: he is one of the most capable public analysts of NSA's capabilities and programs, operating without the institutional constraints that prevent insiders from publishing, and his analytical framework — developed through decades of security research and policy engagement — is specifically suited to identifying the structural vulnerabilities in surveillance oversight that NSA has exploited.
