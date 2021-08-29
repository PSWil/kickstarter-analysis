# Kickstarting with Excel

## Overview of Project

For this project we have a client who is interested in funding a theatre production through the crowdfunding website Kickstarter. In this project we are asked to analyze data from Kickstarter in order to gain a better understanding of Theatre trends. More specifically the client is interested in understanding trends related to the success and failure of Kickstarter campaigns for Plays in the US.

### Purpose

Our purpose for this analysis is to provide the client with in-depth and meaningful analysis that is applicable to the client’s project, and to visualize the data to aid in analysis. In order to achieve this, we need to curate and filter the data set so that the analysis is most relevant to the project the client is working on.

## Analysis and Challenges

In order to properly analyze the data to produce relevant information we took a few steps to organize and categorize the data so that we had more specific variables to work with. First, we added some columns including average donation, parent category, subcategory, date created conversion, date ended conversion and years. Filtering the larger data set we were interested in understanding trends specific to the success and failure of campaigns that were in the subcategory ‘plays’ that were launched in the US. Using pivot tables we were able to create graphs that visualized the data for the client so that they were able to see the outcomes of campaigns based on their launch date (https://github.com/PSWil/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png) and outcomes of campaigns based on their goals ( https://github.com/PSWil/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png). One challenge that I encountered during this process was organizing my pivot tables correctly so that the graph produced matched the expected outcome. 

### Analysis of Outcomes Based on Launch Date

To analyze the data to look at the outcomes of campaigns based on their launch date we need to filter the larger data set to include only the Kickstarter campaigns in the category of theatre and the country of the US. In a new sheet we created a pivot table that was filterable by parent categories and years. In categories we put the date created conversion and modified it to show the campaigns grouped by the month of the year. In series we put the outcomes, and in values with put the count of outcomes. Now on our pivot table we can filter the parent category to show only theatre results and our columns show the number of successful, failed, and canceled campaigns and their totals and the rows show the months of the year. Next, we created a line graph that shows this data in order to analyze it. https://github.com/PSWil/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png

### Analysis of Outcomes Based on Goals

To analyze the data to look at the outcomes of campaigns based on their goals we created a new sheet and organized the data to group successful, failed and canceled campaigns by the dollar amount of the goal they were trying to achieve. To populate the first few columns of our sheet we used COUNTIFS e.g. “=COUNTIFS(Kickstarter!D:D,"<1000",Kickstarter!F:F,"successful",Kickstarter!R:R,"plays")” to group the campaigns. We totaled each row buy using SUM e.g. “=SUM(D2:B2)”. Then got the percentage for each by dividing the correct cells e.g. “=(B2/E2). From this table we created a line graph that visualized the outcomes of campaigns based on their goals that we used for the analysis. https://github.com/PSWil/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png

### Challenges and Difficulties Encountered

I was nervous to begin working with such a large data set but the instruction in class and online combined with the tools provided in excel helped me get comfortable with organizing and visualizing the data. The biggest challenge for me on this project was getting more comfortable with excel in general and working and organizing my pivot tables so that they were displaying the correct information, after several hours I got very comfortable with it.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
When we look at our graph of campaigns based on their launch date we can see some very noticeable trends over the course of a year. One trend immediately stands out is that the percentage of campaigns that are successful is much higher in the months of May, June and July. In addition to that the months of April through August on average have more successful campaigns than the other months of the year. Another trend that stands out is that the rate of failure for Kickstarter campaigns throughout the year remains relatively stable indicating that more campaigns are started in the months of April through August. The data also shows that the absolute worst month of the year to launch a campaign in is December. In summation from the data of campaigns based on their launch date it is generally advisable to launch a Kickstarter campaign for a theatre production in the subcategory ‘plays’ in the months between April and August.

- What can you conclude about the Outcomes based on Goals?
When we look at our graph of outcomes of campaigns based on their goals the data is a little bit harder to interpret. However, we can see that campaigns had the greatest percentage of success when their stated goal was less than $15,000 and had a much higher percentage when less than $5,000. Above this amount the percentage of successful campaigns drops sharply against the percentage of failed campaigns. While the trend reverses itself for the amounts between $35,000 and $45,000 it immediately reverts to failures outnumbering success. This volatility could be attributed to there being less campaigns with larger goals giving us less accurate data. In summation it is generally advisable to limit the campaign goal to an amount less than $20,000.	

- What are some limitations of this dataset?
A possible limitation of the data set that I believe would help to better understand trends in the ‘plays’ subcategory would be adding an additional subcategory under ‘plays’ for things like ‘comedies’ ‘musicals’ ‘dramas’ ect. Using this additional subcategory and filter for ‘backers count’ and ‘average backers donation’ we could get a much better understanding of the demographics of the backers and identify how “popular” some projects are. With that we might be able to more reliably determine why some campaigns are successful at different goals.

- What are some other possible tables and/or graphs that we could create?
Some other tables and graphs that I think would be useful would be one that shows the relation between the success and failure rate by the amount of backers and the average donation. I think it would be interesting to see the relation between the US and other countries when it comes to successful and failed campaigns.
