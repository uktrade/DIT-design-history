---
title: Differentiating between synced and manually added data
description: Making it clear to users when data is read-only so they don't attempt to edit.
author: Jacqueline D'Alcorn
date: 2022-05-06
tags:
  - Synced data
  - Interactions
  - Read-only data
---

## Why we were looking to make changes
This work was done alongside syncing event data from Aventri. The technical solution for this, to prevent duplicate data across systems, was to have read-only content in Datahub. Previously, events and attendees had been manually added to Datahub and were editable. Therefore, we needed to make it clear to users they couldn't edit the synced data and that if they needed to make changes they needed to go to Aventri to do that.

## Changes that were made
### 1. Differentiating between interactions with more data
Interactions created within Datahub have a page that displays all the details about that interaction. That page is linked to from whereever a preview of the interaction is shown, for example on the Contact or Company activity feed.

When we first start to sync data from Aventri we will not have any additional information than what is shown in the preview, so we do not need an additional page. Therefore, the interaction preview would not have a link on the heading and this would need to be clear to users so they do not attempt to click on the heading and think it isn't working. To make this differentiation the interaction preview heading was changed black instead of blue.

![screenshot of heading without a link](interaction--nolink.png)

### 2. Notifing users that data is not editable
In places where users can normally edit data it was important to make it clear that users could not edit the data and to inform them of how to do this. There were several places this affected.

* On the event details page
* On the interaction page for a contact's attendance

Previously there has always been an 'edit' button on these records, but as it is synced data this is not possible. On these pages a notification banner has been added to the header to inform users that the data is synced and not editable. It also tells users how to edit the data if they needed to (by returning to Aventri). This notification banner follows the same pattern as other places in Datahub, for example the notification for archived data.  

![screenshot of interaction details page which has read-only content](interaction-details--read-only.png)

![screenshot of event details page which has read-only content](event-details--read-only.png)
