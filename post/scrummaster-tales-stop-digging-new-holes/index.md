---
title: "Scrum by Example – Stop Digging New Holes"
date: "2012-02-28"
categories: 
  - "books"
  - "scrum"
  - "scrum-by-example"
tags: 
  - "definition-of-done"
  - "legacy-code"
  - "scrum-by-example"
  - "technical-debt-2"
  - "unit-testing"
  - "velocity"
coverImage: "photodune-9444702-yellow-working-sign-xs.jpg"
excerpt: 'We join the team this week in their Sprint Planning session as they start by rechecking'
---

![Yellow vector working sign - image licensed from Photodune](src/content/blog/scrummaster-tales-stop-digging-new-holes/images/photodune-9444702-yellow-working-sign-xs.jpg) The first law of holes is “When you’re in one, stop digging”. [In the last sprint](/blog/scrummaster-tales-technical-debt-is-slowing-the-team) the team discovered that they’re in a hole – in this case they had dug themselves into technical debt.

We join the team this week in their Sprint Planning session as they start by rechecking their Retrospective action items:

- Respect the “Definition of Done” – write Unit Tests (their complete “Definition of Done): Checked In, Peer Reviewed, Unit Tested, Manually Tested)
- Temporarily add Unit Test column to their story board
- Install [Sonar](https://www.sonarsource.org/) (a platform to help visualize Code Quality) to help improve awareness of Code Quality and Technical Debt
- Spend 20% of their time in the next couple of Sprints to tackle Technical Debt Issues _(Ed note: From experience this seems a bit low for teams that have accumulated a fair amount of technical debt, but the team will have to learn on their own)_

They start by discounting their historical velocity (currently at ~20 Story points) by 20% to account for paying down the Technical Debt (16 Story Points). Then they recheck the “Definition of Done” for each story they’re about to commit to. At this stage Product Owner Paula pipes up to protest that all this focus on technical debt doesn’t help her get features out the door. She’s concerned the CEO will be banging on her door soon. Doug explains that if the team doesn’t start to tackle the technical debt now, the delivery of new features will slow down even more, while the bug count rises. He explains that the next 3-4 sprints will be rough as the situation needs to be stabilized _(Ed: He’s optimistic)_ . ScrumMaster Steve reminds Paula that she is responsible for the product that the team delivers. In turn the team is responsible for deciding how much they can deliver and for ensuring its quality. Paula raises the flag of surrender but says she is really concerned and wants to revisit this two sprints from now.

Once the planning actually gets going, the team finds that they can’t even commit to 16 Story Points of work. They realize that it will be hard to write Unit Tests for some of the new stories. The team commit to installing Sonar and then look at the Technical Debt Backlog for key items. Based on what they’ve picked up from “[Laurent method](https://www.artima.com/forums//threaded.jsp?forum=155&thread=182754)” they’ve found a few large files that change frequently. They’ve discovered that several of these are 10,000+ line “[God](https://en.wikipedia.org/wiki/God_object)/[Monster](https://lostechies.com/chrismissal/2009/05/28/anti-patterns-and-worst-practices-monster-objects/) classes”, the class that everything else hangs off. When something small changes in these classes, it ripples through the entire code base.

After the Sprint Planning Meeting, Steve modifies the Story/Task Board to look like:

![Scrum Story / Task board](src/content/blog/scrummaster-tales-stop-digging-new-holes/images/Story-Task-board.png)

Adding the “Definition of Done” at the top (permanently) and a “Unit Test” column (only until Unit Testing becomes a habit).

On **Day 1**, Ian (the unofficial Build Master) and Doug sit down together to get [Sonar](https://www.sonarsource.org/) up and running. After spending a few hours getting it configured in their CI system they have a pretty page of Java projects to visit from their dashboard.![Screenshot from Sonar's own Nemo](src/content/blog/scrummaster-tales-stop-digging-new-holes/images/Sonar-screenshot.png)

After having some fun looking at the worst violations, they come to realize that the default configurations of PMD can be very noisy (with warnings for method name too long and too short). They quickly decide to load up PMD in Eclipse and make a first pass at simplifying rules. Even after simplification they find the code base still has over 10,000 rule violations. They agree to raise the issue in the next [Daily Scrum](/blog/pathologies-of-the-daily-scrum-or-standup). They also decide to write a short note to the team explain which rules they dropped and why. In addition they discovered that their existing Unit Tests only provide 10% Code Coverage.

**Day 2** During Daily Scrum – Ian describes what they’ve learned from installing Sonar and trying to configure PMD. After the meeting the developers have a five minute chat to agree on a strategy to handle the PMD issues. They agree just to eliminate PMD warnings as they work on a class. When there are too many warnings to eliminate in one sitting, they agree to at least chip away at some and create a technical debt card/postit to capture the bigger issue(s).

**Day 3** Splitting the God/Monster classes proves painstaking and slow, first the functionality has to be moved to a new class then that class has to be passed in to all the places it's required, …, finally test cases need to be written.

…_Ed we could keep going but it's clear that the process is slow and painstaking. Let’s take a step back and find some options for the team._

## Analysis

I happen to know that the team haven’t got a lot of experience with Unit Testing or Restructuring Legacy Code. Let’s give them some reading/study options. From experience I start with the simple Unit Testing before growing them to Test Driven Development (and beyond):

- [Unit Testing in Java](https://www.manning.com/books/effective-unit-testing) (Manning MEAP) – Lasse Koskela (early access as the book isn’t completely finished)
- [The Art Of Unit Testing](https://www.artofunittesting.com) (Manning) – Roy Osherove (.NET)
- [Pragmatic Unit Testing in C#](https://pragprog.com/titles/utc2/pragmatic-unit-testing-in-c-with-nunit-2nd-edition/) (Pragmatic Bookshelf) – Andy Hunt and Dave Thomas with Matt Hargett

Once they’ve mastered the basics they will need to start thinking about how to make the larger scale changes that will be necessary. Good reading choices here include:

- [Working Effectively with Legacy Code](https://www.amazon.com/Working-Effectively-Legacy-Michael-Feathers/dp/0131177052/&tag=notesfromatoo-20) - Michael Feathers – its from 2004, but the problems the book helps you solve remain the same
- [Mikado Method](https://www.agical.com/mikmeth/mikadomethod.pdf) (Draft PDF) and [Book Wordpress Site](https://mikadomethod.wordpress.com/book/) - Daniel Brolund and Ola Ellnestam – while still in draft the book looks close to being finished.

In the course of breaking dependencies in the legacy code, the team will likely find a [mocking framework](https://en.wikipedia.org/wiki/Mock_object) handy. In the world of Java things have evolved a lot in the past few years:

- [MockIto](https://code.google.com/p/mockito/) – uses a literate style (my personal preference) without also requiring states i.e. recording/playback so I would definitely take it out for a test drive
- [PowerMock](https://code.google.com/p/powermock/) – promises to handle some of the difficult things to mock (statics, final, etc.) in legacy code
- [JMock](https://jmock.org) hasn’t had a release in a couple of years but is probably still worth a look

## Story

By end of the Sprint the team have completed the Stories they originally committed and they have made some of the Monster classes a bit smaller, and the team realize the size of the problem. They’ve also started to do some of their reading and appreciate the tools that they have available to solve their problems. In addition, since they’ve got Sonar installed they can already see some of the improvements.

_With a spot of luck perhaps in the next few sprints they will make their codebase marginally cleaner and easier to work with._

_**[Scrum by Example](/blog/category/scrum-by-example) is a narrative-style blog series designed to help people new to Scrum, especially new ScrumMasters. If you are new to the series, we recommend you [check out the introduction](/blog/scrum-by-example) to learn more about the series and discover other helpful articles.**_

First image via: [https://photodune.net/](https://photodune.net/). Remaining images by Agile Pain Relief.
