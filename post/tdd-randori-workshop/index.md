---
title: "TDD Randori Workshop"
date: "2008-10-23"
categories: 
  - "software-development"
  - "tdd"
excerpt: 'A few weeks ago I ran my first [Coding Dojo/Randori](/blog/tdd-randori-session) and'
---

A few weeks ago I ran my first [Coding Dojo/Randori](/blog/tdd-randori-session) and while the participants learned from the session there had been a few key flaws:

- The problem was too big
- The problem was in a domain that was unfamiliar to everyone
- The facilitator (me) participated too much _Ouch. It was true_.

This week we ran a second session and had a much better time. The key to success - pick a smaller problem and let people struggle for a good long time before making suggestions. In addition remind them frequently to ask the audience for help.

This week's problem:

Score a [bowling](external:https://en.wikipedia.org/wiki/Bowling) game, (credit to Bob Martin and Ron Jeffries for the idea) based on the following rules:

- A single bowling game consists of ten frames.
- For each frame, a bowler is allowed a maximum of two rolls to knock down all ten pins
- When a Strike is thrown, the current frame is finished
- Scoring: • 0-9 pins knocked down: score the number of pins • Spare: 10 + number of pins knocked down by the next throw • Strike: 10 + number of pins knocked down by the next two throws.

Effectively this means the ball after a Spare is counted twice - once for the spare and once for the strike. With Strikes the next two balls are counted twice.

[**Scoring Examples**](external:https://en.wikipedia.org/wiki/Ten-pin_bowling#Scoring) (from wikipedia): A **Single** strike:

Frame 1, ball 1: 10 pins (strike)

Frame 2, ball 1: 3 pins

Frame 2, ball 2: 6 pins

**The total score from these throws is:**

- Frame one: 10 + (3 + 6) = 19
- Frame two: 3 + 6 = 9

**TOTAL = 28**

**Mulitple** strikes:

Frame 1, ball 1: 10 pins (Strike)

Frame 2, ball 1: 10 pins (Strike)

Frame 3, ball 1: 10 pins (Strike)

Frame 4, ball 1: 0 pins (Gutterball)

Frame 4, ball 2: 9 pins

**The total score from these throws is**:

- Frame one: 10 + (10 + 10) = 30
- Frame two: 10 + (10 + 0) = 20
- Frame three: 10 + (0 + 9) = 19
- Frame four: 0 + 9 = 9

**TOTAL = 78**

It appears this problem was much better suited to where the group is at now. To start the process off I seeded the work with a few tests (TestOneThrow(), TestTwoThrows(), testMutilpleFrames(), testMidFrame()) and a trivial amount of code to satisfy the problem. As the product owner I asked the team to add the following features:

- The bowler throws one spare
- Scoring reverts to normal after throwing a spare
- The bowler throws a strike
- Scoring reverts to normal after a strike
- _Score successive spares_
- _Score successive strikes_
- _Score a perfect game (300 pts)._

We made fairly good progress through the feature list but didn't manage to tackle the last three features. With one of the failing tests early on we had good example of why the parameter order matters in JUnit's asserts. The asserts are written assertEquals(Expected, Actual) = if the test fails JUnit says "Line XXX epxected 42 was 22". Get the parameters in the wrong order and more than a few minutes will be wasted trying to solve the wrong problem.

Towards the end (working on the the bowler throws one strike) the pair at the computer was bogging down unsure why things weren't working. At this stage I intervened and helped add sysout's in every branch to illuminate what paths were being followed, It turns out that several mistakes had been made and the wrong paths were being followed in test cases. While I shouldn't have intervened it did break the log jam and allow the team finish the feature. At this stage the team feels the code is a bit of a mess and so we will pick up the exercise from the same place next time.

Our retrospective generated a much smaller set of notes this time: **Happy**:

- Lots of pizza
- Good problem (everyone understands the rules of bowling)
- Fun to learn about bowling
- Good hands on experience
- Much better level of involvement from the facilitator
- Having some working tests and code to seed the exercise is much better than starting from a blank file.

**Sad**:

- Need more involvement from the audience.
- Should've brought a mouse - _I did last time Doh_.
- Didn't really understand bowling until halfway through the session

So net result I picked a better problem than last time and we all learned a little about TDD. In addition we all discovered that scoring in bowling looks deceptively simple but in actual fact is a non-trivial problem.

Problem sources for Coding Dojo's:

- Coding Dojo Wiki
- [TDD Problems Wiki](external:https://sites.google.com/site/tddproblems/)
- [Danilo Sato](external:https://www.dtsato.com/blog/2008/10/21/source-of-problems-for-your-coding-dojo/) mentions a few others that I'm not familiar with.

Have you tried a Randori or Coding Dojo? What was your experience?
