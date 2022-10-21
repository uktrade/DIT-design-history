---
title: Events – Preventing users manually adding synced events
description: Making sure duplicate events are not added to Data Hub after they are synced from Aventri.
author: Jacqueline D'Alcorn
date: 2022-10-01
service: Data Hub
epic: Event data
tag:
  - Manually added events
  - Preventing duplicates
related:
  title: Related links
  items:
  - text: Prototype
    href: https://trade.invisionapp.com/prototype/DIT-add-event-cl6297inv012rn0018m1xtuu4/play/fd2b5ead
  - text: Flow diagram
    href: https://trade.invisionapp.com/prototype/DIT-add-event-cl6297inv012rn0018m1xtuu4/play/a88c0e8d
---

***
## Why we were looking to make changes
Once Aventri data is added to Data Hub users will no longer need to manually add those events. Some users are used to doing this so we want to ensure duplicates are not created, at least until users get used to the new process.

***
## Design
An additional question was added in front of the add event form to check with users if the event uses Aventri. If they select 'Yes' a message appears to tell them they don't need to manually add it and leads them to the Event collection search page, so they can find the event. If they select 'No' they proceed to the existing add event form.

##### Diagram showing the new flow after pressing the 'Add event' button

![Diagram showing the new flow after pressing the 'Add event' button](Add-event--Flow-diagram.png)

##### The question added to the add event flow

![Screenshot of the question added to the add event flow](Add-event--stopper-question.png)

## Monitoring usage
After this goes live we will monitor how often 'Yes' is selected. If it is a very low percentage or if usage drops significantly over time this question could be removed.

***
