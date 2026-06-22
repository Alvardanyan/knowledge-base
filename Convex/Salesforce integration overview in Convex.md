# Salesforce integration overview in Convex

## Overview

Transfer key business information from Convex to Salesforce to ensure your Salesforce environment stays up to date, saving you time and minimizing manual data entry.

## Who uses this feature

* Managers, regional managers, representatives, and salespeople
* Primarily for Commercial Service and Commercial Construction business types

## Feature configuration

* Contact [marketing@convexlabs.io](mailto:marketing@convexlabs.io) to set up a demo and get more information about Convex.

## Things to know

- To set up an integration between Atlas and your CRM platform, generate API credentials for Salesforce and share them with your Customer Success Manager (CSM). Your CSM will help you set up the integration and customize data mappings to fit your business needs.

- Atlas sends relevant information, such as the company details, property addresses, and contact information, directly into Salesforce.

- The integration regularly compares data between Salesforce and Atlas. If it identifies any discrepancies or outdated information, it automatically updates the appropriate system to maintain accuracy.

## Push to CRM

Push to CRM is a feature in Atlas that allows you to manually trigger the sync of selected property and contact data into your Salesforce.

1. Go to the navigation menu and click Map, then select a property.

2. From the Properties details panel (PDP) that opens, click Push to CRM.

The integration sends the following information:

- Property details: Company name, address, and any other associated custom fields.

- Contact details: Names, phone numbers, emails, titles, and social profiles.

> **Note:** Make sure to associate a contact with a property if you want to send contact information to Salesforce.

## Customize integration

You can select how the integration works at the beginning of the setup process, such as creating Leads, Accounts, or Contacts.

### Push to Leads:

- The integration creates a Salesforce Lead.

- Matches Account ownership in Salesforce using the Account Owner email stored in Atlas.

- Links the Salesforce Account back to the corresponding property in Atlas.

### Push to Accounts:

- The integration creates or updates an Account record in Salesforce.

- Checks Salesforce to avoid creating duplicate Account records.

- Matches Account ownership in Salesforce using the Account Owner email stored in Atlas.

- Links the Salesforce Account back to the corresponding property in Atlas.

### Optional Record Creation:

- Opportunity Creation: If enabled, an Opportunity is automatically created and linked to the Account.

- Contact Creation: If enabled, the integration:
  - Searches Salesforce for existing contacts by unique Contact ID.
  - Updates existing contacts if Atlas data is more recent; otherwise, creates new contacts.
  - Links each contact to the corresponding Account record.

| Term | Definition |
| --- | --- |
| Lead (Salesforce) | A potential customer, often represented by a single contact record in Salesforce. Use it when you prefer to track early-stage prospects rather than structured Accounts and Contacts. |
| Contact (Salesforce) | An individual in Salesforce typically associated with a company (Account). Created when the integration is configured to sync full CRM structures instead of leads. |
| Account (Salesforce) | A company or business entity in Salesforce. |
| Opportunity (Salesforce) | A potential revenue-generating deal in Salesforce. |

## Sync Salesforce Data to Convex

This workflow brings existing Salesforce data into Convex. It usually runs a single time during setup to show relevant Salesforce Accounts in Atlas.

#### Workflow Behavior:

1. Query Accounts from Salesforce: The workflow retrieves all Salesforce Accounts that meet the following criteria:

   a. Not marked as deleted.

   b. Not already assigned a CRM Contact ID in Atlas.

   c. Not already linked to a Convex Contact.

2. Filter by Atlas User Ownership: Only Accounts associated with Salesforce users who are also part of the Atlas Organization are processed.

3. Match Accounts to Properties in Atlas: For each qualifying Salesforce Account, the workflow checks for an existing link to an Atlas Property using the CRM ID.

> **Note:** CRM ID is a unique identifier from the CRM (such as a Salesforce Account ID) that Atlas uses to match or link records during syncing.

   a. If no CRM ID match is found, it attempts to match the Property by address.

   b. If a match is found, it proceeds to enrich the Property with Account data.

4. Look Up Custom Fields: Defines which Salesforce fields should be pulled into Convex. It is pre-populated with default mappings but can be customized if you use custom fields.

5. Update Property Record in Atlas: The matched Atlas Property is updated with the data from the Salesforce Account.

## Keep Convex up to date

This workflow ensures your Convex account reflects the current state of the CRM by removing contact links when contacts are deleted in Salesforce.

#### Workflow Behavior:

1. Scheduled Interval: The setting controls how frequently the workflow runs to check for deletions in Salesforce.

2. Identify Recently Deleted Contacts: When the workflow runs, it searches Salesforce for deleted contacts from the last run.

3. Remove Contacts from Atlas: For each deleted contact:

   a. It locates the associated contact in Atlas (linked via CRM ID).

   b. It deletes the Salesforce-related data from the contact in Atlas, effectively removing the CRM link but retaining any Atlas-native data.

## Want to learn more?

- See Hubspot integration overview in Convex

- See Pipedrive integration overview in Convex

