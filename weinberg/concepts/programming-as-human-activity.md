---
id: programming-as-human-activity
title: Programming as Human Activity
type: concept
tags:
- programming
- psychology
- software-development
- human-factors
- meta-thesis
links:
- target: learning-not-results
  relation: related_to
  note: Weinberg's thesis that programming is a human activity aligns with Poppendiecks'
    thesis that learning, not results, is the point
  kb: poppendiecks
- target: customer-development
  relation: related_to
  note: Weinberg's emphasis on understanding the human using software connects to
    Blank's emphasis on understanding the customer
  kb: blank
importance: 10
first_appeared: psychology-of-computer-programming-1971
source_tradition: psychology, sociology
key_writings:
- psychology-of-computer-programming-1971
- understanding-the-professional-programmer-1982
- becoming-a-technical-leader-1986
- qsm-vol1-systems-thinking-1992
related_concepts:
- egoless-programming
- general-systems-thinking
- quality-software-management-framework
- congruent-behavior
- moi-model
- technical-reviews-and-walkthroughs
- problem-definition
research_status: draft
---

Programming as human activity is the unifying thesis of [[gerald-weinberg]]'s career. First articulated — though not named — in [[psychology-of-computer-programming-1971]], it is the claim that software development is fundamentally a human activity, shaped by psychology, social dynamics, organizational culture, and interpersonal behavior; and that therefore the primary leverage points for improving software quality are not technical but human.

## The Thesis

At the time [[psychology-of-computer-programming-1971]] was published, the dominant view of programming was that it was an engineering or mathematical activity. Programmers applied formal methods to specified problems and produced correct or incorrect results. The human programmer was, in this view, a mechanism for transforming requirements into code — ideally a transparent mechanism, whose personal characteristics should not affect the output.

Weinberg's intervention was to take seriously the obvious empirical fact that programmers are humans, that humans are not transparent, and that human characteristics — psychological, social, cognitive, motivational — have enormous effects on the quality of software. A team that communicates poorly produces poor software. A programmer who cannot accept criticism of their code produces code that improves slowly. An organization whose culture discourages honest status reporting produces projects that fail predictably. These are not accidents or edge cases; they are systematic consequences of ignoring the human dimensions of a human activity.

## Why This Was Controversial

The thesis sounds obvious now, but it was not obvious in 1971 and was actively resisted by a significant part of the software engineering community. The resistance came from several directions:

- **Scientism.** If programming is an engineering science, then the relevant variables are formal and technical. Human psychology is not engineering. Admitting psychological variables seems to undermine the project of making software development rigorous.
- **Managerial convenience.** Accepting that human dynamics drive software quality means accepting that management decisions, organizational culture, and interpersonal behavior are technical variables. This is uncomfortable for managers who would prefer to treat software quality as a matter of developer skill and process compliance.
- **Measurement difficulty.** Human dynamics are harder to measure than code metrics. A thesis that emphasizes hard-to-measure variables is inconvenient for frameworks that want to show measurable improvement.

Weinberg was patient with all of these objections and engaged them directly throughout his career. The [[quality-software-management-framework]] is, among other things, a sustained demonstration that the human thesis is compatible with rigorous measurement and systematic management.

## The Thesis Across Weinberg's Career

Weinberg returned to the human thesis in every major work:

- **[[psychology-of-computer-programming-1971]]**: Programming teams, communication, [[egoless-programming]], social dynamics of development.
- **[[introduction-to-general-systems-thinking-1975]]**: Systems thinking as the conceptual tool for understanding the human systems in which programming happens.
- **[[are-your-lights-on-1982]]**: Problem definition as a human cognitive and social activity.
- **[[secrets-of-consulting-1985]]**: The consulting relationship as a human relationship; influence as a human phenomenon.
- **[[becoming-a-technical-leader-1986]]**: Leadership as a human activity in technical contexts.
- **[[quality-software-management-framework]] (1992-1997)**: The full systematic treatment — organizational culture, measurement, human communication, and change management as the determinants of software quality.

Each work addresses a different aspect of the same thesis: that the primary leverage for better software is better human understanding and better human behavior, not better algorithms or better tools.

## Influence and Legacy

The human thesis is now mainstream. The agile manifesto's "individuals and interactions over processes and tools" is a direct statement of the thesis, though without explicit citation of Weinberg. The DevOps community's emphasis on culture and psychological safety echoes Weinberg. [[esther-derby]]'s and [[johanna-rothman]]'s organizational consulting work, [[kent-beck]]'s XP, [[tom-demarco]] and [[timothy-lister]]'s Peopleware — all are expressions of the human thesis.

Weinberg's distinctiveness is not that he stated the thesis first (though he was early) but that he spent fifty years developing its implications rigorously and practically across the full range of software development — from individual psychology through team dynamics through organizational culture through management practice. No one else traced the thesis through as many domains with as much concrete detail.
