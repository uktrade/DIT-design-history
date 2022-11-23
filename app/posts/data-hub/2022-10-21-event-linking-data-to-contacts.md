---
title: Events – Linking event data to Contact records
description: When syncing data from another system to Data Hub there is not always a unique identifier to tie the data together with a record
author: Jacqueline D'Alcorn
date: 2022-10-21
service: Data Hub
epic: Event data
tag:
  - Adding contacts
  - Linking data
  - Synced data
  - Interactions
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
When pulling data from Aventri into Data Hub we need to tie the data from Aventri to a record in Data Hub. The most suitable identifier that was captured on all event registration forms was email address. This worked well in most cases, but there were some cases when a matching record could not be found:

* The email address the person registered with was not the same as the one stored in Data Hub
* There was a typo in the email address
* Multiple contacts in Data Hub had the same email address stored e.g. if they used something general like info@example.com
* The person did not exist as a contact in Data Hub

In these cases the system could not automatically tie the data and record together, so we needed to think of other ways to do that.

It was important to tie together the data with a Data Hub record because it is used for reporting. The reporting requires a contact record to be in Data Hub with a Service Delivery (a type of interaction) saved against the record. See post about [Creating Service Deliveries](/data-hub/event-creating-service-deliveries/) for more information.

## Design
### One flow to add or link new or existing contacts
Prior to this users had to manually do a number of processes if they needed to add an attendee to an event who was not already a contact in Data Hub. They would have to search for company, check the contacts, add a contact, go back to the event and then add an attendee - going in and out of several different records to complete the task. This work allows users to do that process all in one flow.

In research we discovered that users add all event attendees as Contacts in Data Hub. Previously, they would check and create each contact as a seperate task. Now with this journey they remain on the event so they can add each contact one after the other.

When viewing the list of people in any of the attendance status tabs on an Event, you can see every person who has that attendance status regardless of whether they have a connected contact record. The people without a contact record have their name shown in black, as it isn't linked to anything. Next to these people is a button named 'Add contact'. After pressing this button the user is taken through a flow which allows them to:
* Find the company the person works for, if it already exists in Data Hub
* Add the company the person works for, if it doesn't already exist in Data Hub
* Connect the person to an existing contact
* Create a new contact record

[Robbie - New company (from verified results) and new contact](https://trade.invisionapp.com/prototype/DIT-events-full-flow-admin-switch-cl98hs5k90072k401n9zpkpjg/play/ac860e6a)
[Adela - Existing company, existing contact](https://trade.invisionapp.com/prototype/DIT-events-full-flow-admin-switch-cl98hs5k90072k401n9zpkpjg/play/9fb10c61)
[Veronica - New company (not verified), new contact](https://trade.invisionapp.com/prototype/DIT-events-full-flow-admin-switch-cl98hs5k90072k401n9zpkpjg/play/46f995ee)
[Beth - Existing company, new contact](https://trade.invisionapp.com/prototype/DIT-events-full-flow-admin-switch-cl98hs5k90072k401n9zpkpjg/play/f5211ed9)

![screenshot of an attendee with a contact record and one without](attendee-non-linked.png)

### Suggestions if there are existing contacts with similar names
If the person is from an existing company and that company has any existing contacts, the user is given the opportunity to select one of those and tie the two together.

If the existing contacts have the same or similar name these are shown at the top of the list. The other contacts (whose names are not similar) are placed into an accordion, giving the user the option to check them but not cluttering with screen with information that is most likely not relevant.

##### Highlighting existing contacts with similar names  

![screenshot of the screen showing existing contacts with similar names](Existing-company--similar-contacts.png)

##### Accordion for users to see all existing contacts, who don't have similar names  

![screenshot of an attendee with a contact record and one without](Existing-company--no-similar-contacts.png)

***
