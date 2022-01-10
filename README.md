# Kickstarting with Excel

## Overview of Project

### Purpose

The purpose of the project is to help an up-and-coming playwright Louise, who wants to start a crowdfunding campaign to help fund her play. It is necessary to organize, sort, and analyze crowdfunding data to determine whether there are specific factors that make a project's campaign successful.


 analysis is to determine how different campaigns fared in relation to their launch dates and their funding goals. Ultimately, this will help Louise make a decision about starting her crowdfunding campaign.



## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
The purpose of this analysis was to check whether there is a correlation between the launch date of campaigns and the outcomes of campaigns (successful or failed). 
During the analysis, the YEAR() function was used to extract the year from the “Date Created Conversion” column. Then a pivot table was created from the KickStarter worksheet. Finally a line chart was created from the pivot table to visualize the relationship between outcomes and launch month. 

### Analysis of Outcomes Based on Goals
The purpose of this analysis was to visualize the percentage of successful, failed, and canceled plays based on the funding goal amount. The COUNTIFS() function was used to collect the outcome and goal data for the “plays” subcategory. As a result, a new table was created that showed dollar-amount ranges so projects can be grouped based on their goal amount. The COUNTIFS() function was used to populate the "Number Successful," "Number Failed," and "Number Canceled" columns. Then the SUM() function was used to populate the "Total Projects" column with the number of successful, failed, and canceled projects. As a result, the percentage of successful, failed, and canceled projects for each range was calculated. The result was shown on the chart titled "Outcomes Based on Goal" to visualize the relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y-axis.

### Challenges and Difficulties Encountered
After creating tables and graphs and saving the file Excel, I opened the file again and the graphs were not displayed on the sheets. But there was still an option to click on the intended area of the graph and I was able to select it. Despite this, the graph was still not visible. I found a way to overcome this difficulty. When the chart area is selected, you need to go to the Chart Design menu and change the chart design to any of the list. Then press control Z to take a step back and return your chart design. After the actions performed, the graph becomes visible again.

## Results

1. Based on the analysis "Theater Outcomes Based on Launch Date", the following conclusions can be drawn:

- The month that launched the most successful campaigns was May. So the best time to start Louise's campaign is May. The closer to the end of the year, the number of successful campaigns is constantly decreasing. Therefore, Louise is recommended to launch her campaign in May or at least in June.
- The worst time to launch Louise's campaign is October. This month has the maximum number of failed campaigns, while the number of successful launches is quite small.


2. Based on the analysis "Outcomes Based on Goal", the following conclusion can be drawn:
The ranges 35000-39999 and 40000-49000 are the best for Outcomes based on goals. In these ranges, the number of successful campaigns is large (about 70%), while the number of failed campaigns is small (about 30%).
Other ranges with a good percentage of successful (close to 80%) and failed (about 20%) campaigns have a range of "Less Than 1000" and "1000-4999". But these ranges have  relatively small goals and might not be of interest to Louise. Ranges 25000-29999 and 30000-34999, as well as ranges with goals greater than 400000, are the worst. In the ranges 25000-29999 and 30000-34999, the percentage of successful campaigns is minimal (about 20%), while the number of failed campaigns is maximum (about 80%). Also, after 40,000, there is a sharp decrease in successful and an increase in failed campaigns. Therefore, the range with Goals 350000-49000 is more preferable for recomendations.

Possible limitations of this dataset might be that the data was taken from a single source the Kickstarter. It would be interesting to analyze the success of campaigns that raised funds through other resources.
