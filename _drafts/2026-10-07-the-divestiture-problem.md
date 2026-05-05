---
layout: post
title: "The Divestiture Problem"
date: 2026-10-07
tags: [technology-strategy, platforms, organisational-design, delivery]
image: /assets/images/unfinished.jpg
excerpt: "Technology M&A integration is a well-documented problem. Technology divestiture is its structural inverse, and almost everything that works in integration fails when applied to separation."
---

Technology M&A integration is a documented discipline. There is a substantial body of practice, hard-won experience, and published frameworks for the challenge of taking two technology estates and making them function as one. Most large consultancies have a practice area. Most technology leaders who have been through an acquisition have a story about what went wrong and what they would do differently.

Technology divestiture is the structural inverse of this problem. It receives a fraction of the attention and has a fraction of the documented practice. The assumption, usually implicit, is that separation is integration run in reverse — that the same frameworks apply in the opposite direction, and that an organisation experienced in combining technology estates will find the process of separating one straightforwardly familiar.

This assumption is wrong in ways that are expensive to discover after the work has started.

Integration combines two dependency graphs. Divestiture splits one. Those are not symmetric operations. When you integrate two organisations, you are making decisions about what to keep, what to consolidate, and what to retire — decisions that, while consequential, are made with the full inventory of both estates visible and the full range of options available. When you separate an integrated estate, you are working with a single dependency graph that was never designed to be split, into which years of integration decisions have woven connections that are not always documented, not always understood, and not always visible until you pull on a thread and discover it is load-bearing.

The technical language for this is entanglement. It is also the right word in the organisational sense: the people, processes, and institutional knowledge associated with a technology estate become entangled over time in ways that are hard to see clearly until separation makes them visible.

## What the dependency graph actually looks like

The first thing a divestiture reveals is that nobody has a complete picture of the dependency graph. This is not negligence. It is the natural consequence of a technology estate that has grown incrementally over years, with each addition made in the context of the existing system and not with an inventory of all future separation scenarios in mind.

Shared services are the first layer. Identity and access management, network infrastructure, data centre facilities, enterprise agreements with major vendors — these are the dependencies that are usually visible early and that look, from a distance, like the separable seams. They are not, in most cases, the hard part.

The hard part is the second layer: the integrations, data flows, and operational dependencies that exist within applications and between them, that were built to serve a combined organisation and that neither side of the separation may fully understand. A reporting pipeline that pulls from twelve systems across both entities. A shared data lake that both operational teams use for analytics that are embedded in daily operations. An identity system that is the source of truth for both organisations and cannot be duplicated without a period in which one side is running on a copy that diverges from the master.

Each of these dependencies was built to solve a problem. None of them was built to be removed.

<!--
PAUL — this piece is timely because you're living it. Write the notes now, even if
the piece publishes after you've left Plains.

The next sections need:
- The specific governance challenge: how do you make technology decisions for an
  asset you are separating when the acquiring organisation's requirements are
  not fully known and the separation timeline is not fixed?
- The modernisation paradox: you are simultaneously simplifying the estate (40%
  footprint reduction) and preparing it to be separated. Those objectives are not
  always aligned.
- The human dimension: the people attached to the technology being divested. How
  does that factor into the technical decisions?
- What you would tell someone starting a divestiture technology workstream

Be careful about what is commercially sensitive. The structural and methodological
observations are fair game. Specific transaction details are not.

Suggested section headings:
## The modernisation paradox
## Making decisions without a buyer
## The human layer
## What integration experience teaches you and what it doesn't
-->
