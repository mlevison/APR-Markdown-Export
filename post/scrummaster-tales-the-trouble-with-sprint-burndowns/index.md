---
title: "Scrum by Example - The Trouble with Sprint Burndowns"
date: "2014-06-19"
categories: 
  - "scrum-by-example"
tags: 
  - "daily-scrum"
  - "scrummaster"
  - "sprint-burndown"
  - "sprint-planning"
  - "story-estimates"
  - "user-stories"
excerpt: '_Julia and Rob – are personas used by the BookStore Team to keep them focused on the needs'
---

![SprintBurndownEstimateHrsRemaining](src/content/blog/scrummaster-tales-the-trouble-with-sprint-burndowns/images/SprintBurndownEstimateHrsRemaining.png)It’s six Sprints after the “[Overtime/Disastrous Release](/blog/scrummaster-tales-overtime-on-a-scrum-team-is-an-unhealthy-sign)”, which set the team back by several months. During the current Sprint Planning, the Team committed to completing the following nine User Stories:

_Julia and Rob – are personas used by the BookStore Team to keep them focused on the needs of real users. Julia is a Frequent Book Buyer and Rob is Rookie or First Time Book Buyer._

- As Julia I want to be able buy a $10 gift card so that I can thank a fantastic client. _Limitation - not delivered just generated -_ Size: 5
- As Julia I want my newly purchased gift card sent by email to its recipient so they can use it quickly. - Size 3
- As Julia I want to be able to refill a gift card I previously purchased. - Size 2
- As Julia I want to be able to buy a gift card in denominations of $25, $50 and $100 so I can have choices in how much money I want to spend. - Size 2
- As Julia I want fancy graphics and text on my gift card to satisfy my inner diva. - Size 3
- As Rob I want to be able to use my new received Gift Card so that I enjoy another book without the pain of paying for it. - Size 3
- As Rob I want to be notified by email when I receive a Gift Card so I can use it quickly. - Size 2
- As Rob I want to see the remaining balance on my Gift Card so I know how much I have left to spend. - Size 1
- As Julia I want to be notified when the Gift Card I sent runs out of money so I can replenish it. - Size 3

The stories have estimates (sized 1, 2, 3, with one 5), are reasonably well split and initial acceptance criteria (_not illustrated here to save space_). Their total of 24 story points seems quite achievable based on the past few sprints velocity. In addition, they break the Stories down into tasks with a total of 323 estimated task hours.

Day by day during Daily Standup, they update the number of Estimated Task Hours of work they currently believe are remaining in the Sprint. This table shows their progress:

<table class="postTable"><tbody><tr><td>Day</td><td>Stories in Progress</td><td>Stories Completed</td><td>Task Hrs Estimated Remaining</td></tr><tr><td>1</td><td>4</td><td>0</td><td>300</td></tr><tr><td>2</td><td>4</td><td>0</td><td>265</td></tr><tr><td>3</td><td>5</td><td>1</td><td>235</td></tr><tr><td>4</td><td>5</td><td>1</td><td>178</td></tr><tr><td>5</td><td>5</td><td>1</td><td>153</td></tr><tr><td>6</td><td>5</td><td>2</td><td>116</td></tr><tr><td>7</td><td>5</td><td>2</td><td>101</td></tr><tr><td>8</td><td>5</td><td>4</td><td>60</td></tr></tbody></table>

Every day during the Sprint, Steve (the ScrumMaster) asks the team, “Are you still on track to hit our goal of nine stories?” At Day Eight, the team has approximately sixty hours of work left, four completed stories and five in progress. Steve asks his Daily Question, “Are we really going to make it?” All of a sudden, the answer is **No**. Steve asks, “Which Stories can we realistically complete?” The team pick two and immediately go and find Sue to tell her which three stories they’re dropping.

As they leave the Daily Scrum, Brad quips, “That’s really not so bad, is it?”

## Analysis

Is it really that bad? Yes.

- If the team can’t regularly hit their commitment, the Product Owner and the Business as a whole will rapidly lose faith in them.
- When the team’s commitment in Sprint Planning doesn’t mean anything to them, then they won’t be focused or motivated to achieve their target.
- When the team miss the commitment on more than a few occasions, predictability goes right out the window.

How did this happen? Sprint Burndowns tracked estimated hours of work remaining to get people to focus on an ideal line (properly called a ‘rhumb’ line). They tend to focus on the rhumb line because that’s what they think management want. They also pay attention to it even when it isn’t drawn, because we assume the natural path to done follows that line. In reality, real Sprint work rarely fits that line.

In addition, tracking task hours tends to get people to focus on the delivery of tasks hours, instead of delivering value. Consider two Teams on Day Eight of a two week Sprint. Assume that they worked on the same Stories for the same Sprint. Team ‘B’ paid careful attention to Sprint Burndown and Team ‘A’ focused on delivering value.

<table><tbody><tr><td><strong>Team</strong></td><td><strong>A</strong></td><td><strong>B</strong></td></tr><tr><td>Estimated Hours Work Remaining</td><td>100</td><td>60</td></tr><tr><td>Completed Stories</td><td>6</td><td>4</td></tr><tr><td>In Progress</td><td>2</td><td>5</td></tr><tr><td>Not Started</td><td>1</td><td>0</td></tr></tbody></table>

Clearly Team ‘A’ is better off even though they have more task hours remaining, since they’ve focused on getting their Stories to complete. With Team ‘B’, even though their Burndown will look closer to the ideal line, we’ve no idea what will really get done - very likely not all of them, since the team will bottleneck on Testing. If Team ‘A’ focus on delivering, they will definitely get at least one of the In Progress Stories to done, and perhaps two. They definitely won’t get the last one done, but the Product Owner won’t be surprised.

**Tricks that help**

- Measure your Sprint Burndown in Number of Stories or Story Points. Only burndown when a Story is completed.
- Limit WIP (Work In Progress) - this forces the team to finish Stories, collaborate, and share knowledge. Rally showed in a [recent study](/blog/stable-teams-really-do-matter) that reduced WIP correlates with getting more Stories to Done and fewer Defects.
- Choose a clear and effective [Sprint Goal](https://www.romanpichler.com/blog/sprint-goal-template/) - in this case a good Sprint Goal might have been: “By the end of the Sprint the Basic Gift Card should be available”. The Sprint Goal allows team members to ensure that their work is driving towards a greater goal. It helps maintain focus more effectively than a random grab bag of Stories. And if something needs to be dropped, it gives greater clarity around that choice.

Some of the most effective Teams I’ve seen dispense with Sprint Burndowns altogether and just focus on the flow of work across the Scrum Wall. They focus on getting the Stories themselves to completion and the tasks are just aids. For those who prefer to use a Sprint Burndown consider - Sample Improved Sprint Burndown:

![Sprint Burndown Number of Stories Remaining](src/content/blog/scrummaster-tales-the-trouble-with-sprint-burndowns/images/SprintBurndownNumberStoriesRemaining.png)

Just counting the number of Stories puts the emphasis on getting Stories to done. Even Story Size in Points can be distortive because it makes large items seem valuable making a cliff like burndown more likely. Just counting Stories puts the emphasis on the delivery of value.

If the team had this, they would have seen sooner that they weren’t going to get everything complete. They could have adjusted their approach to get some Stories done sooner.

Have you been burned by Sprint Burndowns?

_**[Scrum by Example](/blog/category/scrum-by-example) is a narrative-style blog series designed to help people new to Scrum, especially new ScrumMasters. If you are new to the series, we recommend you [check out the introduction](/blog/scrum-by-example) to learn more about the series and discover other helpful articles.**_

Images by Agile Pain Relief Consulting.
