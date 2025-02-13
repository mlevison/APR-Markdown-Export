---
title: "Scrum by Example - Impediments are Holding Back the Team"
date: "2011-12-07"
categories: 
  - "scrum-by-example"
tags: 
  - "daily-scrum"
  - "impediments"
  - "scrum-by-example"
  - "scrummaster"
  - "unit-testing"
coverImage: "stop-sign-FreePik.jpg"
excerpt: 'What is an impediment? Anything that stops the team from delivering value. ANYTHING.'
---

![Stop Sign. Image by FreePik](src/content/blog/scrummaster-tales-impediments-are-holding-back-the-team/images/stop-sign-FreePik.jpg) The team are holding a daily standup mid-sprint. During the meeting Tonia the world's best tester answers the obstacles question by saying: "The test server is down for the third time this week and I will spend the day writing new test cases." Meanwhile Doug doesn't raise any impediments but notes that he has spent his third day trying to write Unit Tests for a previously completed class (_Ed: The team doesn't know about Test Driven Development yet)_. This task was originally estimated to take one day.

## Analysis

What is an impediment? Anything that stops the team from delivering value. ANYTHING. Anything that stops code from being written, tested, deployed and making money. Some examples include:

- Dead computer
- Noise from neighbouring teams
- Missing tools i.e. you need to find memory leaks but the company won't pay for tool to find leaks
- Lack of training i.e. you've been switched from writing Cobol to Java, but provided no support beyond a couple of books to make the transition.
- Focus on Roles
- Mandated to use a company wide tool without an ability to make local decisions
- Focus on reducing costs over delivering value
- Unwillingness to seek new ideas outside of the organization. _This often happens in larger companies that just assume they're the best_
- People who talk agile but walk a more traditional approach
- Focus on tools to solve problems without talking to people first

The standup raised two impediments. Tonia seems to be treating ScrumMaster Steve as ticket taker, i.e. just hand Steve the problem and go onto something else. Her few words in the standup seem to indicate that she believes that the problem is beyond her control so she just gives up assuming it will get solved for her. Doug on the other hand doesn't recognize he has an impediment he's just struggling to to get his work done. The impediment here is subtle, it can either be: Doug is unfamiliar with Unit Testing and needs help to learn **or** some knurly legacy code that isn't unit testable as it stands. In either case Steve needs to understand what the problem is so he knows what kind of help Doug needs.

We will help Tonia and Doug resolve their issues in a few minutes but first lets equip Steve with some simple impediment removal tools. Once an impediment has been raised we need to make it visible. The best way to do this is to maintain a **highly visible** list in an area on the team's task wall. (N.B. a wiki or other online tool isn't considered highly visible.) Impediments that involve individuals should be written to remove the focus from the person and put on the issue, example instead of "Doug needs training for Unit Testing", "Training for Unit Testing". Along with the change in focus it also recognizes that Doug is probably not the only one with the issue. Impediments that can't be  easily fixed just by making them visible and doing some work should be raised in the next retrospective. During the retrospective the team can spend more time planning to tackle the issue.

Scrum will discover many organizational impediments that can't be resolved quickly, it is important that we acknowledge these impediments and don't just sweep them under the rug. In addition we can't just say "That will never change, that's just the way we work". This is the hard part of Scrum.

## Back to the Story

Right after the standup Steve goes and talks to Doug. He discovers that while the legacy code has issues, Doug has very limited experience writing Unit Tests. They sit down together and write up an impediment card that identifies the issue without Doug feeling like he is being singled out or attacked. Steve also writes an impediment card for the test server issue. Steve invites Tonia to join him in tracking down someone from Operations to find out what the test server problem is. Operations reboots the server but suggests the problem is systematic and that they don't have the time to investigate. Later in the day Don (Steve's Director) walks into the team room and reviews the impediments list. Talking to Steve he discovers that the Test Server has become a recurring problem, he promises to start digging from his end to find out more about the deeper issue. Don also promises Steve support in getting books/training around Unit Testing if that will help Doug.

## Analysis

By making even subtle problems **highly visible** the team is able to resolve problems faster. Sometimes the help to remove these problems comes from unexpected places in this case Don, but it could just as easily have been someone else who walked into the team area and offered to help. For example seeing the need for help around Unit Testing maybe someone from another team would volunteer to help.

How does your team address its impediments? How does it make them visible?

Image via: Freepik
