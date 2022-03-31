---
path: "/api/1_fx/3_postings"
title: "Posting messages of invoices from Medius"
section: "Medius FX API"
module: "ERP Integration"
next: "/api/1_fx/6_last"
tags: ["api_fx"]
---
After master data has been imported and Medius AP Automation has been configured, there is time to start work with the posting files. 

Invoices ready for postings can be found in Medius AP Automation GUI, [Message management](https://cloud.mediusflow.com/$TenantNameQA/#/configuration/MessageManagement).

Postings consist of a Request message followed by Response. Start with the Request message which you can find information about here, [Invoice postings data specification](https://success.mediusflow.com/documentation/integration-documentation/technical/fx/specification_postings/).

After an invoice has been posted to ERP, it's time to look at reading back a response. Either a Voucher, Error or Payment information. Read more about [Invoice posting responses](https://success.mediusflow.com/documentation/integration-documentation/technical/fx/specification_responses/).