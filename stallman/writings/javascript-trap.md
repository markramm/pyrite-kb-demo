---
id: javascript-trap
title: "The JavaScript Trap"
type: writing
importance: 7
tags:
- free-software
- javascript
- web
- browsers
- essay
writing_type: essay
date: 2009-01-01
coauthors: []
publication: "GNU Project / Free Software Foundation"
url: "https://www.gnu.org/philosophy/javascript-trap.en.html"
key_concepts:
- free-software-definition
- four-freedoms
- saas-loophole
- digital-restrictions-management
research_status: draft
---

"The JavaScript Trap" (2009) identifies a class of software freedom problems specific to the web browser environment. When users visit web pages that run JavaScript code, they are executing programs on their computers — programs that are typically not free software. [[stallman]] argues that this represents a systematic violation of the [[four-freedoms]] that goes largely unnoticed because users do not perceive web scripts as software they are running.

The core of the argument is that the [[free-software-definition]] applies to JavaScript programs just as it does to any other software. A web page that delivers a nontrivial JavaScript program to a user's browser is distributing software; if that software is nonfree — if the user cannot study, modify, or redistribute it — then the user's freedom is being infringed. The fact that the software is delivered dynamically over a network, rather than installed from a package, does not change its nature.

[[stallman]] distinguishes between trivial scripts (which he considers practically harmless to freedom) and nontrivial programs (which raise genuine concerns). He argues that browser vendors and web developers have an obligation to either license their JavaScript under free software licenses or design their sites not to require nonfree JavaScript for their core functionality. This analysis parallels his earlier argument in [[java-trap]], which identified a similar class of superficially free software that is practically restricted.

The essay has implications for the broader [[saas-loophole]] problem: just as software-as-a-service can provide software functionality without distributing code, nonfree JavaScript can execute proprietary programs on users' machines without triggering the distribution requirements of [[gpl-v2]] or [[gpl-v3]]. The [[agpl]] was one response to the server-side version of this problem; JavaScript presents the client-side version.

The practical outcome of this essay was [[stallman]]'s advocacy for the LibreJS browser extension, which identifies and blocks nontrivial nonfree JavaScript. The essay also influenced [[gnu-project]] guidelines for evaluating free software operating systems' handling of browser JavaScript.
