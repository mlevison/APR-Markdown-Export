---
title: "Advantages of TDD"
date: "2008-10-14"
categories: 
  - "software-development"
  - "tdd"
tags: 
  - "refactoring"
  - "software-development"
  - "solid-code"
  - "test-driven-development"
  - "yagni"
excerpt: 'During last weeks [TDD Randori session](/blog/tdd-randori-session) I was asked, what'
---

During last weeks [TDD Randori session](/blog/tdd-randori-session) I was asked, what are the advantages of TDD. Here is my short list:

- - Writing tests first require you to really consider what you want from the code
    - Short feedback loop
    - Creates a detailed specification
    - Reduced time in rework
    - Less time spent in the debugger and when it is required you usually get closer to problem quickly
    - Tells you whether your last change (or refactoring) has broken previously working code
    - Allows the design to evolve and adapt to your changing understanding of the problem.

- Simplification
    - Forces radical simplification of the code - you will only write code in response to the requirements of the tests.
    - Forces you to write small classes focused on one thing.
    - Helps create loosely coupled code
    - Creates SOLID code (Articles: [Bob Martin](https://butunclebob.com/ArticleS.UncleBob.PrinciplesOfOod) and [Chad Myers](https://lostechies.com/chadmyers/2008/03/08/pablo-s-topic-of-the-month-march-solid-principles/))
- The resulting Unit Tests are simple and act as documentation for the code
- Improves quality and reduces bugs by:
    - forcing us to consider purpose (and the specification of code)
    - simplifying code (many bugs come from the complexity)
    - ensuring changes and new code don't break the expectations of existing code

### Disadvantages?

TDD is hard to learn, especially on your own. You can expect reduced productivity for 2-4 months after starting.

Other articles that discuss the benefits of TDD: [Twelve Benefits of Unit Tests](http://sd.jtimothyking.com/2006/07/11/twelve-benefits-of-writing-unit-tests-first/), Research Supports The Effectiveness of TDD, [TDD Research Findings](https://weblogs.asp.net/mhawley/114005), [How TDD improves development speed and is very cost effective](https://danbunea.blogspot.com/2005/09/how-tdd-improves-development-speed-and.html), [Test Driven Development Requires Less Debugging](https://www.thekua.com/atwork/2007/10/test-driven-development-requires-less-debugging/).

Finally as I stated at the time I believe that these benefits can't be achieved by writing tests after the fact.

Next up will be a short item outlining a one possible TDD adoption strategy.
