# Kickstarting with Excel

## Overview of Project
This project is comparing campaigns in relation to their launched dates and their funding goals. I will need to analyze the project launched dates against their outcomes as well the outcomes based on their goals. I would need to create formulas (such as countifs and sum to name a few) in order to simplify the data in a way that it remains useful and relevant to the task. The campaign outcomes will be visualized by way of pivot tables and charts. The project will seek to answer the following questions:
1. What data is necessary?
2. What story is being told by the data?
3. What questions can be answered?
4. What trends and patterns can be identified within the data?

### Purpose
The purpose of this analysis is to determine how different campaigns fared in relation to their launch dates and their funding goals.

## Analysis and Challenges
Analysis of this project was performed using the Excel tool to mine, analyze and visualize the data. Two analysis was conducted during this research excercise. They are:
1. Outcomes based on Launch Date
2. Outcomes Based on Goals

### Analysis of Outcomes Based on Launch Date
In order to analyze this segement, the relevant data field were identified from the dataset, i.e outcome (successful, failed and canceled) and time (years and months). I started first by isolating the year from the "date of creation", once that was done I was able to create a pivot table to show the outcomes over time, as it relates to the parent category "theater".The pivot table was further used to create a pivot chart to visualize the relationship between the outcomes and launch month.

### Analysis of Outcomes Based on Goals
To analyze the outcomes based on goals, target ramges were identified (0 to 4999). The outcomes (successful, failed and canceled) where then mapped against their goals as well as the subcatergory plays. This was done using the following countifs formula (=COUNTIFS(Kickstarter!$F:F,"successful",Kickstarter!$D:D,">=35000",Kickstarter!$D:D,"<=39999",Kickstarter!$R:R,"=plays"). This formula counts the outcome subcategory within each goal range. Next, would be to calcaulate total of all the projects across each subcategorgy (=SUM(B2:D2). Similarly the percentage of each subcategory was calculated (=B2/$B$14). For visulization, a pivot chart was used.



### Challenges and Difficulties Encountered
The difficulties I faced during this excercise was that I was unaware of how to group items within a pivot table; but only after watching the video shown in the tip section of the excercise was I able to do so successfuly. Another challenge faced was computing the goal amount using the formula countifs. I had to make certain cells an abosulte cell reference (example: $C:$C), else the cells refernece would continue to change when copying and pasting.I also had to check to make sure that the formula works so I filtered manually to the criteria on the kickstart worksheet. Once I was satified that it works, I would copy and paste formula into all relative cell.

## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?
1. The most successful Kickstarter campaigns were started in May, peaked in July. On the other hand, December doesn't seem like a great time to launch a campaign.This is not representative of the information we want to gather.

### What can you conclude about the Outcomes based on Goals?
1. I have found that while there is only a total of 1, 047 Kickstarter campaigns in the sub category "plays", the most successul goal-amount is within the range of "1000 to 4999".

### What are some limitations of this dataset?
Some limitations of this dataset are:
1. Dataset includes some data points that are not representative of the data we want, For example information regarding funding goals for theather building proposals

### What are some other possible tables and/or graphs that we could create?
Some possible graphs that could be created are:
1. Box Plots 
2. Descriptive Statistics
3. Stacked Columns
