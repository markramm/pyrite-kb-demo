---
id: sustainable-pace
title: "Sustainable Pace"
type: concept
importance: 6
tags:
- xp
- manifesto
- work-conditions
originator: "kent-beck"
concept_type: principle
research_status: draft
---

Sustainable pace is the principle that software teams should work at a pace they can maintain indefinitely, without overtime becoming a standard practice. It appears as principle 8 of the [[agile-manifesto-twelve-principles]]: "Agile processes promote sustainable development. The sponsors, developers, and users should be able to maintain a constant pace indefinitely."

## Origin in Extreme Programming

[[kent-beck]] stated the principle most directly in [[xp-explained-first-edition]] as the "40-hour week" practice: no overtime except in genuine emergencies, and never two weeks of overtime in a row. The framing was deliberately provocative in an industry that had normalized "crunch" as a professional norm. Beck's argument was not primarily ethical (though the ethical dimension is present) but practical: tired programmers make more mistakes, miss design opportunities, and produce code that requires more future rework. Overtime that creates technical debt is not a net gain.

## From "40-Hour Week" to "Sustainable Pace"

The language shift from [[xp-explained-first-edition]]'s "40-hour week" to the manifesto's "sustainable pace" reflects both a broadening and a softening. "Sustainable" acknowledges that some work may legitimately exceed 40 hours while preserving the direction: the test is whether the pace can be maintained, not whether a specific number is hit. [[xp-explained-second-edition]] retained the principle with the updated language.

The shift also reflects a concern that "40-hour week" was too culture-specific. In some national work cultures, the norm is below 40 hours; in others, professional identity is bound up with long hours in ways that make the literal prescription awkward. "Sustainable" is a more portable formulation.

## The Business Case

The sustainable pace principle rests on a specific empirical claim that contradicts conventional project management intuition: extended overtime does not reliably increase output. The evidence for this comes from several directions. Industrial fatigue research (predating software) showed that sustained overtime above ~50 hours/week produces declining marginal output within weeks as errors increase. Software-specific research on defect rates and developer cognitive performance corroborates the finding.

The deeper Agile argument is that velocity — measured in [[story-points]] or similar units — should be stable and predictable. Spikes of overtime followed by recovery produce variance that makes forecasting unreliable and planning deceptive. A team that honestly reports its sustainable [[velocity]] produces more actionable data than one that heroically overperforms for short periods.

## Relationship to [[dark-agile]] and the Industry

Sustainable pace is among the most commonly violated of the manifesto's principles. The organizational pressures that produce overtime — missed commitments, unrealistic estimates, death march project cultures — are precisely the conditions Agile claimed to address. When organizations adopt Scrum ceremonies without changing the underlying delivery pressure, Sprint planning becomes a ritual for committing to overtime rather than a tool for calibrating realistic scope. This pattern is a defining characteristic of [[dark-agile]].

The [[agile-industrial-complex]] largely ignores sustainable pace. SAFe's PI Planning model and quarterly Agile Release Train commitments create organizational pressure that practitioners frequently report undermines the principle in practice.
