---
layout: blog
title: "RGESN and GSP™: Two Different Answers to the Same Question"
date: 2026-03-03
author: Luís Cruz
tags: [green software, ecodesign, RGESN, GSP, certification]
description: "RGESN and GSP™ are often mentioned in the same breath. They are not the same thing — and understanding the difference matters if you are serious about sustainable software engineering."
---

RGESN and GSP™ are often mentioned in the same breath. They address overlapping concerns, they both live in the sustainable software space, and anyone evaluating one will eventually encounter the other. But they're not the same thing and understanding the difference matters if you're serious about sustainable software engineering rather than just ticking boxes.

## What each one actually is

**RGESN** (*Référentiel Général d'Écoconception de Services Numériques*) is a French government framework, produced under the *Loi REEN* by ARCEP, ARCOM, and ADEME. It defines ecodesign criteria for digital services, using 148 criteria across 9 areas: Strategy, Specifications, Architecture, UX/UI, Content, Frontend, Backend, Hosting, and Algorithms. Compliance is demonstrated through a public *déclaration d'écoconception*, a structured self-assessment document. It carries regulatory weight in France and is the reference standard for public digital services.

**GSP™** (*Green Software Practices*) is a certification framework operated by GreenSeal, designed to assess whether an engineering organisation has the practices, culture, and measurement capability to systematically produce sustainable software. It covers five areas: Governance & Culture, Training & Knowledge, Measurement & Observability, Software & Architecture Practices, and Continuous Improvement. It is independent of national regulation, which makes it applicable across any stack, platform, or geography.

## The same question, differently framed

Both frameworks are ultimately asking: *is this software environmentally responsible?* But they answer it at different levels of abstraction.

RGESN asks: **does this specific digital service comply with known ecodesign criteria?**

GSP™ asks: **does this organisation have the engineering maturity to produce sustainable software consistently?**

That distinction has real consequences.

## RGESN is a product-level compliance check

RGESN evaluates a product. It asks concrete, verifiable questions: are autoplay videos disabled by default? Does the service work on hardware that's ten years old? Are fonts kept below 400KB per page? These are specific, auditable, and valuable. For a team new to ecodesign, working through RGESN criteria is an effective way to identify low-hanging fruit.

But RGESN has a ceiling. Once you've assessed each applicable criterion and documented your *déclaration*, you're done. There's no mechanism that pushes you to go further or question whether the criteria themselves still reflect the state of the art. The framework was last updated in May 2024 and the next time it changes, you'll need to reassess, but in the meantime nothing in the framework prompts you to keep improving.

There's also a structural challenge: many RGESN criteria are marked N/A depending on service type, making conformance scoring complex and partially subjective. A team building a backend-heavy data pipeline will find that a significant portion of the UX/UI and frontend criteria simply don't apply to them.

## GSP™ is an organisation-level capability assessment

GSP™ doesn't ask whether a specific product has the right image dimensions. It asks whether the team building that product has the measurement infrastructure to know when their images are wasteful and the improvement loops to act on it.

This is most visible in two of the five pillars.

**Measurement & Observability** requires teams to define environmental KPIs, instrument their systems, and track energy and resource consumption over time. This isn't about reaching a threshold — it's about building the observability to surface problems you haven't anticipated yet.

**Continuous Improvement** requires that teams act on what they measure, establish review cycles, and treat sustainability as an engineering discipline rather than a one-time audit.

Together, these create a feedback loop. A team working this way might discover that their ORM generates unexpectedly heavy queries under load, or that a particular service's cold-start behaviour spikes energy consumption at predictable times. These findings won't appear in any referential: they're specific to that system, that workload, that team. A compliance checklist can't find them. An instrumented engineering practice can.

## The core difference

RGESN implicitly defines sustainability as *compliance with known practices*. GSP™ defines it as *continuous reduction of measurable impact*.

The first has a ceiling. The second doesn't.

A team can pass RGESN for a product while having no sustainable engineering practices in place. They ticked the boxes, published the declaration, and moved on. Conversely, a GSP™-certified organisation is more likely to produce RGESN-compliant products as a natural output of their practices. Not because they checked a list, but because they've built the instrumentation to catch problems and the culture to fix them.

## They complement rather than compete

RGESN is a useful starting point: concrete, bounded, and auditable. For teams new to ecodesign, working through its criteria gives them something tangible to do. For organisations operating in France or working with French public sector clients, it may also be a compliance requirement.

GSP™ is what you reach for when you want to go beyond compliance. When the question shifts from "does this product pass the checklist?" to "how do we build the engineering capability to make all our software more sustainable, over time, at scale?" — that's where GSP™ operates.

Used together, the picture is clear: RGESN tells you what a sustainable digital service looks like at delivery. GSP™ gives you the organisational framework to make that a repeatable outcome rather than a one-time achievement.

---

*Interested in assessing your team's green software maturity? [Start with the GSP™ self-assessment →](/gsp/self-assessment)*
