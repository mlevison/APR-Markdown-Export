---
title: "Scrum by Example – Don’t Let Sprint Review be a Missed Opportunity"
date: "2021-10-12"
categories: 
  - "scrum-by-example"
  - "sprint"
tags: 
  - "sprint"
  - "sprint-goal"
coverImage: "APR-Story-of-a-Sprint-board-12.png"
excerpt: 'When last we left our World’s Smallest Online Bookstore team, their Sprint was rocky. To'
---

When last we left our World’s Smallest Online Bookstore team, their Sprint was rocky. To have an effective Sprint Review story, let’s assume that they magically wound back the clock (shazam!) and implemented the changes. As a result, they had the more effective Sprint Planning that we discussed [in the last blog post](/blog/how-sprint-planning-mistakes-can-derail-a-team.html).

So let’s quickly recap that last episode. The team set “Have basic reader review system in place so book buyers can see a variety of opinions about a book” as their Sprint Goal. (They had a weak Goal initially but, after they magically went back in time and did things different, that was the improved result.)

They then selected the following Product Backlog Items:

- Reader can add star ratings to a book
- Reader can write a review of a book (plain text only)
- Reader can add pictures to their reviews
- When a review is written by someone who purchased the book through our store, the system highlights their review as a “verified buyer”
- Registered site users can click a button to vote that a review is helpful
- Reader can format the text of their review
- Reviews feature the date they were written and the location of the author
- They also planned to fix two bugs that affect how books are displayed to buyers.

The Sprint went surprisingly well. They finished the top five of seven items and fixed one bug. (B_y the standards of many teams this is remarkably good._) They are now ready to hold a Sprint Review.

Steve, being a well-organized ScrumMaster, has an agenda in place:

- Remind the audience that the Sprint Review has a focus on the Product
- Restate the Sprint Goal and review if it has been met
- For each feature:
    - Team members demonstrate the features they worked on
    - Team checks features against the Definition of ‘Done’
    - PO accepts or rejects an item\[[1](#footnotes)\]
- PO, Stakeholders, and Team members discuss the Product Backlog and the Product Map (often a Story Map or Impact Map)

Steve has invited all stakeholders to attend, which include the Team’s Director, and the Directors of Support and Marketing.

![Illustration of Scrum team meeting with shareholders, with the Product Owner moderating discussion.](src/content/blog/dont-let-sprint-review-be-a-missed-opportunity/images/APR-Story-of-a-Sprint-board-12-1024x576.png)

At the start of the Review, Steve reminds everyone of their Sprint Goal: “Have basic reader review system ….”.

Paula reports, “The team achieved the core of that goal, with a reader review system ready on staging server. All I have to do is press a button and the new version is live on the site.”

She then hands over the stage to team member Ian to start walking through the features that the team have built.

Director of Support Eric’s phone starts buzzing and he disappears into it, apologizing to the room. “Sorry, we have a problem with some users not being able to see their account order history.”

The first few features that Ian demonstrates garner almost no feedback except people saying vague things like “Good job” and “I like that”. There are no substantive questions or suggestions offered.

When Ian demonstrates the Product Backlog Item “Reviews from a verified buyer are highlighted and displayed above other reviews”, Paula asks a few questions about the behaviour of the feature. She also checks the Definition of Done and learns from the team it is Done except for testing the text-only book review in Safari on MacOS and iPad.

![Placeholder example of an online review with a 1-5 star rating](src/content/blog/dont-let-sprint-review-be-a-missed-opportunity/images/SbE-WSOBS-buyer-reviews-unverified-buyer.png)

Jan, the Director of Marketing, asks, “How are we handling fraudulent reviews? Our reviews have always been from staff. That has been a differentiator. If we take this feature live, we lose our ability to differentiate on that.”

Paula replies, “But we’ve verified that the buyer bought the book, so their review is legitimate.”

“There is a black market for reviews, and the book seller might pay the reviewer $10 for a good review and reimburse them the cost of the book,” explains Jan. “Although we verified that they bought the book, we haven’t verified that they read the book or that this is their honest opinion.”

After a lot more discussion it’s agreed that it’s okay to leave the verified buyer tag on the reviews since most are legitimate. However, they won’t be featured or placed higher on the page. They will just appear in the normal sort order.

Ian is almost afraid to bring up the next feature, “Registered site users can click a button to vote that a review is helpful”. He wonders what unexpected problem will be found next.

As he shows the feature, Jan interrupts. “We can’t have that at all. It’s another source of fraud. Sellers will often pay for many users to click the helpful review button on any review that has 4+ star rating. Their goal is to bury critical reviews.”

![A placeholder example of an online review from a verified buyer of a product](src/content/blog/dont-let-sprint-review-be-a-missed-opportunity/images/SbE-WSOBS-buyer-reviews-helpful-vote.png)

At this point Paula can’t contain her frustration. “Why didn’t you tell us this before? Why wait until we wasted the team’s effort on implementing these features?”

Jan snaps back, “I tried to warn you about fraud weeks ago, but you didn’t listen.”

Realizing that the event has spiralled out beyond his ability to facilitate, ScrumMaster Steve asks for a ten-minute break. When everyone returns to the room, he suggests that they wind down the Sprint Review early, since they now have the list of features that were accepted and the ones that need more work.

As they leave, Ian mutters under his breath, “That was a ton of fun. Next time I’m asked to do the demo, the answer is NO!”

### Analysis

What happened? Steve was exceptionally well-prepared. He had a thoughtful agenda and yet most features got no feedback. Of the people present, some (like Eric) were engaged only with their phone and they never participated in discussing upcoming product priorities.

Done well, a Sprint Review is a point of pride for the team. This one was a downer for their morale, even though some of the work that was completed made the product better.

#### Challenges:

- The Sprint Review was a Show and _Tell_. The goal is to increase engagement with stakeholders and end-users, not _decrease_ it. If you ask the team members who worked on each feature to demo it, it’s likely to result in an unnecessarily long, tedious monologue, or demonstration of every nook and cranny of the feature, putting attendees to sleep. Having Paula demo alone would be just as bad. She might script a better story and make it seem more fun, but “Telling” — aka talking at other people — decreases engagement.
- The Definition of Done wasn’t checked _before_ the Sprint Review. This is critical. It is the way the team and the Product Owner know that they’re on the same page with respect to quality. However, much of the “Done” is just going to put the audience to sleep, so going through the process during the Sprint Review isn’t practical.
- The Director of Support was more engaged with his phone than in participating in the Review. We missed the opportunity for his feedback and we don’t know if his team’s needs are being well represented.
- The surprise around the two features and how fraud mitigation wasn’t included indicates that the Marketing Director wasn’t involved enough in the Roadmap (hint: StoryMap) or Ongoing Backlog Refinement.
- No end users were involved in the Sprint Review. Without their input, all of the feedback that was delivered was theoretical and from people who are involved day-to-day with the Product, so hardly objective.
- Underdeveloped facilitation skills showed through. As Steve grows in the role of ScrumMaster over time, he might prepare in advance for conflict. Knowing that it will or might happen, he could have a short reset exercise ready to go that will cool tempers and improve relations so the Review can continue and the conflict can get resolved, rather than postponed. _In the early stages of a ScrumMaster’s journey, it is a little unfair to expect them to know how to facilitate through conflict._

### What could they do differently next time?

It starts long before the Sprint Review meeting. When the strategic work is done in Product Backlog Refinement, ScrumMaster Steve and Product Owner Paula need to make sure that key stakeholders, like Jan (Marketing) and Eric (Support), are involved. ScrumMaster and Product Owner should also commit to spending a couple of hours a month reviewing the strategy and looking for things that might turn into surprises. When there are items that represent more risk or challenge, Paula can invite the Stakeholders to the Backlog Refinement session so they can provide input and clarity. These two actions will go a long way toward reducing surprises in the Sprint Review.

Seeing a feature get reviewed by the PO and checked against the Definition of Done has never been a recipe to increase engagement. As an alternative, Paula could review features as fully completed, having already checked them against “Done” prior to the Sprint Review. This approach fits well in a world of Continuous Delivery, something many modern teams are already employ. As a good final check just before Sprint Review, Paula could recheck all features to make sure they work well together.

Get End Users in the room. Where humanly possible involve actual users of the product to get feedback, to learn more about their needs, and generate enthusiasm. _There are clear limits as most users won’t have the time or energy to participate every Sprint._

Replace Show and Tell with Show and Play. Have someone who knows the product well show the high-level features. Have each developer pair with a stakeholder/end-user and invite them to play with the product. As much as possible they should focus only on the work completed in this Sprint. Show and Play helps the users and other stakeholders discover how the product actually works, it generates a much deeper level of feedback, and it helps team members learn more about the needs of real users.

A good Sprint Review gets features accepted and deployed. A **great** Sprint Review engages the attendees and creates productive discussion around product direction and business priorities.

### Learn more about how to hold great Sprint Reviews

Consider attending one of our [Certified ScrumMaster workshops](/certified-scrummaster-csm-training), where we discuss the _how_ and _why_ of Scrum, not just the _what_.  You'll get hands-on practical experience, and learn about some of the challenges – and solutions – along with tips on how to help your Team learn and grow to realize their potential.

\[1\] Hint: this shouldn’t be the first time the PO sees a feature

Image attributes: Agile Pain Relief Consulting
