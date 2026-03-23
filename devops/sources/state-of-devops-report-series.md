---
id: state-of-devops-report-series
title: "State of DevOps Reports (2013-present)"
type: source
importance: 9
tags:
- empirical-research
- dora-metrics
- survey-research
- puppet-labs
source_type: survey
date: 2013-01-01
author: nicole-forsgren
research_status: draft
---

Annual survey-based research reports that constitute the empirical backbone of the DevOps movement. Started in 2013 by Puppet Labs with [[nicole-forsgren]] as research partner. The series generated the data that became [[accelerate-book]] (2018).

## Origins and Early History

Puppet Labs (a configuration management tool vendor) commissioned the first State of DevOps Report in 2013 as a practitioner survey. Forsgren, then a professor of information systems, designed the research methodology — using rigorous psychometric scale construction and structural equation modeling rather than the simple correlation analysis typical of industry surveys.

The reports grew rapidly: by 2014-2015, the survey was receiving tens of thousands of responses annually, making it the largest empirical study of software delivery practices in existence.

## The Fork (2017)

In 2017, the series forked:

- **Puppet continued** their own "State of DevOps" report, focused on practitioner adoption and tooling trends
- **DORA (DevOps Research and Assessment)**, the organization Forsgren, [[jez-humble]], and [[gene-kim]] had founded, continued publishing research reports under the DORA brand

The DORA reports maintained Forsgren's rigorous methodology and became the primary source for the causal findings in [[accelerate-book]].

## Google Acquisition (2018)

Google acquired DORA in 2018 ([[google-acquires-dora-2018]]). The State of DevOps Reports have continued under Google's sponsorship, with Forsgren leading research until her departure to Microsoft Research. The reports continue as of this writing, now called the DORA State of DevOps Report.

## What the Reports Proved

The central finding that distinguished this research from all prior DevOps advocacy: elite software delivery organizations deploy on demand (multiple times per day) AND have lower change failure rates than low-performing organizations that deploy monthly or quarterly. Speed and stability are not in tension — they are correlated.

This finding, replicated across multiple years with different survey populations, is the empirical foundation for the DevOps movement's claims. It is the reason [[accelerate-book]] could be written.

## The Four Key Metrics

The research identified four metrics (the [[dora-four-key-metrics]]) that both measure software delivery performance and predict organizational performance (measured by profitability, market share, and productivity):

- Deployment Frequency
- Lead Time for Changes
- Change Failure Rate
- Time to Restore Service

A fifth metric (Reliability/Operational Performance) was added to the framework in later reports (approximately 2021).

## Unique Contribution

The State of DevOps Reports are the primary empirical source for DevOps claims. Every other foundational DevOps text ([[the-phoenix-project]], [[the-devops-handbook]], [[continuous-delivery-book]]) is prescriptive or descriptive; this series is the causal evidence base.
