---
title: Recently viewed data and suggested searches
description: Adding functionality to the data search to display recently visited data and suggested searches based on input.
author: Andy Davies
date: 2022-09-30
service: Data Workspace
epic: Finding information  
tag:
  - Search
  - Interaction

---

## Why we were looking to make changes
1. Previous user research had highlighted that users can be very repetitive in the data they view in Data Workspace and consistently search for the same data, a journey we could improve
2. It was also found that many users don't explore new data on Data Workspace and were unlikely to visit data that wasn't directly related to their task
3. In previous research sessions it was found that if we were to improve the experience for users by assisting them with existing patterns of behaviour or promote unexplored data of relevance then we would have to factor this in to their existing task-based journey
4. To encourage users to explore data in Data Workspace

### User problems
In UR conducted in early 2022 it was found that users don't tend to explore data on Data Workspace, despite data existing which could assist them in their work.

In previous research it was also found that a high proportion of users are very task-orientated and wouldn't browse pages for data which took them away from their intended journey.

## Changes that were made

After a round of user testing to validate the hypothesis that adding recently browsed data and suggested searches would encourage users to browse data and contribute to a more effective user journey for users, then these features were implemented on Data Workspace.

### 1. Recently viewed data
Functionality was added so that when a user presses on the data search on the Data Workspace homepage then the last three (or less) pieces of data accessed by that user would be displayed. This was to give a quick route through to regularly visited data.

The features design and implementation was based on the suggested search used on the [GDS Design System website](https://design-system.service.gov.uk/), following the same interaction and accessibility patterns.

![screenshot of recently viewed data](recently-viewed-data.jpg)

### 2. Suggested search
A suggested search was implemented to encourage users to explore data in Data Workspace. The feature collects inputs from users and then returns results when someone has input text which matches previous user queries. Suggested searches are then displayed, showing previous search queries which match the string and return a result. These queries are ranked by popularity with a maximum of five displayed to the user. This creates a feature which allows users to learn from each other and benefit from real user searches which can show related data to content users are trying to find.

![screenshot of suggested search](suggested-searches.jpg)

***
