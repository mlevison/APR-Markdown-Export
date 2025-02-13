---
title: "Scrum By Example – The Team Learn How to Learn"
date: "2012-03-28"
categories: 
  - "scrum-by-example"
tags: 
  - "daily-scrum"
  - "refactoring"
  - "scrum-by-example"
  - "sonar"
  - "story-splitting"
  - "tdd-randori"
  - "technical-debt-2"
coverImage: "photodune-1277447-dark-dojo-xs.jpg"
excerpt: 'During the Standup Ian reports that he is starting his third day of'
---

![dark dojo - image licensed from Photodune](src/content/blog/scrummaster-tales-the-team-learn-how-to-learn/images/photodune-1277447-dark-dojo-xs.jpg) The Team is struggling to pay off the [Technical Debt](https://agilepainrelief.com/blog/scrummaster-tales-stop-digging-new-holes.html) (or mess) that they’ve spent the last six months accumulating. They’ve started to institutionalize writing Unit Tests (by adding it to “Done”) and they’re using [Sonar](https://www.sonarsource.org/) to help track Code Coverage, PMD warnings, et al. (_Ed: Don’t take Sonar or any other measure as more than a first order view of the code. It hints where you need to look, no more)._

## Story

During the Standup Ian reports that he is starting his third day of refactoring\[[1](#footnotes)\], a [monster class](https://lostechies.com/chrismissal/2009/05/28/anti-patterns-and-worst-practices-monster-objects/) called BuyABook. ScrumMaster Steve’s antenna goes up immediately, after all the team had split all tasks in one day or less. After standup he stops to have a quick chat with Ian to find out what is up. Ian explains that this class depends on many other classes and as a result it is very difficult to test. He continues that he’s been reading the Feathers book: “[Working Effectively with Legacy Code](https://www.amazon.com/Working-Effectively-Legacy-Michael-Feathers/dp/0131177052/&tag=notesfromatoo-20)” but it’s a struggle to put the ideas into practice. When he’s finished, Steve talks to Doug and Martin finding that they’re having similar problems.

Steve puts on his thinking cap. He knows the team needs practice and knows that they need a safe place to do it before they use the ideas in the main stream code. After a few minutes Goggling, he stumbles on the idea of [coding dojos](https://codingdojo.org/) and, based on the experience of others, [TDD Randori Session](/blog/tdd-randori-session.html), [TDD Randori Workshop](/blog/tdd-randori-workshop.html) and [My First Coding Dojo](https://www.lagerweij.com/2011/06/23/my-first-coding-dojo/). The idea behind a Coding Dojo is taken from the world of Martial Arts. It is just a safe place to practice. In this case Steve imagines the team would like to be able to practice the ideas that Feathers proposed, either on an artificial problem or on a small problem in their own code base. He sees them getting together in a meeting room with a projector and solving a small problem as a team.<!--more-->

Reading the experience posts, Steve learns:

- It’s best to start with small problems
- Bring a real mouse, not just a laptop trackpad
- Pair Programming is best – one driver and one navigator
- Ask the pair to explain their decisions, making it clear to the audience what is happening. In addition it keeps the audience engaged.
- Rotate the pair partners every 5-7 minutes
- Get enough Pizza for everyone
- 90-120 minutes is about the right length
- Small steps
- Ask questions if you don’t know what’s going on
- Hold a retrospective at the end

Steve gathers the team together and proposes the idea. They agree instantly, but Ian points out that “BuyABook” class is awfully large to get their heads wrapped around in 90 minutes. Instead they agree to tackle a smaller problem and get the “ChargeBookToMasterCard” under test.\[[2](#footnotes)\] They agree to run the Dojo the next day at lunch.

They gather in a meeting room with a projector, a laptop, and a couple of other developers from a sister team that is also working on the bookstore. Steve had invited everyone to spend a few minutes preparing for the session by studying the code beforehand. After a brief introduction to Coding Dojos (see Wouter Lagerweij’s [presentation via Slideshare](https://www.slideshare.net/wouterla/coding-dojo-in-5-minutes)), Ian frames the problem. ChargeBookToMasterCard is difficult to test because all the existing constructors require access to the MasterCard processing server.

After a few minutes of struggling to understand the myriad of methods on the Mastercard, they realize that “ChargeBookToMasterCard” really only uses three of those of methods. They conclude that using a Facade to wrap the MasterCardProcessor is the simplest way to go. With the Facade they can either pass in the real MasterCard processor, or a fake that can be used for testing. (_Ed: Yes, this essentially manual mocking and real Mock tool would be faster to use)._ Once they’re able to construct a “ChargeBookToMasterCard”, now they can start trying to test the public methods and refactor the ones which are complex. At the end of 90 minutes they’ve got a good start at refactoring a previously challenging class. If they’re happy with the code quality they could check it in, otherwise a developer can use the work as inspiration to do the actual tidy up. Since Coding Dojos invite us to take risk, they usually don’t result in code that you can use.

During the retrospective, Ian says that the exercise has helped him see a way of biting off smaller chunks of work when paying down technical debt. In addition, Doug says he now has a much better understanding of the payment system. The team agree to hold another Coding Dojo next week.

## Analysis

For a couple hours of time and the price of some pizza the team members have gained a little confidence at doing something that had previously seemed hard and risky. While there are still many more hills to climb, knowing that it's possible is often one of the biggest barriers to paying down Technical Debt. When we see just how small some problems are, it becomes a bit easier. In addition, all the developers on the team have learned some new ideas today. It will take months to get the team to the place that we see as possible, but they will only get there one step at a time.

Notes:

\[1\] I always take exception to this misuse of the word "refactoring". [Refactoring](https://refactoring.com/) is “a series of small behavior preserving transformations”. When we have to talk about a multi-day refactoring it's long past the point of small. If they must happen, I call them rework or rebuilding.

\[2\] Serendipity. Just after inventing “ChargeBookToMasterCard” I grabbed Feathers' Legacy Code book of the shelf, opened a random page, and found a very detailed example of the problem we will tackle on pages 106-113 [The Case of the Irritating Parameter](https://books.google.ca/books?id=fB6s_Z6g0gIC&pg=PT134&lpg=PT134&dq=The+Case+of+the+Irritating+Parameter&source=bl&ots=Z4MpQDGSGj&sig=ZUoXSwSDotI7aginC7KnklaOHzE&hl=en&sa=X&ei=KzJzT5nzI8i9gAflru1S&ved=0CB8Q6AEwAA#v=onepage&q=The%20Case%20of%20the%20Irritating%20Parameter&f=false) (link to Google Books)

_**[Scrum by Example](/blog/category/scrum-by-example) is a narrative-style blog series designed to help people new to Scrum, especially new ScrumMasters. If you are new to the series, we recommend you [check out the introduction](/blog/scrum-by-example.html) to learn more about the series and discover other helpful articles.**_

Images via: [https://photodune.net/](https://photodune.net/)
