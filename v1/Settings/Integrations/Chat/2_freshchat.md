## Metadata_Start
## title: Freshchat
## original-url : https://docs.churn360.com/docs/freshchat
## article-id : 528d648f-cc33-4120-b7c6-9b5a2712002b
## seo-title : How to integrate Freshchat with Churn360
## description : Integrating Freshchat in Churn360 allows CSM's to view chat conversation with users and support team from Churn360. 
## Metadata_End
## How to integrate freshchat with Churn360

Integrating Freshchat in Churn360 allows CSM's to view chat conversation with users and support team from Churn360. 


:::(Info) (Note)
"You'll need an API Key and a Domain to integrate Freshchat with Churn360"

 What is an **API Key** and **domain**?
* An API Key is an unique token or a code that is used to identify or authenticate an application.
* A Domain is a unique name that appears in an URL
> For example, When you create a support portal with Freshchat, you get a " **xyz**.freshchat.com" domain by default. This "**XYZ**" is usually a username  you enter while you signup, and this is the domain you need to enter in Churn360 for integrating both applications.
:::
### Pre-requisite to follow 
#### How to generate an API Token in Freshchat

1. Login to [Freshchat](https://www.freshworks.com/live-chat-software/login/){target="_blank"}

2.   Navigate to **Settings** → **API Token** -> **Generate Token**

![1_Screenshot _freshchat _integration_chat](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot%20_freshchat%20_integration_chat.png){height="" width=""}

#### How to get the API Domain from Freshchat

Get the **URL** of the user login ('after logging in'-**The first part of the domain**)

>For example, If the URL is "https:// **xyz**.freshchat.com",  the domain is xyz

![2_Screenshot_freshchat_integration_Domain name\(1\)](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/2_Screenshot_freshchat_integration_Domain%20name%281%29.png){height="" width=""}

### Webhook Settings 
1. On the Freshchat application, navigate to **Setting** → **Webhooks**
2.	Enter the **Webhook URL** of Churn 360 in the Text Field below 

:::(Warning) 
"Contact our support team at **support@churn360.com** to get the webhook URL"
:::
:::(Info) (Note:)
In order to achieve real time data sync, we need to connect to webhooks. This pulls all your real time chat data into Churn360.
:::

![3_Screenshot_Freshchat_integration_chat\(1\)](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/3_Screenshot_Freshchat_integration_chat%281%29.png){height="" width=""}

### Freshchat + Churn360 

1.	To enter the API Token and API Domain name in Churn360 Portal, Navigate to **Settings** → **Integrate**→ **Chat**→ **Freshchat**
![1_Screenshot_Freshchat_Integration](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_Freshchat_Integration.png){height="" width=""}

:::(Info) (**Where to find the Freshchat data in Churn360?**)
Click on the **Customers** tab from the **Home** page; click on any one of the customer name and navigate to the **Engagement tab** to view customer's chat from Freshchat.
:::



