---
id: mit-license
title: "MIT License"
type: license
importance: 7
license_type: permissive
author: "Massachusetts Institute of Technology"
date: 1988-01-01
spdx_id: "MIT"
key_provisions:
- "Permission to use, copy, modify, merge, publish, distribute, sublicense, and sell"
- "Must retain copyright notice and permission notice in all copies"
- "No warranty"
- "No restriction on relicensing or use in proprietary software"
related_licenses:
- bsd-license
- apache-license-2
- gpl-v2
tags:
- permissive
- mit
- popular
- simple
- corporate-friendly
research_status: draft
---

One of the oldest and most widely deployed FOSS licenses, originating at the Massachusetts Institute of Technology. The MIT License is the most popular FOSS license by adoption count as of the 2020s (based on GitHub repository data), and its extreme brevity and simplicity make it attractive across the spectrum from individual developers to large corporations.

## The License in Plain Language

The MIT License grants anyone who receives a copy of the software essentially unlimited rights: use, copy, modify, merge, publish, distribute, sublicense, and sell. The only requirement is that the copyright notice and permission text must be included in all copies or substantial portions of the software. No warranty is provided.

That is the entirety of the license. At approximately 170 words, it is shorter than most legal disclaimers and requires no specialized legal interpretation.

## Strategic Significance

The MIT License represents the permissive pole of the FOSS licensing spectrum, opposite strong copyleft licenses like [[gpl-v2]]. From the free software tradition's perspective, the MIT License's permissiveness is also its weakness: it allows proprietary derivative works, meaning that a company can take MIT-licensed code, modify it, and release the modifications under a proprietary license, denying downstream users the freedoms the original author intended.

From the open source pragmatist tradition's perspective, this permissiveness is the point: maximum adoption, minimum friction, maximum compatibility with every other license. MIT-licensed code can be incorporated into GPL projects (the GPL's copyleft then applies to the whole), into BSD projects, into Apache projects, and into proprietary software.

## Adoption Patterns

The MIT License became standard in several specific ecosystems: the JavaScript/npm ecosystem, where npm defaults suggest it; academic and research software; and library authors who prioritize maximum reuse over freedom preservation. Projects like jQuery, Ruby on Rails, and Node.js use MIT.

The [[apache-license-2]] is MIT's main competitor for permissive licensing, differing primarily in its explicit patent grant — a provision that matters more for projects where patent risk is significant (particularly in corporate contexts). Both [[mit-license]] and [[apache-license-2]] are compatible with [[gpl-v3]]; [[apache-license-2]] is not compatible with [[gpl-v2]].

## The Freedom Debate

The MIT License predates the FOSS movement's explicit ideological formation — MIT's researchers shared code because sharing was the research norm, not because of a theory of software freedom. This history situates the MIT License differently than the GPL: it is not a political document but a practical one. This makes it simultaneously the most adopted FOSS license and, from [[richard-stallman]]'s perspective, inadequate as a vehicle for the [[four-freedoms]] that define free software.
