---
id: risk-management-as-risk-embracement
title: "Risk Management as Risk Embracement"
type: concept
tags:
- risk
- project-management
- uncertainty
- decision-making
links:
- target: critical-chain-project-management
  relation: related_to
  note: 'Both address project uncertainty: Goldratt through aggregated project buffers and critical chain scheduling; DeMarco through probabilistic risk management and organizational risk culture'
  kb: goldratt
- target: managing-variability
  relation: related_to
  note: "Managing variability (not eliminating it) is Reinertsen's formulation of DeMarco's risk embracement: both distinguish beneficial from harmful uncertainty and argue for capacity to absorb it"
  kb: reinertsen
- target: cost-of-delay
  relation: related_to
  note: "DeMarco's probabilistic scheduling in Waltzing with Bears aligns with Reinertsen's cost-of-delay framework: both make the economic cost of uncertainty explicit rather than hiding it behind single-point estimates"
  kb: reinertsen
importance: 7
metadata:
  first_appeared: "waltzing-with-bears"
  key_writings: &id001
  - waltzing-with-bears
  - slack
  - the-deadline
  related_concepts: &id002
  - slack-concept
  - organizational-learning-disability
  - peopleware-thesis
  research_status: draft
first_appeared: "waltzing-with-bears"
key_writings: *id001
related_concepts: *id002
research_status: draft
---

Risk management as risk embracement is DeMarco and [[timothy-lister|Lister]]'s central argument in [[waltzing-with-bears]] (2003): genuine risk management means making risks explicit, probabilistic, and actively managed — not suppressing, ignoring, or downplaying them. Organizations typically treat risk identification as threatening and risk-avoiders as pessimists; DeMarco and [[timothy-lister|Lister]] invert this, arguing that refusing to name risks is the actual threat, and that embracing probabilistic uncertainty is the only path to making sound project commitments.

## The Core Argument

The standard organizational treatment of project risk is denial and suppression. Risk identification is unwelcome because:

- Named risks become commitments to address them
- Admitting uncertainty challenges the premise that projects can be planned with precision
- Risk-aware project managers are often perceived as negative or uncommitted by executives who want confident delivery promises
- Organizations that promise delivery dates without naming risks shift accountability to teams, who then face failure alone when unacknowledged risks materialize

DeMarco and [[timothy-lister|Lister]] argue that this dynamic produces a systematic pathology: risks that are real but unnamed are also risks that cannot be managed. An unacknowledged schedule risk cannot be mitigated, contingency-planned, or communicated to stakeholders in time to adjust scope. When it materializes, it arrives as a surprise that the organization is structurally unprepared to handle — and the [[organizational-learning-disability]] ensures that the failure to name it early is not traced back to whoever created the suppression pressure.

## Risk Embracement vs. Risk Avoidance

DeMarco and [[timothy-lister|Lister]] distinguish risk embracement from risk avoidance. Risk avoidance means refusing to take on projects with significant uncertainty — which in software development would mean refusing virtually all interesting work. Risk embracement means:

1. **Identifying risks explicitly** — naming the specific ways a project might go wrong, who bears each risk, and what the trigger conditions are
2. **Quantifying risks probabilistically** — moving from "this might slip" to "there is a 60% chance this ships before December and a 90% chance it ships before March," using distributions rather than point estimates
3. **Communicating risks to stakeholders** — making risk information available to the people who need it for planning and decision-making, rather than absorbing it within the project team
4. **Planning for risk outcomes** — developing contingency responses before risks materialize, so the organization can respond quickly when they do

The "waltzing with bears" title refers to an old trapper's saying: if you must walk through bear country, you are better off knowing the bears are there. The alternative — pretending there are no bears — does not reduce the risk; it just ensures you are surprised when the bear appears.

## Probabilistic Thinking in Project Planning

One of [[waltzing-with-bears]]'s methodological contributions is the application of probability distributions to project schedule estimation. Rather than committing to a single delivery date, DeMarco and [[timothy-lister|Lister]] argue for presenting a range: the earliest plausible date, the most likely date, and the date by which delivery is nearly certain — with probabilities attached.

This framing does several things:

- It forces explicit acknowledgment that uncertainty exists, which is factually accurate and intellectually honest
- It gives stakeholders information they need to make contingency plans
- It creates a basis for negotiating scope: if stakeholders need a date earlier than the most-likely estimate, they need to reduce scope or increase resources, and the probability distribution makes that tradeoff visible
- It shifts the success criterion from "did we hit the exact date we named?" to "did the outcome fall within the probability range we described?" — which is a much fairer accountability structure

## Why Organizations Suppress Risk Information

DeMarco and [[timothy-lister|Lister]] spend considerable time in [[waltzing-with-bears]] explaining why risk information is systematically suppressed even in organizations that nominally practice risk management. The mechanisms include:

- **Executive pressure for certainty.** Managers who tell their leadership "we have a 50% chance of hitting the date" are often responded to with "give me a plan that guarantees the date," which creates pressure to produce false certainty rather than honest uncertainty.
- **Shoot-the-messenger dynamics.** In organizations where bad news is punished, the rational response is to not surface bad news — including risk information — until it becomes undeniable.
- **Conflation of risk with failure.** Naming a risk is interpreted as admitting weakness or lack of commitment rather than as responsible planning. This conflation is strongest in organizations operating on the [[spanish-theory-of-management]], where confidence and effort are the expected responses to all challenges.
- **Diffusion of ownership.** When no one owns a specific risk — who is watching it, who decides when it has materialized, who has authority to execute the contingency plan — risk lists become performative documents rather than management tools.

## Connection to Slack

The risk embracement argument requires organizational [[slack-concept]] to be actionable. A risk management program that correctly identifies a 30% probability of schedule extension is useless if the organization has no reserved capacity to absorb that extension. Risk contingency planning requires slack — unallocated time, budget headroom, or scope flexibility — and organizations that have eliminated all slack have simultaneously eliminated their ability to respond to risks when they materialize.

DeMarco makes this connection explicit in [[slack]]: the efficiency-maximization impulse that drives out slack is the same impulse that makes genuine risk management impossible. You cannot maintain a 100%-utilized organization and also maintain meaningful risk reserves.

## Influence

The risk embracement framework anticipates several later developments in software project management. Agile's emphasis on iterative delivery — which produces frequent checkpoints at which risk can be assessed and scope can be adjusted — is a structural response to the same problem DeMarco and [[timothy-lister|Lister]] identify: long-horizon commitments made under false certainty. The Monte Carlo simulation techniques later popularized in quantitative project management are a direct descendant of the probabilistic planning approach [[waltzing-with-bears]] advocates.

DeMarco and [[timothy-lister|Lister]] were early in naming the organizational sociology of risk suppression — the political and cultural dynamics that prevent technically sound risk analysis from changing project behavior — which distinguishes [[waltzing-with-bears]] from purely technical treatments of project uncertainty.
