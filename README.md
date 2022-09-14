# Kickstarting with Excel

## Overview of Project:
We did an analysis of how a number of various campaigns-specifically those which belong to 'Theater' category performed based on two criteria- firstly, based on their launch dates and secondly, based on their funding amount goals, with the help of data from the 'Kickstarter' dataset. Our client, Louise asked us to do the above analysis for her, after the success of her play 'Fever'- which came really close to its fundraising goal, in a relatively short amount of time. 

## Analysis and Challenges: 
### Analysis of Outcomes Based on Launch Date:
For the first portion of analysis, that is the analysis of 'Outcomes based on Launch Date Chart', we first extracted the year portion of the date created column which gave us the respective years in which each of the campaigns was started (we would later use those years as a filter in our pivot table). Then we created a pivot table in a new sheet, consisting of two filters- 'Parent Category' and 'Years'. Date created conversion was placed on rows-grouped by the months of the year (by default it displays for all the years). Whereas the outcomes were placed on the columns-namely successful, failed or canceled. And the count of outcomes was placed in the Values portion of the pivot table. Next, we want to create a line chart to visually represent our pivot table, which is as follows: 
Theater_Outcomes_vs_Launch.png

### Analysis of Outcomes Based on Goals:
For the second portion of analysis, that is the analysis of 'Outcomes based on Goals', we first create a new worksheet with 8 columns and 12 rows. The first column is the goal column which is already provided to us, and then by using COUNTIFS() function, we tend to fill the number of successful, failed and canceled events, based on 'outcome', 'goal' and 'Subcategory' columns from the Kickstarter worksheet. Next, we calculate and fill the number of total projects column and finally the percentages of these successful, failed and canceled events based on the total projects. Our next step was to create a line chart that depicts these individual percentages based on goal. The line chart is as follows:
Outcomes_vs_Goals.png

### Challenges and Difficulties Encountered:
Overall, I did not face much challenges completing this analysis because of all the step-by-step description of the assignment. But there were a few little things that made me stuck. For instance, it took me a minute to figure out how to extract years from the dates given for first analysis. I couldn't figure out how to give the line chart a title, initially. For the second analysis, it took me some time to figure out the arguement portion of the COUNTIFS() function. Once figured, it is really not that difficult, but amazing that it can take any number of arguments/conditions. 

## Results:
- What are two conclusions you can draw about the Outcomes based on Launch Date?
1. The most successful theater campaigns were launched in the month of May, 111 campaigns to be precise.
2. The most number of failed campaigns were launched in the month of May, 52 to be precise and was closely followed by June, July and October with 49, 50 and 50 campaigns respectively. 
- What can you conclude about the Outcomes based on Goals?__
The most successful campaigns had a goal set of less than $1000, closely followed by the goal set in the range $1000 to $4999. Whereas, the most failed campaigns (100% to be precise) had a goal set in the range $45000 to $49999. 
- What are some limitations of this dataset?__
The first limitation in the dataset is that the dates that were originally given to us were in the UNIX timestamps. These had to be converted into the MM/DD/YY format. Secondly, some of the column headers are misleading for instance, 'staff_pick' and 'spotlight'.  
- What are some other possible tables and/or graphs that we could create?__ 
Some additional charts that could be created are:
a. The outcomes based on Countries- in order to see which countries had the most successful or failed campaigns.
b. The time period of campaigns and their respective outcomes- how long did the most successful campaigns run for? 



