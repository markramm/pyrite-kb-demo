---
id: dev-ops-cooperation
title: "Dev-Ops Cooperation"
type: concept
importance: 8
tags:
- culture
- collaboration
- wall-of-confusion
- shared-ownership
- founding-insight
concept_type: principle
first_appeared: "10+ Deploys Per Day talk (Allspaw/Hammond, 2009)"
key_writings:
- ten-deploys-per-day-talk
- the-phoenix-project
- the-devops-handbook
related_concepts:
- three-ways
- cams-framework
- blameless-postmortems
research_status: draft
---

Dev-ops cooperation is the founding insight of the DevOps movement: that developers and operations staff must collaborate continuously, share tools, share metrics, share responsibility, and share the consequences of their work — rather than throwing software over a wall from one group to the other.

## The Wall of Confusion

[[andrew-clay-shafer]] gave this structural antagonism a name: the Wall of Confusion. Developers wrote code and threw it over the wall to operations to deploy and maintain. Operations received the code, struggled to deploy it, scrambled to maintain it, and told developers nothing about what was failing in production. Developers had no visibility into operations; operations had no influence over development decisions. The wall between them created queues, delays, blame, and operational failures.

The Wall of Confusion is not a personality problem — it is a structural problem produced by separate organizational incentives. Developers are measured by feature velocity; operations are measured by stability. These metrics are in tension. Optimizing locally produces globally bad outcomes. The DevOps insight is that the organizational structure must change, not just the attitudes.

## The Flickr Demonstration

The specific moment that launched the movement: [[john-allspaw]] and [[paul-hammond]]'s talk at the Velocity conference in 2009, "10+ Deploys Per Day: Dev and Ops Cooperation at Flickr." The [[ten-deploys-per-day-talk]] demonstrated that Flickr was deploying to production more than ten times per day — a number that seemed impossible given conventional operations wisdom of the time, which treated production deployments as high-risk events requiring change control boards and multi-day freezes.

The mechanism was not purely technical. Flickr had built shared tooling (IRC bots that announced deployments to both dev and ops in the same channel), shared metrics (both teams saw the same production dashboards), shared on-call (developers participated in incident response), and a culture of mutual accountability. The Wall of Confusion had been knocked down — not by an attitude adjustment, but by shared infrastructure that aligned incentives.

[[patrick-debois]], watching the talk remotely, was galvanized. He organized the first DevOpsDays ([[first-devopsdays-ghent-2009]]) in Ghent later that year. The movement had a name and a founding moment.

## "You Build It, You Run It"

Werner Vogels, CTO of Amazon, articulated a complementary principle that became widely cited: "You build it, you run it." Amazon's service teams owned their services end-to-end — development, deployment, and production operation. There was no separate operations team to hand off to. The consequence was immediate: developers had to care about operability because they would be paged at 2 AM when it broke.

This organizational design change is the sharpest implementation of dev-ops cooperation. It eliminates the wall structurally rather than trying to paper over it with communication. But it requires significant investment in deployment tooling and on-call infrastructure to function without burning out the engineers.

## The CAMS Framework

[[cams-framework]] (Culture, Automation, Measurement, Sharing) identifies Culture as its first pillar, and dev-ops cooperation is what that culture means in practice. The cultural commitment is: shared ownership of the system's health from code commit to production operation. Automation, measurement, and sharing are the mechanisms; cooperation is the value they serve.

## The First Way

In Kim's [[three-ways]], dev-ops cooperation is a prerequisite for the First Way — fast flow from development to operations to the customer. The Wall of Confusion is a massive queue: work waits for handoffs, approvals, and deployment windows. Removing the wall removes the queue. Flow requires that dev and ops operate as a single system, not as two separate organizations negotiating across a boundary.

## Beyond Dev and Ops

[[the-phoenix-project]] extends the insight. The novel's protagonist discovers that the bottleneck is not just dev-ops cooperation but the broader organizational system: the business throws requirements over its own wall to IT, just as dev throws code over the wall to ops. The Three Ways require cooperation not just between dev and ops but across the entire value stream — business, development, and operations as a single system oriented around customer value. The "Dev-Ops" framing is the founding insight, but the full DevOps vision is a business-wide synthesis.
