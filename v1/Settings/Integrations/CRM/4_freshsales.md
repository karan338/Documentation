## Metadata_Start
## title: Freshsales
## original-url : https://docs.churn360.com/docs/freshsales
## article-id : 707dd1ec-edf6-4ad2-844d-1e8dab2c6cbd
## seo-title : How to integrate Freshsales with Churn360
## description : Integrate Freshsales with Churn360 to map accounts, contacts, and deals from freshsales to Churn360. View Freshsales data on  the **Customers tab** from the **Home page** → click on any one of the **customer names** from the customer grid and navigate to the **Overview**→ **Contacts**(The contact data is pulled-in from freshsales).
## Metadata_End
Integrate Freshsales with Churn360 to map accounts, contacts, and deals from freshsales to Churn360. 

### Freshsales+Churn360
1. Login to your Churn360 portal
2. Navigate to **Settings** → **Integrations** → **CRM**
3. Click on Freshsales from the list of available integrations

![1_Screenshot_Freshsales_Integrations](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_Freshsales_Integrations.png){height="" width=""}

(This opens a blade for the integration, you'll need a **Domain name** and a **API token** for the integration. Follow the below steps to get it.) 

4. Login to your [Freshsales](https://churn360.myfreshworks.com/crm/sales/accounts/view/70005325198?per_page=25){target="_blank"} account
5. Navigate to your **Profile** → **Settings** → **API SETTINGS**

#### An explanatory GIF
![1_ScreenGIF_freshsales](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_ScreenGIF_freshsales.gif){height="" width=""}

6. Copy the **API Key** and the **bundle alias** to a clipboard
7. Now navigate back to your Churn360 portal, put the **bundle alias** in **Domain name** and **API Key** in **API token**.

![3_Screenshot_freshsales_integration_connect_](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/3_Screenshot_freshsales_integration_connect_.png){height="" width=""}

8. Click on **Connect to Freshsales**(This opens a three-step mapping setup)

#### STEP 1 OF 3 (Set CRM Conditions)
1. Filter the deal stage and accounts under CRM conditions in step 1 of the Freshales integration in Churn360
2. Click on **Next**



#### STEP 2 OF 3 (Unique identifier)
:::(Internal) (Private notes)
Choose a **Unique Identifier** from the source fields dropdown ### add this step in future
:::
:::(Info) (What is a **Unique Identifier**?)
A **Unique Identifier** is  a value used to identify each distinctive record.
![5_Screenshot_CRM_Freshsales_CRM_conditions](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/5_Screenshot_CRM_Freshsales_CRM_conditions.png){height="" width=""}

> For example, In an import, you need a unique identifier to associate two different records. It helps to avoid creating duplicate records.
:::

 3. Click on **Next**

#### STEP 3 OF 3 (Field mapping)
4. In the Field Mapping step, you can map Churn360 fileds like  **Customer** and **Contact**  with your **Source CRM Fields** 
:::(Internal) (Add this to 10 th step once two way sync is enabled from our side)
(To enable two-way sync for the fields between the two applications, you can either select them one by one by turning on the individual toggle button, or click on  **Select All** checkbox to select all at once) 
:::

![6_Screenshots_Field_mapping_CRM_conditions_](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/6_Screenshots_Field_mapping_CRM_conditions_.png){height="" width=""}

5. Click on **Finish** 
:::(Info) (Note: )
In order to achieve real time data sync, we need to connect to **webhooks**. This pulls all your real time data into Churn360. But before this, you need to setup **Freshsales Webhooks setup**.
:::

Follow the below steps to create workflows and setup webhooks in Freshsales.

1.	Navigate to **Admin Settings** → **Workflow** → **Create Workflows**
2.	Select **Account,Deals, or Contacts** according to your preference (Generally the data you need to pull into Churn360)
3.	Set up when to trigger this workflow and the conditions.
4.	Select Trigger webhook from the dropdown under Actions to be executed tab 
![4_New_Screenshot_Freshsales](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/4_New_Screenshot_Freshsales.png){height="" width=""}


6. Select **POST Method**
7. Callback Url (Callback URL should be the **Azure function URL** of Production)

:::(Warning) 
"Contact our support team at support@churn360.com to get the webhook URL"
:::
8.	Select Add new custom headers

![2_Screenshot_Addwebhooks_Freshsales_edit](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/2_Screenshot_Addwebhooks_Freshsales_edit.png){height="" width=""}


3. Enter Key as **X-API-Key** (Value Should be API-Key from Churn portal)
4. **API-Key** should be select from the **API key** screen.

:::(Info) (Note:)
Following successful integration with Churn360, Freshsales' API Key will be displayed in the API Key Module.
:::
5. Select the **Sales Account fields** that are required or you can select any **field** you wish
6. Click **Save**.

![5_New_last_Screenshot_Freshsales](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/5_New_last_Screenshot_Freshsales.png){height="" width=""}

:::(Info) (Where to find the freshsales data?)
View Freshsales data on  the **Customers tab** from the **Home page** → click on any one of the **customer names** from the customer grid and navigate to the **Overview**→ **Contacts**(The contact data is pulled-in from freshsales).
:::
