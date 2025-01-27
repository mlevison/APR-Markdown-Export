---
title: "Reinventing Existing Products – Big Bite vs Small Nibble Rewrites"
date: "2016-11-22"
categories: 
  - "agile"
  - "business"
  - "scrum"
tags: 
  - "agile"
  - "agile-culture"
  - "agile-development"
  - "agile-methodology"
  - "technical-debt-2"
coverImage: "big-bit-small-nibble.jpg"
---

![Big Bite Small Nibble - images licensed from Unsplash: Alec Weir, Bonnie Kittle](images/big-bit-small-nibble.jpg)

Twice now in my career I’ve done a massive rewrite to replace an existing product. In both cases, it didn’t end well. Each time, the new product was competing with an existing product that was making the company money. So, of course, the existing product got enhancements on a rickety structure, and on the new product we never caught up. In one case we solved the problem by getting bought out, in the other, the two products lived side by side for far too long.

It’s tempting to say that we’ll just start fresh, write it greenfield (i.e. from scratch). It’s an attractive idea, because we start off with clean code (no legacy) and we’re not hamstrung by decisions of the past.

The problem is that rewrites never happen as rapidly as promised, and never do they deliver everything that is expected. If it must be a massive overhaul and reinvention of an existing product, why not consider doing piece-meal, in-place replacements instead of a total, big-bang rewrite. There are some considerable benefits to this approach:

\-        Existing Product can gain new features and continue to serve client needs while you’re developing new.

\-        Is more resilient against delays in time to market, which is always longer than you expect.

\-        Allows for the organizational pressures that created the original product to change. If they don’t, then the rewritten product will suffer the same problems as the original.

Use a [strangler approach](https://www.martinfowler.com/bliki/StranglerApplication.html). Replace one small part of the system, adding new features, writing tests, etc. as you go. Do that one small chunk at a time, until the new system replaces the old. Bonus points awarded for going from monolithic to a number of mid-sized services (you’ll note I didn’t say the overused MicroServices word).

Hmm, I think I just summarized Feather’s book](https://www.amazon.ca/Working-Effectively-Legacy-Michael-Feathers/dp/0131177052/&tag=notesfromatoo-20) in one paragraph. Another good legacy code book: “[The Mikado Method](https://www.amazon.ca/Mikado-Method-Ola-Ellnestam/dp/1617291218/&tag=notesfromatoo-20)”. Finally, if you need more Legacy Code reading, checkout out our [Legacy Code and Systems.

Image attribution: Unsplash: Alec Weir, Bonnie Kittle
