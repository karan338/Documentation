## Metadata_Start
## title: How to create an API key
## original-url : https://docs.churn360.com/docs/api
## article-id : ca23c6e0-96f4-4b0a-9bc6-4c1c495face2
## seo-title : API
## description : 
## Metadata_End
Churn360 API uses **token-based authentication**. In order to communicate using API (to get your data pushed to Churn360), you must obtain an API token. 
:::(Info) (Note:)
Only users with Admin access can create and view an API key.
:::
#### How to generate an API token ?
1. Login to Churn360
2. Navigate to **Settings** → Navigate to **Configuration** → **API** 
3. Click on the **Create API key** ( This opens a Create API key popup)

![1_New_screenshot_Create_API_Key](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_New_screenshot_Create_API_Key.png){height="" width=""}



4. Enter the **API key name** 
 
5. Select the **checkboxes** under the **policy group** ( It has the policy group and policies that a user can configure to gain access to the following entities through the API.)

![1_New_Screenshot_group_policies_groupandgroup_policies](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_New_Screenshot_group_policies_groupandgroup_policies.png){height="" width=""}


:::(Info) (Note:)
The preview of the selected policy group and policies will be displayed under the **Selected policy group and policies** section of the popup.
:::

4. Click **Save**

![8_New_Screenshot_API_keys](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/8_New_Screenshot_API_keys.png){height="" width=""}

You would have the following data after you have configured the API key
1. The API Key itself.
2. The detail of the user that generated the key.
3. You'll know the created date.
4. Status of the API key ( If the toggle is turned off, the API key will be invalid).

:::(Info) (Note:)
You can also regenerate and delete the API key under Actions.
:::

