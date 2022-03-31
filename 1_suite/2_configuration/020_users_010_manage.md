---
path: "/userimport/user-auth-introduction"
title: "How to get the user into MediusFlow"
section: "User import introduction"
module: "User Import"
next: "/erp/1_sap/1_technical_requirements"
tags: []
---
Each person within the organization that will do work within Medius, needs a user. The users spans between account payable users to users that seldom approves invoices.
There exists a few options for how to do this, the recommended way is to try to use one of the standard services for this to avoid manual maintenance of users within Medius.
[Medius Service](https://cloud.mediusflow.com/$TenantNameQA)


## Office 365(Azure AD)
Most companies have started using Office 365 from Microsofts, which means that the users within the organization is already synced with Microsofts cloud services.
Medius have a pre packaged service that fetches users from Azure AD and also allows logging in with the same credentials as used for all other Office 365 applications.

The simplest way to get going is to visit the 
[Azure marketplace](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/aad.mediusflow?tab=Overview)

If more information is needed use the official docs from Medius at the 
[success portal](https://success.mediusflow.com/documentation/administration_guide/user_login_and_transfer/office365userintegration/)

## AD and ADFS

For companies that have not embraced the Office 365 services, there is an alternative to install a component on a server within the network that upload users from the Active Directory to Medius.

To be able to authenticate the users, a local ADFS server must be in place at the customer network.

[Read more here](https://success.mediusflow.com/documentation/administration_guide/user_login_and_transfer/adfs/#)

## Custom user transfer

In rare cases the standard user transfers is not enough, e.g. where a company wants to streamline the onboarding of new users even more. When this is the case, the REST API for Medius can be used.

The documentation for the REST API can be found at the [success portal](https://success.mediusflow.com/documentation/integration-documentation/getting_started/rest/)

When the custom user transfer is used, the authentication possibilities varies dependent of need. The standard ADFS and Azure AD authentication might not be working with custom build user transfers, so please verify that in advance.
