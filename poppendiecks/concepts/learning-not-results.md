---
id: learning-not-results
title: Learning Not Results
type: concept
tags:
- lean-software-development
- learning
- organizational-leadership
- systems-thinking
- foundational-insight
links:
- target: pdsa-cycle-plan-do-study-act
  relation: influenced_by
  note: PDSA is the operational mechanism for the learning-not-results philosophy
  kb: deming
- target: system-of-profound-knowledge
  relation: influenced_by
  note: Deming's SoPK is the theoretical framework underpinning the learning thesis
  kb: deming
- target: ooda-loop
  relation: related_to
  note: OODA as a learning loop — orientation is where competitive advantage is built
  kb: boyd
- target: orientation
  relation: related_to
  note: Boyd's orientation phase parallels learning as primary value stream
  kb: boyd
- target: customer-development
  relation: related_to
  note: Blank's validated learning is the startup expression of learning-not-results
  kb: blank
- target: lean-startup
  relation: related_to
  note: Lean Startup's Build-Measure-Learn derives from the learning-as-value thesis
  kb: blank
importance: 10
first_appeared: 'Leading Lean Software Development: Results Are Not the Point (2009)'
tps_source: kaizen (continuous improvement) as an organizational learning system;
  Deming's PDCA cycle
key_writings:
- leading-lean-software-development-2009
- lean-software-development-agile-toolkit-2003
- implementing-lean-software-development-2006
related_concepts:
- amplify-learning
- seven-lean-principles
- optimize-the-whole
- empower-the-team
- eliminate-waste
research_status: draft
---

"Learning not results" is the organizing thesis of [[leading-lean-software-development-2009]] by [[mary-poppendieck]] and [[tom-poppendieck]], captured in the book's subtitle: *Results Are Not the Point*. It represents the fullest development of the insight that [[amplify-learning]] introduced in 2003: that in software development, learning is not a means to producing results but the primary thing being produced. Managing for results, on this account, is a systematic category error that undermines the organizational capacity for long-run performance.

## The Thesis

The conventional management view holds that organizations exist to produce results — revenue, features shipped, customer satisfaction scores, cycle time metrics. Learning and capability-building are instrumentally valuable insofar as they improve results. On this model, investing in learning at the expense of short-term results is a trade-off to be made carefully, and usually reluctantly.

The Poppendiecks invert this. In software — and in any domain where the primary competitive variable is knowledge — *organizational learning capacity is the result*. The features shipped, the customers served, the metrics achieved are evidence of learning, not the point. Organizations that optimize for result metrics while neglecting learning capacity are drawing down an epistemic reserve that they are not replenishing. Short-term results improve; long-term capability degrades.

This is not a soft argument about work culture or employee happiness. It is a claim about what software organizations are actually for, and therefore what they should measure and manage.

## Connection to Deming's PDCA

[[w-edwards-deming]]'s Plan-Do-Check-Act cycle is one of the Poppendiecks' primary intellectual antecedents. Deming argued that all improvement is learning: the PDCA cycle is a systematic learning loop — plan an intervention, do it, check whether it worked, act on what was learned. Organizations that skip the Check and Act steps — executing plans without learning from them — cannot improve because they have no mechanism for incorporating feedback.

Deming's System of Profound Knowledge identifies knowledge as one of the four foundational domains (alongside appreciation for a system, understanding of variation, and psychology). For Deming, managing without knowledge of what is actually happening in the system produces management by results — and management by results, he argued famously, destroys an organization.

## Connection to Boyd's OODA

John Boyd's OODA loop (Observe-Orient-Decide-Act) arrives at a similar conclusion from a military strategy context. Boyd argued that competitive advantage in conflict — as in business — comes from cycling through the OODA loop faster and with better orientation than the opponent. The orientation stage is where learning happens: incorporating new observations into an updated model of the world. Organizations with poor orientation (poor learning loops) will make systematically bad decisions even if they are observing and acting quickly.

The Poppendiecks drew this connection explicitly: the competitive advantage of lean software development is not faster feature production but faster learning cycles. An organization that can learn faster than its competitors will eventually outperform them even if it starts behind, because it will converge on the right products, architectures, and processes faster.

## Connection to Blank's Validated Learning

Steve Blank's customer development methodology, developed in the late 1990s and early 2000s, arrived independently at the same insight in the context of startups: the purpose of a startup is not to execute a business plan but to *learn* whether a business plan is viable. Blank's "get out of the building" discipline is a structured learning loop — form hypotheses about customer needs, test them with real customers, update the hypotheses based on what you learn.

Eric Ries formalized this into the Build-Measure-Learn loop in the Lean Startup (2011), naming Blank as a direct influence. The lineage from Deming through the Poppendiecks through Blank to Ries is the learning-as-primary-value insight moving from manufacturing quality management to software development to startup methodology — each translation retaining the core insight while adapting its expression to a new domain.

## Organizational Implications

The practical implications of "results are not the point" are radical for organizational design:

**Measurement systems.** If learning is the point, the most important metrics are learning-rate metrics — not features shipped per sprint but quality of feedback per cycle, or how often teams update their models of customer needs. Current agile metrics (velocity, burndown, cycle time) are result proxies. Learning metrics are harder to measure but more meaningful.

**Incentive structures.** Incentivizing individuals and teams on result metrics — feature counts, code production, story points — creates pressure to protect result metrics at the expense of learning investments. Teams that learn they can boost velocity by cutting test coverage, or accelerating delivery by reducing refactoring, will do so if incentives reward velocity. This is the organizational mechanism by which results-focus destroys learning capacity.

**Leadership role.** [[empower-the-team]] argued for servant leadership; learning-not-results extends this: leaders in a lean organization are primarily responsible for building and protecting learning capacity — creating psychological safety for experiments that might fail, investing in feedback infrastructure, and resisting short-term result pressure that would sacrifice learning investment.

**What counts as failure.** In a results-focused organization, a project that does not ship is a failure. In a learning-focused organization, a project that ships quickly but teaches nothing is the failure — and a project that fails to ship but produces decisive knowledge about what customers actually need is a success.

## The Lineage: Deming to Boyd to Blank to Ries

The Poppendiecks' "learning not results" thesis sits at the intersection of several independent traditions that converged on the same insight:

- [[w-edwards-deming]]: Quality improvement is a learning system (PDCA). Managing by results destroys the learning capacity that produces quality.
- Boyd: Competitive advantage is faster learning cycles (OODA). Orientation — the learning stage — is where the advantage is built.
- Blank: Startup success is validated learning (customer development). The pivot is not a failure; it is evidence of learning.
- [[eric-ries|Ries]]: Build-Measure-Learn is the software product development cycle.

The Poppendiecks' contribution is to have articulated this insight most clearly in the context of software *organizations* — not just methodologies or tactics — and to have connected it to the lean manufacturing tradition through Deming and TPS. This makes [[leading-lean-software-development-2009]] the most philosophically ambitious of their three books, moving from "how to apply lean to software" (2003) to "how to implement lean practices" (2006) to "what lean means for how organizations should be led" (2009). The Poppendiecks continued developing these themes in [[the-lean-mindset-2013]], which broadened the argument from software to organizational capability, and in late essays like [[grown-up-lean-essay-2019]] on [[lean-essays-blog]]. A [[tech-lead-journal-poppendieck-interview-2021|2021 podcast interview]] captures their mature perspective on this trajectory.
