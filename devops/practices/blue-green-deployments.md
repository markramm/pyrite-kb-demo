---
id: blue-green-deployments
title: "Blue-Green Deployments"
type: practice
importance: 5
tags:
- delivery
- zero-downtime
- rollback
- deployment-risk
- continuous-delivery
practice_type: delivery
originated_in: "Described in Continuous Delivery (Humble/Farley, 2010); practiced earlier at various organizations"
related_practices:
- deployment-automation
- canary-releases
status: active
research_status: draft
---

Blue-green deployment is a release technique that eliminates deployment downtime and minimizes rollback time by maintaining two identical production environments: blue (currently live) and green (currently idle). To deploy a new version, you configure and test it in the idle environment, then switch traffic from the live environment to the idle one. If something is wrong, you switch traffic back — rollback takes seconds, not the minutes or hours of a traditional rollback deployment.

## Mechanics

The pattern requires a load balancer or traffic router that can switch between the two environments. In the simplest form:

1. Blue is live; green is idle and running the previous version.
2. Deploy the new version to green. Run smoke tests and validation against green while blue continues serving production traffic.
3. Switch the load balancer from blue to green. Green is now live.
4. Blue is now idle, still running the previous version. If problems appear in green, switch back to blue instantly.
5. Once confident in green, update blue with the new version for the next deployment cycle.

The environments alternate roles: blue is live one cycle, green the next. The key property is that the switch is instantaneous from the user's perspective — no deployment window, no downtime, no "maintenance mode."

## Origins

[[continuous-delivery-book]] (Humble/Farley, 2010) documented blue-green deployments as a pattern within the [[deployment-pipeline]] design. The practice predates the book — Amazon and other high-volume web operations were using variants of this approach in the mid-2000s — but Humble and Farley gave it the naming convention and systematic treatment that made it part of the DevOps vocabulary.

The pattern was made practical by the growth of virtualization and later cloud infrastructure: maintaining two identical environments is only economical when you can provision and deprovision them programmatically. [[infrastructure-as-code]] is the enabling practice: if you define both environments as code, you can guarantee they are actually identical rather than drifting over time.

## Connection to Feedback and Risk Reduction

The blue-green pattern directly addresses deployment risk. One of the barriers to high deployment frequency is the fear that deployments will cause production incidents — and that recovering from those incidents will take a long time. Blue-green deployments remove both fears:

- If the new version fails, rollback is instantaneous (switch the load balancer back).
- The new version can be validated in a production-equivalent environment before any users are affected.

This connects to the [[three-ways]] Second Way: the ability to switch back quickly means the feedback loop on a bad deployment is very short. You detect the problem (via [[monitoring-and-observability]]), switch back, and are back to a known-good state within minutes. Traditional deployments, where rollback means re-deploying the previous artifact, can take much longer.

## Database Schema Challenges

The hardest problem with blue-green deployments is database migrations. Both environments typically share a database; if the new version requires a schema change that is incompatible with the old version, you cannot run both simultaneously. The standard solution is backward-compatible schema migrations: expand-contract pattern (first expand the schema to support both versions, deploy the new application, then contract by removing old schema elements). This requires discipline in schema design but makes blue-green feasible even with database-heavy applications.

## Relationship to Canary Releases

[[canary-releases]] are more granular than blue-green: instead of switching 100% of traffic from one environment to another, canaries route a small percentage to the new version and gradually increase. Blue-green is binary (all or nothing); canary is progressive. The two are complementary: some organizations use a canary phase before the final blue-green switch to detect problems with realistic (but limited) production traffic before full cutover.

## Infrastructure Economics

Blue-green requires maintaining double the production infrastructure during the deployment window. For large systems, this cost can be significant. Cloud infrastructure and container-based deployments (Kubernetes) reduce this cost — you provision the "green" environment for the duration of the deployment, then deprovision it. AWS Elastic Beanstalk, Kubernetes rolling deployments (which can be configured to approximate blue-green semantics), and platforms like Spinnaker all implement variants of this pattern with cost management.

## Connection to Deployment Automation

Blue-green only provides its risk-reduction benefits if the deployment and traffic-switch operations are automated. A manual blue-green deployment — where someone must remember to run the right commands in the right order — reintroduces the variability that the pattern is meant to eliminate. [[deployment-automation]] is the prerequisite: blue-green is a deployment strategy; automation is what makes it reliable.
