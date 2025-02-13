---
title: "Lifecycle of a User Story"
date: "2013-11-04"
categories: 
  - "scrum-by-example"
  - "user-stories"
tags: 
  - "priorities"
  - "product-backlog-refinement"
  - "release-planning"
  - "sprint-planning"
  - "story-estimates"
  - "user-stories"
excerpt: 'To illustrate this I will use vignettes from the WorldsSmallestOnlineBookStore. Each'
---

![Lifecycle image via Wikimedia Commons](src/content/blog/lifecycle-of-a-user-story/images/LifeCycle.png) [User Stories](/blog/definition-of-done-user-stories-acceptance-criteria.html) are often used as a lightweight form of Agile requirement. Their goal is  to replace heavy weight-specification documents with “a Card, a Conversation and a Confirmation”. When people first discover User Stories it's hard to see how they work because we often take a static viewpoint – i.e. we only see them at Release Planning or during implementation. We’re left with many questions: Where do User Stories come from? When are they created? Who is involved in their creation?

To illustrate this I will use vignettes from the WorldsSmallestOnlineBookStore. Each vignette will show what happened to one User Story.

_“As a frequent book buyer I want to save my address so that I don’t have to retype it every time I visit the bookstore”_ During the team’s first Release Planning Session (aka Initial Product Backlog Refinement) this Story was identified. After a few rounds of planning poker the consensus estimate was that it was size 20, allowing for both the initial entry of the address, updating and deleting old addresses. Since this Story appeared to be low priority in the short term, the team moved to other items.

\---------

In Sprint #5, during a Backlog Refinement session, the PO Paula revisited the Story and asked the team if their understanding of the problem had changed in the past two months. They conferred for a few minutes and decided that it was still a 20. Sue grumbled and suggested it was a fairly small piece of functionality for such a large number. Doug suggested a Story split – using CRUD (Create Read Update Delete), he proposed in the short term that the User be allowed to add a new address and use it. However, they wouldn’t be able to update and delete. This would separate the Stories. After a few minutes of conversation around the implications Sue asks them to estimate the three split Stories:

_“As a frequent book buyer I want to save my address so that I don’t have to retype it every time I visit the bookstore.”_

_“As a frequent book buyer I want to delete old addresses so that I don’t have to worry that my books will ship to the wrong house.”_

_“As a frequent book buyer I want to update my existing address to correct small errors so that I don’t have to retype them from scratch.”_

The team determines the “save address” Story is size 8, the “delete address” Story size 5, and the “update address” Story size 8. Based on this Sue moves the “save address” Story to the top of the Product Backlog, “delete address” about 15 items further down and “update address” has been moved so far down it will never be tackled.

Since the slimmer “save address” is now the top Story in the Product Backlog without acceptance criteria, the team spends a few minutes creating criteria for it. They start off by drawing a quick pencil sketch to get the key points across. Based on this sketch they start creating a table of examples:

<table class="postTable" border="1" cellspacing="0" cellpadding="0"><tbody><tr><td valign="top" width="221">1 Sussex Drive, Ottawa, Ontario, Canada, K2K 010</td><td valign="top" width="221">Valid</td></tr><tr><td valign="top" width="221"><span style="color: #ff0000;">Buckingham Palace, London, UK</span></td><td valign="top" width="221"><span style="color: #ff0000;">Address outside of Canada/US</span></td></tr><tr><td valign="top" width="221"><span style="color: #000000;">1600 Pennsylvania Avenue NW</span>Washington, DC 20500</td><td valign="top" width="221">Valid</td></tr></tbody></table>

Rather than try to create an exhaustive list at this point they just create enough to outline the boundaries of the problem.

During the team’s next Sprint Planning session, Sue asks if the team can commit to this Story. They give it the “thumbs up”.

Before the team starts work on the Story, Tonia (QA specialist), Brad (BA), Doug (Developer) and Ian (Developer) meet to finish hammering out the acceptance criteria.

<table class="postTable" border="1" cellspacing="0" cellpadding="0"><tbody><tr><td valign="top" width="221">915 E 7th St. Apt 6LBrooklyn NY 11230</td><td valign="top" width="221">Valid</td></tr><tr><td valign="top" width="221">24 Willie Mays Plaza, San Francisco, CA 94107</td><td valign="top" width="221">Valid</td></tr><tr><td valign="top" width="221"><span style="color: #ff0000;">24 Willie Mays Plaza, San Francisco, CA</span></td><td valign="top" width="221"><span style="color: #ff0000;">No Postal Code</span></td></tr><tr><td valign="top" width="221"><span style="color: #ff0000;">24 Willie Mays Plaza, San Francisco, 94107</span></td><td valign="top" width="221"><span style="color: #ff0000;">No State</span></td></tr><tr><td valign="top" width="221">45 Rosenfeld CrOttawa, ONK2K 2L2</td><td valign="top" width="221">Valid</td></tr><tr><td valign="top" width="221">45 Rosenfeld Cr, Ottawa, ONK2K 2L2</td><td valign="top" width="221">Valid</td></tr><tr><td valign="top" width="221"><span style="color: #ff0000;">45 Rosenfeld Cr</span><span style="color: #ff0000;">Ottawa, ON</span><span style="color: #ff0000;">K2K 222</span></td><td valign="top" width="221"><span style="color: #ff0000;">Invalid Postal Code</span></td></tr><tr><td valign="top" width="221"><span style="color: #ff0000;">45 Rosenfeld Cr, Ottawa, ON</span><span style="color: #ff0000;">&nbsp;</span></td><td valign="top" width="221"><span style="color: #ff0000;">Missing Postal Code</span></td></tr><tr><td valign="top" width="221">….</td><td valign="top" width="221"></td></tr></tbody></table>

(This style is referred to as [Specification By Example](https://en.wikipedia.org/wiki/Specification_by_example) – where the emphasis is that it provides the specification before something is built).

Brad goes off to see if there are any edge cases that the examples don’t cover. Ian and Tonia pair off to turn the examples into Executable Specifications (i.e. acceptance tests) in [Fitnesse](https://fitnesse.org/).\[[1](#footnotes)\] Doug starts to take a crack at the GUI, seeing what parts he will need to assemble. Once the initial tests are written Ian tries build the business logic to support the examples.

A few days later when Ian and Doug think they’ve completed the Story and it meets the examples, they show it to Tonia. Once she sees that satisfies the test cases she spends a while doing some exploratory testing – seeing how the application behaves when a real User plays with it. Satisfied, she calls Paula over for additional feedback. Paula is delighted with the behavior but asks for a few changes to the layout. Once those are made she agrees the Story will be complete.

During the Sprint Ian demonstrates the different ways we can now support accepting addresses from both Canada and the United States.

At the end of the Sprint the team takes the completed Story off the wall and archive it in the filing cabinet (they keep them around for later auditing).

\---------

During Sprint #6, Brad (BA) sees Ian (Developer) in the hallway and they start chatting about the warehouse runners, i.e. the people who fill the book orders. Brad comments he’s seen the runners spend a lot of time retracing their steps because the list of books in for an order is alphabetical - but unfortunately the warehouse isn’t laid out in alphabetical order. They create a new Story:

_“As a runner I want the list of books to be printed in the same order I will find them in the warehouse so I don't have to run as far”_

During the Backlog Refinement session a few days later they bring up the Story. Paula gives it some thought and says, “We’re in the fourth month of operations, and we’re only just starting to see reasonable sales numbers roll in. All improvements right now must be focused on the book buyers and making it easier for them to buy books. At this stage I can’t afford to do any work for the warehouse runners or any other back office staff. Once sales start to increase we can afford to improve the system for our internal Users”. Paula took the index card that the Story was written on and ripped it up.

\------

User Stories aren’t static, one-sentence descriptions written by one person. The User Story is most effective as a tool when several people are involved in its creation. They work as a tool to record the team’s share, understanding not as a one-way missive from the Product Owner. In addition a good User Story evolves over time – as the team gains a greater understanding of the business problem they rewrite it, split it and add acceptance criteria.

\[1\] Fitnesse isn’t the only tool [Cucumber](https://cukes.info/), [RobotFramework](https://robotframework.org/), [SpecFlow](https://specflow.org) and others would have worked well too.

Lifecycle image via Wikimedia Commons
