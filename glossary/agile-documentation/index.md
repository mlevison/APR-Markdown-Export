---
title: "Agile Documentation"
date: "2022-08-26"
relatedTerms: ['behaviour-driven-development', 'user-stories']
---

**Agile Documentation.** Is it an oxymoron? The _Agile Manifesto_ says "Working Software over Comprehensive Documentation". It doesn't say _no_ documentation, and it doesn't say _how much_, if at all.

In an Agile world, we focus our work on delivering value to the customer, not on chronicling the process. At a high level, some teams maintain a one-page system design document. Other teams have used a whiteboard with a "best before" date and, once the whiteboard expires, someone takes a picture with their phone and wipes it clear. If the erased information is still valuable, several people work together to create a new version of the picture based on their current understanding of the system. The elegance is that it starts fresh and it is created collaboratively.

What about the user stories as documentation? They seem like documents at first. The challenge is that they degrade in value over time. They're just intended to be a placeholder that starts a conversation among the team members about the piece of the product that they're building. The problem is that a description that works well as a User Story, isn't meaningful months after the implementation is complete. We forgot the details and, in many cases, the original user story can no longer be found since the system that has been built on it obscures the original.

The acceptance criteria become low-level documentation. Teams that learn Behaviour Driven Development often use the examples created in that approach as their documentation. Even better, if they have mastered the art of automating their examples, they become executable documentation. Executable examples can be run, and if they pass then both the code and docs are in agreement. If they fail, then either the code or the examples need to be updated.

Instead of looking to add more documentation, seek to reduce the need for documentation. In many cases, it exists solely for the handoff to the next group of people (test, deployment, etc). Instead of creating a document; eliminate the handoff. Agile teams should include testing and, with the advent of DevOps they include people with knowledge of operations, so handoffs are eliminated.

Before agreeing to create new documentation, I prefer to ask team members these questions: "In 6-12 months will you be prepared to spend several hours updating this document?" and "How will you know when this documentation is out of date?"

If you expected a template, effective ones don't exist. Ultimately the team members need to negotiate amongst themselves with the Product Owner what documents they need, and what the minimum amount is that is required to do the job effectively.

[Lifecycle of a User Story](/blog/lifecycle-of-a-user-story.html)

#### Resources Links:

- [Agile Requirements Documentation – What’s Really Needed?](https://www.ba-cube.com/blog/agile-requirements-documentation-whats-really-needed/)
- [Best Practices for Agile Documentation](https://tdan.com/best-practices-for-agile-documentation/18936)
- [Four goals of Agile documentation: Part one](https://www.thoughtworks.com/insights/blog/four-goals-agile-documentation-part-one) and [Four goals of agile documentation: Part two](https://www.thoughtworks.com/insights/blog/four-goals-agile-documentation-part-two)
- [A Roadmap to Agile Documentation](https://www.infoq.com/articles/roadmap-agile-documentation/)

