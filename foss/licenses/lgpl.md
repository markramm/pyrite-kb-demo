---
id: lgpl
title: "GNU Lesser General Public License"
type: license
importance: 5
license_type: copyleft-weak
author: "Free Software Foundation"
date: 1991-06-01
spdx_id: "LGPL-2.1-only"
key_provisions:
- "Permits linking of proprietary code to LGPL libraries without triggering copyleft"
- "Modifications to the LGPL library itself must remain LGPL"
- "Users must retain ability to relink the application against modified library versions"
- "Originally called 'Library GPL'; renamed 'Lesser GPL' with v2.1 in 1999"
related_licenses:
- gpl-v2
- gpl-v3
- mit-license
tags:
- copyleft-weak
- fsf
- libraries
- compromise
- adoption
research_status: draft
---

A variant of the GPL designed for software libraries, published by the [[free-software-foundation]] in 1991 alongside [[gpl-v2]]. The LGPL permits proprietary programs to link against LGPL-licensed libraries without the entire proprietary program being subject to copyleft. This "weak copyleft" compromise enabled broad library adoption while preserving copyleft requirements on the library code itself.

## The Linking Problem

Strong copyleft as implemented in [[gpl-v2]] creates a problem for libraries: if a proprietary application links to a GPL library, the entire application could be argued to be a "derivative work" subject to the GPL. This would make GPL libraries unusable in any commercial software — a result that would dramatically limit adoption without clearly advancing user freedom.

The LGPL solves this by drawing the copyleft boundary at the library interface. The LGPL library code itself must remain LGPL, and users must retain the ability to relink the application against modified versions of the library (so they can benefit from library improvements). But the application using the library can be proprietary.

## "Library" to "Lesser"

The original name — GNU Library General Public License — reflected the intent: a GPL variant for libraries. The renaming to "Lesser GPL" with version 2.1 in 1999 was deliberate and philosophical. [[richard-stallman]] explained that "Lesser" was chosen because this license gives users *less* protection than the full GPL — it is a strategic compromise, not a preferred default. The FSF advises project authors to use the full GPL where possible and the LGPL only when necessary to achieve adoption goals that serve users.

This naming history encodes a movement-internal debate: is it better to use strong copyleft and accept limited adoption, or weak copyleft and accept broader adoption with less freedom protection? The LGPL represents the compromise position, adopted pragmatically for specific cases.

## Adoption

Major LGPL-licensed projects include the GNU C Library (glibc) — the standard C library for Linux systems — and many GUI toolkits and language runtimes. The LGPL's adoption made it possible for commercial Linux distributions to include copyleft libraries without requiring that all applications be open source.

The license has declined in relative prominence compared to [[mit-license]] and [[apache-license-2]] for new library projects, partly because permissive licenses eliminate the adoption friction LGPL reduced rather than removed, and partly because the linking analysis has become more complex with modern build systems that blur the library/application boundary.

## Relationship to Other Licenses

The LGPL occupies the middle ground between strong copyleft ([[gpl-v2]], [[gpl-v3]]) and permissive ([[mit-license]], [[bsd-license]], [[apache-license-2]]). It represents the FOSS movement's attempt to balance freedom-protection against adoption — a balance the [[software-freedom-vs-open-source]] debate frames differently depending on which tradition you prioritize.
