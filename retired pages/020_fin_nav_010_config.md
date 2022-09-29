## Settings in Medius for Orderbased Invoices

### Order based coding
Administration → Company → Orderbased → Coding
![](../../images/NAV_coding.png)
Note that this may not be best practice for NAV. In most cases there is no need to modify the order cost coding so it should be locked. If the coding is changed it's important that the account "PO Coding" remains intact for the integration to work.

### Automatic coding order based invoices
Administration -> Company -> Virtual -> Enterprise -> Automatic coding -> Automatic coding order based invoices

Create it for header, line and unit price deviations, within tolerance and approved deviations.
(GL account for rejected deviations will vary between customers)
![](../../images/NAV_automatic_coding.png)

### Item Charge automatic coding order based invoices
1. Activate Item Charge Connection : Administration → Company → Order based → Matching
![](../../images/NAV_Itemcharge_matching.png)

2. Configure the automatic coding of item charge : Administration → Company → Enterprise → Automatic Coding 

    * Add a "Item Number" and/or "Description" filter to identify the item charges that should be auto coded. Wildcards can be used, i.e. "Freight*".
    * Set the corresponding coding for the identified item charge using the prefix for "Item charge", i.e. "IC FREIGHT".
    * "Distribute Proportional" must be "No" for the NAV integration as the split will be done in the ERP system using the specified IC type. 
    
    ![](../../images/NAV_itemcharge_automaticcoding.png)
