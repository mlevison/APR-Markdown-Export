---
title: "Scrum By Example – Technical Debt is Slowing the Team"
date: "2012-02-18"
categories: 
  - "scrum"
  - "scrum-by-example"
tags: 
  - "bottleneck"
  - "cross-training"
  - "daily-scrum"
  - "scrum-by-example"
  - "story-points"
  - "technical-debt-2"
  - "unit-testing"
excerpt: '[Cross Skilling](/blog/scrummaster-tales-the-team-gets-bottlenecked) is starting to'
---

[Cross Skilling](/blog/scrummaster-tales-the-team-gets-bottlenecked) is starting to happen and already there are fewer bottlenecks. Steve is starting to have more time to step back from the day to day and look at the big picture. He’s heard that most Scrum teams become more productive over time and he wonders how is team is doing. He pulls up the CFD for the current release:![CFD-for-Technical-Debt-annotated-image by Agile Pain Relief Consulting](src/content/blog/scrummaster-tales-technical-debt-is-slowing-the-team/images/CFD-for-Technical-Debt-annotated-small.jpg) and immediately notices that the rate at which stories are being selected has slowed down in the past few sprints. Historically the team has a trailing average of 30 story points a sprint. In the past few sprints they’ve only achieved 25 and 22. Is this drop meaningful? Is it related to the team’s cross skilling efforts? Steve decides to ask the team what is going on. He writes a short note, describing the problem he’s seen (without his own suspicions) and asks the team to reflect on the discovery. After Daily Scrum Steve invites the team members to talk about the problems they see:

- Cross Skilling has slowed the team to a small extent
- Interruptions are down, so if anything the team should be more productive
- Unit Tests aren’t getting written for very often
- Ian and Doug report that they’ve spent a fair amount of time in the past few sprints implementing a new story only to find it broke an existing story.
- Its also noted that there are several places in the code that have become rather hairy and are difficult to change safely.

## Analysis

The team have just discovered Technical Debt (see my article “[Technical Debt a Managers Perspective](https://www.infoq.com/articles/technical-debt-levison/)”) or a [mess](https://sites.google.com/site/unclebobconsultingllc/a-mess-is-not-a-technical-debt) (where Uncle Bob would argue that I misuse technical debt). Either way it would appear that the code is slowing the team down. At the start of the project they appeared too fast but now they’re slowing down. In reality they weren’t really going fast, instead they weren’t ensuring that they were really done.

## Back to the Story

Doug remembers reading about the problems of technical debt (aka a mess) recently and suggests that this is probably what they’re starting to see. The team agrees to run a 2 day spike to investigate this issue and they warn Product Owner Paula that this will affect what they’re able to deliver.

Coding Java the team have a rich supply of tools available to them:

- [PMD](https://pmd.sourceforge.net/) – “scans Java source code and looks for potential problems" examples: Dead code, Duplicate Code, missed private and final markers, over complicated code etc.
- [Sonar](https://www.sonarsource.org/) – “Sonar is an open platform to manage code quality” – it uses static analysis tools (including PMD), code coverage tools et al to measure the state of the code. It plugs into the CI server and keeps data on an ongoing basis.
- [Sort](https://www.artima.com/forums//threaded.jsp?forum=155&thread=182754) – Laurent Bossavit taught us this year’s ago: “getting a file list of all source code files, then sorting that list by (decreasing) file size. I start with the largest source file, and see if there's a reason it's the largest”

Doug and Ian decide to use PMD and Sorting by filesize as a starting point, as Sonar takes a bit longer to configure. Each time they find a major issue they take write it down on a large postit note along with some reference information (i.e. the files involved anything else. _Ed note the precise format doesn’t matter – what matters is that the developers understand the issue its describing and will be able to guess which stories they might affect in the future)._ By the end of the first day they’ve come up with over 50 postit that contain noteworthy items (vs. a missing private or final which can be fixed in a few seconds). On the 2nd day they sit down with the rest of the team to prioritize the items using slows us down the most as criteria. During the remainder of the Sprint team members tackle smaller technical debt items (< 2hrs) when the items are related to the story they’re working on.

During the retrospective the Technical Debt problem comes up and the team start to discuss where it comes from. Steve starts by asking the team to review the existing “Definition of Done”:

- Checked In
- Peer Reviewed
- Unit Tested
- Manually Tested

A few minutes of conversation led the team to realize that the while most code was peer reviewed, very little was Unit Tested. Perhaps the bigger issue was that they didn’t have a good idea roughly how much of the code was unit tested or if the existing Unit Tests where of good quality.

Their SMART Actions (see: [Agile Retrospectives](/blog/agile-retrospectives)):

- Respect the Definition of Done – write Unit Tests
- Temporarily add Unit Test column to their task wall
- Install Sonar to help improve awareness of Technical Debt
- Spend 20% of their time in the next couple of Sprints to tackle Technical Debt Issues

Steve promises to post this above the task wall to ensure that the team sees them.

Next week we will see how the team fare _(Ed – I’m stretching this out over several stories because Technical Debt takes time to be weeded out)._

_**[Scrum by Example](/blog/category/scrum-by-example) is a narrative-style blog series designed to help people new to Scrum, especially new ScrumMasters. If you are new to the series, we recommend you [check out the introduction](/blog/scrum-by-example) to learn more about the series and discover other helpful articles.**_

Image attribution: Agile Pain Relief
