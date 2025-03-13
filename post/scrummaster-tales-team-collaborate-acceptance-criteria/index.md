---
title: "Scrum By Example - The Team Collaborate on Acceptance Criteria"
date: "2013-02-05"
categories: 
  - "product-acceptance-criteria"
  - "scrum-by-example"
  - "sprint"
  - "user-stories"
tags: 
  - "acceptance-criteria"
  - "sprint-planning"
  - "user-stories"
coverImage: "photodune-352256-group-of-people-xs.jpg"
excerpt: 'The team has just completed [Sprint'
---

![Group of people - licensed from Photodune](src/content/blog/scrummaster-tales-team-collaborate-acceptance-criteria/images/photodune-352256-group-of-people-xs.jpg)

The team has just completed [Sprint Planning](/blog/creating-acceptance-criteria-waiting-too-long), committing to four stories:

- As a first time book buyer I would like to read a review so I can see if a book is worth reading.
    - A review has text and isn’t empty
    - A review has an author name
    - A review has a title
    - At most a review is 2500 characters long

- As a first time book buyer I would like to see a star rating associated with a review so I can quickly assess if the book is even worth thinking about.
    - Rating from 0 to 5
    - No ½ stars
    - Rating appears at the top of the review

- As a first time book buyer I would like to see reviews by staff members marked separately so that I know whom to trust.
    - The word “Staff” appears in bold before the reviewer’s name
    - All reviews posted from computers inside the Smallestonlinebookstore offices will be considered staff reviews _(This avoids having to tag users as having different roles for now)._

- As a first time book buyer I would like to see reviews by friends highlighted so that I know whom to trust.
    - …

Right after Sprint Planning, Kirby decides he wants to take: “_As a first time book buyer I would like to read a review so I can see if a book is worth reading._” He invited Brad and Tonia to sit down with him and create some examples that illustrated the acceptance criteria to make sure they were completely fleshed out:

- A review has text and isn’t empty
- At most a review is 2500 characters long
- A review has an author name:
    - “Mark Levison” – valid
    - “mlevison” – invalid –  not a proper name
    - “Levison” – invalid – we need at least two names
    - “C. J.” – invalid – initials alone aren’t enough
    - “John C. King” – valid
    - “J C King” – valid
    - “J. C. King” - valid
    - A review has a title

After 30 minutes they think they’ve fleshed out most of the edge cases, and Kirby invites Brad to pair with him as they start writing the first tests. Brad is skeptical, saying, “I’m a BA – how can I contribute while you write code?” Kirby persists, saying, “Let’s just try it for an hour.” Kirby makes a real effort to name the tests to describe the behavior he’s looking to build.

Sample Tests (Java pseudo code):

`@Test public void simpleTwoPartName() {…} // Mark Levison @Test public void oneNameAreNotEnough() {…}  // Levison @Test public void initialsAloneAreNotEnough() {…} // J. C. @Test public void initialsAndLastName() {…} // J. C. King`

While he’s struggling to read the implementation code for now, Brad discovers it’s very easy to read the test code. In addition, his questions help Kirby to better name the domain objects because they’re forced to make sense to a non-technical person.

Kirby checks in as soon as the first part of the review system is completed – in this case just the business logic to process and store a review. That happens before reviews can be entered via the GUI, let alone be displayed with books.

The next day Kirby pairs with Ian as well and drives out the GUI for the story. However, they’re having a lot of trouble with trying to spot the difference between real names and user ID’s, i.e. “Mark Levison” vs. mlevison. Rather than get hung up, he shows Tonia (the World’s Best Tester) what he’s got working so far and asks her to give that a test. While she is open to the idea, she’s still dealing with testing Stories that weren’t tested in the last Sprint. So Kirby asks Martin (Database Guru) if he can pitch in. Martin protests that he has no testing experience. Kirby explains that a rough and ready test by another person is better than waiting. He points out that Tonia will still test the Story; he just wants early feedback. Martin downloads the application from the CI server and fires it up. He remembers hearing about buffer overflow attacks. He tries pasting in over 10,000 characters of text into the review text box. The app crashes. For his next act he tries pasting in all the [Unicode Symbols](https://en.wikipedia.org/wiki/Unicode_symbols) into the review text box. Another crash. He shows Kirby, who laughs and then duplicates the tests and subsequent failures on his own machine. Before trying to solve the two problems Kirby writes two failing Unit Tests. Now he sets about solving the problems. Within half an hour he’s fixed both problems.

## Analysis

This time the team is doing better than it has in the past without anyone’s help. Here’s what I see going well:

- Working with a minimum of three people to ensure that the acceptance criteria are well understood.
- Team members pairing to do the work.
- Brad, the Business Analyst, being open to pairing to write test drive code.
- Martin being open to trying Exploratory Testing.
- When testing, Martin didn’t rely on the code from his machine. By testing with a build from the CI server he ensured that he was testing Kirby’s work, and not his own code.

What seems odd:

- Tonia is testing Stories from the previous Sprint and yet the team has claimed they’re complete.
- Stories are being written to enter reviews before the reviews can be displayed with a book. That seems odd. It would be better to display the book reviews first. After all, we can add reviews to the system in any number of ways; directly in the database, through an API, etc. These options don’t require a GUI. However the reviews are useless if we can’t show them to the customer.

What do you find odd? What do you take away from the team’s experience this week?

_**[Scrum by Example](/blog/category/scrum-by-example) is a narrative-style blog series designed to help people new to Scrum, especially new ScrumMasters. If you are new to the series, we recommend you [check out the introduction](/blog/scrum-by-example) to learn more about the series and discover other helpful articles.**_

Image Credit: Photodune
