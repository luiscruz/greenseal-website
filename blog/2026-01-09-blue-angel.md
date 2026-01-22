---
layout: page
title: "Why do we need GSP™ when we have Blauer Engel?"
---

Although there are not many alternatives to certifying software organizations w.r.t. their commitment to building energy-efficient and environmentally friendly software products, a few options are out there. One of my favorites is Blauer Engel, a sustainability label developed by the German government to certify general consumer products. In this blog post, we will see what it is and why [GSP™] is still the best choice for software organizations that are truly committed to developing sustainable products.

## What is Blauer Engel?

Blauer Engel (German for "Blue Angel") is Germany's official eco-label, introduced in 1978 as the world's first environmental certification label. It identifies products and services with reduced environmental impact compared to conventional alternatives, while still meeting high standards for quality, health, and usability. It applies to many categories, including paper products, textiles, IT equipment, cleaning products, construction materials, amongst others. Since 2020, Blauer Engel has also included software products.

All the criteria are specified in a clear document, publicly available [here](https://produktinfo.blauer-engel.de/uploads/criteriafile/en/171/DE-UZ%20215-202406-en-Criteria-V4.pdf). Although it's an interesting read, let me briefly summarize it for you: to get the label you need to  
1) run and report energy tests on a common use case of the software;  
2) be transparent about hardware and software requirements;  
3) make sure that 5-year-old hardware can run the software product; and  
4) respect user autonomy — using open data formats, well-documented APIs that use open standards, allowing uninstallation, and being free from advertising and user tracking.

## Then why do we need GSP™?

While Blauer Engel is a great initiative and something worth following, it is far from perfect and leaves a lot of space for improvement. Here are a few points they have missed and where [GSP™] brings a fresh solution.

### GSP™ focuses on energy efficiency

[GSP™] goes an extra mile to make sure software teams have a process that enables them to deliver energy- and resource-efficient software and AI features. Although Blauer Engel requires that energy tests are run and reported, the results are not really actionable. They are rather a framework for transparency w.r.t. energy consumption than an enabler of energy efficiency. A few examples of these energy tests have even been publicly disclosed and later reproduced. I definitely recommend reading through the [replication done by Green Coding](https://www.green-coding.io/blog/reproducing-blauer-engel-okular-measurements?utm_source=greenseal.dev) of the Okular measurements.

Blauer Engel is an afterthought. It requires teams to apply for a certification upon releasing the product. When it comes to energy efficiency requirements, they mostly revolve around reporting energy consumption data while running the software. It is also required that there is a replication package that allows reproducing energy tests and results. We argue that this approach does not really change whether code is actually green or not — it mostly makes sure that whatever energy usage it has is clear to the consumer. We consider that a great start, but it is not enough.

With [GSP™], we require teams to continuously monitor the resource usage of their software. It does not need to be anything super sophisticated, but it does require developers to stay on top of which features and components should be prioritised for optimization. We also require green coding — as in coding with resource efficiency in mind — to be promoted and appreciated within software teams.

### Certifying organization vs product

[GSP™] focuses on the organization, while Blauer Engel focuses on the product. While there is no right or wrong here, this subtle difference plays a big role. [GSP™] makes sure that the organization has development processes with a maturity level that enables teams to build software that meets sustainability requirements. In other words, it makes sustainability a natural result of the organization's culture.

This shift in target ensures that energy efficiency is not an extra mile teams need to run in order to get an eco label, but rather something that is intrinsic to their values and way of working. We argue that this shift is more likely to help build better and more sustainable products in the long run.

---

Ultimately, GSP™ is not meant to replace initiatives like Blauer Engel, but to complement and extend them. Transparency is an essential first step, but real impact comes when energy efficiency is built into everyday engineering decisions. By focusing on processes, culture, and continuous feedback, GSP™ aims to make sustainability something teams practice by default — not something they certify at the very end.

To learn more about the certification of Green Software Practices, check out the [GSP™ info pages]({{"/gsp" | absolute_url}}) or schedule a [free call with us]({{"/contact" | absolute_url}}).

[GSP™]: /gsp
