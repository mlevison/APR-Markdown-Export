---
title: "Does Your Grocery Store Limit Work in Progress?"
date: "2011-05-04"
categories: 
  - "business"
  - "teams"
tags: 
  - "bottleneck"
  - "case-study"
  - "examples"
  - "self-organizing-teams"
  - "theory-of-constraints"
  - "work-in-progress"
coverImage: "photodune-4373665-grocery-store-xs.jpg"
---

![Grocery store - image licensed from Photodune](src/content/blog/does-your-grocery-store-limit-work-in-progress/images/photodune-4373665-grocery-store-xs.jpg)Shopping in our local Grocery Store (Farm Boy) on a recent Saturday made me realize what a good job they do Limiting Work in Progress (WIP) and Self Organizing. Driving into the parking lot with my 4yr old, I was dreading the busyness of the store. When I got in, the place was packed, and trying to manoeuvre even a small cart with a 4yr old driving was quite the experience. I had expected the checkout experience to be easily 10 minutes long, an eternity even with the best behaved child.

When I entered the store there were only a few people on cash and the lines seemed to be building. By the time we were ready to checkout half an hour later, all 9 cashes were open and we waited less than two minutes.

What happened? A couple of conversations with cashiers have helped me piece together the key points:

- They all recognize that Farm Boy doesn’t make money until you’ve paid – a Customer with unpaid groceries is Work In Progress. _After all if you only have a few items and see a 10 minute line up you might just leave. Especially if the 1-8 items queue is also deep._
- If there is a line up, cashiers just start opening lanes until the bottle neck is cleared
- Many of the staff can work the cash, so you’re rarely stuck waiting for another cashier
- Staff don’t wait to be told to open cashes they just do it
- When demand ebbs, the cashiers start to close and return to other work

So effectively they’ve seemed to discovered the [Theory of Constraints](https://en.wikipedia.org/wiki/Theory_of_Constraints) (TOC) and they Self-Organize to eliminate the bottleneck. Their system is informal, but even without sophisticated measurements you can still observe and eliminate bottlenecks. Compare this to another large Canadian grocery chain where I often line up for 10+ minutes, just waiting to get to the front of the line. Guess which store gets more of my business?

In the software world, QA, especially when all the tests are run manually, is often the constraint we find. So we need to take steps to eliminate the bottleneck:

- Automate your Regression Tests, so that you have a minimal (if any) manual regression work to do
- Train **everyone** on the team in the basic of QA
- When work builds up in QA, cease writing new code until the existing code has been tested and the tests automated
- Start write your application using Acceptance Test Driven Development

Eventually QA stops being the bottleneck, at which point we re-examine the system to see if the bottleneck has moved again. When that happens, take similar steps all over again to eliminate the next bottleneck.

What bottlenecks have you observed in your grocery store? Your development process?

Another Theory of Constraints post: “[Theory of Constraints in Software Development](https://www.codeforlife.org/2011/05/theory-of-constraints-in-software.html)”

Image via: [https://photodune.net/](https://photodune.net/)
