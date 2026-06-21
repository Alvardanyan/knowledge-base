# Aspire integration overview in Convex

## Overview

Transfer key business information from Convex to Aspire to keep your Aspire environment up to date, saving you time and minimizing manual data entry.

## Who uses this feature

* Managers, regional managers, representatives, and salespeople
* Primarily for Commercial Service and Commercial Construction business types

## Feature configuration

* Contact [marketing@convexlabs.io](mailto:marketing@convexlabs.io) to set up a demo and get more information about Convex.

## Things to Know

• To set up an integration between Convex and Aspire, share the Aspire and Convex information with your Customer Success Manager (CSM). Your CSM will help you set up the integration and customize data mappings to fit your business needs.

• Ensure to provide the following information:

    o Aspire information:

        • Client ID / Secret: To locate or generate the API credentials, see API Search List.

        • Lead Source (Optional): You can add Convex as a Lead Source in Aspire. To do so, add the Lead Source in your Aspire admin panel and provide the name and ID. The ID is at the end of the URL when the new lead source is opened. For example, in the screenshot below, it is 12.

        • Branch Name (Optional): You can provide the Branch Name if you want the leads to be assigned to a specific branch. For best results, include the Branch ID, which is found at the end of the URL when the branch page is open. For example, in the screenshot below, the ID is 2.

        • User matching (On / Off) (Optional): An optional feature where Convex can assign the Aspire Task to a matched user from the Convex Target assignment.

    o Convex information:

        • Org ID

## Push to CRM

After the lead is Qualified, you can push it to Aspire from the Target List workflow. The feature allows you to manually trigger the sync of selected lead and contact data into your Aspire.

1. Go to the navigation menu > Targets, then click a target list.

2. From the target list, select the Qualified leads you want to push.

3. Click Export, and then click CRM.

The Push to CRM was successful notification appears letting you know that the leads have been transferred.

The integration sends the following information to Aspire:

• Contact details:

o First name

o Last name

o Title

o Email

o Office Phone

o Mobile Phone

o Website

o Contact Type (Set as Prospect)

o Active (Set as True)

o Office Address

• Property details:

o Property Name

o BranchID

o LeadSourceID

o Address

o Action (Set as True)

• Issue:

o Created By (Set as Convex)

o Created Date/Time

o Assigned to

o Due Date (Scheduled two days out)

o Property

## View targets in Aspire

In Aspire, we automatically create the Property, associated Contacts, and Property Issues that can be promoted to a new Opportunity.

1. Go to Aspire > Properties.

2. Search for the pushed target and click to open it.

Here you can view all property details, assign a user, and create a new opportunity.

> **Note:** We don't create an opportunity because it may require different opportunity templates or additional details we don't have, such as pricing methods or invoice types. Instead, we create Property Issues (tasks) that can be promoted to a new opportunity.

# Want to learn more?

• See Salesforce integration overview

• See Hubspot integration overview

• See Pipedrive integration overview
