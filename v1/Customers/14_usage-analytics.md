## Metadata_Start
## title: Churn360 Usage Analytics
## original-url : https://docs.churn360.com/docs/usage-analytics
## article-id : 00d86a8f-aca6-4169-9bf7-62b0b8f448ab
## seo-title : Visual Taggger 
## description : 
## Metadata_End
Churn360 usage analytics enables you to send the user activity data from your application to Churn360. 

:::(Info) (Pre-requisite:)
1. **A Churn360 account**. You will need an account with administrator access.
2. **A web app**. This method works best with web applications and does not support mobile apps.
3. **API key** from Churn360.
4. The website must use **HTTPS**.
:::


### Setup  
To establish a connection to use Churn360 usage analytics.

1. Login to your Churn360 account 
2. Navigate to **Settings** → **Integration** → **Usage** → **Churn360 usage API** → **Connect** (You'll receive an API Key )
3. Paste the below javascript snippets under the ``<head>`` tag of your application

:::(Internal) (Private notes)
Need to change the src URL......
:::
``` Javascript
<script src="https://usage.churn360.com/assets/js/usage-collector.min.js"></script>
```
4. Intialize a session using the below method

Structure:
  ```API method
  POST https://usage.churn360.com/api/initialize
{
    "customerIdentifier": <unique-identifier or external id from CRM or email domain or customer name>,
    "userEmail": "john.doe@company.com"
}
HTTP Headers
x-api-key: <api-key> 
  ```
Code:

```
<script type="text/javascript">          
var usageCollector = new churn360.UsageCollector();
  usageCollector.initialize("<API key>","<customerIdentifier>","<emailId>");
      window.addEventListener('load', function () {
        if (localStorage.getItem('Churn360V-TagApikey')) {
          usageCollector.listener();
        }
      });</script> 
```
* * *


:::(Info) (API key)
  API key identifies your application which should be kept safe, has to be called from your backend server(preferrably) or browser to get the session token.
:::
This gives a session token which should be passed in all subsequent calls. 
:::(Info) (Customer Identifier)
 In order to identify the customer for whom the usage is being tracked, one of these identifiers needs to be part of the initialisation, mentioned in the order of preference:
 
*  Unique identifier used across tools like CRM, support, finance etc. 
*  ID of the customer from the CRM.
*  Email domain. 
*  Company name as mentioned in the CRM.
:::
``` javascript
<script type="text/javascript">
      usageCollector.initialize(<API Key>);
    </script>
 ```
#### Session Factory 
The session factory, a server-side approach can help to manage the database connections using a session key. It contains two parameters, sessionkey and callback that are used to regenerate the key after the session expires.

You need a code snippet with a return type promise for the call-back parameter.

```
sessionFactory(sessionKey, callback)
```

| Field |Condition  | Type| Description |
| --- | --- | --- | --- |
| sessionKey | Required | string | This grants user access  to available methods. |
| callback | Required | function | This function executes after a timeout of 20 minutes, giving the browser time to make outbound requests first. |

```
sessionFactory(string, function)
```

:::(Internal) (Private notes)
Need to do this....!!!! Warning ...
sessionFactory(sessionKey: string, callBack: any)
:::


### Methods in Churn360 Usage analytics
There are **three** methods to send end user's data to the churn360 Usage analytics using Churn360 usage API. 

#### 1. Page 
The Page method helps you **find what page the users are on**. Churn360 Usage analytics collects URLs, titles, referrers and paths by default. Anything additional to be tracked in page method can be done using the below format.
``` Javascript
usageCollector.page(additionalfields);	
```

| Field |Condition  | Type| Description |
| --- | --- | --- | --- |
| ```additionalFields``` | Optional | {string:string} (object) | A collection of properties on a page. **Note**:  If you want to record properties from a page, use ```additionalFields```. |

:::(Info) (**Note:**)
Additional fields are optional but when you need to add one, you can add it in the format of **{string:string}**.
:::
 
**Format :**

``` Javascript
 usageCollector.page({string, string});
```
 
**Example :**
``` Javascript
  let additionalFields = {
      "domain":document.domain,
      "projectId":"075129da-99dc-466b-beff-166e2655550d",
      "environment": "dev",
      "subscripition": "premium"
    }
    usageCollector.page(additionalFields);
```


#### 2. Track
**Track** method helps you know **the record of any actions your user performs on any page**.
The track method follows the below format:
``` Javascript
usageCollector.track([event],[feature],[additionalFields]);
```

| Field | Condition | Type | Description |
| --- | --- | --- | --- |
|```event```  | Required |String |The name of the event you’re tracking. |
| ```feature```| Optional |String | It records the feature of the instance.|
| ```additionalFields```| Optional |{string:string} (object)  | A collection of properties on a page.```additionalFields``` |
:::(Info) (**Note:**)
The **event** and **feature** parameters needs to be entered in string format  i.e., **String**; Additional fields are optional but when you need to add one, you can add it in the format of **{string:string}.**
:::

**Format :**
``` Javascript
usageCollector.track(string, string, { string: string } );
```
**Example :**

``` Javascript
let additionalFields = {
  "projectId":"075129da-99dc-466b-beff-166e2655550d",
  "environment": "dev",
  "subscripition": "premium",
  "productId": "a069d9a5-6256-4001-9728-826f15",
     };
  usageCollector.track("view more clicked","product details", , additionalFields);
```
#### Identify
It records your user traits including the **User ID**, **email**, **name** and more. 
```
usageCollector.identify(traits,UserId)
```
| Field | Condition | Type | Description |
| --- | --- | --- | --- |
| ```Traits```| Required |Object |A dictionary of traits you know about the user, like **email** or **name**.  |
| ```UserId``` | Required | String | The database ID for the user. If you don’t know who the user is yet, you can omit the userId and just record traits. |
:::(Info) (**Note:**)
The required format for ```traits``` is 
``` Javascript
{
firstName: string;
lastName: string;
email: string;
phone?: string;
address?: {
                street: string;
                city: string;
                state: string;
                postalCode: string;
                postalCode: string;
                country: string;
}
}
```

:::
**Example:**

``` Javascript
let traits={
firstName: "David",
lastName: "Thomson",
email:"Thomson@Example.com",
phone:"1234567890",
address:{
   street:"39 Thunder Road",
   city:"Oakland",
   state:"California",
   postalCode:"94612",
   country:"United States"
}
}
usageCollector.identify(traits);
```
:::(Info) (**Default fields :**)
Churn360 Usage analytics collects URLs, titles, referrers and paths by default.
:::

The above are the basic methods to share the usage data to churn360 Usage Analytics.

:::(Warning) 
To get more support, contact at contact@churn360.com
:::
