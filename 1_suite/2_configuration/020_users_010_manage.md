Each person within the organization that will do work within Medius, needs a user. The users span between account payable users to users that seldom approves invoices.
A few options exist for how to do this. The recommended way is to use one of the standard services to avoid manual maintenance of users within Medius.


## Office 365(Azure AD)
Most companies have started using Office 365 from Microsoft, which means that the users within the organization is already synced with Microsoft's cloud services.
Medius have a pre-packaged service that fetches users from Azure AD and also allows logging in with the same credentials as used for all other Office 365 applications.

The simplest way to get going is to visit the 
[Azure marketplace](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/aad.mediusflow?tab=Overview)

If more information is needed use the official docs from Medius at the 
[Medius success portal](https://success.mediusflow.com/documentation/administration_guide/user_login_and_transfer/office365userintegration/)

## AD and ADFS

If your organization has not embraced the Office 365 services, there is an alternative to install a component on a server within the network that upload users from the Active Directory to Medius.

To be able to authenticate the users, a local ADFS server must be in place at within your network.

[Read more here](https://success.mediusflow.com/documentation/administration_guide/user_login_and_transfer/adfs/#)

## Custom user transfer

In rare cases the standard user transfer is not enough, e.g. when a company wants to streamline the onboarding of new users even more. If this is the case, the REST API for Medius can be used.

The documentation for the REST API can be found at the [success portal](https://success.mediusflow.com/documentation/integration-documentation/getting_started/rest/)

When the custom user transfer is used, the authentication possibilities varies dependent of need. The standard ADFS and Azure AD authentication might not be working with custom build user transfers, so please verify that in advance.
