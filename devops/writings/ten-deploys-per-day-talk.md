---
id: ten-deploys-per-day-talk
title: "10+ Deploys Per Day: Dev and Ops Cooperation at Flickr"
type: writing
importance: 9
tags:
- founding-moment
- continuous-delivery
- dev-ops-cooperation
- flickr
writing_type: talk
date: 2009-06-23
author: john-allspaw
coauthors:
- Paul Hammond
publisher: "Velocity Conference 2009"
key_concepts:
- continuous-delivery
- dev-ops-cooperation
research_status: draft
---

The catalyzing talk of the DevOps movement. Presented by [[john-allspaw]] (VP Engineering, Flickr) and Paul Hammond (Director of Engineering, Flickr) at [[velocity-conference]] on June 23, 2009.

The talk demonstrated that developers and operations could work together using shared tools, shared metrics, and shared on-call responsibilities to deploy to production more than ten times per day — at a time when many organizations deployed monthly or quarterly.

## Why This Talk Was Catalyzing

The talk arrived at a moment when Agile development had been established in many organizations, but the dev-ops wall remained: developers delivered code, operations deployed it, and each blamed the other when things went wrong. Allspaw and Hammond showed not only that the wall could come down, but that it could come down at scale (Flickr had millions of users) with measurable improvement in both velocity and stability.

[[patrick-debois]], who would found [[devopsdays-conference]] four months later at [[first-devopsdays-ghent-2009]], watched the talk via livestream. By his own account, this talk was the immediate catalyst for organizing the first DevOpsDays event. The connection from this talk to the naming of the "DevOps" movement runs directly through Debois.

## Content

The talk covers:

- **Shared metrics**: Dev and ops using the same dashboards to see what's happening in production
- **Shared tools**: IRC bots announcing deployments, Ganglia for graphs, Nagios for alerts — all accessible to both teams
- **Feature flags**: Deploying code that is not yet activated, enabling gradual rollout and instant rollback
- **Shared on-call**: Developers participating in on-call rotations rather than throwing code over the wall
- **Blameless culture**: The framing that deployments going wrong is a systems problem, not an individual failure

## Relationship to Subsequent DevOps Texts

The practices Allspaw and Hammond described — feature flags, shared metrics, collaborative deployment — were codified in [[continuous-delivery-book]] (2010) and [[the-devops-handbook]] (2016). Etsy, where Allspaw subsequently became CTO, became a canonical DevOps case study and the source of the "blameless postmortem" practice that [[john-allspaw]] systematized.

The talk is available as slides (with extensive speaker notes) at slideshare; the video was hosted on the Velocity Conference site.
