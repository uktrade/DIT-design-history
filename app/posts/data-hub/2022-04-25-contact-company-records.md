---
title: Making Company and Contact records consistent
description: Creating a consistent layout for records, which allows space to filter activity and has comparable content and actions in the header area.
author: Jacqueline D'Alcorn
date: 2022-04-25
service: Data Hub
epic: Finding information
tag:
  - Activity tab
  - Contact filter
  - Company filter
  - Interactions
  - Record header
---

***
## Why we were looking to make changes
1. Lots more data was going to be added to the platform, with automatic-sync from other systems. Therefore it was crucial for users to be able to find what they are looking for.
2. The design was inconsistent across the platform.
4. Having different ways to do things on different pages increases the amount of learning required from users and increases cognitive load.

***
## Changes that were made
### 1. Making the interaction card design consistent across Data Hub
See the [post on changes to interaction cards](/data-hub/interaction-cards/).

### 2. Making language consistent
#### Using ‘Activity’ instead of 'Interactions'
On Contact records the phrasing 'interactions' was used, whereas on Company records 'Activity' was used. Having inconsistent language for the same content makes it harder for users to find what they are looking for.

Interactions was originally used because the feed was only displaying contact between DIT and the company or contact but as we are adding additional data to this feed, which is not always direct contact, the phrasing 'activity' was more accurate. For example, on a Company record there is activity shown from HMRC and Companies House that gives information about export and accounts. This change of language has been changed in the sidebar, breadcrumbs, heading and subtext.

![screenshot of where Interactions label was used](contact--interactions-label.png)

### 3. Moving the content tabs to the top  
Reasons for making this change:
1. Having the tabs along the top leaves additional space for the content in each tab. This was important because it provided a space, in the same location as other pages across Data Hub, for filters to be added. These were likely to be needed with the addition of more data sources.
2. To make the layout consistent across the Contact and Company records. This makes it easier for users to navigate. Previously, tabs on the Contact record were down the left side whereas on the Company record they were along the top.
3. Follows the GDS tabs pattern

* **Tabs on a Contact record**

![screenshot of tabs on a Contact record](contact--tabs.png)

* **Tabs on a Company record**

![screenshot of tabs on a Company record](company--tabs.png)

### 4. Adding filters
The addition of extra data sources meant there would soon be more data shown on both the Contact and Company records. Therefore it was important to provide users with a way to filter the data so they could find what they were looking for. The filter follows the same pattern that is used across Data Hub, which also follows the GDS pattern.

Filters that were added:
* For Contact: adviser, team
* For Company: contact, adviser, team
* For both: Interaction type, Interaction topic, Data source

### 5. Adding contact details and key actions to the header
The information shown in the header was different for the Contact and Company records. The Contact record only displayed the person's name and company. Whereas the Company record had contact information, an action button and a link to full details. This made it much easier to find information, rather than scrolling down the page and making the sure finding the correct tab to access those details.

Changes made:
* Contact details shown in header
* 'View full details' link to get to other record details, which are rarely used. This only shows when there are further details (all the further details are optional fields).
* 'Add interaction' button made green and moved to the header. This is a key action users come to these records to complete so needed to be easy to access no matter what part of the record they were viewing. During a 3 month period (1 Feb to 30 Apr 2022) 31% of views of the interactions tab on the contact record clicked on the Add interaction button.
* On Company record, the 'Refer this company' button has also moved to the header, as this is a global actions not just tied to Activities.
* Edit and Archive moved under the ‘View options’ button, as these are less common actions.

![screenshot of header on a Contact record](contact--header.png)

***
## Screenshots of changes
#### Contact record – before
![screenshot of previous contact record](contact--previous.png)

#### Contact record – after
![screenshot of contact record after changes](contact--after.png)

#### Company record – before
![screenshot of previous company record](company--previous.png)

#### Company record – after
![screenshot of company record after changes](company--after.png)

***
