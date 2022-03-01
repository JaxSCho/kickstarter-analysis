# Kickstarting with Excel

## Overview of Project

### Purpose

Using the Kickstarter dataset, we were able to help Louise plan a crowdfunding campaign for her play *Fever* by analyzing potential factors, such as average donation and length of the campaign, that may contribute to a successful fundraising campaign. We've learned that Louise's campaign came close to its fundraising goal in a short amount of time. This project will provide further insights into how different campaigns fared regarding their launch dates and funding goals. 

## Analysis and Challenges

The following analysis presents how the launch date and funding goals related to the outcome of crowdfunding campaigns for theater/play categories. A description of possible challenges or difficulties encountered is also provided.

### Analysis of Outcomes Based on Launch Date

To consider if theater campaigns tend to be more successful during a specific time of year, we examined the number of successful, failed, and canceled theater campaigns based on the month of their campaign launch date using the Kickstarter dataset (Figure 1). Live campaigns were removed from this analysis since the outcome of these campaigns is unknown. Using filters, Figure 1 displays data for only theater campaigns and, therefore, allows us to focus on projects similar in scope and type to Louise's vision.

![theater_outcomes_vs_launch](https://github.com/JaxSCho/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)
<b>Fig.1 - Theater Campaign Outcomes Based on Launch Date</b>

### Analysis of Outcomes Based on Goals

Using the Kickstarter dataset, we also reviewed the percentage of successful, failed, and canceled play campaigns by their funding goal (Figure 2). This analysis can provide insight into how fundraising goals relate to the success of play campaigns. Live campaigns were removed from this analysis since the outcome of these campaigns is unknown. 

![outcomes_vs_goals](https://github.com/JaxSCho/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)
<b>Fig.2 - Play Campaign Outcomes Based on Funding Goal</b>

### Potential Challenges and Difficulties

Since the Kickstarter dataset had to be manipulated in various ways using Excel, several challenges and difficulties could have been encountered when generating the results of this project. For instance, if the use of parent category and outcomes filters was overlooked when creating Figure 1, different conclusions may occur since the scope of the data would differ. Also, the percentage for each outcome in Figure 2 is dependent on the outcome counts and the total number of projects per the listed funding goal range. Therefore, typing errors in the COUNTIFS() statements used for these values can generate incorrect findings. Creating a "check sum" value based on a different counting approach allows us to confirm our results independently.      


## Results

The results of this analysis were created using [Kickstarter dataset](https://github.com/JaxSCho/kickstarter-analysis/blob/main/Kickstarter_Challenge.zip). This document provides the background tables and charts for this analysis and can further project insights.

- What are two conclusions you can draw about the Outcomes-based on Launch Date?

  1. Upon observation, we can determine that theater is a popular and successful type of campaign overall since the number of successful theater campaigns is greater than the number of failed or canceled theater campaigns throughout the year.

  2. We can also conclude that theater fundraising campaigns are more likely to succeed if they are launched in May and June. The number of successful campaigns is more than twice as many failed campaigns during these two months (i.e., 111 successful vs. 52 failed and 100 successful vs. 49 failed in May and June, respectively). 

- What can you conclude about the Outcomes-based on Goals?

One apparent observation is that there were no canceled play campaigns in the Kickstarter dataset. We can also identify that successful play campaigns generally have lower fundraising goals than failed campaigns. If the funding goal is less than $35,000, there is a clear negative correlation between the funding goal and the success of meeting the fundraising goal. However, there were more successful play campaigns vs. failed play campaigns at two higher funding goal intervals, ranging between $35,000 and $45,000 (i.e., 66.7% success rate). Upon further inspection, only about 0.9% of the 1,047 play campaigns have fundraising goals between this interval. Therefore, caution should be used when drawing conclusions from such a small sample of outcomes.

- What are some limitations of this dataset?

The data only contains campaigns launched from 2009 to 2017. Therefore, future campaigns with different economic environments or spending patterns (i.e., play production closures and spending habits in 2020 - 2022 due to the COVID-19 pandemic) may have contrasting funding campaign outcomes. Also, there was minimal data on canceled theater/play campaigns, and therefore, we are unable to gain insight into why these campaigns were canceled. Based on our prior findings, the mean and median failed pledge amounts are much lower than the successful pledges, which reveals that failed play campaigns are unsuccessful for reasons other than having lofty fundraising goals. Additional details such as incentive usage and initial concept interest could provide further insights into why specific campaigns were successful.

- What are some other possible tables and/or graphs that we could create?

Other possible tables and graphs could be created using the data available. Understanding the relationship between a campaign outcome based on geography and the duration of a campaign could help determine additional factors that contribute to a successful campaign. Since the campaign's success is determined if its funding goal is met, further inspection of the data relevant to the investors, such as amount pledged, number of backers, and average donation, may reveal similar investor characteristics in successful campaigns. Performing a correlation analysis or multiple logistic regression analysis can create a more comprehensive picture of the factors contributing to a successful campaign, such as how the factors relate to each other and the campaign outcome.  
