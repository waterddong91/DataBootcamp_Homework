# Excel- Kickstart My Chart

## Background

Over $2 billion has been raised using the massively successful crowdfunding service, Kickstarter, but not every project has found success. Of the more than 300,000 projects launched on Kickstarter, only a third have made it through the funding process with a positive outcome.

Getting funded on Kickstarter requires meeting or exceeding the project's initial goal, so many organizations spend months looking through past projects in an attempt to discover some trick for finding success. For this week's homework, you will organize and analyze a database of 4,000 past projects in order to uncover any hidden trends.

## Kickstarter Chart

![Kickstarter Table](Images/FullTable.PNG)

Used the Excel table provided, modified and analyzed the data of 4,000 past Kickstarter projects as you attempt to uncover some market trends.

* Used conditional formatting to fill each cell in the `state` column with a different color, depending on whether the associated campaign was successful, failed, or canceled, or is currently live.

  * Created a new column O called `Percent Funded` that uses a formula to uncover how much money a campaign made to reach its initial goal.

* Used conditional formatting to fill each cell in the `Percent Funded` column using a three-color scale. The scale starts at 0 and be a dark shade of red, transitioning to green at 100, and blue at 200.

  * Created a new column P called `Average Donation` that uses a formula to uncover how much each backer for the project paid on average.

  * Created two new columns, one called `Category` at Q and another called `Sub-Category` at R, which use formulas to split the `Category and Sub-Category` column into two parts.

  ![Category Stats](Images/CategoryStats.PNG)

  * Created a new sheet with a pivot table that will analyze your initial worksheet to count how many campaigns were successful, failed, canceled, or are currently live per **category**.

  * Created a stacked column pivot chart that can be filtered by country based on the table you have created.

  ![Subcategory Stats](Images/SubcategoryStats.PNG)

  * Creatde a new sheet with a pivot table that will analyze the initial sheet to count how many campaigns were successful, failed, or canceled, or are currently live per **sub-category**.

  * Created a stacked column pivot chart that can be filtered by country and parent-category based on the table you have created.

* The dates stored within the `deadline` and `launched_at` columns use Unix timestamps.

  * Created a new column named `Date Created Conversion` that will use [this formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html) to convert the data contained within `launched_at` into Excel's date format.

  * Created a new column named `Date Ended Conversion` that will use [this formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html) to convert the data contained within `deadline` into Excel's date format.

  ![Outcomes Based on Launch Date](Images/LaunchDateOutcomes.PNG)

  * Created a new sheet with a pivot table with a column of `state`, rows of `Date Created Conversion`, values based on the count of `state`, and filters based on `parent category` and `Years`.

  * Created a pivot chart line graph that visualizes this new table.

* Created a report in Microsoft Word and answered the following questions.

1. Given the provided data, what are three conclusions we can draw about Kickstarter campaigns?
2. What are some limitations of this dataset?
3. What are some other possible tables and/or graphs that we could create?

* Created a new sheet with 8 columns:

  * `Goal`
  * `Number Successful`
  * `Number Failed`
  * `Number Canceled`
  * `Total Projects`
  * `Percentage Successful`
  * `Percentage Failed`
  * `Percentage Canceled`

* In the `Goal` column, created 12 rows with the following headers:

  * Less than 1000
  * 1000 to 4999
  * 5000 to 9999
  * 10000 to 14999
  * 15000 to 19999
  * 20000 to 24999
  * 25000 to 29999
  * 30000 to 34999
  * 35000 to 39999
  * 40000 to 44999
  * 45000 to 49999
  * Greater than or equal to 50000

  ![Goal Outcomes](Images/GoalOutcomes.PNG)

* Used the `COUNTIFS()` formula, count how many successful, failed, and canceled projects were created with goals within the ranges listed above. Populated the `Number Successful`, `Number Failed`, and `Number Canceled` columns with this data.

* Added up each of the values in the `Number Successful`, `Number Failed`, and `Number Canceled` columns to populate the `Total Projects` column. Then, used a mathematical formula, found the percentage of projects that were successful, failed, or canceled per goal range.

* Created a line chart that graphs the relationship between a goal's amount and its chances at success, failure, or cancellation.

*Evaluate the number of backers of successful and unsuccessful campaigns by creating the summary statistics table.

* Created a new worksheet and created a column each for the number of backers of successful campaigns and unsuccessful campaigns.

  ![Images/backers01.png](Images/backers01.png)

* Used Excel to evaluate the following for successful campaigns, and then for unsuccessful campaigns:

  * The mean number of backers.

  * The median number of backers.

  * The minimum number of backers.

  * The maximum number of backers.

  * The variance of the number of backers.

  * The standard deviation of the number of backers.

* Used the data to determine whether the mean or the median summarizes the data more meaningfully.

* Used the data to determine if there is more variability with successful or unsuccessful campaigns. 
- - -
