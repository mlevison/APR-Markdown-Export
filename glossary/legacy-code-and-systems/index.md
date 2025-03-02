---
title: "Legacy Code and Systems"
date: "2021-05-04"
relatedTerms: ['approval-tests', 'technical-debt']
excerpt: 'Legacy code is often described as code checked into the system without a unit test. A'
---

Legacy code is often described as code checked into the system without a unit test. A popular definition from Michael Feathers, author of Working Effectively with Legacy Code.

The term “legacy code” is commonly used to refer to a codebase that has become increasingly difficult to maintain. There might be a number of reasons: complexity, hard to read, use of old apis or idioms. Maybe the original developers have left and their successors don’t understand the design choices that were made to get there.

The issue with legacy code is often made worse by a lack of reliable automated tests, so team members can’t easily tell if changes they make break the existing system.

## Fixing Legacy code

Fixing legacy code does not come with a magic wand.

- **Churn + Complexity** - Look for the biggest pain points first - look for the files that change the most frequently, that also have high code complexity
- **Time** - Understand fixing this isn’t an overnight activity. Instead of taking a year off to fix all the problems, a more realistic approach - take at least 30% of the team’s time to work on remediation.
- **Fence and Add Tests** - Identify testable boundaries, start writing automated tests that prove the behaviour of the system inside the boundary is stable.
- **Incremental Tidy Up** - within the boundaries of passing tests, take small steps to improve.
- **Pair or Ensemble Programming** - a big problem with legacy code is that no one understands it. Pairing and Ensemble will spread knowledge throughout the team and reduce the time it takes to understand.
- **Continuous Integration** - Checkin Frequently and keep rerunning automated tests.
- **Static analysis tools** - can help to a limited degree, hile these tools can help identify complex code, they don’t tell you what do with the code.
- **Microservices** - another popular but limited tool. Splitting a large mess into smaller parts might seem beneficial, but remember that a mess divided is still a mess.

Finally have empathy for the people who wrote this code. It might even have been an younger version of yourself. The real magic is in putting the focus on improving the readability of the code and raising the bar on quality Sprint over Sprint.

[Reinventing Existing Products – Big Bite vs Small Nibble Rewrites](https://agilepainrelief.com/blog/reinventing-existing-products-big-bite-vs-small-nibble-rewrites.html)

#### Resource Links:

- [An Agile Approach to a Legacy System](https://cdn.pols.co.uk/papers/agile-approach-to-legacy-systems.pdf)
- [Changing Legacy Code Safely](https://codemanship.wordpress.com/2019/12/12/changing-legacy-code-safely/)
- [Changing untested code, without breaking it](https://understandlegacycode.com/changing-untested-code/)
- [Characterization Testing](https://michaelfeathers.silvrback.com/characterization-testing)
- [Cleaning Code – Tools and Techniques for Legacy Restoration Projects](https://www.infoq.com/presentations/large-legacy-techniques-tools)
- [Code Retreat](https://coderetreat.org/)
- [Demystifying the Dependency Inversion Principle](https://blog.thecodewhisperer.com/permalink/consequences-of-dependency-inversion-principle/)
- [Get your Legacy C into a test harness](https://wingman-sw.com/articles/tdd-legacy-c)
- [Getting into a large codebase](https://understandlegacycode.com/getting-into-large-codebase/)
- [How To Do Large Scale Refactoring](https://www.infoq.com/news/2010/08/large-scale-refactoring)
- [Leapfrogging Online Payments & Burying Tech Debt](https://www.infoq.com/presentations/refactoring-erlang)
- [Legacy Application Strangulation : Case Studies](https://paulhammant.com/2013/07/14/legacy-application-strangulation-case-studies/)
- [Legacy Code Rocks (entire blog)](https://legacycoderocks.libsyn.com/)
- [Migrating legacy applications – 7 points for doing it the agile way](https://www.ontheagilepath.net/2015/11/migrating-legacy-applications-7-points-for-doing-it-the-agile-way-and-avoid-big-bang-intransparent-approaches.html)
- [Monolith to Microservices Using the Strangler Pattern](https://dzone.com/articles/monolith-to-microservices-using-the-strangler-patt)
- [Pragmatic Techniques for Maintaining a Legacy Application](https://www.infoq.com/articles/Pragmatic-Legacy-App-Maintenance)
- [Refactoring Legacy Applications: A Case Study](https://www.infoq.com/articles/refactoring-legacy-applications)
- [Refactoring Legacy Code](https://code.tutsplus.com/series/refactoring-legacy-code--cms-633)
- [Safely restructure your codebase with Dependency Graphs](https://understandlegacycode.com/blog/safely-restructure-codebase-with-dependency-graphs/)
- [Seventeen Secrets of the Great Legacy Makeover Masters](https://www.infoq.com/presentations/17-Secrets-Legacy-Code)
- [StranglerFigApplication](https://martinfowler.com/bliki/StranglerFigApplication.html)
- [Strangler Pattern: How to Deal With Legacy Code During the Container Revolution](https://cloudnativenow.com/topics/cloudnativedevelopment/strangler-pattern-dealing-with-legacy-code-in-the-age-of-containers/)
- [The Strangler pattern in practice](https://www.michielrook.nl/2016/11/strangler-pattern-practice/)
- [Strategies for Effectively Managing Legacy Systems](https://www.infoq.com/presentations/strategies-for-effectively-managing-legacy-systems)
- [The Pain of Implicit Dependencies](https://blog.thecodewhisperer.com/permalink/the-pain-of-implicit-dependencies/)
- [What your tests don’t need to know will hurt you](https://blog.thecodewhisperer.com/permalink/what-your-tests-dont-need-to-know-will-hurt-you/)
- [Wrestle Legacy C and C++ into a Test Harness – Linker Errors](http://blog.wingman-sw.com/wrestle-legacy-c-cpp-into-tests-linker-errors)

##### LEGACY CODE AND SYSTEMS BOOKS

- _[Beyond Legacy Code: Nine Practices to Extend the Life (and Value) of Your Software](https://www.amazon.ca/Beyond-Legacy-Code-Practices-Software/dp/1680500791/&tag=notesfromatoo-20/&tag=notesfromatoo-20)_ – David Scott Bernstein
- _[The Mikado Method](https://www.amazon.ca/Mikado-Method-Ola-Ellnestam/dp/1617291218/&tag=notesfromatoo-20/&tag=notesfromatoo-20)_ – Daniel Brolund, Ola Ellnestam
- [_Working Effectively with Legacy Code_](https://www.amazon.com/Working-Effectively-Legacy-Michael-Feathers/dp/0131177052/&tag=notesfromatoo-20/&tag=notesfromatoo-20) – Michael Feathers

