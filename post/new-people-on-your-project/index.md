---
title: "New People on Your Project"
date: "2010-06-03"
categories: 
  - "agile"
  - "teams"
coverImage: "19631-scaled.jpg"
excerpt: 'On any project it will take from 2-4 months for the team to integrate a new person and'
---

![Two male partners shaking hands at the office - image by senivpetro via Freepik](src/content/blog/new-people-on-your-project/images/19631-1024x683.jpg)Your project schedule says that you will get 2 more team members this week and 3 more next month. How do you integrate them into the team? How do you bring them on board? How do you avoid slowdowns? In a word you can’t avoid the slowdown – adding new people to the project will slow the existing team down.

On any project it will take from 2-4 months for the team to integrate a new person and recover from the slowdown:

- The person will need to be trained: In your code base, how your application works, what coding style is, how you application works, …
- This person will disrupt the Teams Formation (see [Tuckman’s model of team formation](external:https://en.wikipedia.org/wiki/Tuckman%27s_stages_of_group_development)) – this is an especially important cost when the team has already reached the performing stage. This happens because the new person alters communication paths and will force people to renegotiate relationships around the **entire** team.
- The person will be a drag on the team requiring support to learn new tasks.
- The person will increase the communication complexity (i.e. the number of communication paths) within the team.

All of this leads us to discover [Brook’s law](external:https://en.wikipedia.org/wiki/Brooks's_law): “adding manpower to a late software project makes it later” (from the Mythical Man Month 1975, reprinted in 1995). The physics of people hasn’t changed in 35 years.

So what can you do to solve this problem?

- Say no – if its too late in the project – in many cases 4-5 months before release is too late.
- Can’t say no consider what Project Udall ([Surviving Object-Oriented Projects](external:https://www.amazon.com/gp/product/0201498340/&tag=notesfromatoo-20) Alistair Cockburn, p20) did: Halt the big project, start a small project and add only the people who can contribute to its success to the new project. _While its expensive to have people sitting idle, it may be cheaper than having them slow the project down._
- Bring on all the new people at once so at least you pay the costs once in the life of the project as opposed one person at a time.
- Create a new team staffed by the new people with one or two old-timers. They won’t get very much done for a while, but at least they get in the way of the others.
- Get them to help with the exploratory testing, with the focus being the stories that are being written in that Sprint of iteration.
- Ask them to write or refactor some automated acceptance tests.
- Get them to read and write Unit tests – start by reading existing Unit tests, after all these should explain the code. If they’re not already [Good Unit Tests](external:https://www.infoq.com/news/2009/07/Better-Unit-Tests/) then take the time to improve. If they’re good then do some small refactorings in the main code base – after you can trust your tests can’t you :-)
- Ask them to [pair](/blog/pair-programmin) with another developer

Just remember adding more people to a project is a way of slowing your project down.

Image by senivpetro via Freepik
