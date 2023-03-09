## Metadata_Start
## title: Custom data source
## original-url : https://docs.churn360.com/docs/custom-data-source
## article-id : 069d43c0-e57f-4bdc-96fb-f601ecdee522
## seo-title : Custom data source
## description : Custom data sources are a built-in Churn360 feature for user-specific scenarios. With the aid of APIs and API endpoints, you can collect data by mapping data fields from different sources to Churn360.
## Metadata_End
Custom data sources are a built-in Churn360 feature for user-specific scenarios. With the aid of **APIs** and **API endpoints**, you can collect data by mapping data fields from different sources to Churn360.

* * *

### How to configure Custom data source ?
1. Login to your Churn360 account 
2. Navigate to **Settings** → **Integrations** → **Custom data sources**
3. Click on **Create data source** button (This opens a five step  Custom data source setup popup.)
![1_New_Screenshot_data_source_Information](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_New_Screenshot_data_source_Information.png){height="" width=""}
 
4. Enter a **Data source name** and **Endpoint** 

 :::(Info) (Note:)
 An endpoint is an Internet resource locator (URL) where users of a particular service can access it. Customers can access those services' functions by using that URL. The endpoint is a point of connection where exposed HTML files or live server pages can be accessed. 
:::
![3_New_Screenshot_Authorization_custom_data_dsource](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/3_New_Screenshot_Authorization_custom_data_dsource.png){height="" width=""}


5. Select **Oauth** or **API key** from Authorization method
6. Choose  **Header** or **Query string**   to append your Authorization token 

:::(Info) (Note:)
* An API header specifies the data that can be submitted or returned in an API request. In your API definition, it can be created in several places. 
*  The term "**query string**" refers to the question mark that comes after the parameters and their values in an endpoint.
> For example, "**/ccadmin/v1/orders?limit=5**" 

:::

![3_New_Screenshot_API_Information_custom_data_source](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/3_New_Screenshot_API_Information_custom_data_source.png){height="" width=""}


7. Add API Information such as **API Name** and  **Endpoint** → turn on **auto sync** toogle to sync data in real-time; Set **Sync interval**  from the dropdown.

8. Click on **Connect** 

![5_New_Screenshot_Unique_identifier_Custom_data_source](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/5_New_Screenshot_Unique_identifier_Custom_data_source.png){height="" width=""}


9. Select a **Unique identifier** from the dropdown ( A Unique Identifier is a value used to identify each distinctive record. )

10. On the field mapping step, you can map the **Custom fields**  created for Customers module in Churn360 with the data pulled from the  **API endpoints**


11. Click on **Finish**

* * *

#### Where do you find data after custom data source configuration ?
You can find the data under **Custom fields** that you have mapped with the source fields in the field mapping setup.

![1_ScreenGIF_Customer_custom_fields_screengif](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_ScreenGIF_Customer_custom_fields_screengif.gif){height="" width=""}
