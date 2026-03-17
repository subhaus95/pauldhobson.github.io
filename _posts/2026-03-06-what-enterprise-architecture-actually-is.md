---
layout: post
title: "What Enterprise Architecture Actually Is"
date: 2026-03-06
tags: [enterprise-architecture, technology-leadership, strategy]
image: /assets/images/building-construction.jpg
excerpt: "The job description says technology governance. The actual job is organisational therapy, cat herding, and learning to inch things forward without snapping the elastic band."
---

The job description says technology governance. It mentions frameworks, architectural standards, review processes, and alignment with business strategy. All of that is true in the same way that "manages relationships with stakeholders" is true of diplomacy. Technically accurate. Completely missing the point.
All Enterprise Architecture definitions are wrong, but some are useful.

Enterprise architecture, when it works, is a combination of organisational therapy, cat herding, and the careful management of tension between what should exist and what actually can. The people who are good at it are not primarily technical experts. They are people who can hold a clear model of where an organisation is trying to go while simultaneously dealing honestly with where it actually is — and who have the patience and political skill to inch the distance between those two things smaller, year by year, without ever making the mistake of trying to close it all at once.

## Do you actually need this?

The honest answer is: probably, but not necessarily in the form you've seen it done elsewhere, and not necessarily at the scale you might assume.

The question a CEO, COO, or CIO should ask is not "do we have an enterprise architecture function?" It is: given the type of organisation we are, the stage of development we're at, and the specific risks and constraints we face — what kind of architectural thinking do we actually need, and what control planes are worth maintaining? Those are different questions, and conflating them is how organisations end up with either too much architecture overhead or none at all.

The lifecycle point matters first. A high-growth business acquiring customers and expanding into new markets needs architecture that can say yes quickly, absorb technical debt consciously, and stay coherent enough not to create unmergeable hairballs. The emphasis is on enabling speed, not enforcing standards. The architecture practice in this mode is light, opinionated, and focused on the few decisions that are genuinely hard to reverse. A mature business optimising margin and managing complexity needs almost the opposite: standardisation, consolidation, integration coherence, and the discipline to retire things rather than just adding to them. The architectural control planes that matter in growth are not the same as the ones that matter in optimisation, and organisations that don't adjust as they move between modes accumulate the wrong kind of overhead.

The type of organisation shapes the practice even more fundamentally. EA at NASA is a specific and demanding discipline: multi-decade programmes, safety-critical systems, federal contracting requirements, thousands of interdependent components built by different contractors over different eras. A mistake in architectural governance there can cost a mission or worse. The formality, the standards, the review processes are not bureaucracy for its own sake — they are the minimum viable governance for systems where the failure modes are catastrophic and the timescales are generational. EA at a municipal city government is entirely different: the constraints are democratic accountability and procurement rules more than technical coherence; the technology serves dozens of disconnected service domains (utilities, permits, social services, public safety) that have no particular reason to share architecture; and the pace of change is determined by political cycles and budget processes that architectural elegance cannot override. EA at a global commercial real estate business is different again: the architecture question is largely about data — valuations, market intelligence, portfolio analytics, the technology stack needed to integrate acquisitions quickly — and the control plane that matters most is the one governing how information flows through the organisation, not the one standardising application infrastructure.

None of these organisations needs the same thing. The error is importing the architecture practice of one context into another — applying NASA-grade governance to a fifty-person growth-stage business, or assuming that the lightweight practice appropriate to a data-driven commercial business is adequate for infrastructure that controls physical operations. The architecture function should be calibrated to the specific combination of scale, risk, complexity, and strategic mode of the organisation it serves. Getting that calibration right is itself an architectural decision, and it is one that deserves more deliberate attention than it usually receives.

## The business model is the architecture

The most important thing an architect needs to understand about any organisation is not its application portfolio. It is its business model: where value is created, where cost is incurred, what the growth levers are, and what the organisation is currently optimising for.

This matters because technology architecture is downstream of business architecture in ways that most architecture functions don't fully internalise. An organisation that is in growth mode — acquiring customers, expanding into new markets, launching new products — needs technology that prioritises speed and flexibility over efficiency and standardisation. An organisation in optimisation mode — defending margin, reducing complexity, integrating acquisitions — needs almost the opposite. The technology choices that make sense in one context are the wrong choices in the other, and a lot of architectural debt is created by organisations that don't notice when their mode has changed.

Risk has the same structural importance. The risk tolerance of a technology architecture should reflect the risk profile of the business it supports. A highly regulated business in a safety-critical environment should have an architecture that makes compliance and reliability non-negotiable, even at the cost of agility. A business competing on speed of innovation should accept more technical debt and more operational complexity than a mature business with stable, predictable operations. An architect who applies the same standards regardless of context is not governing well — they are governing uniformly, which is different.

The implication is that architects need to be genuinely literate in how the business works. Not deeply expert — that's a different role — but literate enough to ask the right questions and understand the answers. What are we optimising for this year? Where does cost go that we can't fully explain? What are the decisions that we keep circling back to without resolution? The answers to those questions shape the architectural priorities more than any framework.

## Organisational therapy

Large organisations do not have complete self-knowledge. They have accumulated systems, processes, and structures over time, each of which made sense in context and most of which are no longer fully understood by anyone currently working there. The people who built the systems have moved on. The problems the systems were solving have evolved. The assumptions that were built into the design have never been made explicit and therefore have never been questioned.

One of the real jobs of an architect is to help the organisation see itself clearly. This sounds philosophical but it is intensely practical. It means building the models — of capabilities, of data flows, of system dependencies — that make visible what the organisation has, how it actually works, and where the bodies are buried. It means asking the questions that reveal the decisions that were never made: "who owns this?" — silence — "what does this system do?" — "we're not entirely sure" — "when was the last time this was reviewed?" — "we think there was a review in 2016."

The therapy analogy holds in a specific way: the goal is not to fix things on the patient's behalf but to help them develop the self-awareness to make better decisions. An architect who spends their career producing architectural artefacts that describe the organisation has not done the job. An architect who has helped the organisation understand its own complexity well enough to navigate it — who has shifted the mental models of the people making decisions — has.

This work is slow, invisible, and impossible to put in a dashboard. It is also probably the highest-leverage thing an architecture function does.

## Cat herding

Enterprise architects have almost no direct authority over the people whose cooperation they need to accomplish anything. The teams building systems, the product owners setting priorities, the budget holders deciding what gets funded, the executives sponsoring initiatives — none of them report to the architecture function, and most of them are not primarily motivated by architectural coherence. They have their own objectives, their own constraints, and their own views about what matters.

Getting anything done in this context requires the skills of a diplomat more than the skills of a technologist: understanding what other people are trying to achieve, finding genuine overlaps with architectural goals, and making it easier to do the architecturally sensible thing than to do something else. The architects who get traction are not the ones with the best technical arguments — organisations are full of people with excellent technical arguments that achieved nothing. They are the ones who understood the political economy of the organisation well enough to work with it rather than against it.

This is cat herding in the truest sense. You are not in control. You are creating conditions. You are removing friction from the paths you want people to take and occasionally placing small obstacles on the paths you don't. You are building relationships with the people whose cooperation you will need before you need it. You are accumulating credibility slowly and spending it carefully. You are learning which battles matter and which ones are not worth the cost of winning.

## Balance in the Force

The defining tension in architectural work is between what should exist — the technically coherent, strategically aligned, efficiently structured state that architectural thinking points toward — and what can realistically be achieved given the organisation's appetite for change, its available capacity, and the thousand other things it is also trying to do.

Architects who live entirely on the idealism side of this tension produce beautiful reference architectures and achieve very little. They are right about where the organisation should go and wrong about what it can do, and the gap between those two things is where their influence evaporates. Architects who live entirely on the pragmatism side achieve incremental improvements and gradually lose the ability to distinguish improvement from drift. They accommodate every compromise and eventually cannot explain why anything is the way it is.

The sustainable position is somewhere between the two, and it moves constantly. You hold the ideal clearly enough to use it as a navigational reference — to be able to say, of any proposed decision, whether it takes the organisation toward or away from where it should be going. And you accept that almost every actual decision will be a compromise, because organisations are not clean slates and the people in them are not waiting to be organised by an architecture team.

The elastic band is the right metaphor for this. The tension between current state and target state is what creates movement. Too little tension and nothing moves; the organisation is comfortable where it is. Too much tension and the band snaps — the organisation rejects the change, the initiative is cancelled, and the architecture team loses credibility and influence. The skill is maintaining just enough tension to keep things moving: identifying the decisions that will produce meaningful progress, making the case for them in terms the organisation can accept, and accepting imperfect outcomes while keeping the direction of travel clear.

## Inching forward

The timescales on which enterprise architecture operates are long. The transformation of a large organisation's technology estate — moving it from wherever it is to something coherent, flexible, and well-suited to its strategic purpose — takes years, sometimes decades. It is not a project with a completion date. It is a direction of travel.

This means that the measure of whether an architecture function is doing its job is not whether the organisation has reached its target state. It is whether the organisation is moving consistently toward it, and whether the decisions being made today are making future progress easier rather than harder. An imperfect decision that leaves the door open for improvement next year is better than a perfect decision that the organisation won't accept and therefore won't implement.

Inching forward is not a consolation prize. The organisations that make steady, compounding progress on their technology foundations end up in substantially better positions than the organisations that periodically attempt transformations and spend the intervening years managing the aftermath. Big-bang change is appealing in theory and brutal in practice: the disruption is front-loaded, the benefits take longer than expected to materialise, and the organisation's capacity to absorb further change is depleted at exactly the moment the next challenge arrives.

The architects I've seen do this work well share a particular quality: they are genuinely comfortable with imperfection and genuinely committed to progress. They don't need the organisation to be where it should be. They need it to be moving. And they have learned to find satisfaction in the movement, even when — especially when — it is slow.
