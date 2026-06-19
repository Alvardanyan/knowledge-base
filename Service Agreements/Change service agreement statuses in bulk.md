# Change service agreement statuses in bulk

## Overview
Perform bulk status changes to efficiently update multiple Service Agreements at once. Apply status adjustments to streamline renewal preparation, maintain workflow consistency, and organize agreements in bulk.

## Who uses this feature
* Administrators, accountants, project managers, and operations managers
* Primarily benefits Commercial Service and Replacement business types, and Residential Service and Replacement business types
* Applies to all trades

## Things to know
* You can apply a bulk status change to agreements that are in compatible lifecycle stages.
* Bulk status changes can be applied to agreements in Draft, Active, and Auto-Renew statuses.

## Change service agreements status in bulk
1. Go to the navigation bar and click Follow Up.
2. In the side menu, click Service Agreements.
3. From the Service Agreements page, select the agreements you want to apply a bulk status change to.
4. Click Actions, and from the dropdown select Change Statuses.
![image alt](https://github.com/Alvardanyan/knowledge-base-portfolio/blob/da1d270f9e7751a97e9e87fc1610e7ae90bce21a/images/change-service-agreements-status-in-bulk-image-02ulpzpr.jpg)
5. From the pop-up that opens, select the new status you want to apply.
![image alt](https://github.com/Alvardanyan/knowledge-base-portfolio/blob/dcf3928a58af9c33ab5c758526a741fd4ddf5627/images/change-service-agreements-status-in-bulk-image-2zdwodhk.jpg)
6. When finished, click Change Statuses.

The **Statuses Changed Successfully** message appears to confirm that the new status has been applied.

The following status changes are allowed:

- From **Draft** → Sent, Accepted, Activated, Rejected.
- From **Sent** → Draft, Accepted, Rejected, Activated.
- From **Accepted** → Draft, Sent, Activated, Rejected.
- From **Rejected** → Draft, Sent, Accepted.
- From **Auto-Renew** → Draft, Sent, Accepted, Activated, Rejected.

> **Note:** If the agreement status is **Activated**, you can't change it.


## View errors
View, troubleshoot, and re-run the bulk actions if you received an error message.

1. Click **View Errors** on the error message.

A drawer opens where you can view the details of the error.

2. Click the **Agreement ID** to open the agreement in a new tab and fix the errors.

3. When finished, return to the drawer and click **Re-run Change Status**.

## Understand possible errors

View and understand the error types when changing the agreement status in bulk.

| Error Type        | Error Details                              |
|------------------|--------------------------------------------|
| Missing Fields    | All required fields must be filled.        |
| Invalid Status    | Cannot activate from Rejected.             |
| Other             | An unexpected error occurred.              |

## Want to learn more?
* See Create a service agreement step 6: Finalize Status
* See Follow up on service agreements
