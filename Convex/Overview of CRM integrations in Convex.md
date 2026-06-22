# Overview of CRM integrations in Convex

## Overview

Convex CRM integration enables seamless data transfer from Convex to your CRM platform,
automatically creating or updating records while preventing duplicate entries.

## Who uses this feature

* Managers, regional managers, representatives, and salespeople
* Primarily for Commercial Service and Commercial Construction business types

## Feature configuration

* Contact [marketing@convexlabs.io](mailto:marketing@convexlabs.io) to set up a demo and get more information about Convex.

## Types of integrations

Convex offers 2 types of integrations: standard and custom.

### Standard integration

Standard integration provides property-based data transfer to your CRM through predefined
standard mapping. The integration continuously monitors data in the Convex and your CRM
platform. When changes are detected, it automatically updates the outdated system to keep
both platforms in sync.

Convex standard integration works with three CRM platforms:

- Salesforce

- HubSpot

- Pipedrive

The integration facilitates data transfer from Convex to these CRM platforms through a Push to
CRM function, creating or updating records such as properties, companies, and contacts.

> **Note:** Reach out to your Customer Success Manager (CSM) to guide you through the setup
process.

### Custom integration

You can specify the exact data you want transferred to your CRM through a custom, non-
standard mapping tailored to your specific requirements. Anything that falls outside the
standard property-based transfer can be customized to meet your business's needs.

> **Note:** If you opt for custom integration, you will work with a 3rd-party trusted development
group to do this work.

## FAQ

#### What is the primary function of the Convex standard integration?

The Convex standard integration syncs key property-based data, such as company, property, and
contact information, between Atlas and CRM platforms such as HubSpot, Pipedrive, and
Salesforce, reducing manual work and ensuring data consistency.

#### What is the primary function of the Convex custom integration?

The primary function of the Convex custom integration is to enable tailored data transfer from
Convex to your CRM by allowing you to define exactly what data is transferred and how it's
mapped, beyond the standard property-based setup, to meet your specific business
requirements.

#### Is the data flowing through the standard integration secure?

Yes, security is a top priority. Data is stored securely within your organization's private Convex
account, and only authorized users within your organization can access the synchronized data.
Data moving between Convex and your CRM (HubSpot, Salesforce, Pipedrive) is encrypted.

#### What is required to set up a standard integration?

To set up a standard integration, follow these steps:

1. Generate API credentials for your CRM platform.

2. Provide the credentials to your Customer Success Manager (CSM).

The supported CRM platforms include:

- HubSpot

- Pipedrive

These credentials enable Atlas to communicate securely with the CRM system.

#### What is the purpose of the "Historical Data Pull" workflow?

The Historical Data Pull workflow is used to initially populate Convex with existing data from
your CRM. It usually runs once during the initial integration setup. This workflow queries the
CRM for relevant records and attempts to match them with existing records in Atlas.

#### How does the integration handle data discrepancies and updates between Atlas and the
CRM?

The integration includes mechanisms for ongoing synchronization to keep data accurate and
consistent. After the initial Push to CRM or Historical Data Pull, the integration continues to
monitor contact data across both systems (Atlas and the CRM). If changes are detected in one of
the systems, the integration identifies the outdated source and automatically updates it to align
with the more recent information. This ensures that both Atlas and the CRM reflect the latest
data.

#### How does the Push to CRM feature work?

The Push to CRM feature in Atlas is a user-initiated action that triggers an immediate data sync
from Atlas to your CRM. The integration then automatically creates or updates records
depending on the CRM and configuration within the CRM platform.

1. Go to the navigation menu and click Map, then select a property.

2. From the Properties details panel (PDP) that opens, click Push to CRM.

#### Can the integration be customized to fit specific business needs?

Yes, custom integrations allow you to define the exact data you want transferred and how it
should be mapped to fit your business requirements.

## Want to learn more?

- See Salesforce integration overview in Convex

- See HubSpot integration overview in Convex

- See Pipedrive integration overview in Convex
