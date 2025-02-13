---
title: "Scrum By Example - The Story of Production Support"
date: "2011-10-04"
categories: 
  - "scrum"
  - "scrum-by-example"
tags: 
  - "multitasking-cost"
  - "production-support"
  - "scrum"
  - "scrum-by-example"
coverImage: "photodune-1105342-tripod-xs.jpg"
excerpt: 'When we left Steve and the team they were just getting the shipping features ready and'
---

![Tripod - image licensed from Photodune](src/content/blog/scrummaster-tales-the-story-of-production-support/images/photodune-1105342-tripod-xs.jpg)_This article has been updated. You can find the newest version of this content [here](/blog/scrum-production-support.html)._

When we left Steve and the team they were just getting the shipping features ready and were waiting to go ‘live’ with the site. This turns out to be a blessing and a curse. It's a blessing because the business is making money; a curse because with it come support issues.

Steve spends some of his time and energy just watching the team and their flow every day. In the first two Sprints after the release the team struggles and fails to meet its planning commitments. At first he’s OK and just says its the inevitable post-release hiccups (_I don’t agree with Steve on this one, it’s not inevitable; I think it was a first warning sign – Editor_), but when it’s clear that this is continuing into the 3rd Sprint he starts to get worried. Steve notices that team members are often being interrupted several times a day. Most of the interruptions are support issues.

During the Retrospective Steve chooses a [timeline](https://www.energizedwork.com/weblog/2006/10/timeline-retrospective) to help the team remember/discover what happened in the past two weeks. It’s worse than even Steve realized; team members spent most of their time on Production Support. After some more discussion they discovered there were three major classes of issue:

- Issues where a team member just had to help support understand how to help the customer
- Issues that required a small code change and could be made by most team members
- Issues that required the specialized skills of one or two team members

## Analysis

The team can do a number of things:

- Choose one team member per Sprint who will become the first point of contact for support. Some issues they can deal with themselves and others they will have to find help with. _NB This job should rotate so it’s not always the same person._
- If there are multiple teams, in any one Sprint one team takes the support hit. _This is the same strategy as the first at scale._
- Wait until the day’s end before interrupting another team member for help on a support issue
- Monitor the production support issues and track their effects on the team’s productivity. Example: usually in the days that follow handling a support issue the team is able to complete fewer Stories. Remember, its not just the cost of fixing the issue that needs to be tracked, but additional costs, such as deployment and [multitasking cost](https://www.infoq.com/articles/multitasking-problems).
- Based on historical needs acknowledge in planning that there is a tax of 20-30% to be paid for support. _This is my least favorite solution because it doesn’t help make the situation better; it just increases awareness of it._

No matter what, every time a support issue comes up, do a [root cause analysis](https://www.energizedwork.com/weblog/2006/01/root-cause-analysis-using-5-whys) or use [A3 Problem solving](https://www.crisp.se/lean/a3-template) to identify the real issue and reduce the number of times it hits the team in the future. In addition, we have to help the organization see the costs of what is happening, the support calls might be what the organization needs at the moment but needs feedback as to the impact.

_Update: One of my readers (Sergey Kotlov) pointed out that in some cases the frequent production support issues are of a database/admin support type and suggests that the team has missed an opportunity to provide support with tools to help. He’s absolutely right; in that case the PO might want to prioritize work to create support tools so the development team can stay focused. Thanks to Sergey for his suggestion._

Image via: [https://photodune.net/](https://photodune.net/)
