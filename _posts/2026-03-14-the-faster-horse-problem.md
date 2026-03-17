---
layout: post
title: "The Faster Horse Problem"
date: 2026-03-14
tags: [automation, technology-strategy, organisational-design]
image: /assets/images/horse.jpg
excerpt: "Automation presents two opportunities. One is transformative — rethinking what a process is for. The other is just a faster version of something that shouldn't exist in its current form. Most organisations default to the second."
---

The quote attributed to Henry Ford — "if I had asked people what they wanted, they would have said a faster horse" — is almost certainly apocryphal. Ford probably never said it. But the idea it captures is real and worth taking seriously: the people inside a system are often the least well-positioned to imagine what a different system might look like, because their mental model of what is possible is shaped by the system they are already in.

The relevance to automation is direct. When an organisation decides to automate something, it faces a choice that is rarely made explicit. One path takes the existing process and makes it faster, cheaper, or less labour-intensive. The other path asks what the process is actually for and builds something designed for that purpose — which may look quite different from what existed before.

Both are legitimate. But they are not the same opportunity, they do not require the same investment, and they do not produce the same outcomes. Treating them as interchangeable is one of the more reliable ways to invest significantly in automation and achieve less than expected.

## The fork

The first kind of automation — call it efficiency automation — takes a process as given and reduces the friction within it. A manual data entry task becomes a script. A multi-step approval workflow becomes a configured rule engine. A report that took a day to produce is generated overnight. The process logic is preserved; the mechanism that executes it changes.

This is useful. It reduces cost, reduces error, and frees people to do other things. In contexts where the process is fundamentally sound and the constraint is execution capacity, it is exactly the right intervention.

The second kind — transformative automation — starts from the question of what the process is supposed to achieve and designs for that outcome, unconstrained by how it has historically been done. It tends to produce something that looks less like "the old process, automated" and more like "a different approach to the same problem." Sometimes it eliminates process steps that existed only because manual execution required them. Sometimes it changes who is involved and when. Sometimes it makes previously impractical approaches — real-time rather than batch, individual rather than aggregate, predictive rather than reactive — suddenly feasible.

The risk of the faster horse is not that it delivers nothing. It delivers exactly what it promises: a faster version of what existed before. The risk is that what existed before was shaped by constraints that no longer apply, and that automating it locks in those constraints at scale.

## This pattern is older than AI

The Swansea University Earth Observation group in the mid-1990s needed more compute. Geospatial analysis of satellite data is computationally intensive, and the Sun Microsystems Sparc workstations we used were increasingly the constraint. The obvious answer — the faster horse — was more Sparcs. The problem was budget: Sparc workstations were expensive, and the group couldn't afford to simply expand.

The question that unlocked the solution was the right one: what did we actually need? The requirement was compute capacity for scientific analysis. There was no fundamental requirement for Sparc hardware specifically. That reframing opened up a completely different option: Slackware Linux on commodity PC hardware, built in-house. Five Sparc 5s became fifteen dual-CPU Linux workstations for roughly the same total cost — and the Linux machines were substantially faster. We later extended this to Beowulf clustering, building basic parallel processing capability from commodity parts at a time when that kind of infrastructure would otherwise have required a significantly larger budget.

The transformative option was not obviously available until someone asked the right question. The faster horse would have been a modest improvement that preserved the underlying constraint. The transformative option removed the constraint entirely by questioning whether it was actually a constraint.

The structural reason this worked is that the technology landscape had shifted in a way that the existing mental model hadn't registered. Sun Sparcs had been the right answer for a long time. The assumption that they remained the right answer was never examined because the question had never been reopened. Linux and commodity hardware had reached a threshold where they were genuinely competitive — but that threshold only became visible once someone stopped assuming the answer and started asking the question.

This is the dynamic that the faster horse problem captures. The mental model of what is possible is shaped by what has been done before. Asking a different question is not a technical act; it is a cognitive one.

## Why organisations default to it

The pull toward efficiency automation is strong and mostly rational. It is easier to scope, easier to cost, and easier to explain to stakeholders who approved a budget line for a specific process improvement. The requirements are legible because the existing process is legible. The success criteria are clear: does it do what the old process did, faster and cheaper? The risk is bounded because the logic is already understood.

Transformative automation requires a different kind of work upfront — understanding intent rather than process description, which means engaging the people who own outcomes rather than the people who execute steps. It tends to take longer to define, longer to justify, and longer to build. It creates more stakeholder uncertainty because the end state looks unfamiliar. And it requires organisational willingness to change how work is done, not just how it is executed — which brings it into contact with all the cultural and structural resistance that process change typically encounters.

There is also an audit trail problem. When an automation project delivers "we automated the existing process and it now runs in four hours instead of four days," the value is visible and attributable. When it delivers "we redesigned the process and the outcome is now achieved in a fundamentally different way," the comparison to the baseline is harder to draw and the credit is harder to assign. Organisations with strong accountability structures often find it easier to approve the former.

The result, across many organisations and many automation programmes, is a large portfolio of processes that are now executed faster and at lower cost, and a persistent sense that automation has not delivered the step-change improvement that was anticipated. It hasn't, because step-change improvement was never what was funded.

## What transformative automation actually requires

The starting point is a clear answer to a question that sounds simple and is often surprisingly hard: what is this process for? Not what does it do — what is it for? What decision does it inform, what outcome does it enable, what risk does it manage?

The reason this is harder than it sounds is that many processes have accumulated steps over time that no longer serve the original purpose. They exist because they solved a problem that has since been solved differently, because they were required by a regulation that has since changed, or because they were added during an incident and never revisited. Asking what a process is for often reveals a gap between what people assume it does and what it actually accomplishes.

Once the intent is clear, it becomes possible to ask whether automation opens up approaches that weren't previously feasible. Can the decision be made in real time rather than at the end of a batch process? Can an exception be handled at the point it arises rather than escalated through multiple layers? Can the process be restructured around the outcome it is trying to achieve rather than the steps that manual execution required?

This is not a licence for unbounded redesign. Processes exist within constraints — regulatory, operational, relational — that automation doesn't remove. But identifying which constraints are real and which are artefacts of how things have always been done is necessary before deciding what to automate.

## Making the call

Not every process is worth reimagining, and not every automation opportunity is transformative. The question is whether the current process design is fit for purpose, or whether it reflects constraints that no longer apply.

A few signals that the faster horse is the wrong investment: the process produces a result that is used differently from the way it was designed to be used; the people executing it apply significant informal judgment to compensate for limitations in the formal process; the process was last redesigned more than a decade ago and the environment it was designed for has changed substantially since. Any of these suggests that automating the existing design will preserve its limitations alongside its logic.

The current wave of AI-enabled automation makes this question more consequential than it has been at any previous point. The capabilities now available are genuinely different in kind from earlier generations of automation technology: they can handle unstructured inputs, exercise something resembling judgment across ambiguous cases, and operate in domains that were previously considered too complex for automation. Applied to well-designed processes, they offer significant value. Applied to bad processes, they will produce bad outcomes faster, at greater scale, with higher confidence.

That last part is the real faster horse problem. A horse that is merely fast is a limited liability. An automated process that is wrong at speed, and wrong consistently, and wrong in ways that are harder to detect because they look like system behaviour rather than human error — that is a different order of problem. The time to ask what the process is for is before the automation is built, not after.
