## Introduction
It's important to setup a good company structure that reflects not only your legal entities but also reflects how the legal entities are organized.
Best practice guidelines for establishing the company structure is found on the Medius Success Portal here: [Company structure design guidelines](https://success.mediusflow.com/documentation/administration_guide/administration_pages/configuration_tutorials/company_structure/)

If you have many legal entities or a complex organization structure it is recommended to consult your implementation partner to build the organizational structure in Medius.

Company codes are added in Medius using this administration page: [Add companies here](https://cloud.mediusflow.com/$TenantNameQA/#/Administration/Medius.Core.Entities.Company)
When adding companies you have to fill in the accounting currency of each company. A new Medius deployment is preconfigured with the most common currency codes but if the currency code you need is missing from the list you can add it by following the below instruction.

The company configuration holds a lot of details and provides many possibilities. In this step we'll only add the basics. Detailed company configuration will be covered in other sections.
Guidance to all company configuration options in Medius can be found in this Success Portal section: [Success portal company configuration](https://success.mediusflow.com/documentation/administration_guide/administration_pages/company/)

### Add a virtual company node
The virtual company structure can be used to setup a scalable company model where master data and configuration is shared depending on needs. Below is the minimum level of virtual structure required in a D365BC context. 
This should be extended in accordance with your company structure design.

Add a virtual company below root as described below. This is the preferred company to do any changes that are common for all D365 Business Central (BC) companies. All the BC companies that are created should have this virtual company as parent to follow best practice. 

1. Click **Add**.
2. In the field *Name*, fill in the name of the virtual node. Proposed naming convention is the name of your organization followed by "Root", e.g. "Medius Root".
3. Enter any value into the field *Organization Number* - this field is technically required but is not utilized.
4. Choose **Root company** in the field *Parent company name*.
5. Switch the value of *Is Virtual* to **Yes**.
6. Choose the currency code that applies to the majority of companies within this company group as *Accounting currency*.
7. In the field *Company Id*, enter a company id according to the following format: "Company_Root" where **Company** is the name of your organization, e.g. "V_Medius_Root".
8. Add *External System Id* according to the following format: "company[Company_Root]" where **Company** inside of brackets is the name of your organization, e.g. "company[Medius_Root]".
9. Navigate to the tab **Enterprise** and further to the tab **General**  and set the field *ERP Id* to "NAV"
10. Click **Save**.

![](../../images/AddVirtualCompany.png)

### Create the rest of the companies
Add the rest of the companies that are provided from the customer. If many companies are to be added you may consider to have another virtual level, i.e. country based for different settings in different countries. Note that it's not recommended to add these levels after the leaf companies have been created. Please take some time to evaluate the possibility of companies added in the future to create a good initial company structure.

1. Click **Add**.
2. In the field *Name*, fill in the company name in NAV. This must be the exact name as spelled in NAV.
3. Enter any value into the field *Organization Number* - this field is technically required but is not utilized.
4. Choose your recently added virtual company node, i.e. V_Medius_Root, in the field *Parent company name*.
5. Check that the value of *Is Virtual* is **No**.
6. Choose the accounting currency for this specific company in field *Accounting currency*. The chosen currency should be the same as the accounting currency in the ERP system.
7. In the field *Company Id*, enter the company id that represents this specific company in your ERP, i.e. NAVSE_01.
8. Add *External System Id* according to the following format: "company[Company Id]" where Company Id inside of brackets is the same value as recently entered in field *Company Id*.
9. Click **Save**

The above needs to be set once per company, and it needs to match what is sent in the integration.

![](../../images/AddCompany.png)
