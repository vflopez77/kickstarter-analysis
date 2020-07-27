Module 1 Challenge Analysis

# Analysis of Play Campaign Outcomes by Launch Date and Goals

## Overview 
Using the Kickstarter data, which contains goal, pledged, and outcome data for all kinds of campaigns, we will look at breakdowns of play campaigns outcomes to see if there are correlations between outcomes and launch date or outcomes and goals.

### Purpose
Our client, Louise, wants to better understand if launch date or goals affect outcomes for play campaigns so she can plan her next campaign.

## Analysis and Challenges
A pivot table was created for the Launch Date analysis.  This allowed us to filter the data for only the theater parent category and breakdown the outcomes by month.  The underlying data of any data point can be seen by double clicking on that cell in the pivot table.  We then graphed the data so see if there were any observable trends.

We used COUNTIFS() formulas for the Goal analysis.  By embedding the criteria in the formulas, we are able to look at all the whole data and only count what we want.  Multiple formulas were entered for 12 different goal ranges, and Successful, Failed, and Canceled (sic) outcomes.  We then created a line graph to visualize the Outcomes vs. Goals.

### Analysis of Outcomes Based on Launch Date
This is the visualization of Outcomes by Launch Date:
<img src=/Resources/Theater_Outcomes_vs_Launch.png></img>
This is the underlying pivot table:
<img src=/Resources/Launch_Date_Pivot_Table.png></img>

### Analysis of Outcomes Based on Goals
<img src=/Resources/Outcomes_vs_Goals.png></img>

The COUNTIFS() formulas did not use the data visible on the sheet as the goal criteria was column was only labels, so there could be errors in the formula criteria which would not be obvious.


### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
