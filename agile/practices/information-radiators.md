---
id: information-radiators
title: "Information Radiators"
type: practice
importance: 5
tags:
- organizational
- alistair-cockburn
- transparency
- visual-management
practice_type: organizational
originated_in: "Agile / Crystal (Alistair Cockburn)"
status: active
research_status: draft
---

Information radiators are large, visible displays of project status placed in team workspaces so that anyone — team members, stakeholders, passing management — can see the team's current state without asking. The term was coined by [[alistair-cockburn]]. Examples include physical task boards (index cards on a wall), burndown charts, build status monitors (a screen showing whether the current build is green or red), and cumulative flow diagrams.

## Intellectual Contribution

The term "information radiator" is deliberately metaphorical: it radiates information passively and continuously, like heat — anyone near it receives the information without actively seeking it. This contrasts with "information refrigerators": documents and reports that store information but require active retrieval.

Cockburn's insight connects to the [[crystal]] methodology's emphasis on osmotic communication — the passive absorption of project information that happens when a team is co-located and can overhear conversations and see shared displays. Information radiators are the physical infrastructure for osmotic communication. They make the team's state legible to the whole organization without requiring meetings, reports, or status queries.

The practice embodies [[agile-manifesto-four-values]]' commitment to [[individuals-and-interactions]] over processes and tools: the information radiator is a tool in service of interaction, not a substitute for it. A task board that triggers daily conversation is doing its job; a task board that no one looks at is furniture.

Information radiators also connect to [[self-organizing-teams]]: when the team's state is visible, team members can self-coordinate without management direction. The board shows what is in progress, what is blocked, and what is waiting — each team member can see what needs doing and act accordingly.

## Types and Examples

The task board (to-do / in-progress / done columns with story cards) is the most common form. Burndown charts show remaining work versus time, making sprint trajectory visible. Build monitors display [[continuous-integration]] status — red means the build is broken, green means it passes. Cumulative flow diagrams (associated with Kanban) show work distribution across pipeline stages over time.

## Current Status

Digital information radiators (Jira boards, GitHub project boards, dashboard tools) have largely replaced physical boards in distributed teams, at some cost to visibility and tangibility. The practice's core principle — make the team's state legible to everyone without asking — survives the medium shift.

Related practices: [[daily-standup]], [[sprint-review]], [[continuous-integration]], [[retrospective]].
