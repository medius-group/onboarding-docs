### Queue deployment tasks

If you have choosen to create an empty tenant, then activation will be queued to be executed as soon as any prerequisites are met. If you opt to copy from test to production, then:

* Modules that are active in QA and require no further deployment will be automatically activated.
* These modules will automatically display a 'pending' status as soon as the tenant request has been made.
* The activation of other modules can be queued.


<DeploymentQueueModules deploymentTask="Deploy_Production_Tenant"/>
