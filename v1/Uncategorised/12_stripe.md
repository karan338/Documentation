## Metadata_Start
## title: Stripe
## original-url : https://docs.churn360.com/docs/stripe
## article-id : e85ca810-07cd-475f-86a4-ec8717bf5682
## seo-title : Stripe
## description : 
## Metadata_End

Integrate **Stripe** with **Churn360** allows you to view all your finance related data right inside Churn360 If you are using Stripefor your billing and subscription based data handling and processing. 

#### Pre-requisite to follow

1. Login to your **Stripe account**
2. Click on the **Developers** button on the top right of the page adjacent to the Test mode toggle
3. Click on **API keys** 
4. Click on the **Reveal test key** under **TOKEN** field in **Standard keys table** as shown below
![1_New_Screenshot_APIKeys_Stripe](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_New_Screenshot_APIKeys_Stripe.png){height="" width=""}


5. Click and copy the **Secret key**


#### Stripe + Churn360
1. Once you have the  **API key** and the **Domain**, Login to your Churn360 account

:::(Info) (Note:)
**API Key** mentioned here is the **Secret key** you copied from Stripe.
:::
2. Navigate to **Settings** → **Integration** → **Finance**
3. Click on **Stripe** and enter the **API Key** and **Domain Name** retrived from Stripe
4. You can choose a Customer identifier from a **Pre-defined field** or **custom field**


:::(Internal) (Private notes)
Integration >>> stripe 

Custom→ Unique identifier

API Token will be fetched from stripe

Mostly need to be mapped with Custom fields 
:::



