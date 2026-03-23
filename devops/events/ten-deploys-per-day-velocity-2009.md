---
id: ten-deploys-per-day-velocity-2009
title: "10+ Deploys Per Day at Velocity 2009"
type: event
importance: 9
tags:
- flickr
- velocity-conference
- dev-ops-cooperation
- continuous-deployment
- founding-moment
date: 2009-06-23
location: "Velocity Conference, San Jose, California"
participants:
- john-allspaw
- paul-hammond
significance: "The talk that catalyzed the DevOps movement by demonstrating dev-ops cooperation at scale"
research_status: draft
---

June 23, 2009. [[john-allspaw]] (VP of Operations at Flickr) and Paul Hammond (Director of Engineering at Flickr) presented "10+ Deploys Per Day: Dev and Ops Cooperation at Flickr" at O'Reilly's [[velocity-conference]]. It became one of the founding documents of the DevOps movement.

**What they showed.** Flickr was deploying to production more than ten times per day — a frequency that the conventional IT wisdom of 2009 would have called reckless. Allspaw and Hammond demonstrated how they did it: shared tools between dev and ops (both groups had access to deployment systems and monitoring), shared metrics (everyone could see production health), shared IRC channels (communication was continuous and transparent), and — crucially — a culture where ops didn't automatically blame dev when things went wrong, and dev didn't throw code over a wall to ops.

The talk crystallized [[dev-ops-cooperation]] as a practice rather than a vague aspiration. It answered the implicit question: if Agile is about moving fast, what does moving fast look like in operations?

**The Belgium connection.** [[patrick-debois]] was watching the Velocity livestream from Belgium. The talk gave him the concrete example he had been missing — proof that the integration Shafer and he had discussed at [[agile-infrastructure-bof-2008]] was not merely theoretical. He began organizing what became [[first-devopsdays-ghent-2009]] within months.

**Intellectual contribution.** Allspaw's framing of operations as an engineering discipline — and his insistence that deployment frequency and stability were not in fundamental tension — challenged the ITIL/ITSM assumption that change was the enemy of stability. This would later be formalized in [[continuous-delivery-book]] (Humble and Farley, 2010) and empirically validated by [[nicole-forsgren]]'s DORA research.

The talk is available on YouTube and has been watched hundreds of thousands of times. It remains one of the clearest demonstrations of what the movement was reaching toward.
