# Scope of work: Add forms to service agreement visits (tasking)

## Overview

Add forms to the service agreement visit by associating them with a service directly in Step 4: Scope of work. This gives you visibility into linked forms and lets you add or remove them at the visit level, ensuring technicians know exactly what work to perform and which forms to complete.

## Who uses this feature

- Administrators, estimators, project managers, operations managers, and CSRs
- Primarily benefits Commercial Service and Replacement business types
- Applies to all trades

### Feature configuration

- Account configuration is required to use this feature. Please contact Technical Support for details.

## Things to know

- The feature works best when paired with the ServiceTitan Field Mobile App.

- Associate a form with a service in 2 ways:
  - Manually, when creating a service agreement visit: Select a form you want to attach each time you create a Service Agreement visit.
  - Automatically through the Pricebook: Associate the form with a service in the Pricebook so that whenever the service is added to a service agreement visit, the form comes along with it by default.

- Only forms that meet the following criteria are available for association with a service:
  - The status is Published.
  - Assigned to a Job.
  - The type is ST Form.

## Benefits of using this feature

- Accurate cost estimation and consistent execution: By adding services and forms directly to Service Agreement Visits, you can estimate the cost of each agreement up front and ensure every technician follows the same standardized process. This lets you plan with confidence, no more spreadsheets or external tools. Attaching required inspection, safety, and compliance documents at the visit level guarantees consistent field execution, regardless of who dispatches the work.

- Upfront customer communication: Include services directly in the agreement document, ensuring your customers understand what's planned. The services, the equipment that those services will be performed on, and the materials that will be used are all exposed to the Document Template Engine (DTE) for inclusion in the customer-facing agreement document.

- Clear Technician Guidance: Technicians know exactly what work to perform and which forms to complete when they arrive at the job. This minimizes errors and reduces unnecessary back-and-forth with the office. For more information, see Track equipment-related tasks for a Service Agreement visit in the ServiceTitan Field Mobile App.

- Post-visit customer communication: Customers receive clear invoices showing what was completed, enhancing trust and satisfaction. No extra post-visit effort is needed to itemize exactly what was performed, as the data is already there.

> **Note:** Select the Scope of Work Services and Scope of Work Materials components when creating a document template for Service Agreements to reflect this.

- Equipment Service History: The only way to populate equipment service history is by associating the services and materials with the actual installed equipment. Instead of relying on technicians to spend more time tapping on their iPads, associate the services with the equipment when building the visit. This is the highest upstream way to ensure that you build equipment service history over time, with no extra effort required from technicians. For more information, see Manage installed equipment.

- Pricebook alignment: Extend Pricebook automation to service agreement visits by linking forms to specific services, such as RTU Maintenance Checklist or Boiler Inspection Form. This ensures alignment between office workflows and field execution while saving time.

## Add forms to visit

1. On the Scope of Work screen, click +Add Visit or Edit (icon).
2. On the Edit Visit screen that opens, scroll down to the Services section.
3. Click +Add Service.
4. From the list, select a service and click Add Service.
5. Click the Equipment (Optional) dropdown to link the service to the Installed Equipment you added in Step 3: Equipment for the service location.
6. From the Forms column, click the dropdown and select a form.
7. Enable the toggle Required to make the form mandatory for the technician to complete. For a mobile view, please see Track equipment-related tasks for a Service Agreement visit in the ServiceTitan Field Mobile App.
8. When finished, click Update Form.

After the agreement is activated and the visit is booked into a job, technicians can see the service and forms associated with the job.

> **Tip:** For an accurate, prescriptive technician experience, we strongly recommend associating each service with the installed equipment on which it will be performed. This ensures technicians see the correct instructions, history, and required forms at the visit.

> **Note:** If the service already has a form associated with it in the pricebook, it appears automatically.

## Want to learn more?

- See Create a service agreement step 3: Equipment
- See Create a service agreement step 4: Scope of Work
- See Track equipment-related tasks for a Service Agreement visit in the ServiceTitan Field Mobile App
- See Create document template for Service Agreements with Template Manager
- See Manage installed equipment
