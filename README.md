# Kickstarting with Excel

## **Overview of Project**

### **Purpose**

This project was to assess kickstarter campaign data for a variety of categories and countries. The purpose of this project was to analyze campaign outcomes, specifically for Theater campaigns and plays in particular. The goal of the analysis was to identify theater outcomes based on their launch date as well as outcomes for plays based on goal numbers and to identify any conclusions from the analysis of these numbers. 

## **Analysis and Challenges**

To perform my analysis, I first had to make sure all filters were cleared from my 'Kickstarter' spreadsheet. I then had to create new sheets within my spreadsheet to hold the analyses I wanted to do ('Theater Outcomes by Launch Date' and 'Outcomes Based on Goals').

#### *Analysis of Outcomes Based on Launch Date*

To create the pivot table for my outcomes based on launch date, I selected all of my data from the 'Kickstarter' spreadsheet. Then I inserted a pivot table and placed the pivot table into a new sheet in the workbook. I selected the filters based on years and subcategory, with outcomes as my row option, date created conversion as my columns option, and count of date as my outcomes. Lastly, I inserted a line plot graph using the data in my pivot table.

Copy of pivot table:
![](Module%201%20Challenge/Resources/Outcomes by Launch Date Pivot.png)

Graph of Theater Outcomes Based on Launch Date:
![](Module%201%20Challenge/Resources/Theater_Outcomes_vs_Launch.png)

### *Analysis of Outcomes Based on Goals* 

To analyze my outcomes based on goals data, I had to sort the Kickstarter plays data based on goal numbers. To do so, I created buckets of goal amounts in increments of $5,000. Then I created COUNTIF formulas to pull the data and count the number of plays within each goal range based on number successful, number failed, and number canceled. To count the number of total projects for each goal range, I performed a SUM formula to count all plays within that goal range (number successful, failed, and canceled). Once I found the total number of projects for each goal range, to find the percentage for each category (successful, failed, and canceled), I simply took the cell that contained the number of plays for the category I was trying to find (successful, failed, or canceled) and divided by the total projects. Lastly, I inserted a line plot graph using the data in my table.

![](Module%201%20Challenge/Resources/Formula_Canceled_CountIF.png)

![](Module%201%20Challenge/Resources/Formula_Failed_CountIF.png)

![](Module%201%20Challenge/Resources/Formula_Successful_CountIF.png)

![](Module%201%20Challenge/Resources/Formula_Failed_CountIF.png)

Graph of Outcomes Based on Goals:
![](Module%201%20Challenge/Resources/Outcomes_vs_Goals.png)

### *Challenges and Difficulties Encountered* 

Fortunately, I did not run into many challenges while conducting this analysis. 

One minor challenge I ran into when selecting the data for my pivot table for my outcomes based on launch date data, was the date created time conversion and editing the rows in the pivot table so they showed the months rather than years and quarters. I noticed there were multiple options under the Rows box. By deleting some of the options, I was able to remove higher level data and get down to the month level.

The primary challenge I ran into was making sure for my outcomes based on goals data, when I was creating my COUNTIF formula that I was accurately inputting the conditions for each goal amount bucket that was created. One way I overcame this was to refer back to the module practice and revisit the COUNTIF formula sections. I also went into the 'Kickstarter'spreadsheet and manually filtered the Goal column for amounts that fell into the goal amount bucket to double check my work and make sure my formula was inputted correctly.

## **Results**

From our data on outcomes based on launch date, we can conclude the most successful months for plays are in the summer during the months of May and June. These are also the months were there are the most plays launched. 

From our data on outcomes based on goals, there does not appear to be any correlation between goal amount and success rate. Projects with very low goals and those with high goals (less than $1000 and greater than $50,000 for example) have similar rates of success (76% compared to 67%) and failure (24% compared to 33%).

One limitation of this dataset is that the total number of projects are not equally distributed within each goal band in the dataset. For example, excluding projects with a goal amount of $10,000 to $14,999, all other projects with goal amounts of $19,999 or below had at least 100 projects or more. When we examine the number of projects with goal amounts of $20,000 to $49,999, the total projects are 20 or less which is a lot less in comparison. There was only one project with a goal between $45,000 to $49,999. With a limited number of projects within certain goal bands as defined in the dataset, there is not much data for us to draw a solid conclusion about correlation between goal amount and project success or failure rate.

Other possibilities we can look at and assess using this dataset are filtering the theater and play outcomes by countries to determine if there are any differences in performance and outcomes based on country as well as time of year. Through this analysis we can compare performance based on time of year for each country as well as country to country performance comparison.
