---
id: forking-as-governance
title: "Forking as Governance"
type: concept
importance: 7
concept_type: governance-model
first_appeared: "cathedral-and-the-bazaar-1997"
key_writings:
- cathedral-and-the-bazaar-1997
- homesteading-the-noosphere-1998
- producing-open-source-software-2005
- success-of-open-source-weber-2004
related_concepts:
- bazaar-model
- open-source-definition
- copyleft
- four-freedoms
tags:
- governance
- forking
- exit-rights
- community
- power-dynamics
research_status: draft
---

The right to fork a project's codebase is the ultimate check on maintainer or organizational power in FOSS. Because the source code is available and the license permits redistribution — a condition guaranteed by both the [[four-freedoms]] and the [[open-source-definition]] — any sufficiently motivated community can create an independent copy of a project and develop it under new leadership. This structural feature makes FOSS governance fundamentally different from corporate or institutional governance: the "governed" can exit with the full productive asset. In Albert Hirschman's framework, FOSS governance grants voice and exit simultaneously, and the exit option is unusually powerful because it carries the entire codebase.

The threat of forking disciplines maintainers and sponsoring organizations even when forking never actually occurs. A project leader who makes unpopular technical decisions, ignores community input, or attempts to change licensing terms faces the knowledge that the community can walk away with the code. This latent threat functions as a governance mechanism without requiring formal constitutions, elections, or oversight bodies — though many mature FOSS projects develop those too. The [[debian-project]]'s formal governance structure (elected project leader, social contract, developer votes) coexists with the background possibility of forking; Debian's governance is, in a sense, the formalization of what the fork threat accomplishes informally.

The historical record provides several instructive examples of exercised forks. When Oracle acquired Sun Microsystems in 2010, the community's concern about Oracle's stewardship of OpenOffice.org led to the creation of LibreOffice under The Document Foundation — a fork that rapidly became the dominant continuation, with most active developers migrating. MariaDB forked from MySQL in 2009 (approximate) when the MySQL founder, Michael Widenius, grew concerned about Oracle's control following the Sun acquisition announcement; MariaDB is now the default MySQL-compatible database in most Linux distributions. In 2014, the io.js project forked from Node.js over frustrations with Joyent's governance of the project — specifically, the slow release cycle and perceived corporate control over technical direction. The io.js fork was later reunified with Node.js under the Node.js Foundation, demonstrating that forks can function as governance interventions that succeed by forcing institutional change rather than permanent separation. The XFree86-to-X.Org transition (2004) followed a similar pattern: a licensing change by XFree86's leadership prompted the community to fork and create X.Org, which replaced XFree86 entirely.

The fork right has structural prerequisites that licenses must satisfy. Strong [[copyleft]] licenses like [[gpl-v2]] and [[gpl-v3]] guarantee fork rights by requiring that source code be available and that derivative works carry the same license — ensuring that the fork inherits the same freedoms as the original. Permissive licenses like [[mit-license]] and [[apache-license-2]] also permit forking but do not prevent the fork (or the original) from being relicensed as proprietary. The [[open-source-definition]]'s criteria — particularly free redistribution, source code availability, and permission for derived works — can be read as a codification of the minimum conditions for forking to be possible. Without these conditions, the exit option disappears, and governance reverts to conventional institutional authority.

The fork right is rarely exercised precisely because it is always present. Forking a project is costly: it splits the contributor community, duplicates effort, fragments the user base, and creates compatibility headaches. Most forks fail — the forking community often lacks the resources to maintain the project independently, and the network effects that made the original project valuable do not transfer automatically. But the cost of forking is finite, and a sufficiently motivated community can bear it when the alternative — remaining under governance they reject — is worse. This dynamic means that FOSS maintainers and sponsoring organizations operate under a constraint that proprietary software companies do not face: their authority depends on continued legitimacy, not on legal control of the asset. The [[bazaar-model]]'s effectiveness depends, in part, on this background condition — distributed development works because contributors can leave if coordination fails.
