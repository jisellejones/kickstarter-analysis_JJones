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
* Is there any pattern in the amount of funding goals and the success of theater campaigns for plays? 
* Are campaigns for plays in some goal ranges more successful than campaigns in other goal ranges?

---
## Analysis and Challenges
The crowdfunding data used in this analysis was pulled from the University of Oregon Data Analysis Boot Camp database. The data was filtered and analyzed using Excel's formulas, statistical tools, and graphic displays. 


### Analysis of Outcomes Based on Launch Date
How do different theater campaigns fare in relation to their launch date? Are some months of the year better than others for launching theater campaigns? In order to answer these questions, we filtered the theater data by month and disagregated the data by outcome then created a line graph from the data (graph 1). For successful campaigns, we see a spike in the number of successful campaigns in May. While the number of successful campaigns begins to decline after May, there is still a high number of successful campaigns in June. This could indicate that starting a campaign in May or June may yield the highest success rate, but we need to dive further into the data before making a conclusion.

While the overall data for outcomes based on launch date show a high number of successful campaigns during the month of May, the data also show a spike in the number of campaigns that fail. In fact, the month of May shows the highest number of failed campaigns of all the months. This leads to the question, "Is the higher number of both successes and failures during the month of May due to the higher number of total campaigns started during the month of May?" In order to answer this question, we found and compared the percentages of successful and failed campaigns for each month (graph 2). The graph based on percentages still shows an increase of succesful campaigns in the month of May, but now we see a decrease in the percentage of failed campaigns during the same month indicating that, indeed, beginning a campaign in the month of may could yield higher rates of success. 

Are some months of the year worse than others for launching theater campaigns for plays? From graph 2, we can see that the percentage of failed campaigns remains somewhat constant around 30% from January through September and then then increase to 43% in October and 47% in December. We also see a significant decrease in the percentage of successful campaigns in December. This suggests that October and December would be poor months to begin a campaign.

---
*(graph 1)*
![Theater_Outcomes_vs_Launch](https://github.com/jisellejones/kickstarter-analysis_JJones/blob/main/Theater_Outcomes_vs_Launch.png)

---
*(graph 2)*
![Theater_Outcomes_vs_Launch_Percentage](https://github.com/jisellejones/kickstarter-analysis_JJones/blob/main/Theater_Outcomes_vs_Launch_percentage.png)
---
### Analysis of Outcomes Based on Goals
How do different theater campaigns for plays fare in relation to their funding goals? Is there any pattern in the amount of funding goals and the success of theater campaigns for plays? Are campaigns in some goal ranges more successful than campaigns in other goal ranges? To answer these questions, I created a frequency table using Excel's countifs() formula to sift through the data and count the number of plays with specified outcomes (successful, failed, canceled) based on different ranges of campaign goals. I compiled this data in a frequency chart then used Excel's sum() function to find the total number of campaigns that fall within different ranges in order to find the percentage of successful, failed, and canceled campaigns. We combined this data in the line graph shown *(graph 3)*

Campaign goals of less than $1,000 show a 76% success rate and campaigns goals between $1,000 and $4,999 have a 73% success rate. These are the highest success rates indicating that it is best to set campaign goals within these ranges. From the graph, we can see a pattern of decline in the percentage of successful campaigns after these ranges to $29,999. Then the percentage of successful campaigns begins to increase again dropping significantly when campaign goals hit $45,000 or more. Failed campaigns follow an opposite trend. 

It is important to point out that campaigns with goals of $35,000 to $44,999 show success rates of 67%. It may seem that this should indicate a likelihood of success when setting goals within these ranges; however, there were only 9 campaigns within this range, I do not believe this is enough data to draw a solid conclusion.

It was impossible to do any analysis on the canceled campaigns as there were 0 campaigns canceled for this data set. The lack of canceled campaigns for this data set leads to the question, "What could cause campaigns to be canceled?" and, "Why are there canceled campaigns in other categories/subcategories, but not for plays?"

---
*(graph 3)*
![Outcome_vs_Goals](https://github.com/jisellejones/kickstarter-analysis_JJones/blob/main/Outcomes_vs_Goals.png)


### Challenges and Difficulties Encountered
When trying to reach a conclusion about which month might be best or worse to begin a campaign, it was difficult to reach a conlusion from looking at only the number of outcomes. It was difficult to differentiate between the success of campaigns being correlated with the month of the year or the higher number of campaigns launched. In May 166 campaigns were launched versus December when only 75 campaigns were launched, so we had to consider a different method of analysis to eliminate the number of campaigns.

When comparing the outcomes to the campaign goals, the data showed a 67% success rate for campaigns with goals from $35,000 to $44,999. Based on percentages alone, it would seem reasonable to conclude that these goal ranges would be more likely to yield successful campaigns; however, there are only 9 campaigns total for this range of campaign goals. I would be unreasonable to make any conclusions based on such a small amount of data. 

---
## Results
From these analyses, we can conclude that May is the best month to begin a campaign. We can also conclude that beginning a campaign in December may increase the likelihood of the campaign failing.

Campaigns that have a campaign goal of less than $5,000 are more likely to be successful than campaigns that have campaign goals of $5,000 or more. The number of campaigns was small for campaign numbers with goals in the range of $25,000 to $49,999 rendering the analysis inconclusive for campaign goals in these ranges. However, out of 14 

While there was a substantial amount of data for this dataset, the data was gathered from many different countries. In order to determine the likelihood of success in a particular country, further filtering could be applied to determine if conclusions drawn for all countries applies to a particular country. 

Unfortunately, there was not enough data in the plays category to capture patterns within the canceled campaigns during particular months of the year. There was no data about canceled campaigns when determining the outcomes of campaigns based on campaign goals. Future analyses may consider taking a closer look at this data set by analyzing canceled campaigns across all parent categories or all subcategories of theater campaigns rather than simply the play subcategory.

Since the data comparing campaign outcomes to campaign goals was gathered as different ranges, a box plot or scatterplot may offer some deeper insight into the data.

Future analyses may also consider looking at correlations between the successful and failed campaigns in months where a greater percentage of campaigns were successful and months where a greater percentage of campaigns failed along side the campaign goal data for those months to determine if there are better or worse campaign goals during different months of the year.

It would be interesting to research the 2 successful campaigns with campaign goals amounts of $50,000 or more. Was there a sponsor for these campaigns before they launched? Were these campaigns launched in a specific country?
