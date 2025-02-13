---
title: "More Notes on Story Splitting"
date: "2010-12-03"
categories: 
  - "agile"
  - "scrum"
tags: 
  - "agile-development"
  - "invest"
  - "sprint-planning"
  - "story-splitting"
  - "user-story"
coverImage: "photodune-8431094-done-text-and-check-mark-xs.jpg"
---

![Done image licensed from Photodune](src/content/blog/more-notes-on-story-splitting/images/photodune-8431094-done-text-and-check-mark-xs.jpg) In response to my recent [Story Splitting post](/blog/story-slicing-how-small-is-enough.html), I had a few questions and couple of confusions that need clearing up.

A few elements of the [INVEST](https://xp123.com/articles/invest-in-good-stories-and-smart-tasks/) criteria need some discussion:

- Negotiable – the details are negotiated with the Product Owner as the team goes to implement the story. However that negotiation is a two street and not an excuse to ask for scope creep.
- Valuable – the story has to be valuable to a User however that may not be enough value to be worth releasing at this moment. Instead it may take several stories together to be sufficient value for the end user. For example if we imagine the login page for a new site that needs to support its own signup system, Facebook, Twitter and OpenID. It may not be worth releasing the page without all the elements yet they still maybe good places to make a split.
- Small – Bill’s original definition says small. I prefer ‘Sized Appropriately’. So things that are to be developed in the near term (perhaps 4-6 sprints) should be broken down into Stories and Estimated. Things that are further out should remain as EPICS.

Should we Slice at all? One person has suggested that if a story doesn’t want to be small then there is no point in breaking down. He went to suggest that Sprints/Iterations are just artificial boundaries. My counter is that even when its difficult splitting stories still gives you several advantages:

- The Product Owner has more opportunities to change direction. With my signup example if supporting their own signup takes too long, the Product Owner may choose to drop the Twitter option.
- More frequent touch points with the Product Owner and Customer allow for better steering of the direction of the team.
- If the company changes direction mid-stream the larger the story the more WIP (work in progress) that needs to be either removed or finished up.
- Smaller stories allow more of them to be “Done” early in the iteration, allowing an earlier handoff to QA for teams that haven’t yet adopted ATDD.
- Large Stories make it easier to get lost in the details and fall down a rabbit hole (ask any of my team members at Databeacon).
- Large Stories make it more likely that we will bottleneck.

Finally I’m always being asked for more Story Splitting Examples. Think back 1995 when Amazon hadn’t launched, we’re developing the site that will become Amazon:

_Original Epic_: “As a first time user I want the to buy a book so that I can read it in my home”

To start let's try splitting on Workflow:

- As a first time I user I want to add a book to my cart so I can buy it.
- As a first time user I want to checkout my cart so I can buy the contents
- As a first time user I want to enter my home address so I can get my book shipped home
- As a first time user I want to see the shipping costs calculated for my home address.
- ….

Maybe for calculating the shipping costs for all 50 states and 10 Canadian provinces is still too big. Then let's split it again. In this case I’m going to assume that shipping costs are the same for certain groups of states/provinces:

- As a first time user I want to see the shipping costs calculated to CA, NV and AZ
- As a first time user I want to see the shipping costs calculated to NY, MA and PA
- As a first time user I want to see the shipping costs calculated to ON, MB, QC

Now a CRUD (Create Update Read Delete):

As a first time Amazon user I want to remember my address so I don’t have to retype it next time I come back

- I want my address saved
- I want to use my address when I next return
- I want to edit my address
- I want to delete out of date addresses

The first one is an example of story that isn’t “valuable” to user by itself. Nonetheless if it’s the only splitting possibility you have that it can still be useful.

Finally when do you stop splitting? At the lower end no smaller than two developers one or two days. Smaller than that and the stories have effectively become tasks. _Update: After discussion with Tobias (see the comments), I think a better statement would be that teams should complete 5-10 stories a sprint. This forces the stories to be small without tying them to days._

Slides from a recent Webinar are [here](/wp-content/uploads/2020/01/User-Story-Splitting-2008-Webinar-slides.pdf) (pdf).

Image via: [https://photodune.net/](https://photodune.net/)
