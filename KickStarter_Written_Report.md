# Kickstarting with Excel

## Overview of Project
An in-depth look at how theater KickStarter campaigns have done in relation to their launch dates and their funding goals.
### Purpose
Louise is a playwright looking to fund her play Fever using KickStarter.  The purpose of this project is to analyze the KickStarter dataset in order to gain a visual understanding of the outcomes of other theater KickStarter campaigns based on their launch dates and their funding goals for Louise.  This will help Louise to compare how her KickStarter campaign has fared in relation to others.
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
In order to gain an understanding of the outcomes of Kickstarter campaigns based on launch date a pivot table was created.  First a new column labeled "years" was created based on the date created conversion column in the KickStarter workbook using the year function, =YEAR().  A pivot table was then created based on the KickStarter sheet and placed on a new sheet.  The pivot table was filtered based on "Parent Category" and "Years", outcomes were places in the legend, date created conversion was placed on the axis, and count of outcomes was used as the value.  The column labels were then filtered to show only successful, failed, and canceled outcomes ad they are the most relevant to us, the row labels were grouped to show the months of the year, and the Parent Category was filtered to show only the data for theater as we are only interested in theater Kickstarter campaigns for Louise.  Campaign outcomes were then sorted in descending order so that successful campaigns were ordered first.  From this pivot table we created a line chart to help give Louise a visual of the relationship between the outcomes and the month the KickStarter campaign was launched.
### Analysis of Outcomes Based on Goals
To help gain an understanding of KickStarter outcomes based on goals, a new chart was created.  First a new sheet was created with 8 columns: Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, and Percentage Canceled. Dollar ranges were added to the goal column from less than 1000 to 50,000 or more in 5000 dollar increments to group projects based on their goal amount.  The Countifs function, =COUNTIFS(), was used to populate the Number Successful, Number Failed, and Number Canceled columns.  The Sum function, =SUM(), was then used to populate the Total Projects column and the percentage of successful, failed, and canceled projects was then calculated for each row.  A line chart was then created to help create a visual analysis for outcomes based on goal set.
### Challenges and Difficulties Encountered
There was difficulty with understanding how to use the COUNTIFS function in Excel.  To overcome this additional help was found online.  I searched the function and read more about it and watched videos of it in use to gain a deeper understanding.
## Results

- After futher analyzing outcomes based on launch date we can conclude that May and June were the most successful months for launching a campaign and that the least successful time to start a campaign is in December.

- Analyzing outcomes based on goal shows us that the smaller the monetary goal you set, the more likely you are to be successful in reaching that goal; while campaigns with goals of $45,000 or greater are least likely to be successful.

- What are some of the limitations of this dataset? One of the limitations of the dataset is that it only includes date up to 2017 so we cannot say for sure if recent campaigns have followed the same trends that we saw from 2009-2017.  

- What are some other possible tables and/or graphs that we could create?We could also create a graph that shows the percentage of campaigns that were successful, failed, or cancelled based on the month that they were launched to help us gain a deeper understanding of how many campaigns were successful, failed, or canceled.  We could also create a chart that compares the date created and date ended to the outcomes to help determine whether shorter or longer campaigns are most likely to be successful.
