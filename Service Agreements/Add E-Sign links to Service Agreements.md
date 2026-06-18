# Add E-Sign links to Service Agreements

## Overview

You can add an electronic signature link to your service agreements when you email them to your customers, allowing them to review and sign the agreements electronically. You can also set up alerts to get notified when a customer views or signs an agreement.

## Things to know

- Enable service agreement-related alerts to notify employees when a customer views or signs an agreement.
- Adding the E-Sign component to an existing Service Agreement template does not impact Service Agreements with Activated status.

## Who uses this feature

- Administrators, accountants, estimators, project managers, and operations managers
- This feature is restricted and only available for The Works Package
- Primarily for Commercial Service and Replacement

## Feature configuration

- Account configuration is required to use this feature. Please contact Technical Support for details.

# Create service agreement document template

ServiceTitan provides a pre-designed service agreement template already set up with basic design elements and components that are ready for printing.

However, these templates are not editable. For example, you may want to customize your service agreement document to have the E-Sign feature by business unit.

To quickly start creating a service agreement template customized for your business, we recommend making a copy of a pre-designed template and customizing it to suit your branding and business requirements.

1. Go to the top toolbar and click Settings > Operations > Document Templates.
2. Search for the Service Agreement - ST Default template and click More > Duplicate.
   
   ![Alt text](https://github.com/Alvardanyan/knowledge-base/blob/7c7bd6fe8cbaddfd851ebab0d0dbc8a3111d49eb/images/add-e-sign-to-service-agreements-image-0m4rwbw1.png)
4. On the Copy template screen that opens, enter a new Template name and leave the Template Type as Service Agreement.
5. When finished, click Duplicate.
6. From the Template Manager page, edit your content as needed:

   a. Edit the template details: The Template Details section lets you define the print settings of your invoice template, such as paper size, page margins, and more.

   b. Edit the template design: The Template Design section lets you add components to your invoice template. Components are placeholders that contain the elements essential to your invoice. For example, placing a Bill To component on the template means the Bill To customer appears on that area of the invoice you designated.

   c. Add E-Sign component: Drag the E-Sign component to add it to your Service Agreement Document Templates to deliver service agreement proposals electronically with an electronic signature link.

   ![Alt text](https://github.com/Alvardanyan/knowledge-base/blob/7c9bda957d4be789c677294f1c6d52d7299b65cb/images/add-e-sign-to-service-agreements-image-e0u8m7sr.png)

7. When finished, click Save and Publish.

# Customize E-Sign component

After you drag the E-Sign component and add it to the desired section of your Service Agreement document template, follow these steps to customize the E-Sign type from the Content window:

1. Sign Label: You can click Edit to customize the Sign label name. To hide a selection, click Show so it changes to Hide.

2. Choose the Signature Type: E-Sign offers four different field types. Click the Type dropdown to select one of the following options:

   a. Signature – The customer's full signature.

   b. Initials – The customer's initials.

   c. Date Signed – The date the Service Agreement was signed.

   d. Full Name – The customer's full name.

3. Use Multiple Components if Needed: Each E-Sign field must be added separately. If you need a Signature, Date signed, and Initials, you need to place three separate E-Sign components in the document.

# Create Service Agreement email template

Boost your brand by customizing your email templates with information specific to your business. To create a default email template for Service Agreement proposal emails, follow these steps:

1. Go to the top toolbar and click Settings.
2. In the side panel, go to Invoicing > Emails.
3. On the Email Settings screen that opens, click Service Agreements.
4. Add your company name and email in the Name and the Sender email fields under the From section.
5. (Optional) In the BCC field, enter the name and email address to which you want to send a blind carbon copy of the Service Agreement. Customers cannot see the BCC recipient in their email.
6. In the Subject field, enter a subject line for your email. For example, you can enter: "Your Service Agreement from [your company name]."
7. In the Body field, add placeholders for the information you want to show up on the email. Placeholders let you add customer-specific content to your templates. For example, start the email with "Hello {CustomerName}" and continue from there. When the email is sent, {CustomerName} is replaced by the full name of the customer. You can also:

   - Add a clickable link to your business, as well as your company logo, to the body of the email. If you use social media, add those links, too. For more, see HTML code.

   Note: The BCC field is not available for E-Sign email templates.

   Tip: If you want to know which Service Agreement you're referring to, add the {ServiceAgreementName} placeholder to the Subject field.

   - If you run multiple businesses, use the {BusinessUnitName} and {BusinessUnitPhoneNumber} placeholders in the statement email template to help your customers identify the company they did business with, in the statement email.

   - To add an electronic signature link to your email template, make sure to add {OnlineServiceAgreementLink} to the default email Body. This automatically includes the electronic signature link in future service agreement emails.

8. In the Preview section, check to ensure everything looks correct, and then click Save.

# Send Service Agreements with E-Sign component

When you customize the service agreement template to include the E-Sign component, the link appears anytime you send the SA email to a customer.

![Alt text](https://github.com/Alvardanyan/knowledge-base/blob/7c9bda957d4be789c677294f1c6d52d7299b65cb/images/add-e-sign-to-service-agreements-image-6b5eugon.jpg)

Note: Use these placeholders if each customer is assigned to only one business unit.

When the customer opens the email and clicks the agreement link, they are taken to the SA website, which displays all the details. Here, they can View and Sign Agreement.

After signing, the customer receives a copy of the signed agreement through email.

The service agreement now has the Accepted status. Change it to Activated to proceed.

# Create Service Agreement alerts

Use alerts to notify office employees and technicians when a customer views or signs a service agreement. Use alerts to ensure that your entire staff stays on track and up-to-date.

1. Go to the top toolbar and click Settings.
2. In the side panel, click Integrations > Alerts.
3. In the Alerts section that opens, click Add to add a new alert.
4. In the Add alert window that opens, enter the alert details:

   a. Type: Select the Customer Viewed Service Agreement or Customer Signed Service Agreement alert. The alert details open according to the alert type you selected.

   b. Delivery Method: Select the channel by which you want to send the alert.

   c. Recipients: Enter the name of the users who you want to get the alert.

5. When you're finished, click Save.

# Send service agreements to customers

Email the Service Agreement proposal to your customers with the E-Sign.

1. After reviewing the agreement in step 7 of creating a service agreement, click Send.
2. In the Send Service Agreement window, fill out the following fields:

   a. From: The email address the agreement is sent from. This field will pre-populate from the service agreement email template setup.

   b. To: The email address(es) the agreement is sent to.

   c. Subject: Subject of the email. This field will pre-populate from the service agreement email template setup.

   d. Summary: Body of the email. This field will pre-populate from the service agreement email template setup.

   Note: Both Email and SMS method is selected by default.

   e. Require E-Sign: This checkbox will be selected if the service agreement document template you selected includes an E-Sign component in Step 1: Summary and Design of the service agreement creation process.

3. Make sure the Include proposal PDF email box is checked to include the proposal PDF in the email.
4. Click Send to email the proposal with the attached PDF to the customer.
5. When the agreement is successfully emailed, the agreement status is automatically updated to Sent.

# Want to learn more?

- Visit ServiceTitan Academy and enroll in Creating & Managing Service Agreements
- See Create a service agreement step 1: Summary and design
