---
layout: post
title: "What Enterprise Architecture Actually Is"
date: 2026-03-06
tags: [enterprise-architecture, technology-leadership, strategy]
excerpt: "Enterprise architecture has an image problem. The discipline that should be making large organisations clearer and more coherent has spent decades producing diagrams nobody reads and frameworks nobody applies."
---

Enterprise architecture has an image problem. The discipline that should be making large organisations clearer and more coherent has spent decades producing diagrams nobody reads and frameworks nobody applies. The result is a word that makes engineers roll their eyes and executives nod politely before moving on to the next agenda item.

That's a shame, because the underlying problem enterprise architecture is trying to solve is real and increasingly urgent: large organisations accumulate technology debt not just in code, but in decisions — decisions about what systems exist, how they connect, what they're for, and who's responsible for them. Without some discipline around those decisions, organisations don't drift, they fracture.

## The gap between the idea and the practice

Enterprise architecture as a formal discipline emerged in the 1980s and 1990s, shaped by frameworks like Zachman and later TOGAF. The core insight was sound: large technology estates need coherent governing principles, and someone needs to hold the long view when everyone else is focused on the immediate.

What went wrong was the operationalisation. TOGAF in particular — the dominant framework for two decades — is less a guide to doing architecture and more a comprehensive taxonomy of what an architecture function might one day produce. The frameworks invited organisations to build elaborate documentation structures: business architecture, application architecture, data architecture, technology architecture, each with its own views and artefacts and review processes.

The documentation became the work. Architecture review boards were established not to make better decisions faster but to ensure that all decisions had been reviewed. Architects spent their time producing artefacts that demonstrated compliance with process rather than improving the quality of choices. The function accumulated overhead without accumulating influence.

The signal that an architecture team has lost the plot is when you ask them what decisions they've shaped in the past six months and they list processes rather than outcomes. Not "we advised against this acquisition target because the integration cost was being systematically underestimated" but "we reviewed fourteen change requests and all were approved." The former is architecture working. The latter is governance theatre.

## What architects actually do (when it's working)

The most useful description I've found is that architects translate — between business intent and technical capability, between what an organisation wants to be and what its systems will allow it to become.

This translation work takes several forms. At the strategic level, it means helping leadership understand the technology implications of business decisions before those decisions are made. An acquisition target looks different when you understand that integrating it requires replacing four core systems over three years. A cost reduction programme looks different when the systems earmarked for consolidation are also the systems on which everything else depends. Architecture that operates at this level earns the trust of the business because it improves decisions that matter.

At the investment level, it means maintaining a coherent view of the technology estate — what exists, what it costs, what it enables, and what it constrains — so that investment decisions aren't made in isolation. Without that view, organisations repeatedly invest in capabilities they already have, unknowingly create dependencies that limit future flexibility, and discover integration costs at the worst possible moment.

The third form is institutional memory. Organisations forget why things are the way they are. Systems built to solve problems that have since changed get treated as constraints rather than choices. Architecture is partly responsible for maintaining the record of why decisions were made, which makes it possible to revisit them intelligently when circumstances change.

## The useful parts

Stripped of the framework overhead, a few architectural practices consistently add value in large organisations.

Capability mapping — building a model of what the organisation needs to be able to do, independent of the systems currently used to do it — is one of the more powerful tools in the discipline. It creates a common language between technology and the business, exposes where capabilities are duplicated or absent, and provides a stable foundation for investment decisions even as the technology changes. A capability map is slower to go stale than an application portfolio because business capabilities change more slowly than systems.

Integration architecture is undervalued and under-resourced in most organisations. How systems exchange data, what they guarantee about that exchange, and who is responsible when those guarantees fail — these questions determine a significant proportion of operational risk in complex environments. Getting integration right is not glamorous work, but getting it wrong is expensive in ways that take years to fully manifest.

Roadmapping that connects to delivery is rare and valuable. Most technology roadmaps are wish lists constrained by budget rather than plans constrained by capacity and dependency. Architecture that treats delivery feasibility as a first-class concern — that models dependencies, surfaces conflicts, and identifies the sequence in which things actually need to happen — is genuinely useful to the organisations trying to execute against it.

## Why it matters more now

The complexity of enterprise technology environments has increased substantially over the past decade. Cloud infrastructure, SaaS proliferation, API-connected ecosystems, and the integration of AI into operational workflows have all added layers of architectural decision-making that didn't exist before. The number of systems a large organisation operates, and the number of meaningful connections between those systems, has grown faster than most organisations' capacity to govern them.

The IT/OT convergence adds another dimension in industrial settings. Connecting operational technology — the systems that run physical infrastructure and industrial processes — to enterprise IT introduces architectural challenges that the conventional enterprise playbook wasn't designed to address: different reliability requirements, different security models, different standards and protocols, different operational risk tolerances.

AI is creating a new set of architectural decisions about data, model governance, and the integration of probabilistic systems into deterministic business processes. These decisions are being made right now, often without a clear architectural framework, and some of them will be expensive to revisit.

The organisations that will navigate this well are the ones that have invested in the architectural thinking that makes complex environments legible. Not the organisations with the most complete TOGAF artefacts, but the ones with the clearest view of what they have, why they have it, what they're trying to become, and what the path looks like from here to there.
