---
id: java-trap
title: "Free But Shackled — The Java Trap"
type: writing
importance: 6
tags:
- free-software
- java
- platforms
- dependency
- essay
writing_type: essay
date: 2004-01-01
coauthors: []
publication: "GNU Project / Free Software Foundation"
url: "https://www.gnu.org/philosophy/java-trap.html"
key_concepts:
- free-software-definition
- four-freedoms
- gpl-copyleft-mechanism
- software-patents-opposition
research_status: draft
---

"Free But Shackled — The Java Trap" (2004) addresses a specific problem that arose when free software programs were written in Java: the Java runtime environment was at the time proprietary software distributed by Sun Microsystems, which meant that users of Java-based free programs were required to run nonfree software to execute them. [[stallman]] argues that this dependency negates the freedom of the programs themselves.

The problem is structural. A free software program is only as free as the platform required to run it. If running program X requires nonfree software Y, then the user's practical freedom to use X on a fully free system is compromised. The user must either abandon free software principles to use X, or forego X entirely. This makes writing free software for a proprietary platform a form of involuntary complicity with that platform.

[[stallman]] applies this argument to Java specifically, but notes that it applies to any nonfree platform: writing free software for Windows, for a proprietary JVM, or for other nonfree environments creates the same structural problem. The free status of the program itself does not help users who must run nonfree software to execute it.

The practical recommendation in the essay is for free software developers to avoid dependencies on nonfree platforms — or, if they write for Java, to use only free Java implementations such as GNU Classpath. [[stallman]] also discusses the [[software-patents-opposition]] dimension: Sun's Java was encumbered by patents that complicated the development of free Java implementations.

The essay became somewhat less urgent after Sun released Java under the [[gpl-v2]] in 2006-2007, transforming the Java platform from a proprietary system to a free one. The general principle, however — that free programs must be runnable on free systems, and that platform dependencies can undermine software freedom — remains relevant and is echoed in [[javascript-trap]] and [[android-and-users-freedom]].
