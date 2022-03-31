---
path: "/erp/4_d365bc/1_deploy_connector"
title: "Deploy the connector in Business Central"
section: "D365 Business Central"
module: "ERP Integration"
next: "/erp/4_d365bc/1b_hcm_installation"
tags: ["d365bc"]
---
For integration with D365BC, Medius need an extension to be installed for each D365BC Instance to be connected. The Extension will only add stand-alone objects, no existing objects will be replaced. Timestamp fields will be added to some master data tables using TableExtension (not interfering with existing standard objects). The extension code will be used for setting up the integration, fetching data from D365BC and for posting invoices to the ERP.

## For D365BC OnPremise
You will receive the Extension Package from you Medius integration consultant. The extension needs to be installed/upgraded by you as a customer or your D365BC Partner.
In the next step you will also install the HCM component that will act as a secure tunnel to the local network to reach the BC On-Premise instance.

**Important!** Before you can use the extension objects your license needs to be updated to include the Medius code module. To accomplish this you need to provide your customer license number and send this to your Medius consultant so your customer license can be updated. When the module is added to your license you need to create a new license file to be imported to your D365BC instance.

## For D365BC Cloud
For D365BC Cloud you can download the Extension from the Extension Marketplace, either by navigating there through your web client and then then search for "Medius - AP Automation" or use the direct link here: [D365BC - Medius AP Automation](https://appsource.microsoft.com/en-us/product/dynamics-365-business-central/PUBID.medius%7CAID.mediusflow-d365bc%7CPAPPID.c055570e-7914-4f44-8f10-6aa9d377495c?tab=Overview)

**Note!** For the Cloud Extension there is no need for any addition to your customer license.

## General information
More information on how to deploy the objects in Microsoft Dynamics can be found here: 

[D365BC – Deployment guide](https://success.mediusflow.com/documentation/cts-documentation/Cloud-Connectors/D365BC/D365BC_technical/D365BC_deploymentguide/)

More information about what the extension contains can be found in the product definition here: 

[D365BC – Integration Product Definition](https://success.mediusflow.com/documentation/cts-documentation/Cloud-Connectors/D365BC/D365BC_product/#integration-package-content)
