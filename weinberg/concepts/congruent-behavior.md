---
id: congruent-behavior
title: "Congruent Behavior"
type: concept
importance: 8
tags: [communication, team-dynamics, psychology, satir, organizations, leadership]
first_appeared: "qsm-vol3-congruent-action-1994"
source_tradition: Satir's communication stances
key_writings: [qsm-vol3-congruent-action-1994, qsm-vol4-anticipating-change-1997]
related_concepts: [satir-change-model, egoless-programming, programming-as-human-activity, moi-model, quality-software-management-framework]
research_status: draft
---

Congruent behavior, as [[gerald-weinberg]] applies it in [[qsm-vol3-congruent-action-1994]], is [[virginia-satir]]'s concept of communication in which a person attends simultaneously and honestly to self, other, and context. Satir developed the framework in family therapy; Weinberg translated it into observable organizational behaviors that managers and consultants can recognize and work with.

## Satir's Framework

Satir identified five communication stances based on which elements of the situation a person attends to and which they discount:

**Congruent.** The person attends to self, other, and context simultaneously. Their internal experience, their words, and their body language are aligned. They say what they mean, they hear what the other person is saying, and they take the actual situation into account. This is the healthy stance.

**Blaming.** The person attends to self and context but discounts others. They see problems as caused by other people. In software teams: the manager who blames developers for schedule slippage without examining process or requirements; the developer who blames QA for finding bugs late. Blaming is often loud and confident.

**Placating.** The person attends to others and context but discounts self. They agree with everyone, avoid conflict, and suppress their own views. In software teams: the developer who says "sure, we can do that in two weeks" knowing they cannot; the manager who approves every feature request to avoid disappointing stakeholders. Placating looks cooperative but is a form of dishonesty.

**Superreasonable (Computing).** The person attends to context but discounts both self and others. They hide behind abstractions, data, process, and logic. In software teams: the architect who responds to every human concern with a technical framework; the project manager who communicates only in Gantt charts and burn-down rates. Superreasonable behavior feels safe to its practitioner because it seems objective, but it severs the human connections that make organizations function.

**Irrelevant (Distracting).** The person discounts self, others, and context. They respond to every situation with humor, distraction, or topic changes. In extreme form this is a dissociative response; in milder form it's the person who defuses every tense meeting with a joke and nothing ever gets resolved.

## Translating Satir for Software Organizations

Weinberg's insight was that these stances — developed to describe parents and children in family therapy — map directly onto observable behaviors in software organizations. The patterns are recognizable because they stem from the same underlying dynamic: when people feel threatened or overwhelmed, they adopt coping stances that discount part of reality in order to manage their anxiety.

In software contexts, Weinberg observed:

- **Code reviews** are a high-stakes trigger for incongruent behavior. Authors who placate ("you're right, I'll change it") without evaluating the feedback technically are just as problematic as authors who blame reviewers for not understanding their design.
- **Project status meetings** reliably surface superreasonable behavior — people hiding behind metrics when the honest message is "we are in trouble."
- **Deadline pressure** intensifies blaming dynamics between teams (development vs. QA, development vs. product management).

The title of QSM Vol. 3 — Congruent Action — signals that effective software management requires congruent behavior from leaders. A manager who responds to technical problems with blaming cannot create the conditions for honest problem-solving. A manager who placates cannot make decisions that require disappointing someone. A manager who goes superreasonable cannot support people through the emotional disruption of the [[satir-change-model]]'s chaos stage.

## Relationship to Egoless Programming

[[egoless-programming]] can be understood as a specific application of the congruence model to the act of code review. The defensive programmer who cannot accept criticism of their code is in a blaming or superreasonable stance — either blaming the reviewer or retreating into technical abstraction to avoid engaging with the feedback. Egoless programming creates the conditions for congruent participation in review.

## Organizational Diagnostic Use

Weinberg and colleagues at [[aye-conference]] and [[weinberg-and-weinberg]] used congruence patterns as a diagnostic tool. Observing which stances predominate in an organization's meetings and communications gives a rapid read on the health of that organization's communication. An organization dominated by superreasonable behavior (all metrics, no human conversation) will struggle to recognize and respond to the human dynamics that drive its outcomes. An organization dominated by placating will fail to surface problems until they are crises.

This connects to [[cultural-patterns-of-software-organizations]]: higher-pattern organizations tend to have more congruent communication, because congruence is what makes honest feedback loops possible. Without congruence, the feedback loops that distinguish Pattern 3 and Pattern 4 organizations from Pattern 0 and Pattern 1 cannot function. The practical communication implications of congruence are explored in [[what-did-you-say-1992]], which focuses on listening and feedback in technical contexts.
