# Kickstarting with Excel

## Overview of Project
Past analyses of crowdfunding data, showed a possible correlation between the success of Kickstarter campaigns, their launch dates, and their funding goals. This analysis will dive more deeply into the outcomes of Kickstarter campaigns in relation to their launch dates and funding goals.

---
### Purpose
This analysis proposes to answer the following questions:
* How do different theater campaigns for plays fare in relation to their launch date?
* Are some months of the year better than others for launching theater campaigns for plays?
* Are some months of the year worse than others for launching theater campaigns for plays?
* How do different theater campaigns for plays fare in relation to their funding goals?
* Is there any pattern in the amount of funding goals and the success of theater campaigns for plays? Are campaigns in some goal ranges more successful than campaigns in other goal ranges?

---
## Analysis and Challenges
The crowdfunding data used in this analysis was pulled from the University of Oregon Data Analysis Boot Camp database. The data was filtered and analyzed using Excel's formulas, statistical tools, and graphic displays. 


### Analysis of Outcomes Based on Launch Date
How do different theater campaigns fare in relation to their launch date? Are some months of the year better than others for launching theater campaigns? In order to answer these questions, we filtered the theater data by month and disagregated the data by outcome then created a line graph from the data (graph 1). For successful campaigns, we see a spike in the number of successful campaigns in May. While the number of successful campaigns begins to decline after May, there is still a high number of successful campaigns in June. This could indicate that starting a campaign in May or June may yield the highest success rate, but we need to dive further into the data before making a conclusion.

While the overall data for outcomes based on launch date show a high number of successful campaigns during the month of May, the data also show a spike in the number of campaigns that fail. In fact, the month of May shows the highest number of failed campaigns of all the months. This leads to the question, "Is the higher number of both successes and failures during the month of May due to the higher number of total campaigns started during the month of May?" In order to answer this question, we found and compared the percentages of successful and failed campaigns for each month (graph 2). The graph based on percentages still shows an increase of succesful campaigns in the month of May, but now we see a decrease in the percentage of failed campaigns during the same month indicating that, indeed, beginning a campaign in the month of may could yield higher rates of success. 

Are some months of the year worse than others for launching theater campaigns for plays? From graph 2, we can see that the percentage of failed campaigns remains somewhat constant around 30% from January through September and then then increase to 43% in October and 47% in December. We also see a significant decrease in the percentage of successful campaigns in December. This suggests that October and December would be poor months to begin a campaign.
---
*(graph 1)*
![Theater_Outcomes_vs_Launch](https://github.com/jisellejones/kickstarter-analysis_JJones/blob/main/Outcomes%20Based%20on%20Launch%20Date.png)

---
*(graph 2)*
![Theater_Outcomes_vs_Launch_Percentage](https://github.com/jisellejones/kickstarter-analysis_JJones/blob/main/Theater_Outcomes_vs_Launch_percentage.png)
---
### Analysis of Outcomes Based on Goals
How do different theater campaigns for plays fare in relation to their funding goals? Is there any pattern in the amount of funding goals and the success of theater campaigns for plays? Are campaigns in some goal ranges more successful than campaigns in other goal ranges? To answer these questions, we created a frequency table using Excel's countifs() formula to sift through the data and count the number of plays with specified outcomes (successful, failed, canceled) based on different ranges of campaign goals. 

From the line graph, we can see that 


---
*(graph 3)*
![Outcome_vs_Goals](https://github.com/jisellejones/kickstarter-analysis_JJones/blob/main/Outcomes_vs_Goals.png)


### Challenges and Difficulties Encountered
When trying to reach a conclusion about which month might be best or worse to begin a campaign, it was difficult to reach a conlusion from looking at only the number of outcomes. It was difficult to differentiate between the success of campaigns being correlated with the month of the year or the higher number of campaigns launched. In May 166 campaigns were launched versus December when only 75 campaigns were launched, so we had to consider a different method of analysis to eliminate the number of campaigns. 





---
## Results
From these analyses, we can conclude that May is the best month to begin a campaign. We can also conclude that beginning a campaign in December may increase the likelihood of the campaign failing.

Campaigns that have a campaign goal of less than $5,000 are more likely to be successful than campaigns that have campaign goals of $5,000 or more.

While there was a substantial amount of data for this dataset, the data was gathered from many different regions. In order to determine the likelihood of success in a particular region, further filtering could be applied to determine if conclusions drawn for all regions applies to a particular region. 


Unfortunately, there was not enough data in the plays category to capture patterns within the canceled campaigns during particular months of the year. There was no data about canceled campaigns when determining the outcomes of campaigns based on campaign goals. Future analyses may consider taking a closer look at this data set by analyzing canceled campaigns across all parent categories or all subcategories of theater campaigns rather than simply the play subcategory.




- What are some other possible tables and/or graphs that we could create?
Since the data comparing campaign outcomes to campaign goals was gathered as different ranges, a histogram or scatterplot might be more useful when analyzing the data to determine. 

Future analyses may also consider looking at correlations between the successful and failed campaigns in months where a greater percentage of campaigns were successful and months where a greater percentage of campaigns failed along side the campaign goal data for those months to determine if there are better or worse campaign goals during different months of the year.

It would be interesting to research the 2 successful campaigns with campaign goals amounts of $50,000 or more. Was there a sponsor for these campaigns before they launched? Were these campaigns launched in a specific region?
