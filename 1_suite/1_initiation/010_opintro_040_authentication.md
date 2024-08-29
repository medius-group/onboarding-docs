# Test

Once the test application tenant is created: 
* Users are required to authenticate to access the Onboarding Portal.
* The Onboarding Portal shares its authentication mechanism with the Medius suite.
* The Admin role is required, and any user with that role will be able to log in.
* If you have logged into APA, then you have also logged into the Onboarding Portal, and vice versa.
* An onboarding admin user account is set up by default upon test tenant creation, and the credentials for the account are sent to the primary contacts (as defined in the Onboarding Portal settings).
* **NOTE** that user creation within the Medius tenant may require a discussion with the implementation partner, as user profile creation is typically a dedicated project activity.
> *Please liaise with your implementation partner before creating accounts in the Medius tenant!*

# Production

When the production application tenant is created:
* You will need to authenticate against production instead of test. 
* A task for this purpose is available on platform level.
* When executing it you will be logged out and prompted for new log in. 
* After successful log in, any remaining deployment activities for production will be enabled.
