---
title: "Mythbusting - Collective Code Ownership"
date: "2008-05-07"
categories: 
  - "software-development"
tags: 
  - "code-ownership"
  - "martin-fowler"
  - "software-development"
coverImage: "working-together-xs.jpg"
excerpt: 'A number of writers equated Collective Code Ownership (CCO) with "no ownership" or chaos.'
---

![Working together - image licensed from Photodune](src/content/blog/mythbusting-c/images/working-together-xs.jpg) In researching "[Are there weaknesses with Collective Code Ownership?](external:https://www.infoq.com/news/2008/05/weaknesses_collective_code)" for a news item on InfoQ I was struck by the number of myths that get repeated around Collective Code Ownership. I thought it time to burst a few balloons.

A number of writers equated Collective Code Ownership (CCO) with "no ownership" or chaos. Yet nothing could be further from the truth. Let's revisit [Martin Fowler's definition](external:https://www.martinfowler.com/bliki/CodeOwnership.html) (he's a better writer than I):

> **Collective code ownership** abandons any notion of individual ownership of modules. The code base is owned by the entire team and anyone may make changes anywhere. You can consider this as no code ownership, but it's advocate prefer the emphasis on the notion of ownership by a team as opposed to an individual.

Now its not easy to practice CCO and to make it work you need an agreed on set of coding/formatting standards. You also need to practice pair programming to help maintain the required discipline. But its not chaos.

Simon Lin mentions a team that shared a single version control account. I'm not sure where this myth commons from. CCO says that we all own the code and that we're all responsible for maintaining it but nothing is said about sharing the same account. I think that responsibility requires that we're accountable for what we change.

Ralf's Sudelbücher argues that "[Collective code ownership is limiting software quality](external:https://weblogs.asp.net/ralfw/archive/2006/04/01/441639.aspx)", in a rather lengthy note from two years ago. His core argument appears to be that generalizing specialists can't know all of the domains that they need to code and so produce weaker code. The number of domains that a project might encompass has grown so large (ASP .NET, SQL, ADO, ...) that no one programmer on the team can command a knowledge of them all. On this last point we agree. However I don't think that means that team members who aren't specialists can't produce good quality, simple code in other problem domains. Simplicity is easy to appreciate no matter what the problem domain. In addition most new API's follow well established patterns for a lot of methods (i.e. open/close) that make it easier to pick up the basics. To solve the remainder of Ralf's problem: when coding in area where you don't know the speciality well either pair with the specialist or get them to review it after the fact. Effectively implementing Martin Fowler's [Weak Code Ownership](external:https://www.martinfowler.com/bliki/CodeOwnership.html). At least this way we avoid the inevitable bottlenecks when we really on the point hats to do all the work.

One fact I'm coming to believe: to achieve the discipline required for CCO to work you need more than just common development standards. You also need to write most of your code using Pair Programming and Test Driven Development (at worst Test Minutes Afterward). Without these practices, consider using [Weak Code Ownership](external:https://www.martinfowler.com/bliki/CodeOwnership.html) where each module/package has an owner/evangelist who's role is to ensure that the conceptual integrity is not only maintained but explained to other team members.

Image via: [https://photodune.net/](external:https://photodune.net/)
