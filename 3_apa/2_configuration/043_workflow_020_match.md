1. Medius.OrderbasedInvoice.Platform.RulePerspective.ConnectInvoicePerspective
    * Determines where Medius should look for orders where the vendor on the invoice is different from the purchase order.
    * How to automatically connect Purchase Order to Invoice

2. Medius.OrderbasedInvoice.Platform.RulePerspective.ConnectInvoiceLinePerspective
    * Determines what connection methods the system will utilize, and in what order.
    * Normally set to: Head Total --> Line Detail --> Line Total --> Manual
    * Connections to service based order lines are inactive by default and needs to be activated/prioritized.
    * How to automatically connect Goods Received to an invoice

3. Medius.OrderbasedInvoice.Platform.RulePerspective.Distribution.OrderbasedSingleDistributionPerspective
    * Determines where to route invoices for the Connect workflow step. Typically not changed from the APRole entry, which routes invoices to the user/role specified as responsible for this workflow step in the company settings.

4. Medius.OrderbasedInvoice.Platform.RulePerspective.DueDateDeviationPerspective
    * We typically do not utilize the due date matching.
    * Inactivate the Match entry

5. Medius.OrderbasedInvoice.Platform.RulePerspective.AnalyzeHeaderTotalAmountDeviationDistributionPerspective
    * Determines how the system tries to route Head Total deviations that are out of tolerance

6. Medius.OrderbasedInvoice.Platform.RulePerspective.AnalyzeLineAmountDeviationDistributionPerspective
    * Determines how the system tries to route Line Amount deviations that are out of tolerance

7. Medius.OrderbasedInvoice.Platform.RulePerspective.AnalyzeUnitPriceLineDeviationDistributionPerspective
    * Determines how the system tries to route Unit Price deviations that are out of tolerance

8. Medius.OrderbasedInvoice.Platform.RulePerspective.AnalyzeQuantityLineDeviationDistributionPerspective
    * Determines how the system tries to route Quantity that are out of tolerance

9. Medius.OrderbasedInvoice.Platform.RulePerspective.AnalyzeExceptionTypeUnitPriceLineDeviationDistributionPerspective
    * Determines how the system tries to route Unit Price deviations for ExceptionTypes that are out of tolerance

10. Medius.OrderbasedInvoice.Platform.RulePerspective.AnalyzeExceptionTypeLineAmountDeviationDistributionPerspective
    * Determines how the system tries to route Line Amount deviations for ExceptionTypes that are out of tolerance

11. Medius.OrderbasedInvoice.Platform.RulePerspective.Authorization.DeviationAuthorizationConfigurationPerspective
    * Activate TurnOnDeviationAuthorization if you want a check of Deviation Limits of the user approving a deviation and escalation if exceeded

12. Medius.OrderbasedInvoice.Platform.RulePerspective.Authorization.DeviationNextAuthorizerPerspective
    * Determines how deviations that has been escalated are routed. Typically, not changed.

13. Medius.OrderbasedInvoice.Platform.RulePerspective.Authorization.InvoiceAmountAuthorizationInitialDistributionPerspectiv
    * Determines how order-based invoices initially are routed for approval IF they have been stopped for approval by a Document Validation Rule.

14. Medius.OrderbasedInvoice.Platform.RulePerspective.Authorization.InvoiceNextAuthorizerPerspective
    * Determines how escalated order-based invoices are routed. Typically, not changed.
