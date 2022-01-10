# Kickstarting with Excel

## Overview of Project
  Louise is a upcoming playwright who wants to start a crowdfunding campaign to fund her new play called Fever. Initially, I did an analysis of the crowdfunding data that she had to see if there were any trends in the successful, failed, canceled, and live campaigns. The analysis was to help her get an idea of what she needed to launch her own campaign and if their was a possibility that her current goal could be met.

### Purpose
  After launching her campaign for Fever, she was able to almsot reach her goal in a short amount of time. Now she wants to see the progress that other campaigns had in regards to their launch dates and funding goals. 

## Analysis and Challenges
  I began my analysis by creating a new column, years, in the original Kickstarter data set. I pulled the year from the date each of the campaigns were created. Then, I made a pivot chart where I filtered the data by the parent category theater and by the year. After adding 'year' to the row column, I was able to further break it down to show the months of the year. The columns of the chart displayed the number of successful, failed, canceled, and the total. Afterwards, I created a line chart so it would make it easier for Louise to view and see the trend. See the graph below:
  
  ![Theater_Outcomes_vs_Launch.png](Documents/Data Analysis/Module 1- Excel/Resources)
  
  
  In the second part of my analysis, I created another line chart as well. This graph contained the percentage of successful, failed, and canceled plays based on their funding goal amount. I began by creating a new table where I used the COUNTIFS function to help  obtain the outcome and goal data for the subcategory plays. I created 12 different goal ranges that included less than 1000 to greater than 50000. In the table I also created 4 columns to count the number of successful, failed, canceled, and total projects. Then, I used the COUNTIF function to get the count for each of the ranges and each of the columns. The other half of my columns in the table were the percentage of each successful, failed, and canceled campaign. I used the ROUND formula to find that percentage. I divided the amount calculated by the COUNTIFS function by the total number of projects from that row. Finally, with that information I created the line graph below:
  
  ![Outcomes_vs_Goals.png](Documents/Data Analysis/Module 1- Excel/Resources)
  
 The line graph showed the relationship between goal-amount ranges and the percentage of successful, failed, or canceled projects.
  

### Analysis of Outcomes Based on Launch Date

After looking at the pivot chart I created that showed the outcomes for theater based on their launch data, I noticed the most successful time is during the summer time. During May, June and July, the amount of successfull plays peaked. Afterwards, the number began to steadily decline. However, it is important to note that during this same time is also when the number of failed projects is the highest. And just like the successful ones, afterwards the number declines. Even though this particular time is the peak for both the number of successful plays is about twice the amount of those that failed.

### Analysis of Outcomes Based on Goals

Based on the table I created with the different goal-amount ranges, there is certain amounts where the campaigns tend to be more scuccessful. For the following ranges: less than 1000, 1000 to 4999, 35000 to 39999, and 40000 to 44999 the percentage of successful campaigns are double the percentage of failed campaigns. For all the other ranges the majority of the time it is abouta 50% chance of success or failure.

### Challenges and Difficulties Encountered

In the beginning, I found the COUNTIFS formula part a little challenging because the formula was lengthy in my opinion. When I wrote the first set of formulas for the successfull column, I missed common things like quotation marks, dollar signs, commas, or parentheses. It was frustrating because it does get hard to see that a simple comma is missed in a formula that long. I had to slow down, and I broke down each part of the formula and wrote it out. For example, the beginning of my formula is =COUNTIFS(Kickstarter!$F:$F,"successful", and after I wrote it, I looked over it very carefully for any errors. Then I continued to the next part, I found this very helpful and I was able to master the rest of the formulas I needed. 

## Results

- Based on my analysis from the Outcomes based on Launch Date I can conclude that the best time to start a crowdfunding campaign is during the summer especially during the months of May and June. Another conclusion woulf be that it is also better to launch during the beginning of the year versus towards the end of the year. I would especially avoid the last 3 months of October, November, and December. The total amount of successful campaigns are almost double the amount of failed campains throughout the year.

-  After analyzing the Outcomes based on Goals, I see that overall the total percentage of failed campaigns is higher than the total percentage of successful campaigns. Therefore, I would recommend that the goal is carefully chosen. The campaigns that were successful had a low goal of less than 1000 to 4999 or a higher goal of 35000 to 44999. 

- A limitation that this dataset has is that we did not pick specific time range. The table I used in Outcomes based on Launch date showed all months but the years ranged from earlier than 2009 and older than 2017. I think we could of had a clearer conclusion if we did a time span of just 5 or maybe even 10 years instead of a gap that large.

- Some other possible tables we could have created would be to filter by specific years and then look at all the months within those given years. Also, for the Outcomes Based on Goals line graph, I think a bar chart could of been better than a line graph. The different sizes in bars could of made it more visually appealing and easier to see the diffferences. To give Louise more variety, we could of done a separate pivot table with focus on another country of her interest to see how that country compared to the US.
