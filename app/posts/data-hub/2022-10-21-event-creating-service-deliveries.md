---
title: Events – Creating Service Deliveries for event attendance
description: Ensuring Service Deliveries are created for event attendance so reporting is accurate.
author: Jacqueline D'Alcorn
date: 2022-10-21
service: Data Hub
epic: Event data
tag:
  - Service Deliveries
  - Synced data
related:
  title: Related links
  items:
  - text: Prototype
    href: https://trade.invisionapp.com/prototype/DIT-events-full-flow-admin-switch-cl98hs5k90072k401n9zpkpjg/play/ac860e6a
  - text: Flow diagram
    href: https://trade.invisionapp.com/freehand/Create-Service-Delivery-from-DH-Event-record-U2jGrUD2C?zoomToItems=Y2w2ejN5MjV3MDAzczNyNnFiaWwwaHk0dw%3D%3D
---

***
## Why we were looking to make changes
Service Deliveries are used for reporting and to show when something has been delivered. This is important for people's targets. One example of this is when someone attends an event. This is only a Service Delivery if they attend, not if they register and do not attend.

Service Deliveries for event attendance require several bits of information before they can be created:

* [A contact record associated to the attendee](/data-hub/event-creating-service-deliveries/)
* [Event details, such as the organiser and team who were responsible for the Service Delivery](/data-hub/event-creating-service-deliveries/)  

The data coming from Aventri did not have this infomation and did not always connect to contact record. This is why other flows needed to be created, which are talked about in other posts linked above.

## Changes that were made
After we had flows and designs for entering all the information needed for a Service Delivery, there was just one more hurdle to jump over. Data Hub had no way to recognise if data had changed from Aventri, for example to know if the attendance status of someone who registered for an event had now changed to attended. So it was not able to automatically create service deliveries. This meant a user would need to manually press a button to do this.

There is a good side to this though, as we discovered during our research that different regions deal with Service Deliveries differently. In some regions they create a Service Delivery for every attendee but in other regions they only create a Service Delivery for one person at each company. This meant automation would be difficult anyway.

A button was added to the Attended tab of an event. After pressing this button there are 4 routes:

* The add event details form, if the details have not already been added
* An alert to say there are no attendees with contact records who do not already have a Service Delivery created (so there is nothing to add)
* An alert to say only some of the attendees have contact records and Service Deliveries can only be created for those
* A list of attendees with contact records

The list of attendees are all selected by default, as the most common action is to add Service Deliveries for everyone.

The list is sorted by company name A-Z (with the option to switch to Last name). This is so users can easily see the companies with multiple attendees and deselect those ones.

##### Alert shown when there are no attendees to add Service Deliveries to

![Alert shown when there are no attendees to add Service Deliveries to](10-Service-deliveries--alert-none-to-create.png)

##### Alert shown when not all attendees have contact records

![Alert shown when not all attendees have contact records](10-Service-deliveries--alert.png)

##### Screen to select the attendees to add Service Deliveries for

![Screen to select the attendees to add Service Deliveries for](11--Service-deliveries--select.png)

***
