---
layout: blog
title: "What TS 20125 Actually Asks of Requirements Gathering and End of Life"
date: 2026-08-03
author: Luís Cruz
tags: [green software, ecodesign, ISO, TS 20125, GSP, certification, standards]
description: "Requirements gathering and end of life are two ISO/IEC TS 20125-1 phases organizations consistently struggle to show real accountability for. Here's why that's an organizational gap, not a product one, and what GSP™ Level 2 now requires because of it."
---

Ask most engineering organizations who owns the environmental footprint of a system after it's decommissioned, and you'll get a shrug. Ask who decided a feature should be built in the first place, from a sustainability standpoint, and you'll get the same shrug. In the TS 20125 gap assessments we've run, requirements gathering and end of life are consistently the two life cycle phases with the least real accountability behind them, even at organizations that are otherwise doing well on the phases in between.

That's not really a gap in the standard. TS 20125 does address both phases, with concrete ecopractices for setting an environmental budget upfront and for decommissioning responsibly. The gap is one level up. A product's TS 20125 conformance declaration tells you the practice happened for that product, this time. It doesn't tell you whether the organization behind it has a named owner for that practice, measures it, or learns from it well enough to do it again on the next product. That's an organizational question, not a product one, and it's exactly the question GSP™ exists to answer. TS 20125 sets ecopractices for a service, verified only through the organization's own conformance declaration, not third-party certification. GSP™ certifies the organization's capability to build sustainable software repeatedly, which is a different and, for these two phases especially, more useful thing to certify.

We recently strengthened GSP™ Level 2 to make that organizational accountability explicit for both phases, following a review of Level 2 against all six TS 20125 life cycle phases. It's the same continuous-improvement discipline our Level 2 criteria already expect of any certified organization, under our Continuous Improvement category, applied to our own scheme. If you haven't read our explainer on what TS 20125 actually is, start there (/blog/2026-06-25-iso-20125/) for the six-phase background. Here's what changed in Level 2 and why.

## Requirements gathering: making the upstream decision accountable

Two additions now sit in GSP™ Level 2 for this phase.

**Environmental KPIs defined before a build starts.** Teams routinely set a performance budget, a cost budget, sometimes a security bar, before writing a line of code. An environmental budget almost never makes that list, and when it does, it's rarely owned by anyone specific enough to be held to it later. GSP™ Level 2 now requires a defined environmental KPI, agreed before the build starts, backed by evidence that the organization does this consistently, not just for one flagship product it happens to be audited on.

**Feature necessity as an environmental question.** Whether a feature should be built at all is itself a sustainability decision, not a separate product conversation that happens to precede one. The most efficient code is code that never runs. A conformance declaration for a single service won't tell you whether the organization behind it routinely asks this question or asked it once for the record. GSP™ Level 2 now expects an organization to show this question gets asked as standard practice, not as a one-off.

## End of life: closing the accountability loop

Three additions cover this phase.

**Assigned decommissioning responsibility.** Someone has to own shutting a system down, named before it's needed, not improvised after the fact by whoever's on call when a contract lapses. This is an organizational habit, not a per-product checkbox, which is why it belongs in an organizational certification rather than a product declaration.

**Measuring the footprint of decommissioning itself.** Turning something off isn't free. Data migration, archival storage, hardware disposal and the process of winding down all carry their own footprint that's easy to overlook. An organization that measures this as a matter of course looks very different from one that happened to measure it once because a standard asked.

**Lessons learned from decommissioning, captured.** What made a system expensive or wasteful to retire should feed back into how the next one is designed. That feedback loop is the whole point of an organizational capability certification: the difference between a practice that existed once and a practice the organization actually keeps.

## Two more additions, and what we left out

The same review touched two other phases worth a mention. In design, we added infrastructure and hosting selection, the single most impactful of the seven additions in this update. Where you run a system determines a large share of its footprint before a single optimization is applied. In operations, we added carbon-aware scheduling, but kept it as a Supporting requirement rather than Core, because technical maturity for this varies enormously across organizations and we're not willing to certify something teams can't yet reasonably do.

We also deliberately kept three things out of Level 2: CI/CD environmental gates, formal obsolescence review, and design-for-decomposability. These aren't oversights. They're deferred to Level 3 on purpose, because they demand a level of process maturity that isn't a fair bar for Level 2. Level 2 should be demanding and attainable. Level 3 is where we ask organizations to push further. Keeping the two levels honest about that difference is part of what makes either of them mean something.

## Why this needs an organizational certification, not just a product one

Requirements gathering and end of life don't feel like engineering work, which is exactly why they end up with the weakest accountability industry-wide. Requirements gathering feels like a product conversation. End of life feels like someone else's problem, on a future date nobody's calendar reaches. A product-level conformance declaration can confirm a practice happened once. It can't confirm an organization is set up to keep doing it, with a named owner, a measurement in place, and a habit of learning from what didn't go well.

That's the case for certifying the organization, not just the service. If your organization can point to a TS 20125 conformance declaration for one product but can't say who owns decommissioning for the next five, that's worth looking at closely.

If you want to see exactly how GSP™ Level 2 maps to all six TS 20125 phases, or want a second set of eyes on your own organization's coverage, get in touch (/contact/). And if you haven't looked at GSP™ (/gsp/) itself yet, this is a good moment to.
