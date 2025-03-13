---
title: "Kanban Portfolio View"
date: "2024-12-18"
categories: 
  - "beyond-scrum"
  - "kanban"
  - "organizational-improvement"
  - "portfolio-management"
  - "scrum"
coverImage: "scrum-alone-not-enough-kanban.jpg"
excerpt: '_(Presented as Part 3 in the [Scrum Alone is Not'
---

![Beyond Scrum: Scrum Alone Is Not Enough - portfolio kanban](src/content/blog/kanban-portfolio-view/images/scrum-alone-not-enough-kanban.jpg)

_(Presented as Part 3 in the [Scrum Alone is Not Enough](/blog/scrum-alone-is-not-enough "Scrum Alone is Not Enough") series.)_

In the last post of this series I talked about [Portfolio Management](/blog/portfolio-management), and how it aims to ensure that a team is always working on the highest priority work, without outside pressure taking their focus away from a manageable goal. Portfolio Management has value, but it also comes at the cost of increased overhead, loss of some control for Product Owners, and reduced ability to adapt in the moment, so let’s use it wisely.

## Focus on Delivering Value, Not on Keeping Teams Busy

**1\. The most important advice for Portfolio Management is to structure stable teams to minimize dependencies out of the gate, or at least cross-skill to reduce them.** If we need red yarn\[[1](#footnotes)\] to visualize dependencies (thanks, SAFe), we must fix the underlying problem, not mask it.

**2\. Watch the work items, not the workers.** Our job is to deliver value, not keep people busy. Prioritize finishing work items, not starting more work.

**3\. Make your Product Portfolio visible.** When teams see the work, they deliver more value. We're visualizing the Portfolio so that we can see: - Where the work items (e.g. Features/Epics/Large PBIs) are in their journey - Where work is getting stuck (Is it waiting for other teams? Approval? ...) - Dependencies between teams - The flow of work from beginning to end

To make the Product Portfolio visible, we use a **Product Portfolio Board. You can use any board to visualize but, in most cases, a Kanban Board is the best to start.**

Why do we need a board? Simple, it helps everyone make better decisions about the work, so we're always maximizing value. How do we do this? Design the board by asking what information they need to make better decisions.

_In most organizations, work items spend more time waiting than getting done. Often three times more. If you want to deliver value faster, eliminate the waiting._

## Basic Portfolio Kanban Board

Let's start simple. Gather your team and map out how work flows through your organization. Think big chunks of work (about a week's worth), not tiny details.

The details: gather the Product Owner(s), ScrumMaster(s), Team Members and Stakeholders. If the group size is large, either do the work in two rounds or invite-only a couple of representatives from each group. You can do this with the formality of [value stream mapping](https://en.wikipedia.org/w/index.php?title=Value-stream_mapping), or write down an ordered list of the steps. Each step is a possible column on the board. Since we're creating a portfolio view, the minutia of what happens inside a single development team will be a distraction. Consider tracking work at the Feature/Epic level (~1 week's work for each team; T-shirt sizing L/XL; Story Points 13/20/...). Any more fine-grained, and the level of detail will be overwhelming.

I've seen a simple board like the one pictured below work well. Your board will be different; don't copy ours.

![](src/content/blog/kanban-portfolio-view/images/Kanban-Portfolio-View-2024-Basic2-1024x592.jpg)

With the basic board in place, consider how to visualize the problem children of the kanban board. I'll explain below.

### Visualizing the Challenges

Here are the prime offenders on your Product Portfolio board:

**\- Dependencies** (the domino effect) - use colour or tags to visualize these. I like the use of colour because they stand out. Items with dependencies are the ones that are likely to get stuck in the system. To avoid this, ensure that attention is given to dependencies.

**\- Waiting For** (the silent killer) - Sometimes work waits for the next station to pick it up. Consider a separate column. In most teams, work spends more time waiting than it does being worked on. So use a WIP Limit. Once we have too many items waiting, the team should collaborate to help the people at the station get all of the items closer to the finished state. _If we have downstream teams, there will be a waiting-for queue ahead of each downstream team. It also needs a WIP limit._ 

**\- Blocked** (the full stop) - "Waiting for" was bad enough. Blocked is worse. Blocked implies that until something happens, the item will not proceed. Mark these in any way that they stand out.

**\- Work Item Age** (the forgotten items) - A fancy name for the question: how old is this item? Track how long it has been since work started on an item. As items age, there is an increased chance that they're no longer relevant to the system. Item Age also correlates with customer dissatisfaction and defects. Also, older items often have hidden dependencies or blockages that stop them from getting finished.

## Reviewing and Using the Kanban Board

Product Owners, Scrum Masters and representative team members should review the state of the board a couple of times a week.

**\-** Review each item on the board. Is it in the right column (e.g. Considered, Development, Testing, Deployment)?

**\-** Review the whole board, looking for any items that might have a newly discovered dependency or are now blocked when they weren't previously.

**\-** With dependencies and blocked items, determine who will do the dependent work or resolve the blockage. Dependencies and blocked items are significant inhibitors of delivering value, so teams must treat the dependency as a higher priority than their own Sprint work. In a multi-team situation, all teams must set aside 10-15% of their capacity to help other teams. When this doesn't happen, the system will jam up more often.

**\-** Now review Work Item Age. Value is only delivered to the customer when work is truly finished. For the oldest items, check first for unnoticed dependencies or blockages. Then, teams should prioritize finishing these items before starting new work.

Stakeholders review the board with the Product Owner less frequently. Every 2-4 weeks. We're still keeping the stakeholders in the loop. By the time the Portfolio Management meeting arrives, they already know what is complete. They will have more focused, better-quality feedback on the product and its evolution. In addition, whenever there is a blockage that a stakeholder can help with, bring them to the board and discuss the issue.

### Resolve Dependencies

Don't manage them, especially not with red yarn. If there are frequent dependencies between two teams, this suggests a structural problem. Either change the team structure so the dependency is no longer a problem or cross-skill the team to handle the dependency without outside help.

During your multi-team retrospective (you're doing them, right?), discuss the use of the board and how to make better use of what it tells us and how to improve it.

If the conversation gets stuck, return to the board's purpose: Value Delivery over Keeping Teams Busy. Ask questions like: Where do items get stuck the most often? Which dependency can we untangle next? Are there any decision-making bottlenecks to eliminate?

### Don’t Self-Sabotage

Want to guarantee failure? Here's your recipe:

\- Put on blinders - ignore other teams' needs - Play hot potato with decisions - toss them upstairs - Start new stuff - because fixing problems is hard work

_I wish this was sarcasm. But I've seen so many teams behave this way, I have to assume there is an instruction manual that advocates this._

\[1\] [https://scaledagile.com/blog/safe-program-dependency-board-retrospective/](https://scaledagile.com/blog/safe-program-dependency-board-retrospective/)

Updated on December 18, 2024

Image attribution: Agile Pain Relief Consulting unless otherwise noted. Elements of first image [designed by Freepik](https://www.freepik.com/).
