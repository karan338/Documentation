## Metadata_Start
## title: How to view Health score results
## original-url : https://docs.churn360.com/docs/how-to-calculate-healthscore
## article-id : a226d51e-997e-4766-b946-527a2d7216fd
## seo-title : How to calculate Healthscore
## description : Health scores are calculated using the consolidated scores gathered from the different parameters set during the Health score configuration. These are calculated using scores from 0 to 100. 
## Metadata_End
Health scores are calculated using the consolidated scores gathered from the different parameters set during the Health score configuration. These are calculated using scores from **0 to 100**. The parameters include **Support tickets**, **Invoice**, **Credit card**, and **CSM pulse**. The given score of each of these parameters combined must have a **total weightage of 100** while configuring.

![2_Screenshot_Calculating_Health_score](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/2_Screenshot_Calculating_Health_score.png){height="" width=""}

You can also define the grading scale of the configured Health score in Step 1 of the Health score configuration. Click here to know more on how to configure Health score in Churn360.

 

![1_Screenshot_Grading_scale_Calculate_Healthscore](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_Grading_scale_Calculate_Healthscore.png){height="" width=""}  

After the Health score is configured, the Health score of the individual parameters is used to determine the overall health profile.

> For example, the Health score set for individual parameters must have a combined value of 100; This is the weightage from which the grades for the health score are calculated.

![4_Screenshot_Health_score_total_weightage](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/4_Screenshot_Health_score_total_weightage.png){height="" width=""}

Assuming that Health score for each parameter is set to 50 as indicated above, a total weight of 100 is formed. Go to the **Home page** → **Health score** now.

* * *

#### Overview on the Overall Health scoretab 
![1_Screenshot_New_Healthscore_split](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_New_Healthscore_split.png){height="" width=""}

1. Filter results according to the configured Health score
2. Filter results according to the Health score status 
3. Search customer name to filter Health score results for the intended customers
4. Filter results for a particular time period
5. It is the overall score calculated from all the parameters

:::(Info) (Note:)
* The Health score would be 0 if the individual scores for all configured parameters were poor, regardless of the score ratio that was provided to each parameter while configuring the health score.
* For the concerning customers the score is the median of the first and last updated values, 
>For example, the first updated value might be poor and the last updated value can be healthy, and the concerning Health score is calculated with the medium of these values.
* The difference in the trend is the last updated value for the score.
:::
6. It is the difference calculated using the prior data; an arrow is also displayed to show the upward and downward trend in the particular customer's health score. ( Based on the change, the health score value will be updated  in the overall health score)

:::(Info) (Note:)
* You can also view the health score results of an individual customer under **Customer** → **Overview** → **Health score**. ( Health score displayed here will be based on the selection parameters configured.)
![5_Screenshot_New_Health_score_overview_page](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/5_Screenshot_New_Health_score_overview_page.png){height="" width=""}

* You can filter Health score by its name ( This is so that numerous health ratings can be created using different segments, each of which can contain a single customer.) and the time period.

* The metrics are shown using a line graph representation that shows data with a score on its Y-axis aligned with the selected time period on the x-axis. The overall status of the Health score is also shown below the graph.

:::


