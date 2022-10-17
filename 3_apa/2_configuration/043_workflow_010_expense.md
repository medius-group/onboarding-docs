Go to Administration --> Company Business Rules

Inactivate any business rule that shouldn't be used in each of the perspectives listed, and change the priority if the rules left active as appropriate. The list of perspectives below is not exhaustive, but they are more commonly visited during a system configuration than others and should be addressed. Information about all perspectives and business rules can be found [here.](https://success.Medius.com/documentation/administration_guide/perspectives_and_business_rules/#content-start)

1. Medius.PurchaseToPay.Platform.RulePerspective.InitialDistributionPerspective
    * Determines the initial routing of expense invoices. Typically used for bypassing the AP staff. The fallback is to stop invoices for manual routing.

2. Medius.ExpenseInvoice.Platform.RulePerspective.ExpenseSingleDistributionPerspective
    * Determines where to route invoices for the Code and Distribute workflow step. Typically, not changed from the APRole entry, which routes invoices to the user/role specified as responsible for this workflow step in the company settings.

3. Medius.PurchaseToPay.Platform.RulePerspective.FetchResponsibleUserPerspective
    * Determines how the Authorizer column is populated when clicking the "Fetch authorizer" button in the Coding tab of an invoice.
