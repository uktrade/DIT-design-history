---
title: Events – Syncing event data
description: Providing a fuller picture of events, registrants and attendees by syncing data rather than relying on manual entry.
author: Jacqueline D'Alcorn
date: 2022-05-09
service: Data Hub
epic: Event data
tag:
  - Events
  - Syncing data
related:
  title: Related links
  items:
  - text: Roadmap
    href: https://trade.invisionapp.com/freehand/Roadmap-of-Event-sync-f12Fy8ipu
  - text: Hypotheses and problem areas
    href: https://docs.google.com/presentation/d/1vOg9JoFQfsK20mPCqMTGSVw6SrRgvXggmD33ZgNUYeg/edit#slide=id.g11409d3f6c2_1_0
  - text: Adding attendees – Existing manual flow
    href: https://docs.google.com/drawings/d/1k-5V9eQ9qswaAK5AYrqRcoZiL3NsvtGiR5c0eE0no8Y
  - text: User needs and journeys – event data
    href: https://docs.google.com/drawings/d/13S7qMo2JJ3jxnYU55Cwvlq4bIVHsLCGxE6nep4uuifE
  - text: User needs and journeys – reporting
    href: https://docs.google.com/drawings/d/1d2erkuN-51jF-zjXh9av97enqTFAuHqQI4hVWUBIC7k
  - text: User research handover
    href: https://docs.google.com/document/d/1dHod-GLdAzInVvCoh8ukyY_zYCP9OXf2NDVtNYz7Ao0/edit#
---

***
Please note: this is long-term ongoing piece of work with multiple phases. See the roadmap in the related links. This post summarises getting to the stage of understanding why and what we needed to do. Other posts will go into the detail of changes made.

## Why we were looking to make changes
1. Users had to manually enter data into Data Hub, which was a lengthy process
2. Sometimes manual entry was outsourced, which had cost implications
3. Data was not added to Data Hub for all events (only 15% of Aventri events were manually added to Data Hub)
4. There was no set process around what data to enter, particularly around registrations vs attendees and funding applications
5. Data that was entered did not get entered in a consistent format
6. Missing data made it hard to run accurate reports
7. Missing data meant advisers and staff dealing with a company were missing useful information and context that would help with their conversations and help them give more tailored advice.

### User problems
We ran 10 research sessions with users in various roles. These sessions covered why, when and what event infomation was added to Data Hub, the process used to add the data and what it was used for. From these sessions we discovered:

* Users were spending vast amounts time manually adding event data
* This was taking time away from organising and running the events
* Adding new contacts took even longer, as users had to find the correct company to link a contact too. This was challenging as they only had limited information about the company. The challenge was increased by duplicate company records.
* Aventri is used for collecting data about things wider than events and there is not a place to easily record that data Data Hub

> I can process these at about 30 an hour and that is fast because I’ve mastered it. But when you’ve got hundreds and hundreds a week it can take a lot of time.

> This takes ages, it’s such a big part of my job. It’s such a catch 22 because if we do well in our job it means that I have to spend a lot of time getting this onto Data Hub which takes time away from promoting the events and doing my actual job.

***
## Changes made in the initial phase
### 1. Syncing event details
Details about the event such as name, date and location are synced. This means users do not need to manually create the event in Data Hub.

### 2. Syncing details of contacts who register for Aventri events
Every person who registers for the event is synced to Data Hub.

For those who are existing contacts in Data Hub (and can be matched using email address) the event registration is recorded against their record and their company.

For those who are NOT existing contacts in Data Hub their registration can only be seen when viewing the event record.

### 3. Showing attendance information, if it is recorded
Currently, attendance data is not available for all events in Aventri. We can only sync what is available so some events will not have this data in Data hub. Changes to the recording of attendance need to be made in the future to ensure this is always available.

The events that do have attendance recorded will sync to Data Hub. This will update the attendee status. See the [post on changes to attendee status](/data-hub/event-attendee-status/) for more details.

***
