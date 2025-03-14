---
title: "Scrum By Example – Learning How to Estimate"
date: "2012-06-27"
categories: 
  - "estimations"
  - "scrum-by-example"
tags: 
  - "agile-training"
  - "estimates"
  - "new-people"
  - "planning-poker"
  - "product-backlog"
  - "scrum-by-example"
  - "sprint-planning"
coverImage: "photodune-1602425-cards-hand-xs.jpg"
excerpt: '_[Scrum By Example](/blog/scrum-by-example) is a series of stories about ScrumMaster'
---

![Hand of cards - - image licensed from Photodune](src/content/blog/scrummaster-tales-learning-how-to-estimate/images/photodune-1602425-cards-hand-xs.jpg)

_[Scrum By Example](/blog/scrum-by-example) is a series of stories about ScrumMaster Steve who is the ScrumMaster for the WorldsSmallestOnlineBookstore._

Product Owner Paula has learned from her past mistakes (See [Not Ready for Planning](/blog/the-scrummaster-tales)) and she now holds Backlog Grooming/Refinement Sessions whenever she has enough Stories to be worth Estimating (typically every 2-3 Sprints). During these meetings, team members estimate New Stories, split Large Stories, and develop Acceptance Criteria.

With 10 new Stories and a couple of "Epics" that need to be split, Paula has scheduled a Grooming session for the middle of the Sprint. She has invited all the team members to attend; Kirby (see [New People on the Team](external:https://agilepainrelief.com/blog/scrummaster-tales-new-people-on-the-team)) comes but is grumbling, "I don’t see the point in this. It's just going to waste precious coding time. Why can’t this just happen in Sprint Planning?" (_Editor – Kirby hasn’t quite found his rhythm yet_). Paula reminds the team that the meeting exists so the team can ensure that Product Backlog is well prepared for the next Sprint Planning meeting. In addition, it helps her understand how much of the backlog they can realistically complete before the next release in three month’s time (_Editor – yes they have infrequent releases_).

She asks that they start estimating her first new story:

"As a frequent book buyer I want the store to remember me so I can add books to my shopping cart without having to login."

Team members start asking questions requiring clarification:

- Is it okay to leave a cookie behind? _Paula -Yes, although it will need to comply with our privacy policy._
- Ian asks, “Are there any other technologies to consider?”
- Does this include being able to see the book in the shopping cart? _Paula - No._
- What if we don’t have accounts implemented when we start this story? _Paula - Then just use a fake/sample account for now._

When the questions peter out, Team Members begin flipping through their Planning Poker™ cards (_I will have some for my readers soon_),looking for the right numbers. Kirby just looks around in confusion. Nobody had checked to see if he understood the estimation process. There was a pause and Scrum Master Steve asked, “What do you know about our estimation process?” The reply was, “Nothing.” Steve asked if he understood the flaws of traditional estimation – Kirby was sure he had this one down cold, “Yeah, you need to double the figures and then add a fudge factor, but never tell the developers otherwise their work will expand to fit the time available.” There was some nervous laughter, as Kirby has had trouble fitting into the team in the past (see [New People on the Team](external:https://agilepainrelief.com/blog/scrummaster-tales-new-people-on-the-team)).

## Analysis

What are Steve’s options at this point?

- Explain Agile Estimation from scratch – _snoozefest for the rest of the team._
- Ask Kirby to sit out and watch – _better – but we learn more by doing than watching._
- Explain the bare minimums to Kirby and invite him to participate.

As usual Steve doesn’t take my advice and forges his own path.

## Story

Steve decides to explain the flaws with traditional estimates.

- At best they’re in ideal days – which is a problem because management will often assume that a normal day is the same as an ideal day; as humans we’re not adept at estimating in time; estimates in ideal days decay as the team gets better at doing its work.
- Experts do the Estimation (at best) or sometimes it's the Project Managers (not all of whom have development experience). However, experts are the people who have forgotten many of the details it takes to get the work done.
- Estimates are only valid for one person – the Estimator.
- They miss the chance to sample the diverse ideas of the Team.

Instead Steve explains that we use relative estimation. All stories are compared to an existing gold standard much like the [original metre stick](external:https://en.wikipedia.org/wiki/Metre#Prototype_metre_bar). This “standard story” is arbitrarily given a size of ‘2’. In addition the team have also selected  a story approximately 4 times larger and made it an ‘8’.

## Editor's note

When coaching new teams, I suggest stories of size ‘2’, are very small. I expect the typical team to complete 5-10 stories of this size during a Sprint. Stories of size ‘2’ should have few unknowns. When they pick the prototypical ‘8’ I suggest this should be a story that isn't completely understood and still has an unknown or two.

## Story

Now Steve says, “Instead of more explanations, let's just start Estimating.” Someone hands Kirby a set of estimation cards with values 0, 1, 2, 3, 5, 8, 13, 20, … . Steve suggests that anything over 20 is too big and will need further splitting _(Editor – Anything over 13 is too big)._ Paula rereads the first story: “As a frequent book buyer I want the store to remember me so I can add books to my shopping cart without having to log in.” Steve asks if everyone is ready with their first estimate. First round results:

<table border="1" cellspacing="0" cellpadding="0"><tbody><tr><td valign="top" width="83">Tonia</td><td valign="top" width="83">Brad</td><td valign="top" width="83">Martin</td><td valign="top" width="83">Doug</td><td valign="top" width="83">Ian</td><td valign="top" width="83">Kirby</td></tr><tr><td valign="top" width="83">5</td><td valign="top" width="83">3</td><td valign="top" width="83">13</td><td valign="top" width="83">5</td><td valign="top" width="83">8</td><td valign="top" width="83">8</td></tr></tbody></table>

Steve asks the low (Brad) and high (Martin) estimators to explain their thinking. He also starts a 3 minute countdown timer on his iPhone. Brad leads off by saying,“This is a very simple standard shopping cart feature; it’s exactly the same thing I did when I worked on ShopMore; we just have to use a standard shopping cart.” Martin replies, “Yes, we can use a standard shopping cart, but the last time I used the ShoppingKart engine it required a lot of small changes to our database.” Ian points out that ShoppingKart have updated their engine since then and the new version claims to be easier to use. Steve asks the rest of the team if they want to ask any clarifying questions, when the answer is no, they estimate again:

<table border="1" cellspacing="0" cellpadding="0"><tbody><tr><td valign="top" width="83">Tonia</td><td valign="top" width="83">Brad</td><td valign="top" width="83">Martin</td><td valign="top" width="74">Doug</td><td valign="top" width="92">Ian</td><td valign="top" width="83">Kirby</td></tr><tr><td valign="top" width="83">8</td><td valign="top" width="83">5</td><td valign="top" width="83">8</td><td valign="top" width="74">5</td><td valign="top" width="92">8</td><td valign="top" width="83">8</td></tr></tbody></table>

Again Steve asks the low (Doug) and high (Ian) Estimators to explain their thinking. This time Ian says, “While it's been improved, ShoppingKart always present problems,” and Doug says, “I’ve solved this same problem before at another Ecommerce site – it was pretty easy.” Steve calls for a third round of estimates. Little has changed from the last round; the numbers are 5 and 8. Kirby says, “Why not average the numbers?”

## Analysis

![An image of two architects' hands doing work - image licensed from Photodune ](src/content/blog/scrummaster-tales-learning-how-to-estimate/images/architects-xs.jpg)What are the team’s options at this point?

- A difference of one size, i.e. 5 vs. 8, or 8 vs. 13, isn’t meaningful. But a difference of two steps, i.e. 5 vs. 13, is meaningful. _Editor: In this case the team could easily just pick one._
- Averages lead to arbitrarily precise numbers – a precision that doesn’t really exist. In addition, averaging takes away the power of the individual voice.
- Just pick ‘8’. Agile estimation is trying to give equal voice to all opinions; when we pick the largest number we’re saying the other opinions didn’t matter.

In my experience the best thing to do is set aside the story until the end of the estimation session. Often when we return, its size is now entirely obvious when compared with other stories we’ve estimated since. Finally if there is still no agreement, this is telling the team there is uncertainty in the problem. Coming up with an estimate is papering over the uncertainty. Instead, I recommend the team schedule a [Spike](external:https://www.extremeprogramming.org/rules/spike.html): 1-2 days rapid work on the problem, the goal of which is to help the team explore the boundaries of the problem and come up with enough information to produce an estimate. A Spike is committed to, the same as any other work in Sprint planning. When you do run a Spike, you should appreciate that the result is almost always throwaway code.

## Tips

- Story Points are self-calibrating so it does not matter precisely which ‘2’ and ‘8’ the team pick, just as long as they’re used consistently.
- Blind estimates are important – no one shares their estimate until everyone is ready, otherwise people will naturally follow the senior team member’s lead.
- Many ask the question, “How can I make our estimates more accurate?” Don’t spend the time on that; estimates are only useful for answering the question of, “Roughly when will we be done with this list of features?” Focus improvement efforts on getting better at doing the work, i.e. learn Test Driven Development and make your build run faster.
- Timeboxing the discussion in Agile Estimation is critical, otherwise the team can get bogged down when there is already broad agreement. Timebox the discussion to 2-3 minutes per round.

With Estimation the focus is on how big the thing is that we’re building, but an additional benefit of the process is that team members gain a much deeper understanding of the system they’re building.

What have you learned from your Estimation Process? What Estimation tips do you have?

_**[Scrum by Example](/blog/category/scrum-by-example) is a narrative-style blog series designed to help people new to Scrum, especially new ScrumMasters. If you are new to the series, we recommend you [check out the introduction](/blog/scrum-by-example) to learn more about the series and discover other helpful articles.**_

Images via: [https://photodune.net/](external:https://photodune.net/)
