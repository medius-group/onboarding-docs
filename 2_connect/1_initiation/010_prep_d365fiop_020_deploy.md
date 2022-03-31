---
path: "/erp/3_d365fiop/1_deploy_connector"
title: "Deploy Connector in D365FO"
section: "D365 Fi&Op"
module: "ERP Integration"
next: "/erp/3_d365fiop/1b_hcm_installation"
tags: ["d365fiop"]
---
For integration with D365FO, Medius need a D365FO Deployable Package installed. The deployable package contains stand-alone objects and will not override any existing objects in D365FO. The objects consists of X++ classes that is used for setting up the integration, fetching data from ERP and for posting invoices to the ERP. (X++ is the programming language in AX/D365FO)

Installation of the deployable package is done by customer (customer's erp-partner). The customer is responsible for maintaing Medius deployable package together with other 3rd part packages and upgrades/installation of their ERP.

## More information ## 
How to install the deployable package is describeb here:

[D365FO – Deployment guide](https://success.mediusflow.com/documentation/cts-documentation/Cloud-Connectors/D365FO/D365FO_technical/D365FO_deploymentguide/ "LCS Deployment guide")