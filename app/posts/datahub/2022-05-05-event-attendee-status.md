---
title: Adding statuses for event attendance  
description: Providing additional information around event registration and attendance so users in contact with Companies have a fuller picture of the contact's interest.
author: Jacqueline D'Alcorn
date: 2022-05-05
tags:
  - "Events"
  - "Interactions"
---

## Why we were looking to make changes
While we were adding the data source for events we discovered there were additional statuses recorded in the system. These allowed us to see if a person had registered, if they had confirmed their registration and if they attended the event. From these details we could also infer if the person had not attended the event.

This provided a fuller picture of interaction DIT had with a contact. By showing this information in Datahub it would allow users to see if a contact had shown an interest in an event even if they had not attended it. This could provide a potential conversation area or an area to offer advice. It would also provide an opportunity to highlight a similar event or another date for the event if they weren't able to attend.

***
## Changes that were made
### 1. Added different attendance statuses
The statuses we decided on were:
- Registered
- Registration confirmed
- Registration cancelled
- Registered but did not attend
- Attended
- Attendance unknown

This is displayed next to the event name on the interaction in the activity tab. It is shown in grey so it is easier for users to find the status after then have found the event they are looking for.

![screenshot of the attendance status](attendance--status.png)

### 2. Adding filters for the attendance status
Adding interactions for events that contacts have not attended adds more data to Datahub and therefore more data for users to navigate and look through to find that they need. Because of this it is important to provide ways to help users find what they need. Here is a design for a filter that could be added in the future.  

![screenshot of the attendance status filters](attendance--status-filters.png)
