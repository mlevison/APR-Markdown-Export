---
title: "TDD Randori Session"
date: "2008-10-08"
categories: 
  - "software-development"
  - "tdd"
tags: 
  - "coding-dojo"
  - "danilo-santo"
  - "tdd-randori"
  - "test-driven-development"
  - "workshop"
excerpt: 'We ran our first TDD [Randori](https://en.wikipedia.org/wiki/Randori) session at lunch'
---

We ran our first TDD [Randori](https://en.wikipedia.org/wiki/Randori) session at lunch today (approx 15 attendees). I was inspired by Dave Nicolette's session at Agile 2008 and used the [Danilo Santo's](https://www.dtsato.com/blog/2008/08/12/coding-dojo-agile-2008/) paper on their Brazilian Coding Dojo as a guide.

In a Randori we work as a group trying to solve a **small** problem using TDD:

- There is one computer with the video output projected on a screen so all participants can see it.
- Coding is done at the single computer by a pair of developers.
- One half of the pair switches out every 5 or 10 minutes.
- The pair on the keyboard should continuously explain what they are doing.
- The pair on the keyboard should stop when someone from the audience falls off the sled — and only continue when that someone is back on track again.
- The audience should give comments on design only when there is green bar. (During red bar audience can only ask questions)
- The pair should not continue on writing new code if other participants are not happy with the current design (The code should be always well refactored before starting to write new code)
- The pair will use TDD (Test-Driven Development).

I picked the problem based on a complaint I've heard from people after many of the TDD classes: "the examples are too trivial and don't speak to real world problems. I also hear that we don't enough chance to practice TDD".

For our initial example to trying working through we tried: Brian Marick's "[A workbook for practicing test-driven design](http://www.exampler.com/blog/2007/06/26/a-workbook-for-practicing-test-driven-design-draft/)". The problem and sample code come from the world of Hierarchical Data Format (HDF), a library for storing large amounts of scientific data. Brian provides an initial simple implementation and then invites the reader to make some changes:

1. ...
2. Add the ability to read and write unsigned 4-byte integers, something like:
    
    ```
    dataset.defineMember(Like.unsignedInteger(4));
    ```
    
3. Add the ability to write arrays of Strings...
4. Surprise the PO changed their mind_._

So far so good. In the 60 minutes of coding time we had we were able to make solve #2 with an elegant solution, but got hung up in #3. To introduce Strings we had to take a big step, much bigger than TDD would encourage. Net result we got caught in a bit of tangled mess and ran out of time before could tidy it up.

After the session we conducted a very short retrospective using happy and sad post it notes and dot voting (both from [Agile Retrospectives: Making Good Teams Great](https://www.amazon.com/Agile-Retrospectives-Making-Teams-Great/dp/0977616649/&tag=notesfromatoo-20)).

In the Happy category we had:

- Live Exercises are fun.
- Talk about the advantages of TDD were good.
- Good to go through an example with everyone and the discussion that was raised.
- Excellent discussion of choices around refactoring
- The example was good. _Oddly enough this will be contradicted later on._
- Initial Tests went well
- Good Practical Introduction to TDD.

In the Sad category we had:

- Just use a simple Java class and grow it using TDD.
- The problem domain for the example was too abstract for most people and was hard to make sense of. _Solution try a problem domain that people are familiar with i.e. Ron Jeffries Bowling game etc._
- The Example required too much assistance and special knowledge from the moderator.
- Start with no tests on an existing project.
- Too much discussion from the audience.
- The moderator (me) was too involved in the exercise. _Solution maybe I shouldn't be moderator for these sessions._
- Topics not **directly** related to the exercises should be parked. _Oooppss. I've was so focused on the content I forgot to put up a parking lot._
- Let people make mistakes.
- The pilot and co-pilot were often too quiet
- A separate high level introduction to TDD and its advantages was requested.
- **We ran out of PIZZA**. 2 extra large pizzas will not feed 15 people.

**Going Forward**

A single session will not hone anyone's TDD (nor my moderation) skills. I suggest that we continue to meet in the future (every two weeks). For the next session I will find a smaller problem - perhaps a few classes of untested code. We can set the goal testing it, simplifying it and making changes as requested by a mythical product owner.

Beyond this it would be useful to have sessions that focus on: Mocks, Test Doubles, GUI's (Presenter First?), Web Apps, Databases?, other real world problems that teams are encountering as part of TDD. [Test Driven: Lasse Koskela](https://www.amazon.com/Test-Driven-Acceptance-Java-Developers/dp/1932394850/&tag=notesfromatoo-20) is an excellent source book for ideas in this area.

BTW Brian's HDF workbook is an interesting problem I just wouldn't expect to tackle it 60 minutes of coding time.

_Update: I forgot to mention the [TDD Problems site](https://sites.google.com/site/tddproblems/)._

_Update 2: The followup session: [Another TDD Workshop](/blog/tdd-randori-workshop.html)._
