# Kickstarting with Excel

## Overview of Project


### Purpose
I sought to draw conclusions regarding the success/failure of fundraising campaigns using the Kickstarted dataset. First I sorted the data to include just observations in the parent category of "theater" and looked for trends in success level vs. launch date. To finish things off, I sorted the data even further to include just observations in the subcategory of "plays". With this narrowed down set, I observed the success level of campaigns based on the size of the campaign goal.
## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To perform my analysis of theater campaign outcomes based on launch date, I created a pivot table with the rows organized by launch date month and columns organized by outcome(successful/failed/canceled). Then, using the pivot chart function, I generated a line graph displaying the results of the pivot table. With this chart and table, I am able to draw several strong conclusions regarding the success of theater fundraising campaigns based on their launch date.
### Analysis of Outcomes Based on Goals
To analyze outcomes of fundraising campaigns for plays based on goal size, I manually created a chart showing both the number and percentage of successful/failed/canceled plays in 12 different goal ranges. To do this I utilized the COUNTIFS() function on the dataset filtered to show just observations for plays. Then, highlighting the necessary columns, I created a line chart showing the percentage of successful and failed campaigns for each of the 12 goal size ranges. 
### Challenges and Difficulties Encountered
Overall, I didn't encounter any major challenges when executing these two analyses. The one difficulty I ran into came when trying to get my Theater Outcome by Launch Date pivot table to display the correct filtered data. When I first filtered the data on the Kickstarter sheet and tried to create the pivot table, the table still included observations I wanted to filter out (specifically observations that resembled live campaigns). To combat this challenge, I copy and pasted the filtered data into another sheet and then used this new sheet to export the pivot table. This strategy worked successfully to help me create the desired table and chart.
## Results


One obvious but important conclusion that can be made from looking at the Theater Outcomes by Launch Date table and line graph is that theater campaigns historically succeed more than they fail across all 12 possible launch months. This fact is easily seen by the way in which the successful (blue) line never drops below the failed (orange) line on the line chart. 

Another important conclusion that can be drawn from the Theater Outcomes Based on Launch Date analysis is that in 10 out of the 12 possible launch months, the change in number of successes and number of failures move in the same direction. Specifically, in both July and December the number of failures increased from the month before while the number of successes decreased (There are no months in which successes increased and failures decreased). This trend suggests that July and December are poor times to launch theater campaigns, as launching just one month prior would lend a higher likelihood of success and lower probability of failure. 


One conclusion to make about the Outcomes Based on Goals is that for play campaigns with goals between $0-$29999 there is a negative relationship between goal size and campaign success rate. This is evident by looking at the line chart and seeing how the percentage of successful campaigns drops and percentage of failed campaigns increases as goal size rises within this range. 

For plays with goals greater than $30000, however, there does not appear to be a strong relationship between success rate and goal size as there are several jumps and dives in success/failure rate as goal size increases in this range. This is likely due to the fact there are far fewer observations within this second range, which naturally leads to a greater level of randomness.
## Limitations


One clear limitation of the dataset is that the observations don't go into very much detail regarding the structure of each campaign. For example, the number of employees working for each campaign would also figure to have a strong impact on its success. Knowing these specifics would allow users of the dataset to compare their campaign to past campaigns with similar employee structure.

In a similar vein, I believe that greater detail regarding the location of the campaigns would also improve the dataset. As it currently stands, the spreadsheet only discloses what country the campaign was created in, so anybody using the data is not able to filter the data down to a specific state/county/city or other smaller geographic region. Being able to filter the data further by location could uncover more conclusive patterns and trends. 


## Possible Additions


Another pivot table that I think would be interesting to create would be to have all countries as the rows, outcomes as the columns, and a sum of the outcomes as the values. I would also include a filter to allow for filtering by parent category and/or subcategory in order to view specific types of campaigns under this lens. I would then create a bar chart to display the results of the table, placing countries on the X-axis and the bars showing number of successes/failures/cancellations for each country. This analysis would allow me to see which countries certain types of campaigns have more/less success in and vice versa. 
