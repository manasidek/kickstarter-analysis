# **Kickstarting with Excel**

## Overview of Project
### Purpose
The purpose of this analysis is to help Louise understand how different campaigns fared in relation to their launch dates and their funding goals, to help Louise understand ideal launch dates and goals for successful campaigns.

The Kickstarter data available for analysis provided information about campaign outcomes based on launch dates and campaign goals, so analyzing this data provided insights that can help Louise make better decisions.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
After reviewing the Kickstarter data, a Years column was created to give a better understanding about the launch dates. Louise needed to visualize outcomes based on launch dates for ‘theater’ category, for which a pivot table was created to summarize outcomes of all “Theater” campaigns. A line chart was created based on the pivot table as shown in the image below.
![Theater Outcomes Based On Launch Date](https://github.com/manasidek/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
For this analysis, Louise wanted the outcomes of the category ‘theater’ and subcategory ‘plays’ alongside the goals. Thus, a table was created with goals with ranges of $5000 intervals for different outcomes and percentage outcomes were calculated for each range. These percentages were visualized in a line chart as shown below.
![Outcomes Based On Goal](https://github.com/manasidek/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
The date in ‘launched_at” column in the Kickstarter data was not in readable format, so it needed to be extracted using conversion formula to an actual date, which is stored in the column named ‘Date created conversion’. This column was further used to create the ‘Years’ column.

## Results

1. What are two conclusions you can draw about the Outcomes based on Launch Date?

-  Campaigns launched in the month of ‘May’ show a significant success rate compared to other months.
-  Campaigns launched in the month of ‘December’ show lowest success rate compared to other months. There are slightly more failed campaigns compared to successful ones.

2. What can you conclude about the Outcomes based on Goals?
-	 The campaigns of goals of less than $5,000 and those between $35,000 and $45,000 have better success rate as compared to other ranges.

3. What are some limitations of this dataset?
-  Amounts in ‘goal’ and ‘pledged’ columns are formatted in USD but the ‘currency’ column shows other currencies such as GBP, EUR, AUD, etc.

4. What are some other possible tables and/or graphs that we could create?
-  A column that shows duration of each campaign using the difference between ‘Date created conversion’ and ‘Date ended conversion’ columns. Then a table can be created to show percentage outcomes based on duration ranges.
-	 A table showing average goal amounts and percentage outcomes by ‘parent category’ can be created to understand performance of campaigns across categories.
