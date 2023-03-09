## Metadata_Start
## title: Import
## original-url : https://docs.churn360.com/docs/import
## article-id : dc9f203d-9270-4aa8-986f-af5680394b2c
## seo-title : Import
## description : 
## Metadata_End
Churn360's import feature is used to onboard data for **customer**, **contact**, **subscription**, **Plans**, **Invoices** and **Coupens** in a **.csv** file format. This is used to import data to Churn360 without integrating any third-party integration tool.

:::(Info) (Note:)
 Export data from the source application that you need to import into Churn360 ( It can be a CRM tool to for customer data and accounts, a billing tool for billing related data, a support tool for chat.). Churn360 permits data to be imported in a.csv file format, so make sure to export the data in that format.
:::

### Method 1
#### How to import .CSV file data into Churn360?
1. Login to your Churn360 account
2. Click on **Settings**→**Integration**→**Imports**
3. Click on **Upload file** ( .csv file format)

4. Check that the.csv file you import follows our recommended format. To downlod our reccomended format.
5. Select an option from the dropdown as you intend → Click on the **Click here** link to download the sample CSV.

![2_Screenshot_imports_recomennded_format](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/2_Screenshot_imports_recomennded_format.png){height="" width=""}

:::(Info) (Note:)
* You can download the Sample CSV file before uploading it so that you can organise your data accordingly.
* Make sure you select the right entity for which the .csv file is getting uploaded.

> For example, The import would not work, if the user chooses **Customer** from the **import your** dropdown and then uploads **Contacts** file.
:::

![1_Screenshot_Churn360_Imports](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_Churn360_Imports.png){height="" width=""}


Now that your data is transferred and converted to the specified CSV file format, you can import it. You can drag and drop your.CSV file or click and choose a file from the file explorer to import.


If the format is incorrect, the file won't upload and the message "Unsupported format" will appear. 

![2_ScreenGIF_unsupported_file_format](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/2_ScreenGIF_unsupported_file_format.gif){height="" width=""}

You can download the failed records if the file format is proper and the data fields in the.CSV file format are incompatible. You can download the file from failed records to find out the cause.


![3_Screenshot_import_failed_reccords](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/3_Screenshot_import_failed_reccords.png){height="" width=""}

:::(Info) (Note:)
After you download the file from the failed records, the failed reason is recorded and displayed in the reason column if any data is not in the right format.
![8_Screenshot_failed_records_import](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/8_Screenshot_failed_records_import.png){height="" width=""}
:::

### Method 2

You can also import data from **All Integrations** under **Integrations**.

![1_New_Screenshot_Imports_All_Integrations](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_New_Screenshot_Imports_All_Integrations.png){height="" width=""}

:::(Info) (Note:)
You must upload the intended adjustment to the Plans file before making any changes to the field data in the Subscription file. If a user needs to subscribe for a new plan that is not among the ones that are already available.
:::

