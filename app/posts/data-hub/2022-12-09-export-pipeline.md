---
title: Improvements to the export pipeline
description: The existing export pipeline tool in Data Hub was being underutilised and needed a user centred approach to align it with existing users expectations.
author: Peter Farah
date: 2022-12-09
service: Data Hub
epic: Export pipeline
tag:
  - Export pipeline
  - Managing information
  - Tracking information
related:
  title: Related links
  items:
  - text: Export pipeline flow diagram
    href: https://docs.google.com/presentation/d/1l1YKIkDxIRiOjZGiJJtx2raSgNyi6G5t0ZUgzdCPAiw/edit#slide=id.g1a59de11756_1_39
---

***
## Why we were looking to make changes
Currently, the ‘export pipeline’ within Data Hub is heavily underutilised by users. User research has shown that over a 6 month period only 57 users have used the pipeline, with an average of 58 seconds being spent on the page. This results in users having to manually track and manage company exports through using spreadsheets. Some of the key user pain points and user needs highlighted by the research are as follows:
* Users are unaware of the export pipeline functionality on Data Hub
* Users rely on tracking companies’ progress in other ways (spreadsheet, outlook etc.)
* Users want to share access and management to their pipeline details with other colleagues (similar to investment projects’ journey)
* Users want to track export projects the same way as investments

To improve the current service offering for users, the data enhancements team set out to redesign the end-to-end journey for creating, managing and tracking companies export progress on Data Hub. To achieve this, the team have gone through three design iterations and two rounds of usability testing and tree testing, resulting in an MVP version of the export pipeline, which this article will focus on.


***
## Changes that were made
In this work we have gone through three design iterations. Initially, we ran a cognitive walkthrough of our wireframes, iterated the design based on user feedback, and then conducted usability testing on the second iteration of the design. Following the second round of usability testing, and team reviews we have produced a third design iteration, which is the current design as of writing (December/2022).

### 1. Export form redesign
Through our user research we found that users didn’t understand what was meant by the term ‘Project’ and that the existing questions didn’t adequately capture all the relevant information they needed to support a company with an export. To improve this design, we updated the content, changed the order of the questions, refined the number of mandatory questions, and added different components for information capture. The screenshots illustrate the design iterations.

Current form on Data Hub:

![screenshot of current form on Data Hub](current-form-on-data-hub.png)

Form design: iteration v1

![screenshot of Form design: iteration v1](Form-design-iteration-v1.png)

Form design: iteration v2

![screenshot of Form design: iteration v2](Form-design-iteration-v2.png)

Form design: iteration v3 (current design as of December/2022)

![screenshot of Form design: iteration v3 (current design as of December/2022)](Form-design-iteration-v3.png)

Changes included:
1. Changing ‘project title’ to ‘export title’ as users didn’t understand what was meant by project
2. Adding an single form view by adding in ‘Owner’ and ‘Team members’ as this was split out across two pages before
3. Including a drop down option for ‘Year/s’ for total estimated export value, to capture the various forecasted years users use when entering a value
4. Including a wider variety of mandatory questions based on user feedback
5. Including a question to capture exporter experience  

### 2. Redesigned homepage
We updated the current homepage design to provide users with key information and enhanced usability. For the export cards on the homepage, we utilised the feedback to refine what information needed to be displayed in a snapshot view (destination, estimated export value, date for win, main sector, owner and created on). Additionally, on the homepage we designed a filter component to enable users to find specific information quickly. The screenshots illustrate the design iterations.

Current export pipeline homepage on Data Hub:

![screenshot of current export pipeline homepage on Data Hub](Current-export-pipeline-homepage-on-Data-Hub.png)

Export pipeline homepage design: iteration v1

![screenshot of Export pipeline homepage design: iteration v1](Export-pipeline-homepage-design-iteration-v1.png)

Export pipeline homepage design: iteration v2

![screenshot of Export pipeline homepage design: iteration v2](Export-pipeline-homepage-design-iteration-v2.png)

Export pipeline homepage design: iteration v3 (current design as of December/2022)

![screenshot of Export pipeline homepage design: iteration v3 (current design as of December/2022)](Export-pipeline-homepage-design-iteration-v3.png)

Changes included:
1. Updating service name from ‘Export activity’ to ‘Export list’ for consistency with language used across the homepage (e.g. company list)
2. Including show/hide collapsible components to enable a more focused view for users
3. Updating export status titles from lead, won confirmation, and abandoned to active, won, and inactive, for improved clarity
4. Removing ‘edit activity’ call to action as users reported being confused by this
5. Removing ‘Add to export activity’ button for consistency with other investments projects and company lists services


### 3. Streamlined export overview page  
The overview page provides users with a full view of all the information associated with the export entry, that isn’t displayed on the homepage (company contacts, who the export is shared with, exporter experience and notes). In the first and second design iteration, this page included a tab design, where users could choose between ‘activity details’ and ‘edit access’ to be able to view and edit information on the export and change access permissions. However, findings from research showed that users struggled to navigate to the ‘edit access’ page to successfully change access permissions. We addressed this in iteration v3 by having a single overview page that includes the ‘owner’ and ‘team member’ fields from the single page form redesign, enabling users to edit export details and access permissions in a single view. The screenshots illustrate the design iterations.

Export overview page design: iteration v1

![screenshot of Export overview page design: iteration v1](Export-overview-page-design-iteration-1.png)

Export overview page design: iteration v2

![screenshot of export overview page design: iteration v2](Export-overview-page-design-iteration-2.png)

Export overview page design: iteration v3 (current design as of December/2022)

![Export overview page design: iteration v3 (current design as of December/2022)](Export-overview-page-design-iteration-3.png)


Changes included:
1. Included ‘export potential’ and ‘status’ tags above company and export title
2. Removed tab design, enabling a more centred placement of the summary table
3. Changed ‘edit’ button from green to grey to match the data hub design system
4. Content update from ‘delete activity’ to ‘delete’

*Please note, the data used in these examples is not real and is only used for illustrative purposes.
