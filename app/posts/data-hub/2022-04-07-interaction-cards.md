---
title: Interaction cards
description: Ensuring useful information is provided about interactions wherever the summary card is viewed. Making interaction cards consistent across Data Hub.
author: Jacqueline D'Alcorn
date: 2022-04-07
service: Data Hub
epic: Finding information 
tag:
  - Interactions
  - Service labels
---

***
## Why we were looking to make changes
1. Lots more data was going to be added to the platform, with automatic-sync from other systems. Therefore it was crucial for users to be able to find what they are looking for.
2. Content was repeated
3. The design was inconsistent across the platform
4. The design didn't follow GDS patterns
5. Users were encountering some problems

### User problems
The User Researcher on the project had heard a number of comments from users whilst conducting research for other parts of Data Hub. So, while no specific research was run on this area, we had a good feel for the problems users were facing. This included:

* It was hard to scan the content
* It was difficult to find specific information from the list of interactions
* There was not enough information to get an overview of an interaction

***
## Changes that were made
### 1. Making the interaction card design consistent across Data Hub
There was inconsistency with the quantity of information displayed and design of the interaction cards, as shown below.

The design has been brought in line with other parts of Data Hub. It is now closer in design to what is used by many other [services across government](https://live-stuff.herokuapp.com/document-types/finder).

* Previous interaction card on a Contact record:

![screenshot of previous interaction card](interaction-card--previous--contact.png)

* Previous interaction card on a Company record:

![screenshot of previous interaction card](interaction-card--previous--company.png)

* Updated interaction card:

![screenshot of updated interaction card](interaction-card--updated.png)

Changes included:
* Styling of 'Service delivery' label to match the GDS tag pattern
* Meta data in grey to match other goverment services and to allow heading to stand out more
* Removal of accordion so it's easier to scan the information and reduces burden on Users
* Consistent date format, following the [GDS style guide](https://www.gov.uk/guidance/style-guide/a-to-z-of-gov-uk-style#dates)

### 2. Using language that is specific to the interaction type
On the interaction card 'Adviser' was used for all types of interactions, but sometimes this wasn't  accurate. For example, for an event the phrasing 'Organiser' was used in other places on Data Hub.

### 3. Adding the theme and service labels
Labels were added to help users scan down a list of interactions e.g. so they could quickly see the topic of each interaction and decide if they needed to read any more detail about the interaction.

These labels were added to the top of the interaction card, shown below with the example of 'Export' and 'Service or Funding'. These labels are the interaction theme and service type. There are four themes, 19 top-level and over 125 second-level service types within Data Hub.

To keep the labels succinct only the top-level service type are displayed. We didn't have any evidence that users needed the granular second-level service type. Having just two labels would be easier to scan and should provide enough context for users. But this is an area we will test with users.

The top-level service type uses a cut-down label so it doesn't repeat the theme and provides enough information without being too wordy and hard to scan.

![screenshot of labels on interaction cards](interaction-card--labels.png)

### 4. Adding additional information to the card
* Added note preview
* Added communication channel

Additional information was added to give users more context about the interaction while reviewing a company or contact's record. This gives a snippet of the note associated to the interaction and the communication channel. The hypothesis is this information would allow them to decide if they need to read the full interaction record and prevent unnecessary click throughs.

On the Company record, there was very little information displayed. The information displayed was brought inline with the Contact record.

![screenshot of additonal information on interaction cards](interaction-card--additional-info.png)

### 5. Removing information from the interaction card when it is already shown on the page
* Removing contact and company when viewing a Contact record
* Removing company when viewing a Company record

When viewing interactions from a Contact record the card displayed the Company and Contact name within each interaction card. This duplicated information that is displayed at the top of the record. This information always contained the name of the contact and company that was being viewed. This added strain on the user who needed to filter out this information while scanning down the interactions.

![screenshot of repeated information on interaction cards](interaction-card--repeated-information.png)
