---
id: apache-license-2
title: "Apache License 2.0"
type: license
importance: 6
license_type: permissive
author: "Apache Software Foundation"
date: 2004-01-01
spdx_id: "Apache-2.0"
key_provisions:
- "Explicit patent license from all contributors"
- "Patent retaliation clause: patent grant terminates if you bring patent claim"
- "Must retain copyright, patent, trademark, and attribution notices"
- "NOTICE file mechanism for attribution"
- "Compatible with GPL v3 but incompatible with GPL v2"
related_licenses:
- mit-license
- bsd-license
- gpl-v3
- gpl-v2
tags:
- permissive
- apache-software-foundation
- patent-grant
- corporate-adoption
research_status: draft
---

The Apache License 2.0, published January 2004 by the [[apache-software-foundation]], is the dominant permissive license for enterprise and corporate FOSS adoption. Where [[mit-license]] and [[bsd-license]] are silent on patents, Apache 2.0's explicit patent grant makes it the preferred choice for software where patent risk is a concern — which, in practice, means most commercially significant software.

## The Patent Grant Innovation

The critical distinguishing feature of Apache 2.0 is its explicit patent license. By contributing to an Apache 2.0-licensed project, contributors grant all users a patent license for any patents they hold that cover their contributions. This grant is perpetual and royalty-free.

The patent retaliation clause extends this: if you initiate patent litigation claiming that the software infringes your patents, your patent grant under Apache 2.0 terminates. This creates a mutual non-aggression dynamic — Apache 2.0 users agree not to assert patents against each other in exchange for clear patent rights to use the software.

This matters because the absence of an explicit patent grant in [[mit-license]] and [[bsd-license]] leaves a theoretical gap: a contributor could release code under a permissive license while retaining the ability to sue users for patent infringement on that same code. Apache 2.0 closes this gap explicitly.

## Version History

Apache 1.0 (1995) and 1.1 (2000) were ad-hoc licenses without the patent provisions. Version 2.0 (2004) was a substantial rewrite that introduced the patent grant and aligned with modern license drafting norms. The ASF discontinued use of 1.x for new projects.

## GPL Compatibility and Incompatibility

Apache 2.0 is compatible with [[gpl-v3]]: code licensed under Apache 2.0 can be combined with GPL v3 code in a single work. This compatibility was explicitly designed by both the FSF and the ASF.

Apache 2.0 is *not* compatible with [[gpl-v2]], because the patent retaliation clause constitutes an "additional restriction" that GPL v2 prohibits. This means Apache 2.0-licensed code cannot be incorporated into GPL v2-only projects — including the Linux kernel. This incompatibility has practical consequences for ecosystem integration.

## Corporate Adoption

The combination of permissive terms and explicit patent grant made Apache 2.0 the default license for major corporate open source projects: Google (Android, TensorFlow), Microsoft (many projects), Amazon Web Services (numerous tools), and the Apache Software Foundation's own projects. The [[apache-software-foundation]]'s governance model requires all ASF-hosted projects to use Apache 2.0.

From the free software perspective, Apache 2.0 has the same limitation as other permissive licenses: it permits proprietary derivative works. The [[software-freedom-vs-open-source]] debate situates it on the open-source-pragmatist side — it maximizes adoption and provides legal safety for corporate contributors, at the cost of not preserving [[four-freedoms]] for downstream users.
