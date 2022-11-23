---
title: Events – Multiple contacts from the same company
description: Combining interactions when there are multiple contacts associated with an event.
author: Jacqueline D'Alcorn
date: 2022-09-10
service: Data Hub
epic: Event data
tag:
  - Company record
  - Interactions
related:
  title: Related links
  items:
  - text: Design
    href: https://trade.invisionapp.com/prototype/DIT-events-attendees-cl155odxt00172z01d1b7i23m/play/600e69f9
---

***
## Why we were looking to make changes
We set up a test group of users who were given access to the changes we had made for syncing data from Aventri. Features were released as they were built, before they were released to everyone so we could get feedback on them and make changes.

After releasing the initial synced data, [outlined in this post](/data-hub/syncing-event-data/), we received feedback about the Company Activity feed becoming quite cluttered with event interactions. There was an interaction shown for each contact who registered for each event.

***
## Designs
A design was created so only one interaction is shown per event. Any contacts who registered for that event are shown within that interaction.

Contacts can have different attendance statuses, such as registered, attended, did not attend and cancelled. The contacts are grouped under each of these statuses. If there is more than one status for the contacts, the title of the interaction takes the most 'positive' one, for example if one contact attended and one cancelled the title would show as attended.  

When there are more than 6 contacts who registered for the event an accordion is used so the interaction doesn't become too long.

![screenshot of displaying multiple contacts on a single interaction on the company activity feed](Phase1--Company--multiple-attendees.png)

***
