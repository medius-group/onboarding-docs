### Order based coding
Administration → Company → Orderbased → Coding
![](../../images/SAP_coding.png)

### Automatic coding order based invoices
Administration -> Company -> Virtual -> Enterprise -> Automatic coding -> Automatic coding order based invoices

Create it for header, line and unit price deviations, within tolerance and approved deviations.
(GL account for rejected deviations will vary between customers)
![](../../images/SAP_automatic_coding.png)

### Item Charge automatic coding order based invoices
1. Activate Item Charge Connection : Administration → Company → Order based → Matching
![](../../images/SAP_Itemcharge_matching.png)

2. Configure the automatic coding of item charge : Administration → Company → Enterprise → Automatic Coding 

    * Input "*" in Item Number and "PO Sub" in Coding. 
    * Choose always "Yes" for "Distribute Proportional" then a invoice amount will be splited proportionally by the connected PO amounts when a invoice line is connected to multiple PO lines. 
    
    ![](../../images/SAP_itemcharge_automaticcoding.png)



