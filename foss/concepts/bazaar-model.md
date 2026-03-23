---
id: bazaar-model
title: "The Bazaar Model"
type: concept
importance: 8
concept_type: development-model
first_appeared: "cathedral-and-the-bazaar-1997"
key_writings:
- cathedral-and-the-bazaar-1997
- homesteading-the-noosphere-1998
- producing-open-source-software-2005
related_concepts:
- linuss-law
- forking-as-governance
- copyleft
tags:
- development-methodology
- raymond
- linux
- distributed-development
- coordination
research_status: draft
---

The bazaar model is [[eric-raymond]]'s central contribution in [[cathedral-and-the-bazaar-1997]]: a theory of software development in which many distributed developers, frequent releases, and users-as-co-developers produce better software than the carefully planned, centrally controlled "cathedral" approach. The essay gave the [[open-source-schism-and-dotcom-1998-2004]] era its intellectual framework and directly influenced the [[netscape-source-release-1998]] that catalyzed the open source movement's institutional formation.

Raymond drew the contrast from observing [[linus-torvalds]]'s management of the Linux kernel versus the development model of earlier projects, including some GNU projects. The cathedral model concentrates design authority in a small group, plans releases carefully, and restricts access during development — bugs are found by a dedicated team before the public sees the code. The bazaar model inverts these assumptions: release early and often (see [[release-early-release-often]]), treat every user as a potential co-developer, accept contributions from anyone who shows up, and let coordination emerge from the network of contributors rather than from a central plan. The bazaar works, Raymond argued, because of [[linuss-law]]: with enough participants examining the code, bugs become transparent to someone. The low cost of forking (see [[forking-as-governance]]) provides a structural guarantee — if a project's leadership makes poor decisions, the community can fork the codebase and continue independently, disciplining maintainers even when forking never actually occurs.

The essay's influence exceeded its analytical rigor. [[netscape-source-release-1998]] was directly triggered by Netscape executives reading Raymond's essay and concluding that the bazaar model could rescue their browser from Microsoft's competitive pressure. The essay was circulated at the [[foresight-open-source-meeting-1998]] where the term "open source" was coined by [[christine-peterson]], and it provided the methodological argument that [[eric-raymond]] and [[bruce-perens]] used to justify the creation of the [[open-source-initiative]]. Where [[richard-stallman]] argued for open source on ethical grounds (the [[four-freedoms]]), Raymond argued on engineering grounds: the bazaar is a better way to build software. This was the pragmatist pitch that made FOSS legible to corporate audiences and defined the strategic rebranding at the heart of [[software-freedom-vs-open-source]].

The bazaar model has real strengths and real limits. The strengths are well-documented: Linux, Apache, and other large FOSS projects have demonstrated that distributed development can produce software of extraordinary quality and scale. The many-eyes effect described by [[linuss-law]] is genuine for functional bugs — a broad contributor base increases the probability that someone will recognize a problem's root cause. The frequent-release cycle keeps feedback loops short and makes contributors feel ownership. [[karl-fogel]]'s [[producing-open-source-software-2005]] and [[homesteading-the-noosphere-1998]] filled in the social and organizational dimensions that Raymond's original essay left underdeveloped: the reputation economy, conflict resolution, contributor onboarding, and the informal norms that make bazaar coordination actually function.

The limits are equally real, though less frequently acknowledged. The bazaar model works for bug-finding and incremental improvement but struggles with fundamental design decisions, which require the kind of coherent vision that centralized authority provides. The xz backdoor (see [[xz-backdoor-2024]]) exposed a deeper limit: the bazaar assumes that many eyes are actually looking, but critical infrastructure is often maintained by one or two exhausted individuals, and the "many eyes" never materialize for build scripts, test fixtures, or maintainer social dynamics. The bazaar model describes a real phenomenon — distributed development can work — but its success conditions are narrower than the essay's rhetoric suggests. It works best when the project is visible enough to attract contributors, the problem space is decomposable enough for distributed work, and the community has sufficient social infrastructure to coordinate without central planning.
