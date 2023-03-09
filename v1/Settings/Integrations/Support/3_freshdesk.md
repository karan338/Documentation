## Metadata_Start
## title: Freshdesk
## original-url : https://docs.churn360.com/docs/freshdesk
## article-id : 9b76d653-af91-4781-94e1-3a39c1d3e1c9
## seo-title : Freshdesk
## description : 
## Metadata_End
#### Prerequisites to follow:

:::(Info) (Note:)
"You'll need an API Key and a Domain to integrate Freshdesk with Churn360"

 What is an **API Key** and **domain**?
* An API Key is an unique token or a code that is used to identify or authenticate an application.
* A Domain is a unique name that appears in an URL
> For example, When you create a support portal with Freshdesk, you get a " **xyz**.freshdesk.com" domain by default. This "**XYZ**" is usually a username  you enter while you signup, and this is the domain you need to enter in Churn360 for integrating both applications.
:::

#### How to get the API Key?

Follow the below steps to get the API Key from freshdesk 

1. Login to your [Freshdesk](https://freshdesk.com/login){target="_blank"} account
2. On Freshdesk dasboard, click on **My Profile** → **Profile settings** ( You can find the the API Key on the right side of the page)

![1_Screenshot_freshdesk_integration](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_freshdesk_integration.png){height="" width=""}

:::(Info) (Note:)
"The API Key is displayed only after the agent is verified" 
:::
#### How to get the Domain?

Get the **URL** of the user login ('after logging in'-**The first part of the domain**)

>For example, If the URL is "https:// **xyz**.freshdesk.com",  the domain is xyz

![2_Screenshot_Freshdesk_Integration](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/2_Screenshot_Freshdesk_Integration.png){height="" width=""}

### Webhook Settings
:::(Info) (Note:)
In order to achieve real time data sync, we need to connect to webhooks. you'll need to setup webhook for [ticket creation](https://support.freshdesk.com/en/support/solutions/articles/37614-setting-up-automation-rules-to-run-on-ticket-creation){target="_blank"} and [ticket updation](https://support.freshdesk.com/en/support/solutions/articles/99047-setting-up-automation-rules-to-run-on-ticket-updates){target="_blank"}.
:::

1. On Freshdesk, click on **Admin** → **Workflows** → **Automations** 
2. Click on **New rule** button from the **Ticket Creation** tab 
3. Give your rule a **Rule name**
4. Set **conditions** for the new rule (Conditions are set of statements or  criteria your recipients must meet in order to perform the trigger action.)

![1_Screenshot_Freshdesk_Tricket_creation_condition](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_Freshdesk_Tricket_creation_condition.png){height="" width=""}


:::(Info) (Creating an automation rule to run on ticket creation:)
Conditions are set to act as a trigger for this particular rule. [Click here](https://support.freshdesk.com/en/support/solutions/articles/37614-setting-up-automation-rules-to-run-on-ticket-creation){target="_blank"} to know more.
:::



![2_Screenshot_triggeractions_freshdesk\(1\)](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/2_Screenshot_triggeractions_freshdesk%281%29.png){height="" width=""}


Once the rules are created, real time data sync happens allowing you to create, edit, delete, and update new tickets from Freshdesk website

:::(Warning) (**Important**)
Creating a rule in Ticket updation is same as it is in Ticket creation except the below dropdown field 
![1_Screenshot_Freshdesk_ticket_updation_important](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_Freshdesk_ticket_updation_important.png){height="" width=""}


Define an event filter to trigger the webhook to pull the updated Ticket data

"Contact our support team at support@churn360.com to get seperate URLs for Ticket creation and Ticket updation"
:::

:::(Info) (Where to view the data from Freshdesk in Churn 360 Portal)
Click on the **Customers** tab from the **Home** page; click on any one of the customer name to check the support ticket data from Freshdesk.
:::
****
5. Verify the summary of the rules and click on **Save** 

6. To create webhooks for the changes made to any ticket, create a new rule under **Ticket Updates**

:::(Info) (Note:)
You'll need to create a new rule to create webhooks for the changes made to a ticket.
:::

### Freshdesk+ Churn360 

1.	To enter the API Token in Churn360 Portal, Navigate to **Settings** → **Integrate**→ **Chat**→ **Freshdesk**

![1_Screenshot_Freshdesk_integration](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_Freshdesk_integration.png){height="" width=""}

2. Add the **Domain name** and **API token** 
3. Click on **Connect to Freshdesk**


:::(Info) (**Where to find the Freshdesk data in Churn360?**)
Click on the **Customers** tab from the **Home** page; click on any one of the customer name and navigate to the **Overview tab**  and scroll down to view the Support tickets.
:::

![4_Screenshot_Freshdesk_Integration](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/4_Screenshot_Freshdesk_Integration.png){height="" width=""}



