---
title: "Story Slicing, How Small is Enough?"
date: "2010-09-27"
categories: 
  - "agile"
  - "scrum"
tags: 
  - "agile"
  - "invest"
  - "scrum"
  - "software-development"
  - "software-management"
  - "story-points"
  - "user-story"
coverImage: "photodune-3570112-cutting-xs.jpg"
---

![Story Slicing. Cutting - image licensed from Photodune](src/content/blog/story-slicing-how-small-is-enough/images/photodune-3570112-cutting-xs.jpg) When Agile/Scrum Trainers teach about new teams about User Stories, we usually talk about Bill Wake’s [INVEST](https://xp123.com/xplor/xp0308/index.shtml) criteria, which includes Small:

> Good stories tend to be small. Stories typically represent at most a few person-weeks worth of work. (Some teams restrict them to a few person-days of work.) Above this size, and it seems to be too hard to know what's in the story's scope. Saying, "it would take me more than month" often implicitly adds, "as I don't understand what-all it would entail." Smaller stories tend to get more accurate estimates.

This statement is a great start, but it doesn’t explain why or give you much guidance about what to do.

## Why Small Stories?

Why not just give the team large stories that span iterations. Why are always asking if you can slice those stories smaller? A number of reasons:

- Small stories provide focus and a short horizon for the team. It’s easier to get lost in the details with a larger story.
- When you still have development to test handoffs (i.e. before you start doing [ATDD](https://www.methodsandtools.com/archive/archive.php?id=72) (Acceptance Test Driven Development), smaller stories enable more frequent handoffs and allow testers to work on smaller chunks of code.
- Small stories give you the flexibility to reconfigure and adapt to new discoveries or changes. Perhaps the PO discovers that an existing story is now irrelevant; or while coding you discover a surprise. Small stories make it easier to adapt.
- Small stories provide more feedback opportunities at all levels of the system and more opportunities for personal satisfaction; think of the small dopamine rush that happens every time you complete something!
- Large stories increase the risk that your team will deliver nothing at the end of the iteration.
- Your team has a capacity like a drain pipe and just like a pipe the larger the object you try to push through it the more likely it is that blockages and bottlenecks will occur. Perhaps one person who is tied up in the large story may also be the only person who can complete a key piece of another story.

So what is my guidance for new Scrum teams when they’re trying to decide on Story size? **Two people for half an iteration.** Why two people? Because most stories require collaborative effort and I want to encourage pairing/collaboration. Why half an iteration? Because any larger makes it quite likely that the story will not be completed in a sprint. Even stories of this size are still a bit large, and they shouldn’t commit to more than one of these per sprint. For some strange reason with most teams I coach, stories of this size are 13 [Story Points](https://saat-network.ch/2008/02/explaining-story-points-to-management/), I don’t really know why this happens.

All this suggests that most stories are going to be in the range of 1-5 story points by the time the team is ready to commit to them. You can still have Epics and Themes they should just be split into much smaller parts before the team attempts to commit to them.

## But That’s Really Small

If we’re working in bite size chunks, how do we get any meaningful work done? How do you slice them so small? Part of the problem is a frequent misunderstanding around value in stories. The ‘V’ in [INVEST](https://xp123.com/xplor/xp0308/index.shtml) stands for valuable, many people assume that equates to business value or a feature that you can sell for a dollar. When we combine user stories together, they represent features that customers will pay for. But on their own they’re too small for that. Instead value refers to the point of view of the user for whom the story was written in the first place.

So the hard part how do you slice? Some simple ideas:

- CRUD (Create, Read, Update, Delete) boundaries
- Acceptance criteria – often the acceptance criteria on the back of the [Story Card](https://blog.aaladdin.com/?p=33) will give a good hint.
- Happy Path – many stories have exceptional conditions, consider splitting them out
- Simple versions of an algorithm. With a complex algorithm and complex UI, it might be worthwhile to do a simple version of either first and then fill in the detail in the next story. Sometime this can come from making some elements constants instead of looking them up or calculating them

Bill Wake: [Splitting Stories](https://xp123.com/xplor/xp0512/index.shtml), Rachel Davies: [Ideas for Slicing Stories](https://agilecoach.typepad.com/agile-coaching/2010/09/ideas-for-slicing-user-stories.html) and Lasse Koskela: [Ways to Split Stories](http://aqqurite.se/agile/ways-to-split-user-stories-guest-post-by-lasse-koskela) have much longer lists.

What not to do: Split along architectural or technology boundaries, as this will create stories that don’t deliver value to an end user.

When slicing stories imagine using a scalpel and not a butcher’s knife. Go create some story sashimi.

_Update: I was asked for some examples and I've written some in [More Story Splitting](/blog/more-notes-on-story-splitting.html)._

Image via: [https://photodune.net/](https://photodune.net/)
