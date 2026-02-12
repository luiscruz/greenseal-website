---
title: "What no one is telling you about measuring energy of software."
layout: blog
author: Luís Cruz
date: 2026-01-20
---

Software is improving our society in several ways.
Thanks to software, our cars are much safer, healthcare is optimized, knowledge is more accessible, and so on.
All these massive benefits also come with important challenges.
We have all heard of the risks of disinformation, doom scrolling, and so on.
However, there is a silent risk that very few people are talking about: just how power hungry the software behind all our apps and services really is.
All the apps, services, and AI products we use every day are running inside massive data centers that house an incredible number of servers.
These massive data centers consume enormous amounts of resources from their surrounding environments.
We are not talking only about resources such as electricity and drinkable water. This also includes the footprint of building all the hardware, including the carbon footprint of manufacturing and the use of rare materials.


The way we build our software plays an important role here.
There are myriad ways of designing and creating software systems. Some of them are far more efficient than others.
To illustrate this problem, if you drive a big truck just to give a ride to your grandmother to the city or if you drive a small car, you can get the job done with both vehicles, but with the small car you will spend a lot less gas and contribute a lot less to traffic jams along the way.
Although this sounds obvious, software operates so well behind the curtains that we as users cannot tell these two cases apart.
Software development is about getting the job done; if something works as expected, developer teams will simply move on to the next feature.
In software, there is no incentive to turn that big truck into a smaller and more efficient vehicle. There is no incentive for developers to improve the energy effiicency of their code: not from managers, not from product owners, not from users, and not from most other stakeholders involved.

> In software (…) There is no incentive for developers to improve the energy effiicency of their code (…).

To make matters worse, measuring resource usage of software is a lot more difficult than it sounds. Reusing the metaphor of truck/car, in those vehicles one could simply use gas L/100km (or miles/gallon, or kWh/100km, etc.), and then measure the consumption depending on driving style or driving conditions: e.g., urban, highway, mixed, etc. Such standardization allows different vehicles to be compared in a fair way.
When it comes to software, achieving similar standardization is much harder.
The energy consumption of the software depends on the actual hardware where it runs. One cannot compare a software’s or AI’s energy efficiency using different hardware. Those results would probably say more about the hardware efficiency than about the software.

At the same time, every month there are several new hardware platforms where software can run. Even if we compare software using a particular controlled hardware, there is a chance those numbers are not comparable in a way that allows us to draw clear conclusions about the energy efficiency of the software and its features. This complexity also gives room for misinterpretation of energy consumption data and can potentially lead to favoring the wrong software (either by mistake or on purpose…).

This is why there is much more to energy-efficient software than measuring its energy consumption when it runs a given set of use cases.
In particular, rather than having super precise measurements, it is more important to make sure there is an incentive to continuously improve the energy efficiency of the software over time.
This is done with proper monitoring strategies, with the right tools, and with the right development practices.
Making energy efficient code does not need to be an afterthought. It can be embedded in day to day development activities.
By making energy efficiency improvement a natural step in the development process, developers can easily prioritise code improvements that bring visible value.
For example, if the development team knows at any point in time what are the SQL queries that are more resource-intensive across the software product, they will be able to easily prioritise improving those queries and get visible feedback on the improvement.
An interesting detail here is that one does not need the most perfect energy measurement setup; one can rely on simple estimations or proxies of energy, such as memory size, execution time, CPU-hours, and so on.
The simple fact that we improve on rough indicators is already a sign that we are incentivising the creation of software that is more likely to be energy efficient and environmentally friendly.

> One does not need the most perfect energy measurement setup

And when we talk about SQL queries, we can also talk about many other examples. In the context of large language models (LLMs), we can rely on the number of tokens in a prompt and in the corresponding response, or the size of the model required to answer the prompts correctly. We can even consider the billed cost of consuming an LLM API. In the context of machine learning, one could consider memory and CPU usage; in the context of web design, one could consider the size of assets, for example images or other media types.

Another important side effect of following green software practices is that teams learn a great deal about energy efficient coding techniques. Despite all the initiatives around energy patterns, there is still a huge lack of practical tips and guidelines to help make software energy efficient. By following the proper process, not only will you build energy efficient code, but you will also develop your own set of guidelines that very few people have heard about.

Now, the real question is this: when you are developing your software, do you follow a process that enables you to make the software energy-efficient?
Do you monitor the resource consumption of your software?
Do you inspire other colleagues and teams to do the same and to learn from your experiences?


This is where the [GSP™] certification plays an important role: we want to make sure software companies have the right roadmap to build sustainable software by default. In addition, [GSP™] makes sure that those companies get the right recognition for it! If you are doing an extra mile to build green software, you should be able to get credit for it. Not only will your customers learn how cool you are, but you will also inspire others to follow your lead!

[Learn more about the GSP™ certification](/gsp).

[GSP™]: /gsp
