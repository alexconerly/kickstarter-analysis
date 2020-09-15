# Kickstarting with Excel

## Overview of Project

The goal and purpose of this project was to compare the data of a variety of kickstarter campaigns to determine how launch dates and funding goals affected kickstarter outcomes.  The analysis results, including visualizations, are provided to guide a prospective fundraiser named "Louise" with insights for how to achieve the best results in a kickstarter campaign.


## Analysis and Challenges
	
The analysis was performed by utilizing a diverse dataset of kickstarter campaigns in an excel spreadsheet to identify pertinent trends and patterns in order to compare and visualize how launch dates and funding goals affected outcomes.  Challenges in included the need to convert some of the data to new data types and create new columns in order to extract and isolate the appropriate data for the analysis.  Each of these two aspects and their corresponding results are described below:

### Analysis of Outcomes Based on Launch Date

To investigate the relationship in the dataset between kickstarter outcomes and kickstarter launch dates, a pivot table with appropriate filtering was created in a new excel sheet to easily compare the total outcomes for successful, live, failed, and canceled vs each month.  The chart was also filtered appropriately to include only data for theaters.  Additionally, a line chart provided an excellent visual of the correlations.


### Analysis of Outcomes Based on Goals

To determine the correlation between kickstarter outcomes and monetary goals of kickstarters, a table was created to isolate twelve ranges of goal values.  Using these goal value ranges, columns for outcomes (including "number of successful, number of failed, and number of canceled) were created to utilize the "=COUNTIFS" function in excel.  This function provided insight to how each goal range correlated with the number of counts in each categorical column.  Additionally, the SUM function was employed in a "total projects" column to see the total of each goal range for all outcome possibilities.  Finally, this "total projects" column allowed for percentages for each column to be calculated in columns of their own.  Using these percentage values for each outcome and their respective goal ranges, an insightful line chart was then created to visualize how goal ranges affected the percentages of various outcomes.


## Results

- Conclusions for Outcomes based on Launch Date:

From the analysis, it is clear that the outcomes for campaigns in this dataset had a strong correlation with launch date.  Specifically, the most successful campaigns in the dataset occurred when launch dates were near the "middle" of the year (May, June, and July).  However, the campaigns were far less successful in the beginning and end of each year, especially in December.  Interestingly, no cancellations were made from kickstarters which launched in October in the dataset.

- Conclusions for Outcomes based on Goals:

The analysis of the outcomes based on goals demonstrated an unclear correlation in the dataset.  However, some interesting observations exist.  For example, kickstarter campaigns with goals less than $1000, between $25000 and $2999, and greater than $45,000 fared the best in terms of their successful percentage rate.  Also, there were no canceled kickstarters in any goal range.

- Limitations of this dataset:

There are many limitations of the dataset worth noting.  For example, in the "outcomes based on goals" analysis, the chart shows two successful spikes between goals of around $25k and $45k but this may not be evenly representatively of each range because some of the data counts are very low in those ranges.  For example, there are only five samples in the range of $25k to $2999.  Thus, the line chart may not account for the potentially misrepresentative percentages due to small sample sizes in certain goal ranges.  Also, when comparing the outcomes based on launch date, the data is strictly focused on theaters and thus may or may not be representative of all kickstarters.

- Other possible tables and/or graphs that we could create:
Another possible table or graph that could be useful for both analyses may be a bar chart.   Also, a pie chart may be useful for visualizing percentages for the outcomes based on goals analysis.