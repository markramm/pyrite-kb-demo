---
id: security-is-a-process
title: Security Is a Process
type: concept
tags:
- core
- foundational
- methodology
- process-thinking
links:
- target: pdsa-cycle-plan-do-study-act
  relation: related_to
  note: Schneier's 'security is a process, not a product' echoes Deming's PDSA cycle — continuous improvement rather than one-time fixes
  kb: deming
- target: ooda-loop
  relation: related_to
  note: Both reject static achievement in favor of continuous adaptive cycles. 'Process not a product' is the security version of Boyd's argument that tempo beats position
  kb: boyd
- target: pdsa-ooda-parallel-iterative-learning-cycles-across-domains
  relation: related_to
  note: The Deming KB identifies the PDSA-OODA parallel; Schneier extends the same iterative-learning-cycle insight into security — a three-way convergence
  kb: deming
- target: strategy-cycle
  relation: related_to
  note: Wardley's strategy cycle and Schneier's security-as-process both reject one-time analysis in favor of continuous iterative cycles
  kb: wardley
- target: security-through-design
  relation: related_to
  note: 'Both converge: security cannot be added by surveillance alone but must be built in through design. Written in the same post-9/11 context'
  kb: red-rock-eater
importance: 9
metadata:
  first_appeared: the-process-of-security
  key_writings: &id001
  - the-process-of-security
  - secrets-and-lies
  - beyond-fear
  - schneier-on-security-book
  related_concepts: &id002
  - security-mindset
  - threat-modeling
  - security-theater
  - security-economics
  - attack-trees
  research_status: draft
first_appeared: the-process-of-security
key_writings: *id001
related_concepts: *id002
research_status: draft
---

"Security is a process, not a product" is one of Schneier's most quoted formulations — a compact challenge to the dominant commercial framing of security in the 1990s, when software vendors sold encryption tools, firewalls, and antivirus programs as solutions that, once purchased and deployed, could be crossed off a security checklist. The aphorism is from the essay [[the-process-of-security]] (2000), published as [[secrets-and-lies]] was completing its argument, and it anchors a cluster of related ideas about how organizations should think about maintaining security over time.

## The Essay and Its Argument

[[the-process-of-security]] is a short but significant essay in which Schneier argues that:

1. **No product provides complete security.** Every security product has vulnerabilities, and adversaries adapt. A firewall that is impenetrable today may be compromised tomorrow through a newly discovered vulnerability, a misconfiguration, or a social engineering attack that bypasses it entirely.

2. **Deployment is not the end of the problem.** Installing a security product often creates a false sense of completion. Organizations stop paying attention to security after the purchase — but attention is precisely what security requires continuously.

3. **Attacks evolve.** The threat landscape changes. New attack techniques emerge, new vulnerabilities are discovered in deployed systems, new adversaries with new motivations appear. A security posture that was appropriate last year may be inadequate today through no change in the defended system.

4. **Security requires ongoing assessment and response.** What this implies is a security practice, not a security purchase: continuous monitoring, periodic reassessment of threat models, rapid response to newly discovered vulnerabilities, and regular iteration on countermeasures.

## Connection to Secrets and Lies

[[secrets-and-lies]] (2000) is the extended argument behind this aphorism. The book opens with Schneier's repudiation of his earlier work: [[applied-cryptography]] (1994) had (unintentionally, he argues) conveyed that cryptography was the solution to security problems. By the late 1990s, Schneier had concluded that this was precisely wrong. Systems with excellent cryptographic designs were failing in practice — not because the cryptography was broken, but because the surrounding systems (the people, processes, interfaces, administration, physical access) were not treated as part of the security problem.

The "process not a product" formulation is the punch-line of this argument: cryptography and security products are necessary but never sufficient components of a functioning security posture. The posture itself requires ongoing work.

## Implications for Organizations

The process framing has specific organizational implications that Schneier develops across multiple writings:

**Security as a function, not a project.** A project ends; a function continues. Organizations that treat security as a project — "we need to do our annual security review" — are implicitly treating it as a product purchase. Organizations that treat it as an ongoing function build the monitoring, detection, and response capabilities that security actually requires.

**The importance of detection and response.** If no product provides perfect prevention, then the ability to detect compromise and respond quickly becomes critical. Schneier argues that organizations systematically underinvest in detection and response relative to prevention, because detection and response are ongoing operational costs while prevention can be framed as a capital purchase. This is a classic [[security-economics]] distortion.

**Metrics and measurement.** A process can be monitored and improved; a product either works or it doesn't. The process framing implies that organizations should measure security continuously — incident rates, time to detection, response effectiveness — rather than treating security as a binary state.

**The role of iteration.** Processes improve through feedback loops. After a security incident, the process is analyzed, the weakness is identified, and the process is improved. This is fundamentally different from the product mindset, where a breach means the product failed and should be replaced.

## Relationship to Deming and Process Thinking

Schneier does not cite W. Edwards Deming explicitly, but the "security is a process" framing has a structural homology with Deming's argument that quality requires process management, not product inspection. Both arguments target the same organizational failure mode: the belief that problems can be solved through a one-time intervention (purchasing a product, inspecting finished goods) rather than through continuous process improvement. The connections to systems thinking and process orientation in the Deming tradition are intellectually real even if not textually documented.

## Tension with the Security Product Industry

The aphorism was pointed directly at the commercial interests of the security industry that Schneier was part of. He had co-founded [[counterpane-internet-security]] and was building a business in managed security services — a recurring-contract model that embodies the process framing. The "product not a process" critique is simultaneously a statement about security practice and a business model argument: organizations should be buying ongoing security services, not one-time security installations.

This dual role — intellectual critique and business rationale — is characteristic of Schneier's work at the turn of the century. [[secrets-and-lies]] is dedicated to making the reader a more sophisticated buyer and user of security, which is also a way of making them a better customer for the services Counterpane was selling.

## Later Elaborations

The concept deepens in [[beyond-fear]] (2003), where Schneier adds the cost-benefit dimension: security processes should be continuously evaluated for their effectiveness and adjusted when the cost-benefit analysis shifts. A process that was cost-effective when attacks were rare may not be when attacks become common; a process optimized against one class of adversary may be inadequate against a newly emerging class.

In subsequent years, the concept became the intellectual foundation for discussions of incident response, security operations centers, threat intelligence programs, and DevSecOps — all of which operationalize the insight that security is continuous work rather than a one-time achievement.
