---
title: "Complexity and the Cynefin Framework"
date: "2021-02-08"
relatedTerms: ['estimation']
---

We encounter complexity whenever we're asked to estimate how long it will take to fix a bug. Or when we're asked how long it will take to bring a novel product to market. We don't know what we can't know.

This is where Cynefin helps. Unfortunately, this theory has a complicated description. **Cynefin** is a poorly named mental model to help us see that different kinds of problems need different approaches. The word "cynefin" is the Welsh word for "habitat" and is pronounced: kuh-NEV-in. (It took me several years to learn to say it, so you're in good company if you're confused.)

Its creator, David Snowden, calls it a sensemaking tool, i.e. a tool to help you understand which domain your current problem lies in, and what actions to take based on that fact.

![](src/content/glossary/complexity/images/cynefin-chart.jpg)

That's a fancy picture with a lot of words.

### **Clear** Domain

(_This was formerly called Simple/Obvious_). In the world of software development, implementing an algorithm that has an existing recipe is an example. Outside of software, it is any activity that is well understood or that you can find a recipe for.

If it is **clear** what the outcome will be from the start, implementation is a matter of execution. If asked, you could have written down the steps involved in the work beforehand. With a high degree of predictability, estimation is practical and the approach of estimating in terms of hours/days will be more effective.

In the **Clear** domain, write down the plan and execute it, and things will probably go according to plan.

### **Complicated** Domain

In the world of software implementing, an example is a new feature with at least some acceptance criteria, or building a new product in an area where the rough needs have already been understood. Outside of software, it is something that someone has done before, so you know the problem is solvable, but you don't necessarily know what the solution is.

From the starting point, you can see the rough end state. You couldn't write the steps it would take to get to the destination, because they weren't all known and the destination moved a few times along the way. As the destination and the individual work items aren't as well understood, the work is less predictable. Relative estimation, (e.g. Planning Poker) can be used as a tool to help people sense the volume of work and get a rough idea of which items are bigger or smaller. _We often get requests to help teams with more accurate estimation, but in this domain that is simply impossible_.

In the **Complicated** Domain, create a rough plan, start executing, and adapt. In Product Development this is the classical use of Scrum.

### **Complex** Domain

Our original example of a software bug or creating a novel product are both in the complex domain. When we start, they're poorly understood. No one has solved this bug before. No one has built this type of product before. Outside of software, writing a book in an area that we don't know well is an example. We don't know if we can find enough information to describe the area well, or even if the area is well understood.

From the starting point, we don't see anything with clarity. Complexity can stem from the number of variables that affect our problem, the number of sources of information or, worse, the number of completely unknown things. In this environment, we have very little predictability. Estimation in this domain is a waste - more useful is to timebox an activity, saying, "We will do this for some number of hours or days and see how far we get or what we learned."

In a **Complex** Domain, run an experiment and see what it tells you. When working on a bug, it may then become Clear or Complicated. When doing Product Development work, the experiment will tell us what problem our audience wants solved. As the problem is narrowed, we can shift to normal Product Development work (e.g. the **Complicated** Domain). Effectively, this describes some of the ideas behind Lean Startup and Lean U/X.

### **Chaotic** Domain

The system we're part of is off the rails. In the world of software development, this might be a key service that is offline. In the world outside of software, examples might include an oil pipeline that has burst and is leaking.

In a **Chaotic** Domain, take action and contain the problem. Chaos requires novel solutions and is typically transitory. Once the problem is contained, we want to move the problem to another domain (e.g. Complex or Complicated).

### **Confused** Domain

(_Formerly called Disordered._) We don't know where we are. Our job in this domain is to gather just enough information to sense which domain our problem is actually in, and then act from there.

Cynefin doesn't solve any problem for you, it is instead a "lens" to look at the world through. It helps you sense where you're at with a problem and then make better decisions.

#### Resource Links:

- [Cynefin Framework - an Introduction from its Creator](https://thecynefin.co/about-us/about-cynefin-framework/)
- [Cynefin for Everyone!](https://lizkeogh.com/cynefin-for-everyone/)
- [Cynefin: The Tool That Doesn't "Do" Anything](http://www.theillinoismodel.com/2020/05/cynefin-tool-that-doesnt-do-anything.html)
- [On Uncertainty, Prediction, and Planning](https://www.infoq.com/articles/uncertainty-prediction-planning/)
- [Practical Applications of Complexity Theory in Software and Digital Products Development](https://www.infoq.com/articles/practical-application-complexity/)
- [Cynefin Framework — Domains that can help in all environments!](https://medium.com/cynefin-framework-domains-that-can-help-in-all/cynefin-framework-domains-that-can-help-in-all-environments-7a527c3519ed)
- [Understanding the Cynefin framework – a basic intro](https://www.everydaykanban.com/2013/09/29/understanding-the-cynefin-framework/)

#### Estimation in Complexity:

- [Cynefin Context Cards – Enabling Discovery and Delivery and Innovation in Agile teams](https://dandypeople.com/blog/cynefin-context-cards/)
- [Complexity Poker/Estimation](https://media.dandypeople.com/2018/09/context-tactics-cards-printout.pdf)
- [Estimating Complexity](https://lizkeogh.com/2013/07/21/estimating-complexity/)

#### Exercises to Understand Cynefin:

- [Cynefin simulation – create aha feeling in 20 min](https://dandypeople.com/blog/cynefin-simulation-create-aha-feeling-20-min-plan-deliver-complex-situations/)
- [New exercises for teaching Cynefin](https://www.chriscorrigan.com/parkinglot/new-exercises-for-teaching-cynefin/)
- [Teaching the five Cynefin domains using physical exercises](https://www.chriscorrigan.com/parkinglot/teaching-the-five-cynefin-domains-using-physical-exercises/)

