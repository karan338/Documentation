## Metadata_Start
## title: HubSpot
## original-url : https://docs.churn360.com/docs/hubspot
## article-id : 5141d948-5f3f-4d5c-80e7-c20d42e8435d
## seo-title : How to integrate HubSpot with Churn360
## description : ntegrate your HubSpot CRM to sync your Customer and Contact information to Churn360. Use Churn360 to understand how your customers use your product
## Metadata_End
Integrate your HubSpot CRM to sync your Customer and Contact information to Churn360. Use Churn360 to understand how your customers use your product.

 ###  HubSpot + Churn360
 1. Login to the **Churn360** portal
2. Navigate to **Settings** →**Integrations** →**CRM**
3. Click on **HubSpot**  

![1_Screenshot_Integration_hubspot](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_Integration_hubspot.png){height="" width=""}


4. Click on **Connect to HubSpot**, this redirects to the **HubSpot login page**

![2_Screenshot_Integration_hubspot](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/2_Screenshot_Integration_hubspot.png){height="" width=""}

5. Enter your **HubSpot** credentials and click on  **log in** 
 :::(Info) (Note:)
* If you have multiple accounts, Select the account you want to integrate and click **Choose account** button(You'll need to do this right after the 5th step, this redirects you to the Churn360 portal). 
:::
6. Select between **deals** and **company** in **choose your customer from** dropdown (The selected entity here is considered as customer in churn360).
![1_New_screenshot_CRM_conditions](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_New_screenshot_CRM_conditions.png){height="" width=""}

7. Filter the deal stage under CRM conditions in step 1 of the HubSpot integration in Churn360

:::(Info) (Note:)
The deal stage under every pipeline in HubSpot is displayed in this filter. Choose the deal stage to pull in deals inside Churn360 after the integration.
![2_NewScreenshot_CRM_conditions_hubspot_filters](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/2_NewScreenshot_CRM_conditions_hubspot_filters.png){height="" width=""}


:::
8. Click on **Next**

:::(Info) (What is a **Unique Identifier**?)
A **Unique Identifier** is  a value used to identify each distinctive record.
![1_Screenshot_Unique_Identifier_hubspot](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_Unique_Identifier_hubspot.png){height="" width=""}


> For example, In an import, you need a unique identifier to associate two different records. It helps to avoid creating duplicate records.
:::

9. Click on **Next**
10. In the Field Mapping step, you can map Churn360 fileds like  **Customer** and **Contact**  with your **Source CRM Fields** 
:::(Internal) (Add this to 10 th step once two way sync is enabled from our side)
(To enable two-way sync for the fields between the two applications, you can either select them one by one by turning on the individual toggle button, or click on  **Select All** checkbox to select all at once) 
:::

![\[2_Screenshot_Fieldmapping_HubSpot_Integration](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/%5B2_Screenshot_Fieldmapping_HubSpot_Integration.png){height="" width=""}

11. You can map custom fields created for **customer** and **contact** inside Churn360 to the fields in Hubspot from here. [Click here](/v1/docs/custom-fields) to know more on how to create Custom fields in Churn360. 
![3_New_Screenshot_Custom_fields_field_mapping_hubspot](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/3_New_Screenshot_Custom_fields_field_mapping_hubspot.png){height="" width=""}
12. In step 4, you can select the interval timing for real-time data sync 
:::(Internal) (Private notes)
Add screenshot 
:::
13. Click on **Finish** 

:::(Info) (**Where to find the HubSpot data in Churn360?**)
View HubSpot data on  the **Customers tab** from the **Home page** → click on any one of the customer names from the customer grid and navigate to the **Overview**→ **Contacts**(The contact data is pulled-in from HubSpot).




:::

:::(Info) (Note:)
* You can find tasks from HubSpot inside workspace task in Churn360 portal; You can also find it from the individual customer page.
![3_ScreenGIF_Tasks_Hubspot](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/3_ScreenGIF_Tasks_Hubspot.gif){height="" width=""}

* You can find your support tickets inside overview tab under the individual customer page.

![2_New_ScreenGif_Support_tickets_Hubspot](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/2_New_ScreenGif_Support_tickets_Hubspot.gif){height="" width=""}

* You can find your notes inside engagements tab under the individual customer page.
:::
#### FAQs
1. Which entity from HubSpot is considered Customers in Churn360?
   **Ans** : You can choose between **Companies** and **deals** from Hubspot to be considered as Customers in Churn360.

2. What if the same company is involved in several deals with various contacts?
      **Ans** : If it is the same company under different deals in HubSpot, it will be considered as a single customer in Churn360, yet we pull-in all the contacts under different deals of a same company.
:::(Info) (Note:)
Even if a same company is associated with multiple deals in HubSpot, it is still considered as a single customer in Churn360.
:::
:::(Internal) (Private notes)
Edit all the answers and notes to include the point about configuration, if Customer identifier is present the deal -customer consideration is different vs when CI is not present, Also confirm if you can skip the CI step. 
:::
