## Metadata_Start
## title: Chargebee
## original-url : https://docs.churn360.com/docs/integrate-chargebee-churn360
## article-id : 23be3ab1-bce0-454c-990a-ee8ea4362db4
## seo-title : How to integrate Chargebee with Churn360
## description : Integrating Chargebee with Churn360 allows you to view all your finance data right inside Churn360

You'll need a API key and a Domain name to integrate Chargebee with Churn360
## Metadata_End
## How to integrate Chargebee with Churn360
Integrating Chargebee with Churn360 allows you to view all your finance data right inside Churn360.

You'll need a **API key** and a **Domain name** to integrate Chargebee with Churn360.

### **Pre-requisite to follow**
1. Login to your **[chargebee account](https://app.chargebee.com/login){target="_blank"}**
1. Navigate to **Settings** → **Configure Chargebee**, scroll down and click on **API keys** under **API Keys and Webhooks**
2. Click on the **'+ Add API'** Key button
3. Choose the **Full-access key** option → Select **All** 

:::(Info) (Note)
Choosing **All** allows full access to your Chargebee site. When you create a chargebee account, you get a " **xyz**.chargebee.com" domain by default. This "**XYZ**" is usually a username  you enter while you signup, and this is the domain you need to enter in Churn360 for integrating both applications.

> Example,  if the **URL** is  https://abcd-test.chargebee.com, then the domain name is  **abcd-test**
:::

:::(Info) (Note:)
In order to achieve real time data sync, we need to connect to Chargebee the webhooks.
:::

### Webhook Settings 

1.	Login to **Chargebee**
2.	Click on **Settings** → **Configure Chargebee** → **Webhooks** (under **API Keys and Webhooks**)
3.	Click on **'+ Add Webhook'** button
4.	Enter the **Webhook Name** (a convenient name), **Webhook URL** 

:::(Warning) 
"Contact our support team at support@churn360.com to get seperate URLs for Ticket creation and Ticket updation"
:::
5.	Under the **Events to send**, choose the following events

*    **Subscription Created**
*	**Subscription Activated**
*	**Subscription Changed**
*	**Subscription Cancelled**
*	**Subscription Renewed**
*	**Subscription Reactivated**
*	**Subscription Deleted**
*	**Payment Failed**
*	**Payment Refunded**
*	**Payment Succeeded**
*	**Authorisation Succeeded**
*	**Authorisation Voided**

![2_Screenshot_Chargebee_Integration_setup\(2\)](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/2_Screenshot_Chargebee_Integration_setup%282%29.png){height="" width=""}


6.	Click on **Create**

### Chargebee + Churn360
1.	Once you have the **API key** and the **Domain**, Login to your Churn account

2. Navigate to **Settings**→ **Integration** → **Finance**
3. Click on **Chargebee** and enter the **API Key** and **Domain Name** retrived from **Chargebee**

4. You can choose  a Customer identifier from a **Pre-defined field** or **custom field**

:::(Info) (Note:)
* A **customer identifier** mentioned here is like a unique identifier used to identify customer and map their respective subscription records.
* You may choose a pre-defined field, if the dropdown list includes the unique identifier field you want.
* If a field you want to map isn't among the pre-defined fields mentioned in the selection, you may pick Custom field and add a unique identifier field within the required entity (a customer or subscription).

:::
![1_Screen_GIF_Chargebee_new_one](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screen_GIF_Chargebee_new_one.gif){height="" width=""}

:::(Info) (Where to find the data in Churn 360?)
Click on the **Customers** tab from the **Home** page; click on any one of the customer name to check the subscription and finance data retrieved from Chargebee.
:::
![3_Screenshot_Chargebee_integration](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/3_Screenshot_Chargebee_integration.png){height="" width=""}

