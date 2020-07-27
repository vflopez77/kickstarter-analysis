Module 1 Challenge Analysis

# Analysis of Play Campaign Outcomes by Launch Date and Goals

## Overview 
Using the Kickstarter data, which contains goal, pledged, and outcome data for all kinds of campaigns, we will look at breakdowns of play campaigns outcomes to see if there are correlations between outcomes and launch date or outcomes and goals.

### Purpose
Our client, Louise, wants to better understand if launch date or goals affect outcomes for play campaigns so she can plan her next campaign.

### Analysis of Outcomes Based on Launch Date

A pivot table was created for the Launch Date analysis.  This allowed us to filter the data for only the theater parent category and breakdown the outcomes by month.  The underlying data of any data point can be seen by double clicking on that cell in the pivot table.  We then graphed the data so see if there were any observable trends.

This is the visualization of Outcomes by Launch Date:

<img src=/Resources/Theater_Outcomes_vs_Launch.png></img>

This is the underlying pivot table:

<img src=/Resources/Launch_Date_Pivot_Table.png></img>

### Analysis of Outcomes Based on Goals

We used COUNTIFS() formulas for the Goal analysis.  By embedding the criteria in the formulas, we are able to look at all the data and only count what we want.  Multiple formulas were entered for 12 different goal ranges, and Successful, Failed, and Canceled (sic) outcomes.  We then created a line graph to visualize the Outcomes vs. Goals.

This is the visuatlization of Outcomes by Goals:

<img src=/Resources/Outcomes_vs_Goals.png></img>

This is the underlying Outcomes by Goals data table:

<img src=/Resources/Goal_Outcome_Table.png></img>

Here is a sample COUNTIFS() formula:

=COUNTIFS(Kickstarter!$R:$R,"plays",Kickstarter!$D:$D,">=1000",Kickstarter!$D:$D,"<5000",Kickstarter!$F:$F,"successful")

### Challenges and Difficulties Encountered

For the Goals analysis, the COUNTIFS() formulas did not use the goal data visible on the sheet as the goal criteria column was only labels.  Each formula had to be individually edited and there could be errors in the formula criteria which would not be obvious.

## Results
### Conclusions about the Theater Outcomes Based on Launch Date analysis:
- The best part of the year to launch campaigns is May-July.  The worst part of the year to launch campaigns is November-January

### Conclusion about the Outcomes based on Goals analysis:
- The most successful campaigns set goals of 35,0000 to 50,000.

### Limitations of Dataset:
- There are different currencies that are not converted to be equivalent.  

### Other possible Tables or Graphs:
- Percentages of Successful Outcomes by Month