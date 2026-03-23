---
id: docker-inc
title: "Docker, Inc."
type: organization
importance: 5
tags:
- devops
- containers
- infrastructure
- tooling
org_type: company
founded: "2013"
location: "San Francisco, California"
key_figures: []
url: ""
research_status: draft
---

Docker, Inc. is the company that made Linux containers mainstream, transforming how software is packaged, distributed, and deployed. Its tool, Docker, became one of the defining infrastructure technologies of the mid-2010s DevOps mainstream adoption period.

The company originated as dotCloud, a platform-as-a-service provider. Solomon Hykes presented Docker at PyCon 2013 — at the time it was an internal tool for building and running containers. The presentation demonstrated a way to package an application with all its dependencies into a portable, isolated container that would run consistently across different environments. The response was immediate and significant; Docker rapidly became the most-watched project on GitHub.

Docker's DevOps significance lies in solving a specific and persistent problem: the gap between "it works on my machine" (development) and "it works in production" (operations). Containers create a standard packaging format that is consistent across development, testing, and production environments, eliminating the class of failures caused by environment differences. This made [[continuous-delivery]] pipelines more reliable and made [[infrastructure-as-code]] more tractable for application deployment (as distinct from server configuration management).

Docker Hub (the public container registry) and Docker Compose (multi-container application definition) extended the tool from individual containers to full application stacks and created the distribution infrastructure that made containers a standard unit of software delivery.

The orchestration layer — how to run many containers across many machines — was initially addressed by Docker Swarm, but Kubernetes (open-sourced by Google in 2014) won that competition decisively. The Kubernetes ecosystem built on Docker's container format while superseding Docker's own orchestration approach. This is a significant qualification on Docker's technical influence: it defined the container format and the cultural practice of containerization, but not the operational infrastructure that runs containers at scale.

[[john-willis]] served as Evangelist at Docker, connecting the company's tooling to the DevOps community narrative. Docker's tooling era (2013-2017 roughly) coincides with the mainstream enterprise adoption phase of DevOps, when the cultural movement acquired a standardized technical infrastructure.

Docker Inc. has had significant financial difficulties and several ownership changes. The company's institutional trajectory is complex and does not reflect the enduring cultural influence of the container format it created.
