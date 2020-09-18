# Kickstarting with Excel

## Overview of Project

The goal and purpose of this project was to compare the data of a variety of kickstarter campaigns to determine how launch dates and funding goals affected kickstarter outcomes.  The analysis results, including visualizations, are provided to guide a prospective fundraiser named "Louise" with insights for how to achieve the best results in a kickstarter campaign.


## Analysis and Challenges
	
The analysis was performed by utilizing a diverse dataset of kickstarter campaigns in an excel spreadsheet to identify pertinent trends and patterns for how launch dates and funding goals affected outcomes.  Challenges included the need to convert some of the data to new data types and create new columns in order to extract and isolate the appropriate data for the analysis.  Each of these aspects and their corresponding results are described below.

### Analysis of Outcomes Based on Launch Date

To investigate the relationship in the dataset between kickstarter outcomes and kickstarter launch dates, a pivot table with appropriate filtering was created in a new excel sheet to easily compare the total outcomes for successful, live, failed, and canceled for each month.  The chart was also filtered to include only data for theaters.  Additionally, a line chart provided an excellent visual of the correlations.

![pivot table](https://github.com/alexconerly/kickstarter-analysis/blob/master/images_for_readme/ScreenShot_pivot.png)

### Analysis of Outcomes Based on Goals

To determine the correlation between kickstarter outcomes and monetary goals of kickstarters, the data was filtered to focus on "plays" (a subcategory of "theater").  A table was created to isolate twelve ranges of goal values.  Using these goal value ranges, columns for outcomes (including "number of successful, number of failed, and number of canceled) were created to utilize the "=COUNTIFS" function in excel.  This function provided insight to how each goal range correlated with the number of counts in each categorical column.  Additionally, the SUM function was employed in a "total projects" column to see the total of each goal range for all outcome possibilities.  Finally, this "total projects" column allowed for percentages for each column to be calculated in columns of their own.  Using these percentage values for each outcome and their respective goal ranges, a line chart was then created to visualize how goal ranges affected the percentages of various outcomes.

![countifs](https://github.com/alexconerly/kickstarter-analysis/blob/master/images_for_readme/Screenshot_Countifs_table.png)

## Results

### Conclusions for Outcomes based on Launch Date:

From the analysis, it is evident that the outcomes for campaigns in this dataset had a strong correlation with kickstarter launch dates.  Specifically, the highest number of successful campaigns occurred when launch dates were near the "middle" of the year (May, June, and July).  However, the campaigns were far less successful in the beginning and end of each year, especially in December.  Moreover, there were also more failed campaigns in the middle of the year, indicating there were more campaigns overall in the summer.  Even so, the spike in May, June, and July was slightly less drastic for failed campaigns than for succesful ones.  Ultimately, this suggests the best time to start a theater-related kickstarter campaign may be near the summertime.

![](https://github.com/alexconerly/kickstarter-analysis/blob/master/images_for_readme/Screenshot_Outcomes_Launchdate_Chart.png)

### Conclusions for Outcomes based on Goals:

The analysis of the "outcomes based on goals" resulted in a weaker correlation but offered interesting observations nonetheless.  For example, kickstarter campaigns with goals less than $1000 and between $35k and $45k produced the highest success rates for plays.  In contrast, kickstarter goals for plays with ranges around $25k and above $45k fared the worst in terms of their successful percentage rate.  Also, there were no canceled kickstarters for plays in any goal range.

![](https://github.com/alexconerly/kickstarter-analysis/blob/master/images_for_readme/Screenshot_Outcomes_Goals_Chart.png)

### Limitations of this dataset:

There are many limitations of the analysis worth noting.  For example, in the "outcomes based on goals" analysis, some of the goal ranges include only small samples of observations.  Specifically, there are only five samples with a goal between $25k and $2999 and only one sample with a goal between $45k and $4999.  As such, althouth these two ranges demonstrate significantly low success rates for kickstarter goals, their small sample sizes have greater potential to misrepresent the population.  Also, the analyses for "outcomes based on launch date" and "outcomes based on goals" were filtered for "theaters" and "plays", respectively, and, therefore, may not be representative of all kickstarters.

### Other possible tables and/or graphs that may be useful:
Other possible tables or graphs that could be useful for further research of both analyses include a bar and whiskers and a pie chart.  The bar a whiskers could allow us to identify and exclude outliers which could potentially misrepresent the dataset.  A pie chart, could be useful for visualizing percentages for the outcomes based on the goals analysis.  Finally, the same analysis charts that were used to analyze theaters could also be used to analyze plays and vise versa.
