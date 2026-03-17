---
layout: post
title: "Platform Engineering at Scale"
date: 2026-03-10
tags: [platform-engineering, technology-strategy, team-topology]
excerpt: "Platform teams create leverage — but only when the organisational design matches the technology model. Most platform programmes get one right and ignore the other."
---

Platform teams create leverage — but only when the organisational design matches the technology model. Most platform programmes get one right and ignore the other.

The technical case for platform engineering is well-rehearsed: shared infrastructure, standardised deployment pipelines, reduced cognitive load for product teams. What gets less attention is the organisational design question — how the platform team positions itself relative to the rest of engineering, what authority it has, what it doesn't, and how it avoids becoming either a gatekeeper or a ghost.

## What a platform team is actually for

The most useful reframe for platform engineering is treating the platform as a product — not a project, not a shared service, but a product with internal customers whose satisfaction you are responsible for.

This matters because it changes everything about how the team operates. A shared services team thinks in terms of tickets, queue depth, and resource allocation. A product team thinks in terms of outcomes: is the platform reducing the time it takes to deploy a new service? Is it actually being used, or are teams routing around it? Are the teams using it more capable than the teams that aren't?

The concept of the "golden path" is useful here. A well-designed platform doesn't mandate a single way of doing things — it makes one way significantly easier than the alternatives. The golden path is the route the platform team has engineered to be low-friction, well-supported, and reliable. Teams are free to leave it, but doing so carries a cost: you're on your own. That asymmetry is what drives adoption without requiring enforcement.

The failure mode is trying to do both: mandating the platform while also pretending it's optional. This produces the worst of both worlds — compliance without adoption, and adoption without satisfaction. Teams use the platform because they have to, and build shadow systems for everything the platform doesn't cover. The toil moves rather than disappears.

## Why Conway's Law is the real constraint

Melvin Conway's observation — that organisations design systems that mirror their own communication structures — has become something of a cliché in engineering circles. It deserves more serious attention than it usually gets.

The implication for platform engineering is direct: you cannot build a coherent platform if the teams responsible for it are fragmented, siloed, or operating across misaligned incentives. The platform will reflect those fractures. Integration points will be poorly defined because no single team owns the boundary. Standards will be inconsistent because teams have no mechanism to align. The platform will work in parts and fail at the seams.

I've seen this play out in organisations where the platform engineering initiative was technically credible but organisationally incoherent. The infrastructure team owned provisioning. The security team owned policy. The developer experience team owned tooling. No one owned the end-to-end experience of a developer trying to ship a new service. Each team had a coherent internal model; no one had a model that corresponded to what a developer actually encountered. The result was a platform that was excellent in documentation and painful in practice.

Conway's Law also points toward the solution. The organisational structure of the platform team should mirror the architecture you want to produce. If you want a coherent developer experience, someone has to own that experience end-to-end. If you want reliable integration between infrastructure and application layers, the teams responsible for both need to work in close proximity.

## The authority problem

Platform teams sit in an uncomfortable position between two failure modes. Too little authority and the platform becomes optional in ways that undermine its purpose: every team builds its own variation, economies of scale evaporate, and the cognitive load the platform was meant to reduce ends up distributed across every team that decided to go their own way. Too much authority and the platform team becomes a bottleneck — every new service requires a review, every exception requires an approval, and teams that need to move quickly learn to treat the platform as an obstacle.

The governance models that work are neither laissez-faire nor centralised control. They share a common structure: clear standards for the things that genuinely need to be consistent (security posture, observability, deployment reliability), and deliberate flexibility everywhere else. The platform team holds the line on the non-negotiables and stays out of the way on everything else.

What makes this hard is that the line between non-negotiables and preferences shifts over time, and the platform team is rarely neutral about where it falls. Teams that have built something tend to believe others should use it. Resisting that tendency — holding genuinely open the question of what the platform should mandate — is harder than it sounds and more important than it seems.

## What changes at different scales

At twenty engineers, you don't need a platform team. You need consistent practices and someone who cares about developer experience. Formalising that into a team structure introduces overhead the organisation can't absorb and creates a team whose mandate is too thin to be meaningful.

At two hundred engineers, the absence of a platform team starts to show. Deployment processes diverge. Observability is inconsistent. The time it takes to provision a new service varies by an order of magnitude depending on which team you ask and who they know. The cost of that inconsistency is diffuse — it doesn't appear in any single incident or any single team's velocity — but it accumulates steadily.

At two thousand engineers, the platform is load-bearing infrastructure for the entire engineering organisation. The platform team's decisions about standards and interfaces shape what the whole organisation can and cannot do. At this scale, architectural governance isn't optional and the platform team's relationship with product and application teams needs to be actively managed, not left to emerge.

The mistake is applying the two-thousand-engineer model to the two-hundred-engineer organisation, or assuming the twenty-engineer approach will scale. The right model changes as the organisation changes, and the transitions between them are rarely as clean as they look in diagrams.

## Getting the transition right

Moving from ad-hoc shared services to a genuine platform model is as much an organisational change programme as a technical one. The technical work is often the easier part.

The pattern that works: start with the pain. Don't build the platform you think the organisation should want — build the platform that removes the friction the organisation is currently feeling. That means talking to the teams that are doing the work, understanding where time is lost and where consistency breaks down, and treating that intelligence as the product backlog.

The organisational change runs in parallel. The platform team needs a mandate that is real enough to be meaningful and bounded enough to be achievable. The engineering leadership needs to be willing to hold the line when teams push back on standards, and willing to adapt the standards when teams push back for good reasons. The difference between those two situations — a team resisting because the standard is genuinely wrong, versus resisting because change is uncomfortable — is one of the harder judgements in this work.

Measure what matters: deployment frequency, lead time for new services, time spent on toil that the platform should be eliminating. Not the platform team's output — the impact on the teams it exists to serve.
