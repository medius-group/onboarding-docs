---
path: "/mediusflow/application-related/5_contract_flow_configuration"
title: "Recurring Invoice functionality workflow settings"
section: "Application settings"
module: "AP Automation"
next: "/userimport/user-auth-introduction"
tags: ["contract"]
---
This section covers the Recurring invoice application settings that need to be configured based upon your organization's structure and processes. 
We recommend that this is done in cooperation with your implementation partner that can guide you through this process.

If you want to learn more about Medius Recurring Invoice functionality you will find more information at the links below:
* [Supplier contract](https://success.mediusflow.com/documentation/user_guide/supplier_contract/)
* [Recurring invoices](https://success.mediusflow.com/documentation/user_guide/contract_based_invoice/)

Before getting started it is recommended to study the introduction to [Recurring invoice workflow](https://success.mediusflow.com/documentation/administration_guide/applications/contract/workflow/) and go through all workflow steps presented in subpages. 
Based on findings and preferred workflow Medius should be configured in the areas presented below.

## Recurring invoice application responsible settings
In Medius you assign users or roles responsible for different steps of the process. 
These settings determine what users or group of users that are responsible to perform certain tasks.

Best practice is to use roles instead of individual users to be able to share workload as well as easier administration if 
there are changes to responsibilities/teams. 

Verify standard setup or apply desired adjustments here: [Supplier contract responsible settings](https://cloud.mediusflow.com/$TenantNameQA/#/Administration/Medius.Core.Entities.Company).

1. Choose what Company to apply settings to. It is recommended to apply settings at virtual level for minimal administration.
2. Go to tab "Contract".
3. Go to sub tab "Responsible".

Read more about these settings [Recurring invoice responsible documentation](https://success.mediusflow.com/documentation/administration_guide/administration_pages/company/contract_based/)

## Business rule settings
Much of how the workflow is with business rule configuration. It is not required to adjust business rule settings but they should be reviewed and confirmed/adjusted to fit your organization's processes and needs. 

Here you will find a complete list of the business rules for Recurring invoice application to be verified: [Recurring invoice application business rules](https://success.mediusflow.com/documentation/administration_guide/perspectives_and_business_rules/#expense-invoice).



