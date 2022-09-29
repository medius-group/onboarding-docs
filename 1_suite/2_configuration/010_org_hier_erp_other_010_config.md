## Introduction
It's important to setup a good company structure that reflects not only your legal entities but also reflects how the legal entities are organized.
Best practise guidelines for establishing the company structure is found on the Medius Success Portal here: [Company structure design guidelines](https://success.mediusflow.com/documentation/administration_guide/administration_pages/configuration_tutorials/company_structure/)

If you have many legal entities or a complex organization structure it is recommended to consult your implementation partner to build the organizational structure in MediusFlow.

Company codes are added in Medius using this administration page: [Add companies here](https://cloud.mediusflow.com/$TenantNameQA/#/Administration/Medius.Core.Entities.Company).
When adding companies you have to fill in the accounting currency of each company. A new Medius deployment is preconfigured with the most common currency codes but if the currency code you need is missing from the list you can add it by following the below instruction.

The Company configuration holds a lot of details and provides many possibilities. In this step we'll only add the basics. Detailed company configuration will be covered in other sections.
Guidance to all company configuration options in Medius can be found in this Success Portal section: [Success portal company configuration](https://success.mediusflow.com/documentation/administration_guide/administration_pages/company/).

### Add a virtual company node
The virtual company structure can be used to setup a scalable company model where master data and configuration is shared depending on needs. Please follow thw below steps to create virtual nodes in the company structure as 
identified in the company structure design.

1. Click **Add**.
2. In the field *Name*, fill in the name of the virtual node. Proposed naming convention is the name of your organization followed by "Root", e.g. "Medius Root".
3. Enter any value into the field *Organization Number* - this field is technically required but is not utilized.
4. Choose **Root company** in the field *Parent company name*.
5. Switch the value of *Is Virtual* to **Yes**.
6. Choose **-** as *Accounting currency*.
7. In the field *Company Id*, enter a company id according to the following format: "Company_Root" where **Company** is the name of your organization, e.g. "Virtual_Medius_Root".
8. Add *External System Id* according to the following format: "company[Company_Root]" where **Company** inside of brackets is the name of your organization, e.g. "company[Medius_root]".
9. Navigate to the tab **Enterprise** and further to the tab **General**  and set the field *ERP Id* to "FX" if the File exchange API is used, if the REST API is used a value decided together with the integration party is needed to ensure that postings are being picked up by the intended integration.
10. Click **Save**.

![](../../images/AddVirtualCompany.png)

### Add your companies
Now add the company codes of your organization by repeating the below steps for each company code.

1. Click **Add**.
2. In the field *Name*, fill in the name of the company.
3. Enter any value into the field *Organization Number* - this field is technically required but is not utilized.
4. Choose your recently added virtual company node **Root company** in the field *Parent company name*.
5. Check that the value of *Is Virtual* is **No**.
6. Choose the accounting currency for this specific company in field *Accounting currency*.
7. In the field *Company Id*, enter the company Id that represents this specific company in your ERP, i.e. 001, MED, US02.
8. Add *External System Id* according to the following format: "company[Company Id]" where Company Id inside of brackets is the same value as recently entered in field *Company Id*.
9. Click **Save**

![](../../images/AddCompany.png)

