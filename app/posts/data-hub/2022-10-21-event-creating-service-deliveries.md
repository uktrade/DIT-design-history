---
title: Events – Creating Service Deliveries for event attendance
description: When syncing data from another system to Data Hub there is not always a unique identifier to tie the data together with a record
author: Jacqueline D'Alcorn
date: 2022-10-21
service: Data Hub
epic: Event data
tag:
  - Service Deliveries
  - Synced data

---

***
## Why we were looking to make changes
When pulling data from Aventri into Data Hub we needed to tie the data from Aventri to a record in Data Hub. The most suitable identifier that was captured on all event registration forms was email address. This worked well in most cases, but there were some cases when a matching record could not be found:

* The email address the person registered with was not the same as the one stored in Data Hub
* There was a typo in the email address
* Multiple contacts in Data Hub had the same email address stored e.g. if they used something general like info@example.com
* The person did not exist as a contact in Data Hub

In these cases the system could not automatically tie the data and record together so we needed to think of other ways to do that.

It was important to tie together the data with a Data Hub record because it is used for reporting. The reporting requires a contact record to be in Data Hub with a Service Delivery (a type of interaction) saved against the record.








## Changes that were made
### 1. Differentiating between interactions with more data
Interactions created within Data Hub have a page that displays all the details about that interaction. That page is linked to from whereever a preview of the interaction is shown, for example on the Contact or Company activity feed.

When we first start to sync data from Aventri we will not have any additional information than what is shown in the preview, so we do not need an additional page. Therefore, the interaction preview would not have a link on the heading and this would need to be clear to users so they do not attempt to click on the heading and think it isn't working. To make this differentiation the interaction preview heading was black instead of blue.

![screenshot of heading without a link](interaction--nolink.png)

### 2. Notifing users that data is not editable
In places where users can normally edit data it was important to make it clear that users could not edit the data and to inform them of how to do this. There were several places this affected.

* On the event details page
* On the interaction page for a contact's attendance

Previously there has always been an 'edit' button on these records, but as it is synced data this is not possible. On these pages a notification banner has been added to the header to inform users that the data is synced and not editable. It also tells users how to edit the data if they needed to (by returning to Aventri). This notification banner follows the same pattern as other places in Data Hub, for example the notification for archived data.

![screenshot of interaction details page which has read-only content](interaction-details--read-only.png)

![screenshot of event details page which has read-only content](event-details--read-only.png)

***
