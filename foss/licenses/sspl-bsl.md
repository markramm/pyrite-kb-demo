---
id: sspl-bsl
title: "SSPL and Business Source License"
type: license
importance: 5
license_type: source-available
author: "MongoDB (SSPL) / MariaDB (BSL)"
date: 2018-10-01
key_provisions:
- "SSPL Section 13: if you offer the software as a managed service, you must release ALL supporting infrastructure code under SSPL"
- "BSL: not open source at release; converts to specified open source license after a time delay (typically 4 years)"
- "Neither license is OSI-approved"
- "SSPL: source code available but service providers cannot use without full infrastructure disclosure"
related_licenses:
- agpl
- gpl-v3
- apache-license-2
tags:
- source-available
- mongodb
- mariadb
- saas-loophole
- cloud-providers
- not-open-source
research_status: draft
---

Two licenses that emerged in 2018-2019 as commercial FOSS companies attempted to prevent cloud providers from offering managed services based on their software without contributing back. Neither is an OSI-approved open source license; both represent a departure from the FOSS tradition into "source-available" territory — source code is visible, but use rights are restricted in ways open source licenses do not permit.

## Server Side Public License (SSPL)

MongoDB introduced the SSPL in October 2018, relicensing MongoDB from [[agpl]] after determining that the AGPL was insufficient to prevent cloud providers from offering MongoDB as a managed service. The SSPL's Section 13 dramatically extends the copyleft condition: if you offer the software as a service, you must release not just your modifications to the software, but the entire software stack used to provide the service — including orchestration systems, monitoring, storage layers, and other infrastructure code.

This is a deliberately unacceptable condition for any cloud provider with proprietary infrastructure, making the license function as a commercial fence while remaining technically "open" (source code visible). The FSF evaluated the SSPL and declined to recognize it as a free software license. The OSI declined to approve it. Debian and Fedora dropped MongoDB from their repositories over the license change. Red Hat followed.

MongoDB then offered a commercial license to providers who could not accept SSPL terms — making the business model explicit: SSPL functions as a price barrier, not a freedom guarantee.

## Business Source License (BSL / BUSL)

The Business Source License was created by Michael Widenius (the founder of MariaDB and original MySQL developer) as an alternative approach. Rather than restricting use types, BSL restricts commercial use at time of release but includes a "Change Date" after which the software converts to a specified open source license (typically Apache 2.0 or GPL). The conversion delay is typically four years.

BSL attempts to give companies a time-limited monopoly on commercial use of their software while ensuring eventual open source availability. It was designed to prevent the "free rider" problem — companies building on FOSS without contributing back — while maintaining the eventual FOSS commons.

HashiCorp adopted a variant of BSL (BUSL) in 2023 when it relicensed Terraform away from the Mozilla Public License, triggering the OpenTofu fork by the Linux Foundation.

## Significance to the Movement

The SSPL and BSL represent the FOSS movement's most visible recent crisis: the tension between the open source model's value generation and the difficulty of capturing enough of that value to sustain development. [[magic-cauldron-1999]] addressed this tension in 1999; [[roads-and-bridges-2016]] and [[working-in-public-eghbal-2020]] documented its intensification. The SSPL and BSL represent one answer — restrict use at the license level — that the movement's core institutions (OSI, FSF, Debian) have rejected as incompatible with open source principles.

The [[agpl]] was the movement-internal attempt to solve the same problem. The SSPL can be read as a judgment that the AGPL failed — that cloud providers found ways to avoid its requirements or simply accepted it and did not contribute back. Whether that judgment is accurate remains contested.

The SSPL/BSL moment illustrates the structural conflict in [[open-core-business-model]]: companies that build on FOSS communities need to capture enough value to sustain development, but the mechanisms for capturing value tend to restrict the freedoms that make the communities valuable in the first place.
