---
id: problem-definition
title: Problem Definition
type: concept
tags:
- problem-solving
- requirements
- consulting
- analysis
- design
links:
- target: get-out-of-the-building
  relation: related_to
  note: Both insist on understanding the real problem before building solutions —
    Weinberg through problem definition discipline, Blank through customer contact
  kb: blank
importance: 8
first_appeared: are-your-lights-on-1982
source_tradition: ''
key_writings:
- are-your-lights-on-1982
- exploring-requirements-1989
- rethinking-systems-analysis-and-design-1982
related_concepts:
- programming-as-human-activity
- general-systems-thinking
- helpful-model-of-consulting
- quality-software-management-framework
- weinberg-laws-and-rules
research_status: draft
---

Problem definition is the discipline of understanding what problem you are actually trying to solve before you begin solving it. [[gerald-weinberg]] and [[donald-gause]] developed this as a sustained subject in [[are-your-lights-on-1982]] (subtitled "How to Figure Out What the Problem Really Is") and extended it in [[exploring-requirements-1989]].

## The Central Argument

The central argument of [[are-your-lights-on-1982]] is that most "solution failures" are actually "problem definition failures." People, teams, and organizations spend enormous effort solving the wrong problem brilliantly. The discipline of problem definition is the practice of resisting the pull toward solution and instead asking: what is the problem we are actually facing?

The title comes from an illustrative example in the book: a new building creates traffic congestion at its entrance, and various expensive solutions are proposed (traffic signals, road widening, routing changes) before someone asks whether people could simply be encouraged to stagger their departure times. The expensive solutions were excellent solutions to the wrong problem. The actual problem was different from the stated problem.

## Key Heuristics from the Book

**A problem is a difference between what is and what should be.** This definition is simple but operationally powerful. Defining a problem requires specifying both the current state and the desired state — and being honest about both. Vague desired states produce vague problems that cannot be solved.

**The problem belongs to someone.** Problems don't exist in the abstract; they exist for specific people in specific situations. "Who has the problem?" is one of the most productive diagnostic questions Weinberg and Gause offer. The answer often reveals that different stakeholders have different problems, and that the stated problem is a coalition of incompatible individual problems.

**Solutions often create new problems.** Every solution changes the situation, which changes the problem. The traffic light that reduces congestion creates a new problem for pedestrians. Problem definition is not a one-time upstream activity; it recurs throughout any serious problem-solving effort.

**Don't trust the problem as stated.** Weinberg and Gause are deeply skeptical of "the requirements" as given. Requirements express someone's proposed solution, not the underlying need. "We need a new reporting module" states a solution; the underlying problem might be that managers lack the information they need to make decisions, or that they receive too much information to process, or that the information arrives too late. Requirements analysis that takes stated requirements at face value is not requirements analysis.

**The Phantom Problem.** Some problems, when examined carefully, dissolve — they were artifacts of how the situation was framed, not genuine features of the situation. Pursuing the phantom problem is expensive and produces no lasting value.

## Relationship to Requirements Engineering

[[exploring-requirements-1989]], written with [[donald-gause]], extends the problem definition discipline into a systematic approach to requirements elicitation. The key move is similar: before asking what the system must do, ask what problem the system is intended to solve, and ask whether that is the actual problem. Ambiguity in requirements is usually evidence of unresolved problem definition, not imprecision in writing.

## Connection to Consulting and Systems Thinking

The [[helpful-model-of-consulting]] depends on problem definition discipline. An expert consultant who accepts the client's stated problem at face value and provides the requested solution may be solving the wrong problem efficiently. A helpful consultant asks "what is the problem you're trying to solve?" and keeps asking until the actual problem — usually different from and more tractable than the stated one — becomes visible.

From a [[general-systems-thinking]] perspective, problem definition failures are a form of model failure: the stakeholder's mental model of their situation is inaccurate in ways that make the stated problem a poor representation of the actual situation. The consultant's diagnostic work is to help the client build a more accurate model — which requires the [[congruent-behavior]] to tell the client things they may not want to hear about whether their problem definition is sound.
