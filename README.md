# Crowdfunding Campaign Analysis

## Introduction

As part of my GWU Data Analysis & Visualization Boot Camp, I was was tasked with organizing and analyzing a database of 1,000 generated sample crowdfunding projects using Excel.

Excel features used in this project include:
* Excel Formulas
* Conditional Formatting
* PivotTables
* Stacked Column Chart
* Line Chart

## Excel Tasks Completed

1. <b>Conditional Formatting</b><br>
I applied conditional formatting on the campaign outcome column.<br>
![conditional_formatting](Screenshots/conditional_formatting.png)

2. <b>Excel Formala - Rounded Percent</b><br>
I created a column that calculates a rounded percent of the campaign funded using an Excel formula. Column E is the amount pledged and Column D is the campaign goal.
     ```
    =ROUND(E2/D2*100,0)
     ```
3. <b>Conditional Formatting</b><br>
I applied three-color scale conditional formatting to the newly created percent column.
![conditional_formatting_percent](Screenshots/conditional_formatting_percent.png)

4. <b>Excel Formula - Average</b><br>
I created a column that calculates the average donation. Column H is the number of backers and Column E is the amount pledged.
     ```
    =ROUND(IF(H2=0,0,E2/H2),2)
     ```

5. <b>Excel Formula - Text Split</b><br>
I split the category column (Column R), category/subcategory, into two columns, category and subcategory.
     ```
    =TEXTSPLIT(R2,"/")
     ```

A report is inlcuded with conclusions, limitations of the dataset, and other insights.

## Files Included
* CrowdfundingBook.xlsx - Original Excel Workbook
* CrowdfundingBook_Analyzed.xlsx - Organized and Analyzed Excel Workbook
* Crowdfunding_Analysis.docx - Report

Category Stats

Create a new sheet with a pivot table that analyzes your initial worksheet to count how many campaigns were successful, failed, canceled, or are currently live per category.

Create a stacked-column pivot chart that can be filtered by country based on the table that you created.

Subcategory Stats

Create a new sheet with a pivot table that analyzes your initial sheet to count how many campaigns were successful, failed, or canceled, or are currently live per sub-category.

Create a stacked-column pivot chart that can be filtered by country and parent category based on the table that you created.

The dates in the deadline and launched_at columns use Unix timestamps. Fortunately for us, this formulaLinks to an external site. that can be used to convert these timestamps to a normal date.

Create a new column named Date Created Conversion that will use this formulaLinks to an external site. to convert the data contained in launched_at into Excel's date format.

Create a new column named Date Ended Conversion that will use this formulaLinks to an external site. to convert the data contained in deadline into Excel's date format.

Outcomes Based on Launch Date

Create a new sheet with a pivot table that has a column of outcome, rows of Date Created Conversion, values based on the count of outcome, and filters based on parent category and Years.

Now, create a pivot-chart line graph that visualizes this new table.

Create a report in Microsoft Word, and answer the following questions:

Given the provided data, what are three conclusions that we can draw about crowdfunding campaigns?

What are some limitations of this dataset?

What are some other possible tables and/or graphs that we could create, and what additional value would they provide?

Crowfunding Goal Analysis
Create a new sheet with 8 columns:

Goal

Number Successful

Number Failed

Number Canceled

Total Projects

Percentage Successful

Percentage Failed

Percentage Canceled

In the Goal column, create 12 rows with the following headers:

Less than 1000

1000 to 4999

5000 to 9999

10000 to 14999

15000 to 19999

20000 to 24999

25000 to 29999

30000 to 34999

35000 to 39999

40000 to 44999

45000 to 49999

Greater than or equal to 50000

A table and corresponding graph showing the percentage of projects that are successful, failed, and canceled based on their crowdfunding goal.

Using the COUNTIFS() formula, count how many successful, failed, and canceled projects were created with goals within the ranges listed above. Populate the Number Successful, Number Failed, and Number Canceled columns with these data points.

Add up each of the values in the Number Successful, Number Failed, and Number Canceled columns to populate the Total Projects column. Then, using a mathematical formula, find the percentage of projects that were successful, failed, or canceled per goal range.

Create a line chart that graphs the relationship between a goal amount and its chances of success, failure, or cancellation.

Statistical Analysis
Most people would use the number of campaign backers to assess the success of a crowdfunding campaign. Creating a summary statistics table is one of the most efficient ways that data scientists can characterize quantitative metrics, such as the number of campaign backers.

For gaining an in-depth understanding of campaign backers, evaluate the number of backers of successful and unsuccessful campaigns by creating your own summary statistics table.

Create a new worksheet in your workbook, and create one column for the number of backers of successful campaigns and one column for unsuccessful campaigns.

A table containing a column for the number of backers of successful campaigns and a column for unsuccessful campaigns.

Use Excel to evaluate the following values for successful campaigns, and then do the same for unsuccessful campaigns:

The mean number of backers

The median number of backers

The minimum number of backers

The maximum number of backers

The variance of the number of backers

The standard deviation of the number of backers

Use your data to determine whether the mean or the median better summarizes the data.

Use your data to determine if there is more variability with successful or unsuccessful campaigns. Does this make sense? Why or why not?

## References
Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.