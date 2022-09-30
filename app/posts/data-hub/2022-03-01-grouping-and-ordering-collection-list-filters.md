---
title: Grouping and ordering collection list filters
description: Sorting the filters by considering a logical order that we believed users would most benefit from.
author: Caner Uzun
date: 2022-03-01
service: Data Hub
epic: Filters
tag:
  - Companies filters
  - Contacts filters
  - Events filters
  - Interactions filters
  - Investments filters
---

***
## Why we were looking to make changes
Historically, the collection list pages (Companies, Contacts, Events, Interactions and Investments) have been growing in size with new filters being added over time without any thought of a priority. Therefore, we needed to review and order the filters on each collection list to make it easier for users.

After examining the most recent Google Analytics data and cross-checking it with user research findings from previous months, we sorted the filters by considering a logical order from which we believed users would most benefit.

***
## Changes that were made
### 1. Companies list
We created three accordion sections to group filters: "Company details", "Location details", and "Company activity details". Based on expected engagement we decided to keep the "Company details" section expanded and others closed when the filters are loaded. Company details section includes the most popular filters among all such as "Company name" and "Type".

![screenshot of companies list filters](companies-list-filters.png)

### 2. Contacts list
We created two accordion sections to group filters: "Contact details", and "Contact location details". Based on expected engagement we decided to keep the "Contact details" section expanded and others closed when the filters are loaded. Clients details section includes the most popular filters among all such as "Contact name" and "Company name".

![screenshot of contacts list filters](contacts-list-filters.png)

### 3. Events list  
We created two accordion sections to group filters: "Event details", and "Event location details". Based on expected engagement we decided to keep the "Event details" section expanded and others closed when the filters are loaded. Event details section includes the most popular filters among all such as "Event name" and "Organiser".

![screenshot of events list filters](events-list-filters.png)

### 4. Interactions list
We created three accordion sections to group filters: "Interaction details", "Service details", and "Policy details". Based on expected engagement we decided to keep the "Interaction details" section expanded and others closed when the filters are loaded. Interaction details section includes the most popular filters among all such as "Advisor", "From", and "To".

We also made some changes on filter and grouping labels as there'd been user research findings suggesting to do so. We replaced "Kind" with "Interaction type" to make it more clear. Also, we added the "My interactions" title above the "My interactions" checkbox to establish consistency across listing pages.

Finally, we updated "Policy area(s)" label with "Policy areas" to improve accessibility for users who need assistive technologies.

![screenshot of interactions list filters](interactions-list-filters.png)

### 5. Projects list
We created five accordion sections to group filters: "Stage and status", "Project details", "Land date details", "Investment and involvement details", and "Location details". Based on expected engagement we decided to keep "Stage and status" section expanded and others closed when the filters are loaded. Stage and status section includes the most popular filters among all such as "Stage", and "Status".

We also made some changes to filters and labels as there had been user research findings suggesting doing so. We replaced "Country of origin" with "Country of company origin". We changed "Type of investment" to "Investment type" and also updated "Level of involvement specified" to "Involvement level".

Users had also been indicating that "Land date details" filter labels were not easy to understand. We replaced "before/after" with "from/to" as it'd also been consistent with other date filters on Data Hub.

![screenshot of investment projects list filters](projects-list-filters.png)