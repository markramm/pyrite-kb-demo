---
id: gpl-v3
title: "GNU General Public License version 3"
type: license
importance: 7
license_type: copyleft-strong
author: "Richard Stallman / Free Software Foundation"
date: 2007-06-29
spdx_id: "GPL-3.0-only"
key_provisions:
- "Anti-tivoization: installation information must be provided for user-installed modified versions on consumer devices"
- "Explicit patent license from contributors"
- "Compatible with Apache License 2.0 (unlike GPL v2)"
- "Anti-DRM provisions: does not prohibit DRM but waives anti-circumvention law claims"
- "Additional permissions mechanism"
related_licenses:
- gpl-v2
- lgpl
- agpl
- apache-license-2
tags:
- copyleft
- stallman
- fsf
- tivoization
- patents
- drm
research_status: draft
---

The current version of the GNU General Public License, published by the [[free-software-foundation]] on June 29, 2007 ([[gpl-v3-release-2007]]). GPL v3 addressed three problems that [[gpl-v2]] had not anticipated: hardware restriction of software, software patents, and the emerging DRM landscape. Its release was the most publicly debated license revision in FOSS history, and it remains controversial — the Linux kernel has not migrated from [[gpl-v2]].

## What GPL v3 Adds

**Anti-tivoization.** TiVo distributed Linux (GPL v2) in its digital video recorders but cryptographically signed the device software, preventing users from running modified versions. This was technically GPL v2-compliant — TiVo provided the source code — but violated the spirit of [[four-freedoms]] because users could not actually exercise Freedom 1 (to modify) on their own devices. GPL v3's "Corresponding Source" requirement includes installation information — the keys, signatures, or other data needed to install modified software on the device.

**Patent retaliation.** GPL v3 includes an explicit patent license from contributors and a patent non-aggression clause: if you distribute GPL v3 software, you cannot subsequently bring patent claims against downstream users for using it. This closes a gap [[gpl-v2]] left open.

**DRM compatibility.** GPL v3 does not prohibit implementing DRM, but it waives the licensor's rights under anti-circumvention laws (like the DMCA) against users who modify the software to circumvent DRM. This is a careful legal maneuver rather than a blanket prohibition.

**Apache License 2.0 compatibility.** A practical benefit: GPL v3 is compatible with [[apache-license-2]], meaning Apache-licensed code can be combined with GPL v3 code in a combined work. GPL v2 and Apache 2.0 are incompatible.

## The Linux Kernel Decision

Linus Torvalds and the Linux kernel maintainers declined to migrate from GPL v2. Torvalds expressed specific objections to the anti-tivoization provisions, arguing that hardware manufacturers have legitimate reasons to lock down devices (firmware integrity, FCC compliance) and that the GPL should govern software distribution, not hardware design. The Linux kernel's license is "GPL-2.0-only" — not "GPL-2.0-or-later," which would allow GPL v3.

This split means the Linux kernel cannot legally incorporate GPL v3-only code. It is one of the most significant ongoing consequences of the GPL v2/v3 divergence.

## Public Drafting Process

The FSF ran an 18-month public drafting process for GPL v3 (2006-2007), publishing multiple drafts for comment and running discussion committees. This was unprecedented for a license revision and was intended to build legitimacy and community buy-in. The process was partially successful — significant input was incorporated — but the Linux kernel decision demonstrated that legitimacy through process could not overcome substantive technical and philosophical disagreements.

## Relationship to the Free Software / Open Source Split

GPL v3 is a distinctly free-software tradition document. The anti-tivoization provisions reflect [[richard-stallman]]'s commitment to [[four-freedoms]] even when they conflict with corporate hardware practices. The open source pragmatist tradition, more willing to accommodate hardware realities, produced the resistance from kernel developers.

The [[agpl]] (published November 2007, shortly after GPL v3) extended the v3 framework to close the network-use loophole.
