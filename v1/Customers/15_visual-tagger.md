## Metadata_Start
## title: Visual tagger
## original-url : https://docs.churn360.com/docs/visual-tagger
## article-id : 2390f23b-89ff-4646-96d2-1aeaa7903697
## seo-title : Visual Tagger 
## description : 
## Metadata_End
Visual tagger provides the ability for a non-technical person to identify the events on a web-application that needs to be tracked.

:::(Info) (Pre-requisite:)

1. **A Churn360 account**: You will need to have an administrator account with Churn360.
2. **A web app**. This method works best with web applications and does not support mobile apps, but you can tag the mobile-web version of your websites.
3. Your website must use **HTTPS**.
:::


* * *

#### How to configure Visual tagger?

1. Login to your Churn360 account 
2. Navigate to **Settings** → **Configurations** → **Visual tagger**
3. Click on the **Churn360 Visual tagger** link to download the Visual tagger browser extension as shown below
:::(Info) (Note)
 As of now, Visual tagger only supports **Chrome** browser.
:::
7. Click on **Start Visual tagger** button 
![1_Screenshot_VisualTagger_Adding_URL](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_VisualTagger_Adding_URL.png){height="" width=""}

8. Enter the **URL** of the targeted page
9. Click on **Start** ( This takes you to the URL page in a new tab.)
10. Click on **Add** in the sticky bottom bar (This highlights the list of buttons or events that can be tracked on the page.)
11. Click on the intended event or the button to be tracked( This opens a Track event popup as below)

![1_Screenshot_new_new_Track_event](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/1_Screenshot_new_new_Track_event.png){height="" width=""}


:::(Info) (Note:)
>  You'll need to fill in the compulsory fields.

#### The elements you need to know:
**CSS Selector**: The CSS selector will be automatically pulled in for the **clicked** event. It identifies **unique elements** or **identical elements** for which clicks should be tracked, and you can also enter the CSS Selector manually if you need to.

**Inner text**: It is the label of the click event you need to track; This is also pulled in automatically.

**Event name**: The name of the event for which the configuration is being set up. This name should be **simple** yet **descriptive**, so the users using Visual tagger remember and identify the events later. (The Character limit is **1024**) 
> For example, we recommend that you use an “Object Action” format (for example, Login Clicked, and use Title Case (capitalize the first letter of each word ) when naming events.

**Feature**: Name of the feature the event belongs to(This is an optional field)
 **Event type**: This is the actual event which will be reported by the Usage collector(click events on an element) 
**Page URL**: Visual tagger reads the URL by itself

 * Static - Usage collector listens and reports events only if the Page URL matches with the URL identified by the Visual tagger.
 * Dynamic -If your URL links contain variables that change dynamically.

> For example, http://www.exampledynamicsite.com/forums/thread.php?**projectid=12345**&sort=date. In a dynamic URL, the project id  changes for each user and project. It tracks the URL omitting the dynamically changing variables in the URLs. 

:::
12. Click on **Save** 

* * *

#### How to edit and remove Visual tagger?

To edit or remove the configured event on Visual tagger, navigate back to the Visual tagger page in Churn360 portal. You will find the configured events there as shown below. Click the edit or delete icons on the configured events to make changes.

![2_Screenshot_created_Visual_tagger_event\(1\)](https://cdn.document360.io/b618a27d-7a6e-4dfb-84d1-30d3ef656644/Images/Documentation/2_Screenshot_created_Visual_tagger_event%281%29.png){height="" width=""} 



