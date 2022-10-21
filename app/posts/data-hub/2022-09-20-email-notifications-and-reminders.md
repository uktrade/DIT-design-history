---
title: Email notifications and reminders
description: Reminding users about investment projects' estimated land dates and investment projects with no recent interaction.
author: Caner Uzun
date: 2022-09-20
service: Data Hub
epic: Notifications
tag:
  - Email
  - Reminders
  - Investment projects
  - Estimated land dates
  - Interactions
---

***
## Why we were looking to make changes
Users have outlined in previous research that Data Hub doesn't remind them of important deadlines as opposed to this is something they expect a CRM to do. They expressed interest in features to help them do this, such as notifications and reminders.

Getting reminded about investment projects' estimated land dates and investment projects with no recent interaction were some of the most popular answers when users were asked what sort of events they'd like to get notified about. Therefore, we focused on these two notification types for a start.

Users mentioned that it would be helpful receiving reminders for estimated land dates as it's easy to miss when processing data cuts at the beginning of the month that covers the previous month. They also mentioned that they aren't always aware that a project has had no interactions and they often rely on individually looking at their investment projects on Data Hub to update their spreadsheets.

Users also expected to be able to choose how and when they receive notifications for different sorts of notifications.

***
## Changes that were made
After understanding the notification types users expected to see and how they'd expect them to work for them, we designed a user flow that involved both a space within Data Hub allowing users to see a list of notifications and an automated email subscription system. Following discussions within the team, the user flow ended up as low-fidelity designs that were ready to be tested with users.

After two rounds of user interviews and additional surveys, we decided to build reminder pages that are dedicated to one reminder type only. This would give users full visibility of notifications they are subscribed to.

As another way of notifying users, we enabled email notifications to be sent at the time users have set for themselves.

We also created a settings page that allows users to choose a notification type and turn reminders and emails off or on. They can also change the timeframe for when they want to get the reminders (before/after a certain event).

### 1. Reminders section on homepage
We listed two new and one existing -"Outstanding Propositions"- reminder type within the Reminders section on the homepage. We added a number of undeleted reminders next to reminder types in brackets. We also implemented a link for the settings page.

### 2. Reminders list
We listed all reminders that are relevant to the user underneath a search results bar that indicates number of reminders waiting to be reviewed by the user. We also added a settings page link to make it easily available to the user in different parts of the journey.

### 3. Reminders settings  
We asked users whether they'd like to get reminders for projects with approaching estimated land dates and for projects with no recent interaction. If users answered 'Yes', we asked them when they'd like to get the reminders. Based on their answer, we revealed a final question that asks whether they'd want to get emails at the same time as reminders.

***
## Screenshots

![screenshot of reminders section on the homepage](Reminders-section-on-the-homepage.png)

![screenshot of reminders page for projects with approaching estimated land dates](Reminders-for-approaching-estimated-land-dates.png)

![screenshot of reminders page for projects with no recent interaction](Reminders-for-projects-with-no-recent-interaction.png)

![screenshot of reminders and email notifications settings page with first accordion expanded](Reminders-and-email-notifications-settings-first-accordion-expanded.png)

![screenshot of reminders and email notifications settings page with second accordion expanded](Reminders-and-email-notifications-settings-second-accordion-expanded.png)

![screenshot of settings page for approaching estimated land dates](Settings-for-approaching-estimated-land-dates.png)

![screenshot of settings page for projects with no recent interaction](Settings-for-projects-with-no-recent-interaction.png)

***
