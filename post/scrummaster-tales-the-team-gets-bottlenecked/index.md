---
title: "Scrum By Example – The Team Gets Bottlenecked"
date: "2012-02-07"
categories: 
  - "scrum-by-example"
tags: 
  - "bottleneck"
  - "project-management"
  - "scrum-by-example"
  - "work-in-progress"
coverImage: "photodune-510956-bottle-xs.jpg"
---

![Old fashioned glass bottle with cork stopper. - image licensed from Photodune](src/content/blog/scrummaster-tales-the-team-gets-bottlenecked/images/photodune-510956-bottle-xs.jpg)It's day four of the sprint and ScrumMaster Steve is studying the Story + Task wall to see how the sprint is progressing. After a few minutes he sees three things that standout:

1. Martin, the only team member who knows how to make changes to the database, has his name on four tasks that are in progress. Two of those tasks are blocking the remaining work on their respective stories.
2. Ian, the business logic developer, has his name on three tasks, two of which are blocked by Martin. The other task is blocking continued work on another story.
3. There are **six** stories in progress even though the team has previously agreed on a WIP (Work In Progress) [limit of 3 stories](/blog/scrum-by-example-the-story-of-an-incomplete-sprint.html) in progress at one time.

## Analysis

The team is currently blocked on Martin’s database related tasks. However even if that bottleneck were resolved they would still be blocked on Ian’s tasks.

The team isn’t respecting its own WIP limits.

## Risks

- With this many stories in progress, many of them will remain incomplete by the end of the sprint.
- Many of the stories require multiple handoffs, example: Brad (BA) –> Ian (Middle Tier) –> Martin (Database Specialist) –> Ian –> … –> Tammy (Tester). Each handoff increases the risks of miscommunication, bugs and other mistakes all due to incomplete knowledge transfer.
- The teams lottery number sits at one. I.E. if any of Martin, Ian or Tammy win the lottery and decide to leave the organization the team will struggle because no one else really knows how to play their role.

## Story

Steve raises this as an impediment at the Daily Scrum and asks for quick meeting right afterwards. He shares the three observations and asks the team what they think. Team members say things like: “Database work isn’t my speciality/skill” and “I wouldn’t be as productive on that”. As a result they say that they moved onto lower priority work. To get through the sprint without another disastrous ending (see: [The Story of an Incomplete Sprint](/blog/scrum-by-example-the-story-of-an-incomplete-sprint.html)), Steve asks what they can do to offload Martin and Ian allowing them to unblock higher priority work. Among other ideas the team decide:

- to temporarily abandon work on the lower priority stories
- to pair with Martin and Ian to get the higher priority stories sooner

During the retrospective the team focused on the problems with only one team member being able to do certain key tasks (Database work, Business Logic). Rather than address it piecemeal Martin suggests that they create a Skills Matrix.

That shows the inventory of skills across the team. (_Ed note – when I facilitate one of these we spend 15-20 minutes coming up with a list of potential useful skills for the team)._ After an hour of work the team assembled a matrix that helped spot many areas where they only had one person who could do the work. It turns out the gaps are larger than can be addressed in the next couple of sprints, so the team decides to focus. They choose:

- Grow Database Skills so at least three team members can make database changes without requiring Martin to oversee all aspects of the work.
- Grow understanding of the Business Logic so that coding team member can work safely in that layer without requiring Ian’s help.
- Teach all team members the rudiments of Exploratory Testing so that stories are tested sooner and developers get earlier feedback on their work. Tammy will receive an additional benefit because most Stories will really be done by the time they reach her. (_Ed Note – they still haven’t discovered ATDD, BDD or even TDD yet)._

To grow skills in those areas they agree to us a mixture of pair programming, interactive workshops and one on one coaching. While these activities will slow the team down in the next few sprints, the benefits of getting higher priority work done faster will soon out weigh.

Finally the team posts the skills matrix in the team area and commits to revisit it in six to eight weeks.

_**[Scrum by Example](/blog/category/scrum-by-example) is a narrative-style blog series designed to help people new to Scrum, especially new ScrumMasters. If you are new to the series, we recommend you [check out the introduction](/blog/scrum-by-example.html) to learn more about the series and discover other helpful articles.**_

_**Update:** As I went to compile a cast of characters I realized that I was using Doug and Martin interchangeably between posts. I changed this post to make Martin our database guy._

Images via: [https://photodune.net/](https://photodune.net/)
