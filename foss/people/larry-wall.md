---
id: larry-wall
title: "Larry Wall"
type: person
tags:
- perl
- patch
- programming-languages
- artistic-license
- collaboration
role: "Perl creator, 'patch' utility author"
research_status: draft
---

Larry Wall (born 1954) made two distinct contributions to the FOSS movement: the `patch` utility and the Perl programming language.

The `patch` utility (1985) is historically significant out of proportion to its apparent simplicity. `patch` applies diffs — the output of the `diff` utility — to source files, enabling asynchronous collaborative development: a developer could mail a diff to a mailing list, and maintainers could apply it without needing direct access. This workflow defined [[patch-based-development]], the dominant FOSS collaboration pattern from the mid-1980s through the mid-2000s, when [[git-release-2005]] and the [[github-platform]] pull-request model superseded it. The Linux kernel's famous patch-by-email workflow depended directly on Wall's tool.

Perl (1987) was the first major general-purpose scripting language to emerge from and be developed as an open source project. It became the dominant language for system administration and early web development (CGI scripts) in the 1990s, and its community — the Comprehensive Perl Archive Network (CPAN) — established early patterns for package distribution and community contribution that influenced later language ecosystems (PyPI for Python, npm for JavaScript).

Wall invented the Artistic License as an alternative to the [[gpl-v2]] for Perl. The Artistic License allowed distribution without imposing copyleft requirements, prioritizing community customs over legal enforcement — reflecting Wall's view that community norms matter more than license terms. The Artistic License was controversial (OSI certified it but critics found it legally ambiguous) and was revised as Artistic License 2.0 in 2006.

Wall's governance of Perl reflected a different model than [[linus-torvalds]]'s or [[guido-van-rossum]]'s: more communal and less architecturally centralized, which eventually contributed to Perl 6 (later renamed Raku) emerging as a separate language rather than a successor — a FOSS governance case study in the costs of design-by-committee and diffuse authority.
