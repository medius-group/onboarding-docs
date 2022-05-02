## Deployment of AX model and information needed for communication ##
For integration with Dynamics AX, Medius needs some objects to be installed in the ERP. The objects are stand-alone objects and will not override any existing objects in ERP. The objects consists of tables, forms and classes that will be used for setting up the integration, fetching data from ERP and for posting invoices to the ERP.

For AX2009 the objects are packaged in a xpo-file and for AX2012 they are packaged in a model-file.
Installation of the model/xpo is done by customer (customer's erp-partner). The customer is responsible for maintaing Medius model/xpo together with other 3rd part packages and upgrades/installation of their ERP.

**More information on how to deploy the objects in Microsoft Dynamics can be found here:** 

[AX - Deployment guide](https://success.mediusflow.com/documentation/cts-documentation/On-Premise-Connectors/AX/AX_technical/AX_deploymentguide/)
