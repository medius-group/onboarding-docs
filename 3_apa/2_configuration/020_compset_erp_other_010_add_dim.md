The coding dimensions in Medius AP Automation should reflect the financial Dimensions set up in your ERP. Once it has been determined what dimensions to make use of in Medius, go to **Administration > Company > [Virtual Company for ERP] > Enterprise > Dimensions**.

If you are not using an ERP-specific integration package provided by Medius, you will usually activate and label dimensions in sequential order, without any gaps in the series. For example, you are likely to use Dimension 1-4. For an integration package provided by Medius, you will need to pay extra attention as there might be gaps in the series. For example, you might use Dimension 1-3, and Dimension 8-9.

1. Click the **Inherited from Root company** checkbox, changing it to **Defined in selected company** for all rows in the table.
2. Set the toggles in the **Active** column for the Dimensions you want to use to **Yes**.
3. Enter the appropriate label provided by the client in the **Name** column. This name will be displayed in the tooltips. These tooltips appear when one of the coding fields is active. In the image below, Name is set to *G/L Account*.
![](../../images/DimensionsSetup1.png)
4. Enter a short version of the label in the **Short name** column. This name will be displayed in the coding field itself. In the image below the short names are *Div*, *GL*, *Dep*, *CC* and *Txt*.
![](../../images/DimensionsSetup2.png)
5. If you are using free text dimensions, for example to let the client enter some kind of transaction text, you should also enter a **Maximum character length** for the string. This should be based on the limit for the corresponding field in the ERP system.
6. Click **Save**.

![](../../images/DimensionsSetupDone.png)

For more information, see the [Dimension value documentation on the Success Portal](https://success.mediusflow.com/documentation/administration_guide/administration_pages/dimension_value/#general).
