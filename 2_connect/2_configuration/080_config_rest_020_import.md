## Master data import
When authentication is in place, it’s time to start with Master data import.

You can read about the how to run the master data: [Running the master data flow](https://success.mediusflow.com/documentation/integration-documentation/technical/rest/scenarios/#running-the-master-data-flow)

Start with a simple entity, i.e. Currency rates.

Important considerations regarding Master data import are:

1. Import structure, [how much data should be sent](https://success.mediusflow.com/documentation/integration-documentation/technical/general/#how-much-data-can-be-sent)
2. [Import order of master data entities](https://success.mediusflow.com/documentation/integration-documentation/technical/rest/generalconsiderations/#import-order-of-master-data)
3. [Master data external system id's](https://success.mediusflow.com/documentation/integration-documentation/technical/rest/generalconsiderations/#master-data-external-system-ids)
4. [Handling cloud maintenance and outage](https://success.mediusflow.com/documentation/integration-documentation/technical/rest/generalconsiderations/#handling-cloud-maintenance-and-outages)

Now it’s time to look at how to set-up a master data scenario: [Running the master data flow](https://success.mediusflow.com/documentation/integration-documentation/technical/rest/scenarios/#running-the-master-data-flow)

To get help in sending your first master data entity, either use the [Test portal](https://cloud.mediusflow.com/$TenantNameQA/api/documentation/) or the [Postman collections](https://success.mediusflow.com/documentation/integration-documentation/technical/rest/specification/#postman-collections).

After you have sent a master data batch to Medius AP Automation, you should have a look at the import que in Medius AP Automation: [Import management](https://cloud.mediusflow.com/$TenantNameQA/#/configuration/ImportManagement).
