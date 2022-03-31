---
path: "/api/2_rest/1_design"
title: "Integration design"
section: "Medius REST API"
module: "ERP Integration"
next: "/api/2_rest/2_testtools"
tags: ["api_rest"]
---
Since you have chosen to use Medius REST API, you have the possibility to set-up an integration that works in the way you want and take advantage of all features Medius AP Automation has to offer.

To be able to get through this process, there need to be a cooperation between your Medius AP Automation solution contact for guidance and your integration and AP resources. Building an integration requires Medius AP Automation knowledge to be able to make decisions regarding Master data and how postings to ERP should behave.

Depending on your scope, what modules that will be used in Medius AP Automation, the approach to the integration can differ. 

* If you only have Expense invoices, the amount of transaction heavy master data imports are probably limited. But if you have lots of Purchase orders the master data transactions can be quite frequent. 
* When building the integration, try to think about how the invoice should be posted in the ERP in the end. That will often tell you what type of master data that would be needed, how frequent master data needs to be exchanged, what information that would be of interest in the posting message. 
* Consider how your ERP works, sometimes information could be fetched at invoice posting directly from ERP instead of the need for master data import and then fetch it again in ERP posting.

You can find all the necessary information on the main page for our [Integration Success documentation](https://success.mediusflow.com/documentation/integration-documentation/). The following pages will try to guide you how to set up communication and how to work with our API's.
