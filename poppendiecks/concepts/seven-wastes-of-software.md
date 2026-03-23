---
id: seven-wastes-of-software
title: Seven Wastes of Software
type: concept
tags:
- lean-software-development
- waste
- tps-translation
- muda
- practical-tools
links:
- target: seven-wastes-muda
  relation: translates
  note: 'Direct translation: Ohno''s manufacturing wastes adapted to software'
  kb: tps
importance: 9
first_appeared: 'Lean Software Development: An Agile Toolkit (2003)'
tps_source: muda (seven wastes of manufacturing) — Taiichi Ohno
key_writings:
- lean-software-development-agile-toolkit-2003
- implementing-lean-software-development-2006
related_concepts:
- eliminate-waste
- seven-lean-principles
- value-stream-mapping-for-software
- amplify-learning
- optimize-the-whole
research_status: draft
---

The seven wastes of software are [[mary-poppendieck]] and [[tom-poppendieck]]'s translation of [[taiichi-ohno]]'s seven manufacturing wastes (*muda*) into software-specific categories, introduced in [[lean-software-development-agile-toolkit-2003]]. They are the operational heart of the [[eliminate-waste]] principle and the primary tool for identifying what to remove from a software development process.

## Manufacturing Wastes and Their Software Equivalents

[[taiichi-ohno]] classified manufacturing waste into seven types, and the Poppendiecks mapped each to a software analogue:

### 1. Partially Done Work
**Manufacturing source:** Inventory (work-in-process between stations)

Partially done work in software includes features that are coded but not integrated, code that is checked in but not deployed, designs that are complete but not implemented, and documentation that is written but not reviewed. Like manufacturing inventory, partially done work ties up capacity, hides defects (integration problems won't appear until integration happens), and introduces risk (requirements may change before the work is finished). The Poppendiecks argue that partially done work is the most insidious software waste because it is invisible — it does not show up on a burndown chart or a utilization report.

### 2. Extra Features
**Manufacturing source:** Overproduction

Features that are built because they seem like good ideas, or because the spec included them, but that customers do not actually use. Studies of software products consistently find that large fractions of features are rarely or never used. Extra features add code complexity, increase testing burden, slow future development, and consume team capacity that could have been spent on features customers actually need. The lean principle is to build only what is needed now — consistent with [[decide-as-late-as-possible]], which argues that future needs are better addressed when they become current needs.

### 3. Relearning
**Manufacturing source:** Overprocessing (doing more work than required)

Knowledge that is learned by one team member but not shared, documented in ways that cannot be found, or lost when people leave. Relearning also occurs when teams reinvent solutions to problems already solved elsewhere in the organization, when documentation does not capture the "why" behind decisions, or when long time gaps between related activities require rediscovering context. [[amplify-learning]] is the affirmative principle that addresses relearning waste: build systems and practices that capture and amplify knowledge rather than losing it.

### 4. Handoffs
**Manufacturing source:** Transport (moving materials between locations)

Every time work changes hands — from business analyst to developer, from developer to tester, from tester to operations — information is lost. The mental model of what was needed, the context that explains why a decision was made, the tacit knowledge of what edge cases to watch for — all of this is partially or wholly lost in handoffs. The more handoffs in a process, the more information-loss waste accumulates. Large organizations with multiple specializations (separate UX, development, QA, DevOps, release management teams) have correspondingly more handoff waste. Self-organizing, cross-functional teams — [[empower-the-team]] — reduce handoff waste by keeping related knowledge in the same team.

### 5. Delays
**Manufacturing source:** Waiting (idle time when work cannot proceed)

Waiting for approvals, waiting for sign-off, waiting for another team to complete a dependency, waiting for a test environment to be available, waiting for a deployment window. Delays are often the largest single category of calendar time in a software process — the Poppendiecks and [[donald-reinertsen]] both observed that the actual work in a software process typically represents a small fraction of the elapsed time; the rest is waiting. [[deliver-as-fast-as-possible]] and [[pull-systems-in-software]] are the principles that address delay waste.

### 6. Task Switching
**Manufacturing source:** Motion (unnecessary movement of workers)

The cognitive cost of switching between tasks. Programmers interrupted in the middle of complex work must rebuild their mental context when they return — studies cited by the Poppendiecks suggest this context rebuilding can take 15–20 minutes per interruption. Multitasking on concurrent projects multiplies task-switching costs. Lean software development argues for limiting work-in-process (WIP) — a principle that [[david-anderson]] formalized into the WIP limits that are the defining practice of his Kanban method. Focused, single-task work is not a luxury; it is the condition for cognitive productivity.

### 7. Defects
**Manufacturing source:** Defects (scrap and rework)

Bugs, security vulnerabilities, performance problems, and design errors that must be reworked. The cost of a defect grows dramatically the later it is found — a bug caught in code review costs minutes to fix; the same bug found in production can cost days of debugging and customer recovery. [[build-integrity-in]] addresses defect waste through test-driven development, continuous integration, and ongoing refactoring. [[shigeo-shingo]]'s *poka-yoke* principle — prevent defects by design rather than detecting them after the fact — is the TPS ancestor of these practices.

## Using the Taxonomy

The seven wastes are not just a classification scheme; they are a diagnostic tool. [[value-stream-mapping-for-software]] uses the waste taxonomy to annotate a value stream map with the types of waste at each step. The goal is to make invisible waste visible — to give teams a shared vocabulary for naming what they observe and a framework for prioritizing what to address.

The Poppendiecks acknowledged that the manufacturing-to-software mapping is imperfect. Software waste is primarily cognitive and relational rather than physical, which makes it harder to see and measure. The value of the seven-waste framework is not that it maps perfectly but that it forces teams to look — to notice what they have normalized and ask whether it adds value.
