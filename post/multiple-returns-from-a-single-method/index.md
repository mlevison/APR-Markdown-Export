---
title: "Multiple Returns from a Single Method"
date: "2008-08-03"
categories: 
  - "software-development"
tags: 
  - "software-development"
coverImage: "doorway-xs.jpg"
excerpt: 'Let's start by looking back to where this idea stems from. As best I can tell objections'
---

![Doorway - image licensed from Photodune](src/content/blog/multiple-returns-from-a-single-method/images/doorway-xs.jpg) It’s funny just about the only thing anyone really objected to from my recent post on [Minimal Coding Style](/blog/minimalist-coding-style.html) was multiple return statements.

Let's start by looking back to where this idea stems from. As best I can tell objections to multiple returns stem from [Dijkstra's](https://en.wikipedia.org/wiki/Edsger_Dijkstra) 1968 paper “[Go To Statement Considered Harmful](https://david.tribble.com/text/goto.html)”. From David Tribble who has written a Retrospective on the letter, from the [introduction](https://david.tribble.com/text/goto.html):

> This paper was written at a time when the accepted way of programming was to code iterative loops, **if-then**s, and other control structures by hand using goto statements. Most programming languages of the time did not support the basic control flow statements that we take for granted today, or only provided very limited forms of them. Dijkstra did not mean that _all_ uses of goto were bad, but rather that superior control structures should exist that, when used properly, would eliminate _most_ of the uses of goto popular at the time. Dijkstra still allowed for the use of goto for more complicated programming control structures.

Here is what I believe about methods:

- Short, Short, Short – at most one screen long – anything more requires the reader to scroll up and down to understand the code.
- Do only one thing – for the ultimate anti example of this: [Munger](http://preserve.mactech.com/articles/mactech/Vol.12/12.05/Handles2/index.html) (MacOS 7/8/9) the swiss army knife of memory allocation that did different things depending on the combination of parameters. _Note the linked article doesn’t describe a fraction of what Munger did. Be afraid._
- Have descriptive (but not verbose) name.
- Be simple and easy for the maintainer to read – this implies reducing the complexity of the control structures.

Some reasons I dislike the single exit argument:

- If there are cases that aren’t applicable (invalid method arguments, …) I like to exit the method early to avoid additional indentation.
- Without early exits we have to keep track of whether each additional branch was intended to execute.
- Without early exits the ‘result’ might accidentally get changed, meaning the wrong value is returned.
- If more code is added later it might accidentally get run even though its author intended the method to be finished.
- If you need to clean up use a try/finally block since even early returns pass through finally blocks.
- If multiple return statements make a method hard to read then the method is probably too large. In addition most IDE’s will allow you to highlight the control statements in any colour you need to make them visible.

More than a few other people have written on this in recent years: [Bruce Eckel](https://web.archive.org/web/20200504122839/https://onthethought.blogspot.com/2004/12/multiple-return-statements.html), [Java Think](https://javathink.blogspot.com/2006/10/short-concise-and-readable-code-invert.html) (Taylor Gauthier), [Java Basics](https://www.leepoint.net/JavaBasics/methods/method-commentary/methcom-30-multiple-return.html), [Peter Ritchie](https://blogs.msmvps.com/peterritchie/2008/03/07/single-entry-single-exit-should-it-still-be-applicable-in-object-oriented-languages/).

Do the person reading your code in the future a favour. Use early return statements to minimize the complexity in your code.

Image via: [https://photodune.net/](https://photodune.net/)
