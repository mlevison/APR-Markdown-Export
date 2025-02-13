---
title: "Scrum by Example - Product Backlog Refinement in Action"
date: "2023-12-12"
categories: 
  - "backlog-refinement"
  - "scrum-by-example"
tags: 
  - "development-team"
  - "product-backlog"
  - "product-backlog-refinement"
  - "product-owner"
  - "scrum-by-example"
  - "scrummaster"
  - "story-points"
  - "user-stories"
coverImage: "AgilePainRelief_BlogIllustrations_Feb2019_ProductBacklogRefinement_B_v1.png"
---

_In Scrum, **Product Backlog Refinement** is an essential meeting of the Product Owner and the Development Team to gain clarity and a shared understanding of what needs to be done through discussion and sharing of ideas. The following is a guide example of how to run an effective Product Backlog Refinement meeting. We know that many people learn more effectively by example, so the story comes first, using our fictional World’s Smallest Online Bookstore (WSOBS) Scrum team. If you’re in a rush and just need a clear definition and facilitation trick, scroll to the end, or review the general information in the framed areas._

**Dramatis Personae:** Steve – a ScrumMaster and the hero of our story Paula – the Product Owner of Steve’s team

Learning from [their recent experience with bad User Stories](/blog/deal-with-bad-scrum-user-stories-as-a-scrummaster.html), ScrumMaster Steve, Product Owner Paula, and the Development Team schedule a Product Backlog Refinement meeting, after lunch,\[[1](#footnotes)\] to refine the User Stories and discuss them ahead of Sprint Planning.

Remember: Scrum doesn’t require User Stories. However, for relatability purposes of this story, we refer to User Story, but you can substitute Product Backlog Item.

![A Product Backlog Refinement meeting is where the Product Owner and the Development Team discuss the items at the top of the Product Backlog.](src/content/blog/scrum-product-backlog-refinement/images/AgilePainRelief_BlogIllustrations_Feb2019_ProductBacklogRefinement_A_v1-1024x607.png)

## What is Product Backlog Refinement

Product Backlog Refinement is a meeting where the Product Owner and the Development Team discuss the items at the top of the Product Backlog. This used to be known as Product Backlog Grooming, but the term ‘grooming’ (to make neat and orderly) has been dropped and replaced with Refinement. The goal of Refinement is to ensure that the Product Backlog is clear and understood by everyone before the Sprint, not just to make it look good.

In Product Backlog Refinement, the entire Scrum Team –Scrum Master, Developers, and Product Owner– work together to review and update Product Backlog Items (PBIs)/User Stories, so they are well-defined and understood by the Team, and properly prioritized. The Product Owner shares relevant information about the product vision from the stakeholder, and the Development Team works with the Product Owner to gain a deeper understanding of why the product feature is needed and what purpose it will serve.

Backlog items are evaluated on their value to the customer, estimated work required, and any dependencies on other product features, then they’re prioritized to deliver the best value to the client every Sprint. Since Product Backlog Items that were completed a previous Sprint are removed from the Product Backlog, there is room for other PBIs to be moved up in priority, or new ones added, as the product evolves, requirements get added, and/or Product Backlog Items are split into more manageable sizes.

Regular Product Backlog Refinement provides an opportunity for both stakeholders and the Scrum team to communicate any necessary changes and be Agile in response. Communication and collaboration ensures that requirements are clearly understood, and expectations are reasonable and achievable. This gives the Scrum Team the information to begin Sprint Planning and the detail they need to effectively execute their Sprint.

By continuously updating and refining the Product Backlog, the Scrum Team always has a sufficient number or prepared Backlog Items and never has to wonder what needs to be done, or what to do next. This enables them to be truly self-organizing and effective in Scrum.

## Getting Ready for Product Backlog Refinement

To prepare for the Product Backlog Refinement event, Product Owner Paula doesn’t use a formal meeting agenda; instead, she has a rough checklist that she shares with the Team:

- Story stubs\[[2](#footnotes)\] or ideas that were initially written by herself, to be rewritten into effective User Stories through discussion with the Team
- [Acceptance Criteria](/blog/definition-of-done-user-stories-acceptance-criteria.html) for topmost items in the Product Backlog
- [Split User Stories](/blog/story-slicing-how-small-is-enough.html) that are too large for their current position in the Product Backlog
- Estimate\[[3](#footnotes)\] Split Stories
- Acceptance Criteria for newly created Stories
- Estimate Stories that don’t yet have estimates
- Create New Stories based on newly identified Stakeholder needs

## Backlog Refinement Is All About Discussion and Asking Questions

![Backlog Refinement Meeting Agenda in Action](src/content/blog/scrum-product-backlog-refinement/images/AgilePainRelief_BlogIllustrations_Feb2019_ProductBacklogRefinement_B_v1-1024x607.png) Paula and the Team review the current list of items in the Product Backlog. They clarify the User Stories by discussing the context for a desired product feature and what kind of value it is meant to give the user. Taking the time to discuss each User Story solves [the earlier problem of bad User Stories](/blog/deal-with-bad-scrum-user-stories-as-a-scrummaster.html) which lacked a clear ‘Why’ statement. It also gives the whole Scrum Team the needed context and clarity to provide useful estimates. ScrumMaster Steve’s guidance toward having this backlog refinement session, instead of blindly launching into Sprint Planning, has been a huge help.

The topmost items are estimated by the Developers and split into a digestible size (i.e. small or 1, 2, or 3 Story Points). In addition, they have at least two or three Acceptance Criteria associated with them.

In order for a User Story to be useful, it must also be specific and focused. Let’s see where this was a problem during this Product Backlog Refinement session, and how the WSOBS team handled it.

About a third of the way down in the Product Backlog there is a Story: “As a Julia\[[4](#footnotes)\] (a Real Estate Agent and Frequent book buyer), I want to be able to buy a gift card to thank a fantastic recent client.” The estimate on this one is 20, so it’s agreed that they need to split this User Story.

As the Scrum Team discusses the Story, they ask Paula several questions for clarification:

- How will the recipient redeem the gift card? _Paula says: it’s already covered in a later story, which is also estimated to be 20._
- Will the gift card be printable or just electronic? _Paula: Electronic for now._
- Does the Story include delivering the Gift Card?  _Paula: Yes, by email._
- Are fancy graphics and clever messaging important? _Paula: Yes, but in the first version, it would be okay to do without them._
- What gift card amounts are supported? _Paula: $10, $25, $50 and $100._
- Are gift cards refillable, or one-time use? _Undecided._

From this discussion, they create some new Stories and estimate them:

- As a Julia, I want to be able to buy a $10 gift card so that I can thank a fantastic client. Limitation - not delivered just generated – Estimate: 5 points
- As a Julia, I want my newly purchased gift card sent by email to its recipient so that they can use it immediately. – Estimate: 13 points
- As a Julia, I want to be able to refill a gift card I previously purchased. – Estimate: 8 points
- As a Julia, I want to be able to buy a gift card in denominations of $25, $50, and $100 so that I have choices in how much money I want to spend. – Estimate: 13 points
- As a Julia, I want fancy graphics and text on my gift card to satisfy my inner diva. – Estimate: 8 points

On seeing that refillable gift cards will cost 8 Story Points, Paula says, “That’s expensive for the value I get,” and pushes it down in priority. She also sees that the combined cost of the $10 gift card Story and the alternative denominations gift card Story is 18 Story Points – quite large. She asks the Team if it would be cheaper to do gift cards with any amount. They come back with an estimate of 8, pointing out that it’s still more complex than the basic Story.

They create a new Story, sized 8, and move onto establishing some basic acceptance criteria:

Basic “Buy Gift Card” Story

- Price Range $5 - 100
- Tax not charged to gift card buyer
- Receipt displayed
- Gift card displayed in buyer’s order history

Basic “Send Gift Card” Story

- Get a friend’s email address
- Assume valid email and don’t do checking - will be handled later
- Send Gift Card via email
- Text-only gift card

“Fancy Text and Graphics” Story

- Looks good in the browser when the buyer sees it
- Looks the same in: Outlook, Gmail, Hotmail, iPad, iPhone, Android phone

All of this discussion leads Paula to realize that being able to use a gift card is as important as buying one. As a result, the Team repeats the whole exercise for the Story to “Use a gift card.”

They wrap up the session by discussing the needs of new publishers who Paula is talking to about selling their products through the bookstore. They outline the rough idea of some Stories to support this need but don’t bother estimating them, as the talks with the publisher are still in their early stages. They can expand and refine them in a future Product Backlog Refinement session if the need arises, rather than spending time unnecessarily speculating now.

## Why Hold Product Backlog Refinement?

Every Sprint, the Team finish a number of User Stories, which means the top of the Product Backlog will have some empty space. So we hold refinement to fill those spaces. Either we move older User Stories up the queue, or we create new User Stories.

The leading cause of poor Sprint Planning –and, therefore, crappy Sprints–  is the team members not understanding the User Stories they’re working on. So we invite all team members to refinement to create a common understanding about what each User Story is.

## When Does Product Backlog Refinement Happen, and How Often Is It Done?

Spread the work throughout the Sprint. No one wants to attend a 2-3 hour meeting in one sitting, so break the event down in two or three sessions of about 45-60 minutes each. I’ve found it effective to schedule a session during the first week of the Sprint and a second one early in the next week. If a third session is required, we still have [time left in the Sprint](/blog/choosing-scrum-sprint-length.html) to run it.

Have frequent and regular Product Backlog Refinement sessions. Making it part of the normal and expected routine reinforces the understanding that reviewing and updating the Product Backlog isn’t a once-and-done thing, it’s an ongoing part of the process.

## Tips for an Effective Product Backlog Refinement Meeting

- Start at the top of the Product Backlog and work down in priority. This ensures that when you run out of time, the most important items will already have been estimated.
- I recommend teams have two to three Sprint’s worth of work that are well-refined. This way the team members always know what is coming up next and there are fewer surprises.
- Some teams establish an agenda of product areas to be addressed in a session. This allows everyone to spend time thinking about that part of the product. In addition, it gives the Product Owner the opportunity to invite relevant outside experts.
- Ask the Team which items are the least clear and address those first.
- The Product Owner should not pre-write User Stories. Instead, they should be created collaboratively with the Team.
- For every item:
    - Read the User Story and associated Acceptance Criteria (if they exist). Have a short, timeboxed discussion to clarify what it represents. If the discussion reveals anything new, either create Acceptance Criteria to document or rewrite the User Story to account for it.
    - Estimate the User Story – some teams use Planning Poker and Story Points. Others just use T-shirt Sizing – S, M, L, XL. _If I coach your team, I would recommend the latter._
    - If the User Story isn’t digestible, then we split the Story into smaller parts.
    - After the Story is split, it will need to be re-estimated.
    - For items at the top of the Product Backlog, the team should create Acceptance Criteria.

## How to Help Your Scrum Team Be Great(er)

Product Backlog Refinement is intended to help your team clearly understand the Product Backlog and the User Stories in it. To ensure you will always have a successful meeting, there are three outcomes I suggest that Scrum Teams aim for:

1. **Greater Understanding** – Merely telling people you want something built will likely result in you not getting what you envision. Instead, start with a collaborative mindset that is focused on engaging the whole Scrum Team – Scrum Master, Product Owner, and Developers – and refining the User Stories based on a shared understanding of what function they are meant to deliver, who it’s meant to help, and why it’s important.
2. **Greater Conscious Engagement** – When you’re involved in creating a User Story, you get to feel a sense of ownership of the product. As a result, you are much more likely to be motivated to engage in getting the product backlog item to truly “done.”
3. **Greater Subconscious Engagement** – Our subconscious does an excellent job of generating connections and seeing relationships between things. However, it works on its own schedule, often slowly. Ideally, you should have a few days separating Backlog Refinement and Sprint Planning, allowing everyone to see the User Stories several times (perhaps on a big whiteboard at the front of the room) before Sprint Planning, giving everyone’s brain time to make connections between seeing the Story and then trying to plan for it.

**Product Backlog Refinement is a vital part of Scrum.**

**It increases the effectiveness and communication of the entire Scrum Team and, as a result, builds a better product for your client.**

_**[Scrum by Example](/blog/category/scrum-by-example) is a narrative-style blog series designed to help people new to Scrum, especially new ScrumMasters. If you are new to the series, we recommend you [check out the introduction](/blog/scrum-by-example.html) to learn more about the series and discover other helpful articles.**_

### Do you want to coach your team towards better solutions?

The WorldsSmallestOnlineBookStore.com Team went from [facing ineffective User Stories](/blog/deal-with-bad-scrum-user-stories-as-a-scrummaster.html), to having a productive Backlog Refinement session and a clear path for the next Sprint. This was largely due to ScrumMaster Steve identifying the challenge and coaching everyone toward a solution that they could apply collaboratively, which improved communication between Product Owner Paula and the Team. If you would like to learn how to handle some of these common, real-life issues that organizations face in their Scrum evolution, [consider attending one of our workshops](/certified-scrum-agile-training), where you’ll receive hands-on learning of the challenges – and solutions – and tips on how to integrate them into your Scrum.

\[1\] Many developers complain that Backlog Refinement interrupts them doing valuable work. We sidestep that problem if scheduled right after lunch or at some other time when they’ve already been interrupted. Key point: decide the time with the team. \[2\] Mark’s note: It is strongly recommended that the Product Owner not show up at Product Backlog Refinement with prepared User Stories. My personal experience is that team members see these items as complete/correct and it kills further discussion on them. It’s much better to bring rough ideas to the session and work with the team to make them real User Stories. \[3\] Caveat: Scrum works perfectly well in an environment where the Development Team doesn’t estimate – in that case, they can skip the estimation portion of refinement. You would also expect a Team that wasn’t estimating to put more effort into splitting Items at the top of the Product Backlog so that they’re approximately the same size. \[4\] In order to better understand different kinds of end users, those working on WorldsSmallestOnlineBookStore.com have started using Personas to give a richer description of each. In this case, the relevant persona is known by the name  “Julia.” Two things matter in this context: she is a frequent book buyer and user of the site, and she gives her real estate clients gift cards to thank them for their business.

Image attribution: Agile Pain Relief Consulting (Updated: December 2023)
