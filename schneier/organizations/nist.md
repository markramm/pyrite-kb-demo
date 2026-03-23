---
id: nist
title: "National Institute of Standards and Technology"
type: organization
importance: 8
tags:
- standards
- cryptography
- AES
- government
- NIST
org_type: government-agency
founded: "1901"
location: "Gaithersburg, Maryland"
url: "https://www.nist.gov"
---

The National Institute of Standards and Technology (NIST) is the U.S. federal agency responsible for developing and maintaining technical standards, including cryptographic standards. It is the government body most directly relevant to Schneier's technical work: NIST ran the [[aes-competition]] in which Schneier's [[twofish-algorithm]] was a finalist, and NIST's cryptographic standards have been both collaborative resources and contested terrain in Schneier's analysis of the relationship between government and cryptographic security.

## The AES Competition

NIST's decision to run the AES competition as an open, international, transparent evaluation was consequential for the cryptographic community and for Schneier specifically. The competition model — publish all candidate algorithms, invite public cryptanalysis, and select based on merit in an open process — was consistent with Schneier's principle (articulated throughout [[applied-cryptography]] and formalized as [[schneiers-law]]) that cryptographic confidence can only be established through sustained public analysis.

Schneier's Twofish team engaged fully with the competition process: they published detailed design rationales, documented their security arguments, and actively participated in the community analysis of other candidates. The [[aes-competition]] was the most rigorous public evaluation of Schneier's technical cryptographic work, and NIST's management of it represented the kind of open standards process Schneier consistently advocated.

## NIST and NSA

NIST's relationship with [[nsa]] has been a recurring complication in Schneier's analysis of cryptographic standards. The NSA, as the U.S. signals intelligence agency, participates in NIST's cryptographic standardization processes and has historically influenced standard selections in ways that were not always transparent.

The most significant instance was the Dual Elliptic Curve Deterministic Random Bit Generator (Dual EC DRBG): a NIST-standardized random number generator that Schneier and others (notably Dan Shumow and [[niels-ferguson]]) flagged in 2007 as potentially containing a backdoor. The [[snowden-revelations]] confirmed in 2013 that NSA had deliberately introduced the backdoor and had paid RSA Security $10 million to make Dual EC DRBG the default in its products. This was a direct corruption of the NIST standards process and a validation of the concerns Schneier had raised six years earlier.

## Post-Snowden Standards Work

The Dual EC DRBG revelation prompted NIST to formally withdraw the standard and to undertake a public review of its cryptographic standards processes. Schneier participated in the public comment period and wrote extensively about what the episode revealed: that the open standards process could be corrupted from within by an agency with the resources, access, and institutional authority of the NSA.

This episode illustrates the tension in Schneier's assessment of NIST: the agency is responsible for the open evaluation model he values (the AES competition) and simultaneously demonstrated capable of participating in the subversion of that model (Dual EC DRBG). The tension is not a contradiction but a structural feature of the relationship between government technical agencies and the intelligence community that Schneier analyzes throughout his [[trust-and-surveillance-era]] and [[systems-subversion-era]] work.
