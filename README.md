# Analysis of Kickstarter Campaigns using Excel

## Overview of Project

### Purpose
You asked how different campagins fared in relation to their launch dates and their funding goals. In this project, I analyze the Kickstarter dataset to visualize campaign outcomes based on their launch dates and their funding goals. Using this analysis, I make inferences about the best time to launch and the best goal range to set in order to have a successful campaign.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
For this analysis, I used the [YEAR function](https://support.microsoft.com/en-us/office/year-function-c64f017a-1354-490d-981f-578e8ec8d3b9) in Excel to extract a 4-digit year from the previously converted launch date. This allowed me to create a pivot table that allowed for separation of campaigns by launch month. It also allows for filtering by year, to see if the seasonal trend changes over time, and filtering by parent category, to focus on the type of campaigns most relevant for you (see sheet "Theater Outcomes by Launch Date" for interactive Pivot Table). The chart below visualizes outcomes for theater campaigns for all years in the data set (2009 - 2017), allowing us to see the seasonality of campaign outcomes. 

![Theater Outcomes based on Launch Date](https://github.com/jrpillai/kickstarter-analysis/blob/1d626631895c48ba1000db11144bcdd1bdd2cec6/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
For this analysis, I used the [COUNTIF function](https://support.microsoft.com/en-us/office/countif-function-e0de10c6-f885-4e71-abb4-1f464816df34) in Excel to determine the number of campaigns that were successful, failed, or cancelled in useful ranges ($5,000 increments) of campaign goal size. I also calculated the percentage of campaigns that were successful, failed, or canceled in each range. The same function also allowed me to filter for only plays. As a result, we can see which goal range is most likely to be successful, and what percentage of campaigns in each range are successful. The chart below visualizes the percent successful and percent failed campaigns in each range of campaign goal size, allowing us to quickly see what size of campaign goal is most likely to succeed.

![Outcomes based on Goals](https://github.com/jrpillai/kickstarter-analysis/blob/1d626631895c48ba1000db11144bcdd1bdd2cec6/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

For the analysis of outcomes based on launch date, one notable challenge is that the data starts in 2009, when there are still relatively few campaigns on kickstarter. If you filter and look at data from earlier years, you see that there are few discernible trends. Clear seasonality emerges by 2014, and the number of campaigns launched from 2014-2017 is large enough that it overwhelms the data from early years. Still, it does raise the question - will this seasonality be persistent, or will it change as the platform ages?


For the analysis of outcomes based on goals, the most obvious challenge is that there are far more campaigns in the lower goal ranges than there are above $15,000. Because there are fewer data points in the larger ranges, apparent trends may actually be caused by other considerations specific to the individual campaigns. Because I analyzed the percent of each range that had a specific outcome, the number of campaigns in each range is obscured. You can see that the number of plays in each range is heavily weighted to the bottom of the spectrum in the image below:

![Total Projects by Goal Size (Plays only)](https://github.com/jrpillai/kickstarter-analysis/blob/688bc4751555276d2a4277e8c0c773749cb66bdc/resources/Plays_by_Goal_Size.png)

## Results

### Outcomes based on Launch Date - Conclusions
The success of theater kickstarter campaings is clearly seasonal. Campaigns launched in late spring and early summer are most successful, and success steadily falls through winter. The best time to launch a campaign is May - June. 

You can also see that in May-June, about twice as many campaigns are successful as fail. At other times of the year, a higher proportion of campaigns fail. Overall however, at least for theater campaigns, there is a good chance of having a successful campaign at any time of year. 


## Outcomes based on Goals - Conclusions
In general, campaigns with lower goals are more successful, with the percentage of successful campaigns falling significantly at the $20,000 to $29,999 interval. Campaigns with a goal less than $5,000 are reasonably successful, with only about one-quarter of them failing. However the distribution is bimodal - there is another group of campaigns around $30,000 - $45,000 that are also quite successful, with about two-thirds of campaigns being successful. 

## Limitations of the Dataset
For the outcomes based on goals, there a far fewer campaigns in the highest range and some data points that are likely outliers, making conclusions less reliable. 

## Other graphs or tables
Other possible graphs or tables might include:
* A table showing the percentage of theater campaigns that were successful in each month. 
* A line graph showing how the seasonality of campaign success has changed over years, with a separate curve for 2014, 2015, and 2016.
* A box and whisker plot showing the spread of campaign goals to identify outliers.
* A revised line graph that has removed the outliers to improve the ability to discern real trends. 

