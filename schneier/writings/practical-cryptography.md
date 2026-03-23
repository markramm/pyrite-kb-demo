---
id: practical-cryptography
title: "Practical Cryptography"
type: writing
importance: 7
tags:
- cryptography
- reference
- implementation
- protocols
- engineering
writing_type: book
date: "2003-01-01"
publisher: "John Wiley & Sons"
coauthors:
- niels-ferguson
key_concepts:
- schneiers-law
- security-is-a-process
research_status: draft
---

Practical Cryptography, co-authored with [[niels-ferguson]] and published in 2003, is the technical successor to [[applied-cryptography]]. Where Applied Cryptography was a comprehensive reference covering essentially all published cryptographic algorithms, Practical Cryptography takes a different approach: it is opinionated, selective, and explicitly concerned with what cryptographic tools practitioners should actually use rather than cataloging everything that exists.

## The Departure from Applied Cryptography

The contrast between the two books is deliberate and reflects Schneier's intellectual evolution between 1994 and 2003. Applied Cryptography presented algorithms neutrally — here is how DES works, here is how RSA works, here is how to implement them. Practical Cryptography makes value judgments: here is what you should use, here is what you should avoid, and here is why. The shift from encyclopedic reference to opinionated guide reflects the [[security-thinking-pivot]] that [[secrets-and-lies]] had announced in 2000.

Ferguson and Schneier are direct: they tell readers not to implement their own cryptographic primitives (consistent with [[schneiers-law]]), to use a small set of well-analyzed algorithms rather than seeking novelty, and to think carefully about key management — which they identify as the hard part of cryptographic systems, harder than algorithm selection.

## The Key Management Emphasis

Practical Cryptography's most significant technical contribution may be its extended treatment of key management. Applied Cryptography treated key management briefly; Practical Cryptography devotes substantial attention to it. The insight is that most real-world cryptographic failures are not failures of the algorithms but failures of how keys are generated, stored, distributed, revoked, and used. This focus on operational security rather than mathematical properties reflects the post-[[secrets-and-lies]] sensibility.

## The Ferguson Collaboration

[[niels-ferguson]] co-authored Practical Cryptography as a full intellectual partner, not a technical contributor. Ferguson is a cryptographer of substantial standing in his own right — a co-designer of [[twofish-algorithm]] and [[skein-hash-function]] and a contributor to multiple international cryptographic standards. The book reflects both of their perspectives, and Ferguson's influence is evident in its engineering orientation and its willingness to make strong recommendations rather than presenting options neutrally.

## A Revised Edition: Cryptography Engineering

Practical Cryptography was substantially revised and expanded with a third co-author (Tadayoshi Kohno) and republished as Cryptography Engineering in 2010. The revision updated the technical content and deepened the engineering-oriented treatment, reflecting seven additional years of applied cryptographic practice. Cryptography Engineering is now the more commonly cited version of the work, but Practical Cryptography in its 2003 form is the original statement of the approach.

## Position in the Arc

Practical Cryptography belongs to the transition period at the edge of the [[cryptography-era]] and the [[security-thinking-pivot]]. It is a technical book, focused on cryptographic engineering rather than security systems or policy, but its sensibility — opinionated, practice-oriented, skeptical of novelty and complexity — reflects the perspective Schneier had developed through [[secrets-and-lies]] and [[beyond-fear]]. It is the technical tradition meeting the analytical one.
