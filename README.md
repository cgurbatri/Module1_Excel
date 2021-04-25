# Kickstarting with Excel

## Overview of Project

Client, Louise is interested in starting a crowdfunding campaign for her play, _Fever_. She has an estimated budget of $10,000. To help inform her campaign strategy, we will analyze information in the kickstarter dataset, which contains information regarding fundraising campaign trends from 2009 to 2017. 

### Purpose
Specifically, through analysis of this dataset, we will identify specific factors that make a project's campaign successful and generate insight into how Louise can set up her campaign strategy to mirror other successful ones in the same category.

## Overview of dataset
The dataset contains information for ~4,100 crowdfunding campaigns between 2009 and 2017. The campaigns have either been completed and can be identified as "successful" or "failed" based on if their "pledged" donations is greater than or equal to their "goal" donations. Included in the potential campaign outcomes are also "canceled" or "live" outcomes. The data gathered covers campaigns across 21 countires, with a majority (~74%) of the campaigns originating in the US. Information collected about each campaign include: name, description of campaign (blurb), fundraising goal, pledged goal, outcome, country, currency, date launched, number of donors (backers_count), category, and subcategory. 

### Computational Challenges 
Considering the overview of this dataset, immediate challenges to analysis can be identified as follows:

*Category and Subcategory are listed in the same column, not easily allowing for independent filtering of the parent category and subcategory. This was addressed by splitting this column into two colums ("parent category" and "subctefory) using the "Text to Columns" feature in Excel.

*All dates were listed as a unix timestams. For readibility and analysis these were converted to a standard date format. Ultimately, having the "date created conversion" and "date ended conversion" columns allowed us to gauge the length of each campaign.

### Analysis and Results
Focusing on theater campaigns would be most informative for Louise. Of the 9 parent categories represented in the dataset, theater alone accounted for ~30 percent of all campaigns, suggesting that there is a representative sample from which to draw therater-specific campaign insight. Specifically, ~57% of theater campaigns across all countries represented were successful. This distribution can be visualized in the bargraph below (**Figure 1**).

**Figure 1** 
![Parent_Category_Outcomes_all](https://user-images.githubusercontent.com/45336910/115976272-34f3a100-a53a-11eb-9f9d-c54bbe9a9501.png)

Honing in further on the subctageories, as seen below, there are more campaigns for plays than there are for any other subcategories. Specific to theater subcategories, plays represent ~76% of all campaigns in the theater category. Furthermore, ~65% of all play campaigns are successful. The outcomes for all subcategories can be viewed below (**Figure 2**). 

**Figure 2**
![SubCategory_Outcomes_all](https://user-images.githubusercontent.com/45336910/115976389-98ca9980-a53b-11eb-81cd-446e929847c8.png)

The two figures above suggest that fundraising for plays compared to other categories has been the most successful.

IFactors investigated to gain insight into overall campaign success include: (1) Duration of campaign, (2) Fundraising goal, (3) Amount pledged, and (4) Launch date. A description of the findings is below:

**Duration of campaign** For all campaigns, we found that the average campaign duration was around 30 days and the second most frequent campaign duration was 60 days. Though the trend is not robust, the graph does suggest that longer campaigns are not necessarily more successful, which works in Louise's favor because she ran her campaign for a "short" amount of time (**Figure 3**). 

**Figure 3**
![Duration_Campaign_vs_Outcome](https://user-images.githubusercontent.com/45336910/115978571-4e064d00-a54e-11eb-9438-39b077247825.png)

The same trend is seen when only theater campaigns were considered (**Figure 4**). 

**Figure 4**
![Duration_Theater_Campaign_vs_Outcome](https://user-images.githubusercontent.com/45336910/115978689-472c0a00-a54f-11eb-959d-78293a064c67.png)

The table below describes campaign success in terms of fundraising goals and pledge amounts. 
![Descriptive_statistics](https://user-images.githubusercontent.com/45336910/115978797-29ab7000-a550-11eb-910e-af20486f75a0.png)

These statistics suggest that failed campaigns have much higher fundraising goals, which does not fare well for Louise who is asking for more than twice the average successful kickstarter goal. Additionally, the mean and median pledged amounts for failed kickstarter campaigns are lower than those for successful campaigns, suggesting that failed campaigns are unsuccessful for reasons other than asking for too much money. 

**Outcomes Based on Goals**
To visualize these statistics, we looked at outcomes based on fundraising goals (**Figure 5**). The trend is not robust, but the graph suggests that a successful outcome correlates with a low funding goal (< $1000) and a failed outcome correlates with a higher funding goal (> $50,000). Since Louise's goal is $10,000, the line graph suggests that lowering this fundraising goal will increase her chances of succeeding.

**Figure 5**
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/45336910/115980805-89f4de80-a55d-11eb-93bc-da77160d4593.png)

**Outcomes Based on Launch Date**

Lastly, we looked at outcomes based on launch date specifically for theater campaigns(**Figure 6**).From this line graph we learned that the month in which the campaign is launch influences campaign success greatly -- May is the best month to launch a campaign and December is the worst. 

**Figure 6**
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/45336910/115979417-d5a28a80-a553-11eb-8cd0-063096d885b7.png)


## Recommendations for Louise
* Raise money for a play, since those campaigns have seen the most success. 
* Consider lowering the fundraising goal, since the current goal is double the average goal for a successful campaign.
* Launch the campaign in the spring (ideally, May).
* Consider a campaign length of 30 days or less since these have been slightly more successful than longer campaigns.

## Limitations of analysis
* The dataset only includes campaigns through 2017, more recent data could be more useful to Louise's present-day campaign.
* The dataset is skewed heavily toward campaigns in the US, which is a limitation if Louise wants to launch a campaign elsewhere.

## Other analysis recommendations
* Number of donors vs outcomes
* Average donation vs outcome
* Duration of campaign (included above)
