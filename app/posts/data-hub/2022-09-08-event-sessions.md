---
title: Session details for events
description: Understanding whether session information is useful to users
author: Simon Hobeck and Jacqueline D'Alcorn
date: 2022-09-08
service: Data Hub
epic: Events
tag:
  - Sessions
related:
  title: Related links
  items:
  - text: Round 1 design
    href: https://trade.invisionapp.com/freehand/Roadmap-of-Event-sync-f12Fy8ipu
  - text: Round 2 prototype
    href: https://trade.invisionapp.com/prototype/Event-service-deliveries-cl7pxs7lm02ul3i011ln3axgc/play/df7be024
---

***
## Why we were looking to make changes
During the project to integrate Aventri with Data Hub, the issue was encountered of how to handle Aventri sessions.

Data Hub only captures events, whereas Aventri may have two levels - events and sessions.

The usage of Aventri sessions varies across DIT. In some instances, Aventri sessions are equivalent to Data Hub events. But other times, Aventri sessions can be ignored. There is no automatic way to know which case applies.

Some thought and investigation was done for the concept of sessions in Data Hub.

***
## Designs tested with users
### Round 1 - Nesting session information for all events
This design allows the details of all sessions in Aventri to be viewed in Data Hub. It also displays the attendance status for each session, for each individual. It treats the event level in Aventri as the equivalent to an event in Data Hub and nests the session information below event. All sessions would be grouped together when displayed on a Contact or Company record.

The idea behind this was to provide users will additional information they have not previously had in Data Hub. We wanted to find out whether this extra information was useful and help advisers get a better understanding of a company, and therefore allow them to provide more tailored advice.

#### Outcome of user testing
The designs were shared with ten users who regularly work with Aventri, mostly Marketing & Events managers and those who manage Export Academy events.

Feedback was provided from three users - all found the proposed design complicated and overly complex. They felt it provided information that was not needed. They also felt it grouped events that were not really the same event - the example of Export Academy came up, which is an Event in Aventri with many sessions but those sessions are all individual events. Export Academy is a programme of events that has been running for several years and the sessions do not need to be grouped together in Data Hub. Therefore, this design was not taken forward.

![screenshot of displaying multi-session events on the company activity feed](company--multiple-session-attendees.png)

### Round 2 - An option allowing users to change the event set up
This design allows the user to change the event to become multiple events. If they do this all of the sessions convert to events. The event becomes the event programme which has all the events within it. This allows the user to control how events are viewed to suit each case. Doing it this way means the events can be searched for in the same way as they currently are. It also means the event attendance shows up on the contact and company records when that event occurs (rather than grouped with all the other events/sessions within that event programme).

#### Outcome of user testing
Feedback on this design was well received, as it matched the existing workflow and fulfilled the users immediate requirements. It fitted with the mental model users have for the event set up and provides information only on the events/sessions that are actually useful to users.

##### Question that allows the user to change the event set up

![Showing the question that allows users to change the event set up](event-set-up-switch.png)

##### Fields added to the event
This helps users understand the event hierarchy and what type of event they are viewing. Only events within an event programme have the 'top-level event' field, which links to the overarching event programme where the list of events can be found (shown below).

![Showing the new fields added to an event, which explain the event set up](event-within-programme.png)

##### List of events within an event programme

![Showing how the events within an event programme are displayed](event-programme-list.png)

### Round 3 - Admin-only ability to change the event set up  
After consideration we realised that changing the event set up will be a fairly rare task. It will only be done for large scale event programme and only needs to be once for the event programme. The majority of events would not need to be changed.

There was also concern that users may accidentally change an event programme back to a single event and cause problems with the additional data that had been saved to the events/sessions.

We therefore made the decision to reduce development effort for this feature and make it a task only admin/support staff can do. The display of the event programme and events would however remain as shown in round 2.
