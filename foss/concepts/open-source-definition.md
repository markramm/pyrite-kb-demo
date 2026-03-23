---
id: open-source-definition
title: "The Open Source Definition"
type: concept
importance: 7
concept_type: principle
first_appeared: "osi-founding-1998"
key_writings:
- open-sources-anthology-1999
- free-software-free-society-2002
related_concepts:
- four-freedoms
- copyleft
- forking-as-governance
tags:
- open-source-definition
- osi
- licensing
- certification
- perens
- debian
research_status: draft
---

The Open Source Definition (OSD) is the set of criteria the [[open-source-initiative]] uses to certify licenses as "open source." It was adapted by [[bruce-perens]] from the Debian Free Software Guidelines (DFSG), which Perens had drafted in 1996 while serving as project leader of the [[debian-project]]. The adaptation occurred in the weeks following the [[foresight-open-source-meeting-1998]] and the [[osi-founding-1998]], when the newly formed OSI needed a principled standard for the term "open source" that [[christine-peterson]] had coined. The DFSG provided that standard ready-made: it had already been tested against real licensing decisions within Debian's package inclusion process.

The OSD contains ten criteria. (1) Free redistribution: the license cannot restrict anyone from selling or giving away the software. (2) Source code: the program must include source code or provide a well-publicized means of obtaining it. (3) Derived works: the license must allow modifications and derived works, and must allow them to be distributed under the same terms. (4) Integrity of the author's source code: the license may require that modified versions carry a different name or version number, preserving the distinction between original and derivative. (5) No discrimination against persons or groups. (6) No discrimination against fields of endeavor: the license cannot restrict use to non-commercial contexts or exclude specific industries. (7) Distribution of license: the rights attached to the program must apply to all to whom it is redistributed, without requiring a separate license agreement. (8) License must not be specific to a product: the rights cannot depend on the program being part of a particular software distribution. (9) License must not restrict other software: the license cannot impose conditions on other software distributed alongside it. (10) License must be technology-neutral: no provision may be predicated on any individual technology or style of interface.

The OSD differs from the [[four-freedoms]] in character and intent. The four freedoms are ethical principles: they define what users deserve as a matter of justice. The OSD is a practical certification standard: it defines what criteria a license must meet to earn the "open source" label. In practice, the two frameworks approve nearly the same set of licenses — a license that satisfies the four freedoms will almost always pass the OSD, and vice versa. The divergence is in framing. The four freedoms ground the free software movement's claim that users have rights that software producers must respect. The OSD grounds the open source movement's claim that open development practices require specific licensing conditions. This difference in philosophical orientation is the core of [[software-freedom-vs-open-source]], and it is why [[richard-stallman]] and the [[free-software-foundation]] reject "open source" as a label even though the approved license lists overlap almost completely.

The OSD's function as a certification standard has been tested most sharply by the source-available licensing movement. When MongoDB relicensed from [[agpl]] to the Server Side Public License ([[sspl-bsl]]) in 2018, it submitted the SSPL to the [[open-source-initiative]] for certification. The SSPL's Section 13 extends copyleft conditions far beyond the software itself, requiring anyone offering the software as a service to release the entire supporting infrastructure stack under the SSPL. The OSI's evaluation process concluded that the SSPL did not meet the OSD's criteria — specifically, the extreme breadth of the copyleft condition was judged to discriminate against fields of endeavor (criterion 6) and to restrict other software (criterion 9). MongoDB withdrew the submission before a formal rejection. The episode demonstrated the OSD's value as a boundary: it provides a principled basis for distinguishing open source licenses from source-available licenses that use the rhetoric of openness while restricting use in ways the OSD prohibits. HashiCorp's later adoption of the Business Source License (also under [[sspl-bsl]]) for Terraform similarly fell outside the OSD, triggering the OpenTofu fork — an exercise of the [[forking-as-governance]] mechanism.

The OSD's lineage from the DFSG through [[bruce-perens]] to the [[open-source-initiative]] means that the open source movement's certification standard was originally drafted for an explicitly free-software-committed project (the [[debian-project]]). This genealogy is significant: the OSD is not a weakening of free software principles but a repackaging of them for a different audience. The criteria are substantively compatible with the [[four-freedoms]], even if the institutional homes — the OSI and the FSF — represent different wings of the movement. The OSD's endurance as a standard, maintained through decades of licensing innovation and corporate pressure, reflects its origin in practical experience: the DFSG was not a theoretical document but a working tool for making real inclusion decisions about real software packages.
