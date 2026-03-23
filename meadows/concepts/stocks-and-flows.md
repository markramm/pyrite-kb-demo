---
id: stocks-and-flows
title: Stocks and Flows
type: concept
tags:
- system-dynamics
- accumulation
- rates
- foundational
links:
- target: systems-thinking-fifth-discipline
  relation: related_to
  note: Stocks and flows are the foundational building blocks Senge's Fifth Discipline
    systems thinking rests on
  kb: senge
- target: causal-loop-diagrams
  relation: related_to
  note: Causal loop diagrams are simplified representations of stock-and-flow structures;
    Senge favored CLDs for accessibility
  kb: senge
- target: beer-game
  relation: related_to
  note: Beer game demonstrates stock-and-flow dynamics (inventory accumulation) and
    delays causing bullwhip oscillation
  kb: senge
- target: appreciation-for-a-system
  relation: related_to
  note: Stocks and flows are the formal language for the system interdependencies
    Deming said managers must appreciate
  kb: deming
- target: chain-reaction-diagram
  relation: related_to
  note: Deming's chain reaction (quality->costs->productivity->market) is a causal
    flow chain; stocks accumulate at each stage
  kb: deming
- target: throughput-accounting
  relation: related_to
  note: Throughput, inventory, and operating expense map to flows and stocks; Goldratt's
    metrics are stock-and-flow measures
  kb: goldratt
- target: queueing-theory-applied
  relation: related_to
  note: Queues are stocks; arrival and service rates are flows. Reinertsen's queuing
    theory is stock-and-flow dynamics applied to product development
  kb: reinertsen
- target: wip-constraints
  relation: related_to
  note: WIP is a stock; WIP constraints limit stock accumulation to prevent queue-driven
    delays — direct application of stock management
  kb: reinertsen
- target: flow-control
  relation: related_to
  note: Flow control manages the rates at which work moves through development stages
    — controlling flows to manage stocks
  kb: reinertsen
importance: 9
first_appeared: Industrial Dynamics (Forrester, 1961)
source_tradition: system dynamics
key_writings:
- thinking-in-systems-2008
- groping-in-the-dark-1982
related_concepts:
- feedback-loops
- delays-in-systems
- reinforcing-feedback-loops
- balancing-feedback-loops
- overshoot-and-collapse
research_status: draft
---

Stocks and flows constitute the fundamental grammar of system dynamics, the language through which [[jay-forrester]] at [[mit-system-dynamics-group]] taught systems behave over time. A **stock** is any quantity that accumulates or depletes — water in a bathtub, carbon dioxide in the atmosphere, money in a bank account, trust between institutions, population in a country. A **flow** is the rate at which a stock changes per unit of time: the faucet filling the tub, emissions adding to atmospheric CO₂, interest accruing, births minus deaths.

Meadows made this distinction central to [[thinking-in-systems-2008]], arguing that stocks give systems their inertia and memory. Because stocks change only through flows, and flows often respond to stocks with [[delays-in-systems]], systems cannot turn on a dime. This insight explains why attempts at rapid policy change so frequently produce frustrating results: the stock of CO₂ already in the atmosphere, the stock of infrastructure built for fossil fuels, the stock of trained personnel for an old technology — all of these resist sudden redirection.

The bathtub is Meadows's canonical teaching metaphor. The water level (stock) rises when the inflow (faucet) exceeds the outflow (drain). You cannot know the level without knowing both flows and their history. This seemingly simple insight dissolves a great deal of confused policy debate: people argue about flows (spending rates, emission rates, birth rates) while ignoring the accumulated stocks those flows are filling or depleting.

Stocks also create delays that produce oscillation. In [[overshoot-and-collapse]] dynamics, the stock of a resource declines before the feedback signals that drive reduced consumption can catch up — because those signals themselves flow through delays. The [[limits-to-growth-1972]] world model was essentially an argument about which stocks (population, industrial capital, pollution, resources, food production capacity) were on trajectories that would interact badly in the 21st century.

Forrester's formal notation — boxes for stocks, pipes for flows, valves for flow rates, clouds for sources and sinks outside the model boundary — became the visual vocabulary of system dynamics. Meadows inherited this grammar from her graduate work with Forrester and used it throughout her career, while consistently translating it into accessible language for non-technical audiences.

The practical upshot Meadows drew: before proposing any intervention in a system, map its stocks and flows. Ask what is accumulating, what is depleting, how fast, and through what mechanisms. The answer often reveals why the system is behaving as it is — and why simple, fast solutions tend to fail.
