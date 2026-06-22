# Pipedrive integration overview in Convex

## Overview

Transfer key business information from Convex to Pipedrive to ensure your Pipedrive environment stays up to date, saving you time and minimizing manual data entry.

## Who uses this feature

* Managers, regional managers, representatives, and salespeople
* Primarily for Commercial Service and Commercial Construction business types

## Feature configuration

* Contact [marketing@convexlabs.io](mailto:marketing@convexlabs.io) to set up a demo and get more information about Convex.

## Things to know

- To set up an integration between Atlas and your CRM platform, generate API credentials for Pipedrive and share them with your Customer Success Manager (CSM). Your CSM will help you set up the integration and customize data mappings to fit your business needs.
- Atlas sends relevant information, such as the company details, property addresses, and contact information, directly into Pipedrive.
- The integration regularly compares data between Pipedrive and Atlas. If it identifies any discrepancies or outdated information, it automatically updates the appropriate system to maintain accuracy.

## Push to CRM

Push to CRM is a feature in Atlas that allows you to manually trigger the sync of selected property and contact data into your Pipedrive.

1. Go to the navigation menu and click Map, then select a property.

2. From the Properties details panel (PDP) that opens, click Push to CRM.

The integration sends the following information:

- Property details: Company name, address, and any other associated custom fields.

- Contact details: Names, phone numbers, emails, titles, and social profiles.

> **Note:** Make sure to associate a contact with a property if you want to send contact information to Pipedrive.

## Create Pipedrive Records

Integration creates the following Pipedrive Records:

- Create Organization.
- Create Deal: If enabled, the integration:
  - Maps the data to a Pipedrive Deal.
  - Creates the Deal in Pipedrive.
- Create Persons: If enabled, the integration:
  - Maps the contact data to a Pipedrive Person.
  - Checks if the Person exists already in Pipedrive.
  - Adds the Person to the Deal.

| Term | Definition |
| --- | --- |
| Organization | A company or business entity within Pipedrive. Typically represents customer or prospect accounts. |
| Person | An individual contact within Pipedrive. Each person can be associated with Organizations and Deals. |
| Deal | Represents a sales opportunity within Pipedrive. Deals are typically linked to an Organization and one or more Persons. |

> **Note:** The integration uses the default recommended mapping for Pipedrive. This mapping is customizable based on your needs during setup. Reach out to your CSM for more information.

## Sync Pipedrive Data to Convex

This workflow is used to populate Convex with existing CRM data from Pipedrive. It usually runs a single time during the initial integration to display relevant Pipedrive Organization in Atlas. The workflow then runs on a scheduled basis and only updates the organizations that have changed since the last update.

#### Workflow Behavior:

1. Query Organizations from Pipedrive: The workflow retrieves all Pipedrive Organizations that meet the following criteria:

   a. Changed since the last run (first run includes all organizations).

2. Match Organizations to Properties in Atlas: For each Pipedrive Organization, the workflow checks for an existing link to a Convex Property using the CRM ID.

> **Note:** CRM ID is a unique identifier for a Company or Contact in HubSpot that Atlas uses to match or link records during syncing.

   a. If no CRM ID match is found, it attempts to match the Property by address.

   b. If a match is found, it proceeds to enrich the Property with Organization data.

3. Pull Historical Persons: If Persons are enabled on the customer solution, then this workflow:

   a. Pulls all the Persons from each Pipedrive Organization.

   b. Examines each person and updates with any changes.

4. Check for Errors: The first run reports any errors encountered.

## Keep Convex up to date

This workflow ensures that Atlas reflects the current state of your CRM by removing contact links when contacts are deleted in Pipedrive.

#### Workflow Behavior:

1. Pipedrive Webhook: Pipedrive can be configured to send a webhook request to the solution when a Person is deleted in Pipedrive.

2. Remove Persons from Convex: For each deleted contact:

   a. The workflow locates the associated contact in Atlas (linked via CRM ID).

   b. It deletes the Pipedrive-related data from the contact in Atlas, effectively removing the CRM link but retaining any Atlas-native data.

## Want to learn more?

- See Salesforce integration overview in Convex

- See HubSpot integration overview in Convex
