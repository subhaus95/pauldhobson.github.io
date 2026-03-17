---
layout: post
title: "The IT/OT Boundary"
date: 2026-03-01
tags: [operational-technology, platform-strategy, infrastructure]
image: /assets/images/pipeline.jpg
excerpt: "Industrial organisations have two technology estates that rarely speak to each other. Closing that gap is one of the more interesting problems in enterprise technology right now — and at least when things go wrong, you can visit the site."
---

In August 1997 I gave my first international conference presentation — at IEEE IGARSS in Singapore, a large remote sensing symposium. The paper was on POLDER, a French-built imaging radiometer carried aboard ADEOS, the Japanese Advanced Earth Observing Satellite, which had been measuring the polarisation and directionality of light reflected from the Earth's surface and atmosphere since its launch the previous year.

I came out of the session to find a cluster of colleagues gathered around the bulletin board in the corridor, several of them looking in my direction with expressions that mixed sympathy with something closer to awe. NASDA, the Japanese space agency, had posted a notice. ADEOS had lost power on June 30th — five weeks earlier — when a solder joint on the solar paddle fractured. The joint had been stressed by a thermal differential during an attitude control manoeuvre eleven months before, and had been cracking, silently and invisibly, ever since. One morning the satellite simply went dark. The instrument I had just spent twenty minutes presenting results from, and had staked my future PhD research on, had been dead for over a month.

There is not much you can do about a failed satellite. It is 800 kilometres away, travelling at eight kilometres per second, and the fault is in a solder joint on a solar panel that is now tumbling through orbital night. You write up what you got from the operational period, you wait for the next mission, and you reflect on the particular cruelty of systems that fail in ways that are physically inaccessible.

The consolation with industrial operational technology, as distinct from its orbital equivalent, is that you can at least visit the site (even if it is -40C in Northern Alberta)

## Why the two estates diverged

Operational technology predates enterprise IT as we understand it. SCADA systems, distributed control systems, and programmable logic controllers were being deployed in industrial settings in the 1970s and 1980s — decades before enterprise integration was a coherent concept. They were designed for a specific purpose: reliable, deterministic control of physical processes. Availability was paramount. A system that controlled a pipeline or a power plant needed to run continuously, respond in real time, and fail safely. Connectivity to external networks was not a design requirement. In many cases, the air gap between OT systems and everything else was a deliberate safety feature.

The result was two distinct technology cultures that developed independently. Enterprise IT evolved toward networked systems, standard protocols, and frequent update cycles. OT evolved toward proprietary systems, specialised protocols, and update cycles measured in decades rather than years. The vendors were different, the skills were different, the governance was different. In most organisations, the two worlds rarely needed to interact.

What changed was the business demand for data. As operational analytics became more sophisticated, and as the economics of cloud computing made it feasible to process large volumes of operational data at scale, the value of connecting OT systems to enterprise data infrastructure became increasingly clear. The pressure to close the gap has been building steadily since.

## What convergence actually means

IT/OT convergence is often described as though it were primarily a networking problem — connecting two previously separate networks. That framing understates what is actually involved.

The more substantive work is about data: getting operational data — sensor readings, equipment states, process parameters, alarm histories — out of OT systems and into the analytical and AI infrastructure where it can generate insight. In most industrial organisations, this data exists and has always existed. It has been used locally, by operators and control systems, in real time. What hasn't existed is a reliable, scalable pathway for that data to flow into enterprise systems where it can be aggregated, analysed historically, and used to inform decisions at a different timescale.

The business case is significant. Predictive maintenance — using historical patterns in equipment sensor data to anticipate failures before they cause downtime — is one of the clearest applications, and the economics are compelling in industrial environments where unplanned outages are expensive. Operational efficiency programmes that use real-time data to optimise throughput or energy consumption are another. So is the integration of operational data into enterprise risk and compliance frameworks.

Convergence also introduces risk. Connecting OT systems to broader networks changes their exposure in ways that need to be managed carefully. The consequences of a compromise in an OT environment are different from the consequences of a compromise in enterprise IT — different enough that the standard enterprise security playbook needs significant adaptation.

## The integration challenge

The technical challenges of IT/OT integration are real and should not be underestimated by anyone arriving from an enterprise IT background.

OT systems communicate using protocols that predate the internet and were designed for reliability rather than interoperability: Modbus, DNP3, Profibus, various proprietary variants. Getting data out of these systems requires protocol translation, and doing that at scale across a complex industrial site requires infrastructure — typically some combination of edge computing and industrial data platforms — that differs substantially from conventional enterprise integration patterns.

Historian systems occupy a particular place in this landscape. Most industrial organisations have a process historian — a specialised time-series database that records operational data at high frequency from plant and equipment. Historians are often the most complete source of operational data available, and connecting them to enterprise data infrastructure is usually an early priority in any convergence programme. But historians have their own data models, their own query interfaces, and their own operational characteristics, and treating them as though they were conventional relational databases leads quickly to problems.

Latency and reliability requirements also differ significantly from enterprise IT norms. A query against an enterprise application can tolerate a second or two of response time. A control system cannot. The integration architecture needs to respect those boundaries — which means being clear about which flows are operational (needing OT reliability standards) and which are analytical (tolerating enterprise-level latency).

## Security at the boundary

The security implications of IT/OT convergence deserve more attention than they typically receive in the early stages of a convergence programme, when the focus is usually on data access and integration capability.

OT systems were designed in an era when their isolation was their security. Many of them run software that is years or decades old, on operating systems that no longer receive patches, on hardware that cannot easily be replaced without disrupting operations. In an air-gapped environment, that vulnerability profile is manageable. In a networked environment, it is not.

The instinct to apply standard enterprise security controls — patch management, endpoint detection, network monitoring — often creates new risks in OT environments rather than reducing existing ones. A security patch that requires a system reboot creates downtime. An endpoint agent that consumes CPU cycles affects the determinism of a control system. The OT security challenge requires purpose-built approaches: network segmentation that enforces boundaries between OT and IT without breaking the data flows that convergence is trying to enable, monitoring calibrated to OT baselines, and change management processes that account for the operational implications of security changes.

Getting this right requires IT and OT teams to work together in ways they often haven't before, which is as much an organisational challenge as a technical one.

## Where this is heading

The industrial IoT thesis — that connecting operational assets at scale will generate data value large enough to transform industrial operations — has been asserted for long enough that the assertion itself has lost some credibility. The value is real, but the implementation complexity is also real, and the gap between the two has been wider than anticipated.

What is becoming clearer is the architectural pattern that makes this work: a layered approach in which OT systems remain operationally isolated, edge infrastructure handles protocol translation and initial data processing, and an industrial data platform provides the connectivity layer between the OT world and enterprise analytics and AI infrastructure. Digital twins — software representations of physical assets and processes, fed by real-time operational data — are becoming a meaningful part of this architecture in asset-intensive industries.

The organisations building this capability now are establishing a significant advantage. The industrial data that becomes available when OT and IT systems are properly connected is genuinely distinctive — it reflects physical reality in ways that other enterprise data does not. Training AI systems on that data, building analytical capabilities around it, and integrating the resulting insights into operational decision-making is a multi-year programme. The time to start is before the competitive pressure to do so becomes acute.

And when something goes wrong — when the solder joint fails, metaphorically speaking — you can at least get in a truck and drive to the site. That remains a meaningful advantage.
