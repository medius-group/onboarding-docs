---
path: "/capture/company-setup/setup-company-structure"
title: "Determine fields to capture"
section: "Company"
module: "Medius Capture"
next: "/capture/medius_capture_1_createtenant"
tags: []
---
In order to achieve an efficient end-to-end process it is important to determine what fields that are relevant to capture from your invoices. 

Capture of fields are done at both header an line level. The settings of what header and line level fields that should be active is determined by the layout of the invoice. Thus, some information that is captured at header level for one supplier could be captured at line level for another, e.g. order number.

When determining what field that is relevant for you to include in capture please follow the below general guidelines:
1. Only include fields that are available on the invoice - no fields should be enabled for the purpose of manual keying
2. Only include fields that fulfils a purpose in the processing of the invoice

Field activation can be done at different levels:
## Tenant activation
Fields that are active at tenant level are the fields that are relevant for your organization to capture across ALL legal entities and ALL suppliers
## Company activation
All fields that are active at tenant level can be utilized in a company context. Fields can be configured in 3 different ways at company level.
### Active/Inactive 
Determines whether all tenant fields or a subset of fields are relevant for this particular company code
### Active - enabled by default
Fields that are active and enabled by default will be active and captured for new suppliers. Use this setting for fields that are expected to be active for a majority of your suppliers.
### Active - disbaled by default
Fields that are active and disabled by default will not be active for new suppliers. You have to enable the field at supplier level to make it available for capture. Use this setting for fields that are expected to be active for just a few of your suppliers.

