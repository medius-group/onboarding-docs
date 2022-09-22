
> This relates to deviations between a purchase order invoice and the connected goods receipts.

How to automatically code deviations is something that depends on how your organization handles this situation, and any ERP specific instructions. 
At what level in the company hierarchy these settings need to be added might also be different from one client to another. 
We should try to put them on the virtual company for the ERP if possible.

The instructions below shows how the wizard works and how to set the deviation coding to either coding the invoice to the same coding as the po (SaC) or to a specific account - two of the most common configurations.

Go to Administration --> Company -->[Company]--> Enterprise--> Automatic coding.

First, set up the rules for coding deviations that are within tolerance.

1.	Click on the tab Automatic coding of order-based invoices 
2.	Click the **Save** button
3.	Pick the "External Purchase Order (defined in ERP)" option in the dialogue that pops up
    * "Internal Purchase Order (defined in Medius AP Automation)" is only used together with the **Procurement** module
 
4.	Click the “Next” button
5.	Pick the "Head total amount deviation" option
 
6.	Click the “Next” button
7.	Pick the "Within tolerance" option
 
8.	Click the “Next” button
9.	Pick the "Split proportional" option
 
10.	Click the “Next” button
11.	Pick the "Same as cost" option
12. Click the "Create" button

Repeat these steps for all the options in the Type of Deviation screen, except "Exception type deviation" (there is no "within tolerance" option for this type):
* Head total amount deviation
* Line total amount deviation
* Unit price deviation
* Quantity deviation

Second, set up the rules for coding deviations that are out of tolerance.

1.  Click on the tab Automatic coding of order-based invoices
2.	Click the **Save** button
3.	Pick the "External Purchase Order (defined in ERP)" option in the dialogue that pops up
    * "Internal Purchase Order (defined in Medius)" is only used together with the **Procurement** module
  
4.	Click the “Next” button
5.	Pick the "Head total amount deviation" option
 
6.	Click the “Next” button
7.	Pick the "Out of tolerance" option
 
8.	Click the “Next” button
9.	Pick the "Split proportional" option
 
10.	Click the “Next” button
11.	Pick the "Coding deviation depending on analysis" option
 
12.	Click the “Next” button
13.	Check the "Deviation approved" checkbox and pick the "Same as cost" option
14. On the other side are rejected deviations, this is even more likely to be client specific than other steps 
    * To put rejected deviations on a specific account (while waiting for a credit) or a dummy account to indicate short pay:
        i.	Check the "Deviation rejected" checkbox 
        ii.	Specify the appropriate code string
 
15.	Click the “Create” button

Repeat these steps for all the options in the Type of Deviation screen:
* Head total amount deviation
* Line total amount deviation
* Unit price deviation
* Quantity deviation
* Exception type deviation

Approved deviations of the "Exception type deviation" should more or less always be coded "Same as Cost".
