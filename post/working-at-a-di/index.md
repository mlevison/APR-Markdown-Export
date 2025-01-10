---
title: "Working at a Distance is Hard"
date: "2007-10-22"
categories: 
  - "software-development"
---

Working at a distance is hard. There is a reason all the Agile methodologies recommend co-location.

**You miss**:

- A sense of presence
- Hallway conversations
- Rich shared environment (whiteboards, flipcharts, …)
- Personal cues – you can’t tell when someone is focused or would welcome interruption.
- It’s very difficult to build trust.
- You don’t share the same hours

_In short, don’t do it._ The best anyone can offer is mitigation strategies.

### **Tools we use**

- **Plane tickets** – this is the most important – you can’t build trust with people you don’t know.
- **Instant Messaging** – requirements: support for multi-user chat with History. History is important so that you can see what was said while you were away from work. We use [Jabber](https://www.jabber.org/) with the [Spark](https://www.igniterealtime.org/projects/spark/index.jsp) as our client.
- **Conference calls**
- **Webex** (NetMeeting, et al) – it can be slow and only person can contribute at a time. Works well for demos but poorly for collaboration. Instead we look at the same web page.
- [**Real VNC**](https://www.realvnc.com/en/) – we’ve adopted it as our pair programming tool. It allows the remote developer to access and use the local machine at the same time as the owner. Weaknesses: needs to punched through your firewall when working from home, and your still transmitting pixels. [Tight VNC](https://www.tightvnc.com/) also has a good reputation.

### **Other tools**

- **GoogleDocs Spreadsheet** – everyone can see and edit the same spreadsheet at the same time over the web.
- [Mind Meister](https://www.mindmeister.com/) - collaborative mind mapping over the web. The free edition allows you to maintain 4 mindmaps at a time.
- [Card Meeting](https://www.cardmeeting.com/) (free for up to four users) - collaborative Index cards for the web. In theory this should great for retrospectives and planning meetings. In fact this never gelled for my team. The cards aren't resizable and we found far too big for what we wanted to write. As a result we had to zoom out to see the all the cards - but then we couldn't see the writing.
- [Open Meeting](https://code.google.com/p/openmeetings/) (free)  Demo Portal: https://inno02.fh-pforzheim.de:8080/xmlcrm/
- GotoMeeting, [Yugma](https://www.yugma.com/) - effectively replacements for Webex. I've not tried them as we already have webex accounts.
- Agile Planner (free)  I’ve only see a short demo – but it looks like a very promising tool.
- [XPlanner](https://xplanner.org/) - some teams love it and others (mine included) don't.
- [Campfire](https://basecamp.com/retired/campfire) (a chat room with support for history. We tried and didn’t like it because it was stuck inside a web page. As a result it didn’t get used).
- [PlanningPoker.com](https://www.planningpoker.com) – supports planning poker (aka wide band Delphi) estimates for distributed teams. _Thanks to Mike Cohn and co at Mountain Goat_
- [TracWiki](https://trac.edgewall.org/wiki/TracWiki) (insert your other favorite wiki)

### **Techniques**

- Post Ground Rules (for Meetings et al) at each location. Check for revisions each sprint.
- Starting and ending iterations mid week:
- Not just for teams working at a distance: Friday afternoons – everyone wants to be home; Monday mornings are very low energy. As a result it's better to avoid both.
- Teams spread across countries also face the problem that each country has different holidays – which for the most part fall on a Monday or Friday.
- Team ambassadors who move between teams
- Coach/Facilitator per meeting location – if each location has more than a few meetings then additional facilitators in each location can help the meetings run more smoothly.
- During Daily Scrum even remote team members should standup – helps keep everyone focused.

These tools and techniques are just a starting point. Please help by adding to the list in the comments. You're also welcome to suggest improvements in grouping etc.
