---
layout: post
title: "The Cost of Good Governance"
date: 2026-09-09
tags: [enterprise-architecture, organisational-design, technology-strategy, platforms]
image: /assets/images/city-grid.jpg
excerpt: "Enterprise architecture governance has a failure mode nobody talks about: it works so slowly that the business stops asking permission. At which point it governs nothing."
---

Enterprise architecture governance has a failure mode that is rarely discussed in the literature, because the literature is written by people who believe in governance. The failure mode is this: the process works exactly as designed, and the business routes around it anyway.

This is not defiance. It is adaptation. When the time cost of compliance exceeds the value the governed can attribute to the process, rational actors find alternatives. They scope their projects to fall below the threshold that triggers review. They build in phases that individually don't require sign-off. They move fast and formalise the architecture retrospectively, at which point the governance function is reviewing decisions that have already been implemented and cannot be meaningfully changed. The shadow IT that accumulates in this way is not the product of rogue behaviour. It is the product of a governance overhead that the organisation decided, implicitly and one decision at a time, was not worth paying.

The uncomfortable corollary is that a governance function can have perfect process integrity and zero actual influence. The reviews are thorough. The standards are sound. The decisions being made in the organisation are unaffected by either.

## The speed problem

Architecture review processes are almost universally designed around a worst-case assumption about the complexity of what they are reviewing. The template, the required documentation, the committee schedule, the turnaround time — all of it is calibrated to handle the most architecturally significant decisions the function will ever see. This makes sense as risk management. It makes governance unusably slow for the large majority of decisions that are not architecturally significant but are subject to the same process.

The result is a function that is thorough where thoroughness is warranted and equally thorough where it is not. A team integrating a new SaaS tool into an existing platform submits the same documentation as a team redesigning a core operational system. The review takes the same three weeks. The decision, in the first case, was never in doubt — the tool is low-risk, the integration is standard, the alternative was that the team would have gone ahead without telling anyone. The governance process did not add value. It added three weeks and a set of forms.

At Plains, the redesign of the EA governance model from rigid framework adherence to iterative intervention addressed exactly this. The change was not to reduce rigour for high-stakes decisions. It was to introduce proportionality — to create "no surprises" loops that engaged early and lightly on low-complexity decisions, and reserved genuine depth of review for the decisions that warranted it. The ServiceNow Demand Module made this tractable by creating visibility across all incoming requests: you cannot apply proportionate governance if you cannot see the full population of decisions and sort them by actual complexity and risk.

<!--
PAUL — continue from here.

The Plains governance redesign is the concrete case that earns the abstract argument.
Build it out properly:
- What did the old model look like and why had it calcified?
- What specifically changed — the categorisation logic, the feedback loop timing,
  the relationship between EA and the teams being governed
- What did "no surprises culture" actually mean in practice?
- What did you give up by making governance lighter in some places?

The piece should also acknowledge the genuine tension: lighter governance can mean
missed risks. The argument is not that governance overhead is always wrong — it's
that governance calibrated to worst-case assumptions across all decisions is a
self-defeating choice. Name the risks of the lighter model honestly.

Suggested section headings:
## The proportionality problem
## What the Plains redesign actually involved
## What you give up
## Governance that governs
-->
