---
path: "/mediusflow/application-related/2_expense_flow_configuration"
title: "Expense invoice application settings"
section: "Application settings"
module: "AP Automation"
next: "/mediusflow/application-related/3_match_flow_configuration"
tags: ["invoice"]
---
This section covers the expense invoice application settings that needs to be configured based upon your organisation's structure and processes. 
We recommend that this is done in cooperation with your implementation partner that can guide you through this process.

Before getting started we recommended to study the introduction to [Expense invoice workflow](https://success.mediusflow.com/documentation/administration_guide/applications/invoice/workflow/) and go through all workflow steps presented in subpages. 
Based on your findings and preferred workflow Medius should be configured in the areas presented below in the sub-pages.

## Expense invoice application responsible settings
In Medius you can assign users or roles to be responsible for different steps in the expense invoice workflow. 
These settings determine what users, or group of users, are responsible to perform certain tasks.

The best practice is to assign roles instead of individual users. This will enable shared workload as well as easier administration if
there are changes within your organization.

Verify standard setup or apply desired adjustments here: [Enterprise responsible settings](https://cloud.mediusflow.com/$TenantNameQA/#/Administration/Medius.Core.Entities.Company).

1. Choose what Company to apply settings to. It is recommended to apply settings at virtual level for minimal administration.
2. Go to tab "Expense".
3. Go to sub tab "Responsible".

Read more about these settings [Expense invoice responsible documentation](https://success.mediusflow.com/documentation/administration_guide/administration_pages/company/expense/#responsible).

## Business rule settings
Much of the expense invoice workflow is determined by business rule configuration. It is not a requirement to adjust business rule settings yourself, but these can be reviewed and adjusted to fit your organization's processes and needs together with your implementation partner. 

Here you will find a complete list of the business rules for expense invoices to be verified: [Expense invoice business rules](https://success.mediusflow.com/documentation/administration_guide/perspectives_and_business_rules/#expense-invoice).



