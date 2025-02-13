---
title: "Pair Programming vs. Code Reviews - It's a no Brainer"
date: "2007-12-14"
categories: 
  - "software-development"
coverImage: "casual-executives-working-together-at-a-meeting-with-laptop-xs.jpg"
excerpt: '...(and I’ve done many) are static. One or more people study the code often long after it'
---

![Portrait of casual executives working together at a meeting with laptop. - image licensed from Photodune](src/content/blog/pair-programmin/images/casual-executives-working-together-at-a-meeting-with-laptop-xs.jpg) Ok so I’m about a month behind. Over on [Coding Horror Jeff Atwood](https://blog.codinghorror.com/pair-programming-vs-code-reviews/) asked “**I can't help wondering if pair programming is nothing more than code review on steroids**”. In a word ‘No’.

### **Code Reviews**

...(and I’ve done many) are static. One or more people study the code often long after it was written and attempt to understand it. Most code reviews I participated in are very shallow. We tend to find simple issues that tools like PMD and FxCop could find for you: variable could be final, public method could be private etc. At their very best I’ve seen methods (and sometimes classes) rewritten in response to a code review. Rarely do I see the design questioned. In addition it’s often tough to spot the forest for the trees – buried in the minutia of a class the bigger questions don’t get asked – does this class need to exist? Etc. Finally simplifications of lead to more simplifications but due to the static nature these won’t be found.

### **Pair programming**

...on the other hand is dynamic. It’s an ongoing conversation between two partners.

- One partner focuses on the details – what test case am I’m writing now, what’s the minimal amount of code that I need to satisfy the test. While the other partner is focusing on the big picture: What’s the best design for this problem.
- It’s not just a code review, but ongoing design review.
- Changes are made in real time so as simplifications are made new ones are easily spotted.
- When one member of the pair is stuck the other can step in with an idea.

Some additional benefits:

- Spreads the knowledge of the code base more widely.
- More people are aware of problems as they develop.
- Helps raise everyone’s skill level as pairs learn tricks from each other.
- Reduces the number of places where only one person understands what’s going on.
- Fewer bugs – about 15% fewer according to a study by Alistair Cockburn and Laurie Williams ([PDF](https://collaboration.csc.ncsu.edu/laurie/Papers/XPSardinia.PDF))

One point which Jeff definitely has right – it's hard work. Pairing for eight hours a day is not an option. Most pairs work in two-hour blocks twice a day. For a more detailed article see Jeff Langr: [Pair Programming Observations](https://langrsoft.com/2005/01/09/pair-programming-observations/)

So, Jeff, if you want to discover the benefits of pairing in person (or over a remote connection) give me a shout and we will arrange something.

Image via: [https://photodune.net/](https://photodune.net/)
