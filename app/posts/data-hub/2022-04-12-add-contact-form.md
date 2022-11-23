---
title: Add contact form
description: Rectifying the form in terms of improving user satisfaction on "Add an interaction" journey.
author: Caner Uzun
date: 2022-04-12
service: Data Hub
epic: Forms
tag:
  - Contacts
  - Interaction
---

***
## Why we were looking to make changes
Comprehensive user research on the "Add an interaction" journey was conducted in Q3 2021/2022 suggesting that to improve user satisfaction on the journey, the least complex and quick action would be improving the "Add contact" form.

Users in various user research sessions mentioned that they find adding certain contact information pieces problematic within the page such as "Job title", "Telephone country code", and "Telephone" since they are mandatory fields and these pieces of information are sometimes not available to the user. This challenge was also resulting in bad data being entered into Data Hub records.

***
## Changes that were proposed and made
### 1. First name, last name
As GDS suggests, not everyone's name fits the first-name, last-name format. Since using multiple name fields meant there's more risk that a person's name wouldn't fit the format chosen and would be entered incorrectly we proposed using a single field called "Full name". Eventually, we couldn't make this change as merging two fields was going to bring some query issues in Data Workspace.

### 2. Telephone country code and number
In addition to user research suggestion to make the "Telephone country code" and "Telephone number" field optional, we examined the historical usage data and ended up with the fact that more than 20% of the entries can be considered 'bad data' as they were not real phone numbers.

We merged two fields into one called "Phone number (optional)" and added a hint text for the users who might have struggled with what to do for international numbers.

### 3. Email address  
We relabeled "Email" field with "Email address".

### 4. Contact's address
Users said that sometimes they might be engaging with a company member who is not located where the company HQ is located. Therefore, we kept the field. However, we made a few changes. We first changed the question (label) from "Is the contact's address the same as the company address?" to "Is the contact's work address the same as the company address?".

The conditionally revealed fields following the "No" answer to the initial question were not ordered logically. Postcode lookup functionality was not working properly for the UK addresses. We moved the "Country" selection to the top so that US, Canada and UK-specific fields could be displayed and ordered accordingly.

### 5. Alternative email address and phone number
The usage of both of the fields was significantly low. Therefore, we removed them.

### 6. Notes
We kept the field as optional but changed the label from "Notes (optional)" to "More details (optional)". We also added a hint text to the field: "Add anything you think is important about the contact, for example, an alternative phone number or email address.".

## Screenshots

![screenshot of an empty add contact form](add-contact-empty-form.png)

![screenshot of a filled in add contact form](add-contact-filled-in-form.png)

***
