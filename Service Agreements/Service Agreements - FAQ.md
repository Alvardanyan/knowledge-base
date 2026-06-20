# Service Agreements - FAQ

## Initial setup

### How can I enable the Service Agreements features for my account?

This feature requires account configuration. Please contact Technical Support for details.

### Now that the Service Agreements feature is enabled, what do I need to configure to begin using the features?

Create a service agreement template.

## Service agreement templates

### When is tax calculated?

Tax is calculated when invoices are generated. If you want to include tax to the invoice amounts, make sure to mark the Pricebook Services used by the Service Agreement Template as taxable.

## Proposals

### How do I create a new proposal?

From the Customer or Location screen, select Create Agreement to enter the proposal creation workflow.

### Why isn’t the PDF downloading?

Check your browser’s pop-up blocker, it may be blocking the download.

### How do I edit an existing proposal?

From the Customer or Location screen, go to the Service Agreements table and select the proposal that you would like to edit.

### Why can’t I update a proposal’s status?

There might be incomplete or invalid data in the proposal:

• A workflow step may be incomplete

• Proposed Start Date is in the past

• Visit Window(s) are outside of Service Agreement Duration

• Invalid Duration and Billing Schedule combinations

Enter the proposal creation workflow to rectify these issues before updating the proposal’s status.

## Billing Schedule

### What are the Billing Schedule options?

The billing schedule options available for Service Agreements are the following:

• Time of Service

• Upfront

• Annual

• Biannual

• Quarterly

• Every Other Month

• Monthly

### Why can’t I select certain Billing Schedule options?

If the duration or the agreement is not evenly divisible by 12 months, only the following options are available:

• Time of Service

• Up-front

• Monthly

## Activating an agreement

### What does activating an agreement mean?

Activating the agreement allows you to begin creating requisitions to purchase materials and scheduling visits for the agreement.

### What does the agreement Start Date signify?

It’s when the client-specific pricing (CSP) rules and other things take effect, it is also the official date to calculate the end date and therefore the renewal date. It is also used as the first billing date and starts the billing schedule.

### Why can’t I activate an agreement?

There might be incomplete or invalid data in the proposal:

• A workflow step may be incomplete

• Proposed Start Date is in the past

• Visit Window(s) are outside of Service Agreement Duration

• Invalid Duration and Billing Schedule combinations

Enter the proposal creation workflow to rectify these issues before updating the proposal’s status.

## Visits

### What are Visits and how are they different from Jobs and Appointments?

Visits are best thought of as placeholders for future Jobs and are used to plan the schedule of service for an agreement.

Visits are booked into Jobs, which can then be broken out into Appointments, if necessary. Once a Visit has been booked into a Job, all of ServiceTitan’s existing job functionality becomes available: Job Summary, Preferred Technician, scheduling information, Job Invoice, and more.

### How can I view all of the Visits associated with a Service Agreement?

Go to the Service Agreement screen for the agreement that you wish to review, then click Visits in the left-hand navigation.

### How can I view the Visits associated with all of my Service Agreements?

Go to the Follow Up screen, then click Service Agreement Visits in the left-hand navigation.

### Whenever a visit is performed, how does ServiceTitan calculate the amount of revenue that is recognized?

The amount that is recognized when a visit is performed is proportional to the amount of work being done during that visit; this calculation is done automatically based on the visit cost estimates. For example:

• Total Agreement Price: $100

• Visit 1: 9 labor hours

• Visit 2: 1 labor hour

• (assume that the Labor Cost / Hour and Material Costs are equal for both visits)

When Visit 1 is performed, because it represents 90% (9 labor hours / 10 total labor hours) of the overall work, $90 will be recognized; when Visit 2 is performed, the remaining $10 will be recognized.

## Billing

### How do I generate invoices for Up-front, Monthly, Every Other Month, Quarterly, Annually, and Bi-annual, i.e. Non-Time of Service Billing Schedules?

Use the Recurring Billing feature to search by date range, then create a Recurring Billing Run to generate the invoices.

### For agreements using the Time of Service billing schedule, how does ServiceTitan calculate the job invoice amount?

To calculate the job invoice amount for a particular visit, ServiceTitan is using the Labor (including Extra Travel Time) and Material Costs Estimates for that visit and calculating that visit’s contribution to the Total Cost. That contribution percentage is multiplied by the sum of the Total Markup and Total Surcharge, and then added to the Visit Cost amount, see below:

(Visit Cost Contribution %)=(Visit Cost) / (Total Cost)

(Visit Invoice Amount)=( Visit Cost Contribution %) (Total Agreement Price)

Example:

• 2 Visits

• Visit 1 Cost Estimate = $300

• Visit 2 Cost Estimate = $100

• Total Agreement Price = $500

(Visit 1 Cost Contribution %) =(Visit Cost) / (Total Cost) = $300 / $400 = .75

(Visit 1 Invoice Amount)= (Visit 1 Cost Contribution %) (Total Agreement Price)

( Visit 1 Invoice Amount) = .75 $500

(Visit 1 Invoice Amount)=$375

. . .

(Visit 2 Invoice Amount)= .25 $500

(Visit 2 Invoice Amount)=$125

. . .

(Total Invoice Amount)= $375 + $125 = $500

. . .

(Total Invoice Amount)=( Total Agreement Price)

### How does ServiceTitan handle cases where the Total Agreement Price can’t be evenly divided amongst invoices (based on the agreement duration and billing schedule)?

ServiceTitan rounds down the invoice amount to the nearest whole cent, adding any remainder to the final invoice amount.

Example: $5,000 over 3 years (36 months) with monthly billing schedule

• Month 1 Invoice: $138.88

• Month 2 Invoice: $138.88

• Month 3 Invoice: $138.88

• . . .

• Month 35 Invoice: $138.88

• Month 36 Invoice: $139.20 (+$0.32 compared to all other invoices)

## Materials

### What is the Service Agreement Materials screen used for?

The Materials screen is used to store the required materials lists for each Visit. This is especially useful for Auto-renew agreements where the same materials are required from year to year.

### Do the materials that I add on the Service Agreement Materials screen automatically show up on the job invoice?

At the time of booking the Visit into a Job, any materials that have been added on the Service Agreement Materials screen automatically copy to the Job Invoice.

However, once the Job is booked, any changes made on the Materials screen will not automatically update the Job Invoice. Similarly, any changes made directly to the Job Invoice will not automatically update the Materials screen.

## Profitability

### When planning inventory, how do I report on the required materials across all Service Agreements?

Go to the Reports screen to access the Material Forecast report, which is built from the Service Agreement Visits data source. This report pulls the material lists from all Service Agreements and can be filtered by date range and other properties, and can be exported to aid in the creation of Purchase Orders in the Inventory module.

### Where are the Estimated Costs for each Visit defined?

Labor and Material Cost Estimates are defined in the proposal creation workflow on the Scope of Work step.

### Where are the Actual Costs for each Visit defined?

• Labor (Actual Cost): the sum of the LaborPayItems amounts from the job associated with the Visit

• Burden (Actual Cost): the sum of the LaborBurdenItem amounts from the job associated with the Visit

• Materials (Actual Cost): the sum of the cost of the materials items added to the job invoice associated with Visit

### How is Gross Margin / Labor calculated?

Gross Margin divided by the Labor Cost only (denominator does not include Burden Cost)

## Why don’t I see the Burden Cost?

This feature requires account configuration. Please contact Technical Support for details.
