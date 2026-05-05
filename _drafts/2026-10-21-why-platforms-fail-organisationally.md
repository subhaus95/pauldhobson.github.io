---
layout: post
title: "Why Platforms Fail Organisationally"
date: 2026-10-21
tags: [platform-engineering, organisational-design, technology-strategy, delivery]
image: /assets/images/building-construction.jpg
excerpt: "The five ways platform programmes get the technology right and the organisation wrong. Platform failure is almost never technical."
---

Platform programmes fail in predictable ways. This is not immediately obvious, because the failures tend to look different on the surface — a platform that nobody adopts, a platform that gets adopted and then abandoned, a platform that delivers for some teams and not others, a platform that gradually transforms into the monolith it was supposed to replace. The proximate causes look different. The underlying causes are usually the same.

The thing they have in common is that they are organisational failures, not technical ones. The technology in failed platform programmes typically works. The APIs are sound. The infrastructure is reliable. The developer experience, while sometimes rough at the edges, is not the reason the programme stalled. What failed was the funding model, or the mandate, or the product ownership, or the relationship between the platform team and the teams it was supposed to serve. These failures are harder to diagnose than technical failures because they do not produce clear error messages, and they are harder to fix because they require organisational change rather than engineering effort.

The Platform Engineering at Scale piece on this site describes how platforms are supposed to work. This is a catalogue of how they actually go wrong.

## The five failure modes

**The first is the funding model.** Platform teams are typically funded as internal infrastructure, which means they are funded on a cost basis rather than a value basis. The team has a headcount, a budget, and a mandate to build capabilities that other teams will use. The problem is that internal infrastructure funding has no natural mechanism for surfacing whether the platform is creating value proportionate to its cost. The team can be busy, well-staffed, and technically productive while the organisations it is supposed to serve are building workarounds and complaining quietly that the platform doesn't do what they need.

The value-basis alternative — where platform funding is tied to the adoption and outcomes it enables — is uncomfortable because it creates accountability that infrastructure teams are not used to. It also surfaces the real question that cost-basis funding allows organisations to avoid: if the platform were optional, would anyone use it?

**The second is mandate without authority.** Platform teams are frequently given responsibility without the organisational authority that would make it possible to exercise it. They are told to create standards and enable consistency across a portfolio of products — but the product teams whose cooperation they need have their own priorities, their own leadership, and no formal obligation to adopt the platform rather than building their own. The platform team ends up in the position of an advisory function with a delivery mandate: expected to produce outcomes, equipped only to produce recommendations.

**The third is product ownership by committee.** Platforms are products, and they fail when they are governed as committees rather than owned by individuals. The committee model produces platforms that reflect the consensus of their contributors — which means they reflect the current requirements of all teams equally, which means they reflect the specific requirements of no team adequately. A platform owned by someone with the authority to make decisions about what it does and what it doesn't do, who is accountable for whether teams adopt it, and who can say no to requirements that would compromise its coherence — that platform has a chance. A platform owned by a steering group that meets monthly has a roadmap and no direction.

<!--
PAUL — the first three failure modes are drafted. Add the fourth and fifth,
then move into the body of the piece.

Fourth failure mode candidates:
- The internal customer relationship (platform team treats adoption as compliance
  rather than a product problem)
- The legacy shadow (platform built alongside the thing it was supposed to replace,
  both maintained indefinitely)

Fifth failure mode candidates:
- The abstraction that doesn't abstract (platform that moves complexity rather
  than hiding it)
- The "platform" that is actually just shared infrastructure with a new name

Then the piece needs a section on what successful platform programmes actually do
differently — draw on the Plains Product & Platform operating model shift as the
concrete example.

Suggested section headings:
## The five failure modes [already started above]
## What successful programmes do differently
## The Plains shift
## The question to ask before you start
-->
