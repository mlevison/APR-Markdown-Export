---
title: "Scrum By Example - Waiting Too Long to Create Acceptance Criteria"
date: "2013-01-13"
categories: 
  - "product-acceptance-criteria"
  - "scrum-by-example"
  - "user-stories"
tags: 
  - "acceptance-criteria"
  - "backlog-refinement"
  - "product-backlog-refinement"
  - "scrum-by-example"
  - "sprint-planning"
  - "story-splitting"
  - "user-stories"
coverImage: "photodune-8431094-done-text-and-check-mark-xs.jpg"
excerpt: 'The team was able to get from a very large Story: “As a first time book buyer I want to'
---

![Done image licensed from Photodune](src/content/blog/creating-acceptance-criteria-waiting-too-long/images/photodune-8431094-done-text-and-check-mark-xs.jpg) The recent [Backlog Refinement](/blog/scrummaster-tales-story-splitting-fun) session helped split the upcoming User Stories.

The team was able to get from a very large Story: “As a first time book buyer I want to read a trustworthy review before I buy a book” to:

- As a first time book buyer I would like to read a review so I can see if a book is worth reading.
- As a first time book buyer I would like to see a star rating associated with a review so I can quickly assess if the book is even worth thinking about.
- As a first time book buyer I would like to see reviews by staff members marked separately so that I know whom to trust.
- As a first time book buyer I would like to see reviews by friends highlighted so that I know whom to trust.
- As a staff member I would like to write a book review so that I can help customers choose great books.
- As a staff member I would like to rate a book I’ve reviewed so I can give customers a quick guide.

We’re in better shape than we have been with previous Sprint Planning meetings but the team lacks concrete acceptance criteria.

## Analysis

During the first half of a Planning meeting the team is trying to determine its goal for the Sprint. Specifically, it’s trying to answer the question, “What stories can we commit to?”  To have a realistic commitment the team needs small Stories and a clear understanding of what they will look like when they’re done.

## Story

Brad reads the first Story aloud, “As a first time book buyer I would like to read a review so I can see if a book is worth reading.” He sees an entire new web page, separate styling and a whole lot of infrastructure to support it. Doug, on the other hand, sees a small addition to each book page. He says that no new style sheets need to be developed. After a few more minutes of debate Product Owner Paula intervenes by saying that reviews will just live on the main page for now. In addition, each review must be under a thousand words and in plain text only.

Debate continues around each successive Story until two hours have passed; and the team is still unsure what they can commit to. ScrumMaster Steve has been doing his best to bring team members back to focus, but it’s been a struggle.

## Analysis

The team is struggling because they don’t have clear acceptance criteria. As a result, they don’t agree on the size and can’t agree on what to commit to. They’re spending the Planning meeting focusing on the question of, “What are we trying to do?” as opposed to, “What should we be doing?”

**Acceptance Criteria**:

The goals of Acceptance Criteria are:

- To clarify what the team should build (in code and automated tests) before they start work.
- To ensure everyone has a common understanding of the problem.
- To help the team members know when the Story is complete.
- To help verify the Story via automated tests.

Creating good acceptance criteria is a collaborative effort. Usually, they’re created by the Product Owner working with several other team members. When created in isolation they fail to meet the first two values.

In addition when we create them a few days before the Sprint Planning meeting, team members have time to consider just what they mean, how they fit the product and what is missing.

Let’s wind the clock back for the team to three days before our Sprint Planning meeting.

## Story

Paula asks Ian, Brad and Tonia to come spend half an hour with her. Their goal is to hammer out the acceptance criteria for each Story that might be committed for the next Sprint.

At the end of their white-boarding session they’ve got very rough sketches for the first three Stories that clearly limit their scope. In addition there are also textual criteria:

- As a first time book buyer I would like to see a star rating associated with a review so I can quickly assess if the book is even worth thinking about.
    - Rating from 0 to 5
    - No ½ stars
    - It appears at the top of the review

- As a first time book buyer I would like to see reviews by staff members marked separately so that I know whom to trust.
    - The word “Staff” appears in bold before the reviewer’s name.
    - All reviews posted from computers inside the Smallestonlinebookstore offices will be considered as staff reviews. _(This avoids having to tag users as having different roles for now)._

A few days later during the Sprint Planning meeting, the team spends far less time debating and manages to get to commit to their Stories within the first hour vs. their traditional two or more hours.

When do you write your Acceptance Criteria?

_**[Scrum by Example](/blog/category/scrum-by-example) is a narrative-style blog series designed to help people new to Scrum, especially new ScrumMasters. If you are new to the series, we recommend you [check out the introduction](/blog/scrum-by-example) to learn more about the series and discover other helpful articles.**_

Images via: [https://photodune.net/](external:https://photodune.net/)
