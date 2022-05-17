---
title: Syncing event data
description: Providing a fuller picture of events, registrants and attendees by syncing data rather than relying on manual entry.
author: Jacqueline D'Alcorn
date: 2022-05-09
service: Data Hub
tag:
  - Events
  - Syncing data
related:
  items:
  - text: Test
    href: https://miro.com/app/board/o9J_ldVNkCY=/
---

<span class="govuk-body govuk-!-margin-bottom-9">
  <span class="govuk-tag">{{ service }}</span>
  {% for item in tag %}
    <span class="govuk-tag govuk-tag--grey govuk-!-margin-top-1">{{ item }}</span>
  {% endfor %}
</span>

***
## Why we were looking to make changes
1. Users had to manually enter data into Data Hub, which was a lengthy process
2. Sometimes manual entry was outsourced, which had cost implications
3. Data was not always entered
4. Data that was entered did not get entered in a consistent format

### User problems
We ran X sessions with users to understand

* It was hard to scan the content
* It was difficult to find specific information from the list of interactions
* There was not enough information to get an overview of an interaction

***
## Changes that were made
### 1. Making the interaction card design consistent across Data Hub
There was inconsistency with the quantity of information displayed and design of the interaction cards, as shown below.
