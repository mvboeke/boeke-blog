---
title: 'Switching from Trello to Clubhouse (instead of Jira)'
description: 'Switching from Trello to Clubhouse (instead of Jira)'
date: 2019-09-17
author: Michael Boeke
tags:
 - Product Managment
layout: layouts/post.njk
icon: random
---

I’ve used a bunch of different agile project management tools throughout my career, and all are a pain in some way. Developers I’ve worked with are usually skeptical of project management tools, so I’m happy to work with whatever my team will actually use. That means I've been using Trello for quite some time. It's simple, fast, and provides just enough structure to organize a weekly sprint of work. It' also includes lots of good features like attachments for mockups, to-do lists, and integrations with dev tools like GitHub and Slack.

However, Trello has some limitations, and the more mature your team, product, and process get, the more difficult it can be to deal with those limitations.

## The Limitations of Trello

### No way to group related story cards
The biggest problem is that Trello only has two main layers of organization: a card that is used to represent a story, and a board that collects those cards into stages. However, there is no good way to tie related cards together as they travel across the board. Trello is missing a layer of abstraction that enables you to create a group of stories in one project or “epic”.

### Nowhere for completed cards to go
Once a card travels across the board and is complete, there is no natural place for it to go. If you let the completed column grow too large, the board gets slow and difficult to work with. If you archive the completed cards, it becomes difficult to access recently completed cards when you need to do things like write release notes. The best option we found was to create a new completed column for each sprint, and then send that column to a board of “completed work” at the end of the sprint. Of course, that would eventually fill up and get slow, and we would archive columns older than a few months.

### No good way to organize future work
You can use a separate board to manage a backlog or create a roadmap. However, in my experience backlog boards get big and performance is an issue for boards with lots of columns and cards. There's no good way to prioritize projects/epics because you can only have story cards. And since cards cannot exist on two boards in Trello, as you work on cards the state of your roadmap deteriorates.

### No way to make changes in bulk
Often, you want to make the same edit to multiple story cards at once. Trello makes this a laborious task since you have to modify each card one-at-a-time.

### Hard to find things
Trello search is pretty good, but it's hard to understand which board a card belongs to from the search results. Also, there are only a few ways to filter which story cards appears on a Trello board.

## Why not Jira?
Jira is the 800lb Gorilla in the agile project management space. Some members of my team (myself included) had experience with Jira from previous jobs. Our memories were not fond. We remembered lots of fiddly configuration and loads of time spent managing the tool.

However, some PMs I respect told me that Atlassian had done much to modernize Jira, so I decided to give it a try. I was very impressed with the reimagined UX, it seemed to fit a lot of our needs and the import tool from Trello was easy to use. So I imported our main development board from Trello and invited some teammates to try it with me. That’s when things started to fall apart.

My teammates started getting bombarded with email notifications that they could not control. As the admin, I could not easily shut off notifications for a particular user either. Instead, I was confronted with a gigantic and byzantine matrix of roles and permissions that looked like it hadn’t been refreshed since 2008. That was the end of the experiment.

![Robust Enterprise Configuration](/img/jira_config.jpeg)

## The Clubhouse approach

Clubhouse offers the best aspects of Trello while addressing its shortcomings and with none of the drawbacks we found in Jira’s “enterprise robustness”.

![Clubhouse](/img/clubhouse.png)

### Easy to group related story cards
Epics are a first-class idea in Clubhouse and enable my team to easily group stories together in a natural way.

### Completed cards are handled automatically
The completed state for story cards is an infinite-scrolling column, divided by week. Recent stories are always in view, and older things can be found by scrolling without making the entire board slow as a three-toed sloth. Older story cards are easily searchable or findable with filters.

### Easily organize future work
Using Epics and Milestones, I can create an agile roadmap for things we expect to build over time horizons longer than a one-week sprint.

### Easily make changes in bulk
Doing maintenance on a large group of cards works just like you'd expect. It's so easy, we can make the changes during a planning meeting without slowing anything down.

### Easy to find things
Search works well in Clubhouse, but it's the logical structure of epics, labels, and milestones that make it easy to find what you're looking for.

In addition to all of the above, Clubhouse has the integrations we want (primarily Github and Slack) and other features we find useful, like labels, time estimates, and story-types (feature, bug, or chore).

### Clubhouse shortcomings?
Not much. Reporting options feel a little under-developed. Also, the story estimates options seem too rigid. We were in the habit of using t-shirt sizes (e.g. S, M, L, XL) but you have to choose a numeric value in Clubhouse. Presumably, that’s to support the progress meters at the Epic and Milestone levels. Clubhouse support for multiple teams isn’t great, but they’re working on it.

After 6+ months of working in Clubhouse, it’s been a great fit for my team. It will be my default choice in the future, especially now that it's free for up to 10 users. That makes it work even for side projects and early stage startups with no budget.