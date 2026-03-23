---
id: version-control-everything
title: "Version Control Everything"
type: practice
importance: 7
tags:
- infrastructure
- auditability
- reproducibility
- dora-predictor
- first-way
practice_type: infrastructure
originated_in: "Continuous Delivery (Humble/Farley, 2010)"
evidence_base: "DORA/Accelerate: version control for both application code and system configuration is a predictor of performance"
related_practices:
- continuous-integration
- deployment-automation
status: active
research_status: draft
---

"Version control everything" is the discipline of maintaining every artifact required to build, test, and deploy a system under version control — not just application source code, but infrastructure configuration, database schema migrations, build scripts, test scripts, deployment scripts, and environment definitions. The principle: if it is not in version control, it cannot be reproduced reliably, audited systematically, or restored confidently.

## Beyond Application Code

Version control for application source code has been standard engineering practice since at least the 1970s (SCCS, 1972; RCS, 1982; CVS, 1990; Subversion, 2000; Git, 2005). The DevOps extension is to apply the same discipline to everything else in the delivery system:

**Infrastructure configuration**: server provisioning scripts, configuration management code (Puppet manifests, Chef recipes, Ansible playbooks), cloud infrastructure definitions (Terraform, CloudFormation, Pulumi). If your server configuration is in a configuration management tool but the configuration management code is not in version control, you cannot reproduce the environment reliably or roll back infrastructure changes.

**Database schemas**: schema migration scripts managed by tools like Flyway, Liquibase, Active Record migrations, or Alembic. Without version-controlled migrations, the schema becomes an undocumented artifact that drifts between environments and cannot be reliably reproduced from scratch.

**Build scripts**: the scripts and configurations that compile, lint, test, and package the application. Makefile, Dockerfile, CI configuration files (.travis.yml, .github/workflows/*.yml, Jenkinsfile). These define how the artifact is produced; they must be version-controlled alongside the code they build.

**Test scripts and test data**: automated test suites, test fixtures, seed data definitions. Tests that are not in version control cannot be reproduced or evolved systematically alongside the code they test.

**Deployment scripts**: the scripts and configurations that move the artifact to production — Capistrano configuration, Kubernetes manifests, Helm charts, ArgoCD application definitions.

## Origins in Continuous Delivery

[[jez-humble]] and [[david-farley]]'s [[continuous-delivery-book]] (2010) made "version control everything" an explicit principle. Their argument: the [[deployment-pipeline]] requires a single source of truth from which every environment can be reproduced deterministically. If any piece of the system — configuration, schema, infrastructure — is not version-controlled, that reproducibility is broken. You cannot have a reliable pipeline built on an unversioned foundation.

The book treated this as a prerequisite, not an advanced practice: you cannot do continuous delivery if you cannot reproduce your environments, and you cannot reliably reproduce your environments without version control for everything that defines them.

## Infrastructure as Code

[[infrastructure-as-code]] (IaC) is the conceptual extension of "version control everything" to infrastructure specifically: infrastructure is defined as code (Terraform HCL, CloudFormation YAML, Kubernetes manifests), stored in version control, and applied through [[deployment-automation]] rather than through manual console operations. Version control everything is the discipline; IaC is the practice that implements it for the infrastructure layer.

Without version control, infrastructure configuration lives in the heads of the operators who applied it, in wikis, or in undocumented console state. These "snowflake" environments — unique, hand-crafted, unreproducible — are a source of both operational fragility and delivery friction.

## Connection to the First Way

[[three-ways]] First Way: version control creates the single source of truth that enables automated pipelines to operate without human judgment about what to build, how to build it, or what to deploy where. The pipeline starts with a commit to version control and proceeds deterministically through every stage. If any stage depends on configuration that is not in version control, the pipeline has an external dependency that breaks the determinism.

This is the lean concept of standardization: you cannot improve a process you cannot describe precisely, and you cannot describe it precisely if it is not captured in a reproducible form. Version control is the mechanism for capturing that precise description and making it evolvable.

## Auditability and Compliance

Version control provides a complete audit trail: every change to every file, with author, timestamp, and commit message. For regulated industries, this is directly relevant to compliance requirements — SOC 2, PCI DSS, and HIPAA all require evidence of change management and access control. Version-controlled infrastructure configuration, reviewed through pull requests, provides that evidence automatically. The alternative — manual change logs, ticketing systems, or configuration management databases (CMDBs) — requires separate record-keeping that is always at risk of being out of sync with the actual system state.

## DORA Evidence

[[accelerate-book]] identifies version control for both application code and system configuration as a predictor of software delivery performance. The finding is not just that version control for application code matters (this is table stakes), but that extending version control to system configuration is an additional discriminating factor. High performers are more likely to have their infrastructure and configuration in version control than low performers, and this correlates with higher Deployment Frequency and lower Lead Time for Changes.

The [[state-of-devops-report-series]] has tracked this finding over multiple years. The mechanism: version-controlled configuration enables [[deployment-automation]] to be comprehensive (nothing is manually applied outside the pipeline) and enables recovery to be fast (rollback a configuration change as easily as rolling back a code change).

## Git and the Ecosystem

Git's dominance (from approximately 2010 onward, accelerated by GitHub's launch in 2008) standardized the version control tool and created an ecosystem of tooling built around Git workflows: CI systems that trigger on Git events, code review tools (pull requests/merge requests), GitOps patterns (where the desired state of infrastructure is expressed in a Git repository and reconciled automatically by tooling like ArgoCD or Flux). "GitOps" (coined by Weaveworks, 2017) makes version control the operational control plane — every infrastructure change is expressed as a Git commit, reviewed, and applied automatically. This is "version control everything" as a complete operational philosophy, not just a development practice.
