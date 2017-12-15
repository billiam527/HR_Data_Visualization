# Readme HR_Data_Visualization

## About the autor

William Fisher
Graduate Student 
Mercyhurst University
DATA 620 Data Visualization
Project 2 - Visualization of Video Game Sales and Ratings

## This repository contains:

1. The Jupyter notebook containing code
2. HR_Comma_sep CSV
3. The redame file

## Table of Contents

- [Background](#background)
- [Install](#install)
- [Usage](#usage)
- [Related Efforts](#related-efforts)
- [Project Explaination](#Project-explaination)
- [Conclusion](#Conclusion)

## Background

The dataset consists of a csv file.  The columns consist of the employees satisfaction level, their last evaluation score, the number of projects they have worked on, their average monthly hours, their time (in years) spent at the company, if they have had a work accident, if they left the company, if they have gotten a promotion in the last five years, what department they are a part of, and if their salary is high, medium, or low.
The data comes from: https://www.kaggle.com/ludobenistant/hr-analytics-1/data

The third project follows the following guidelines:
1) Select a dataset of your own choice (simple, complicated, whatever your level of comfort is)
2) Chop the dataset using pandas to fit whatever visualization you have in mind.
3) Clean the dataset and drop missing values - if needed
4) Create two different types of visualization - minimum. Your choice, just make sure they are different kinds - (for example a bar chart and a pie, but not two pies).
5) You can have more visualizations if you want
6) Make sure your readme file is perfect!
7) Submit on github and kaggle (if using kaggle datasets), just github if you are using data from other sources like drivedata.org or other census data.

## Install

This project uses Python & the following python packages:

csv
pandas
seaborn
matplotlib
numpy

## Usage

This is a class project.

## Related Efforts

There are several other students in the Fall DATA 620: Data Visualization class working on similar projects.  Students were supposed to choose different data sets so while content may be similar, the topics should be broadly ranged.

## Project Explaination
Explaination of Jupyter notebook code:

Cell 1: We need to import the neccesary libraries.  For our project we need to import csv, pandas, seaborn, matplotlib, and numpy.  We can also abbreviate these to make it easier to call them later in our code. "A lazy coder is a successful coder."

Cell 2: We then, import our CSV file.  In this case, we use pd and the import csv method to import the data. We then assign the data to the variable data.

Cell 2 and 3:  We can view just the top and bottom of the data using .head() and .tail() respectively.  We do this to get an idea of what all our data contains. In this case we are just looking at the beginning and end but we will do more to see what other values our in our data.

Cell 4: We get some more info about our data by getting a count of the number of salaries.  This will be the data for our first visualization.

Cell 5: We plot the slaries (high, medium, and low) on a pie chart to get a good idea of how many employees make what.  The pie chart makes it clear most employees make a low salary.

Cell 6: This is simply a list of the coumns to help look at the other data in the dataset. 

Cell 7: Next, I set the salary as the index and got a mean of all the data per type of salary.

Cell 8: I took the salary data from cell 7 and looked at it compared to the number of average monthly hours, the number of years an employee has been at the company, and the satisfaction level.
While the satisfaction level and the number of years were expected to correspond to higher salaries I was surprised to see the highest paid workers logged the least amount of monthly hours.

Cell 9: In cell 9 I looked at the correlation between satisfaction level and time spent at the company with a KDE plot.

Cell 10:  In cell 10 I looked at the same data except with a histogram.

Cell 11:  Finally, I looked at the correlation between satisfaction level and the score of an employee's last review.
All of these turned out as expected.  Employees who are at companies for a while stay because they are somewhat satisfied with their jobs.  Additionally, they perform better when they have a higher satisfaction level.

Cell 12-14: I wanted to chop up the data by department to look at some visualizations based on that.

Cell 15: It appears that there are the most accidents in the RandD department.  I do not have a great explanation for why I looked at this particular data, it was just something that caught my eye.

Cell 16: Finally, the data shows us that management has spent the longest time at the company.  This makes sense.  Other positions with longevity include sales and marketing.

## Conclusion

Conclusion: Using various visualizations we are able to gain key insights into companies and their employees.  Some of the data wwas fairly straight forward while some was surprising.  For starters, most employees make a low salary.  While I, personally, did not think most employees would make a high salary I also did not think most would make a low salary.  Instead, I would think that most employees would fall in the medium range, but this is not the case.  Sticking with the topic of salaries, it makes sense that those with the highest salaries spent the most time at the company and have a higher satisfaction level.  I did not expect those with the highest slaries to work the least monthly average hours.  

With the KDE and histogram plots we can see that employees who are at the company the longest have the highest satisfaction rate.  this makes sense as if you were dissatisfied you would probably leave.  We also see with the scatter plot, that those who had a higher evaluation score were also more likely to be satisfied with their work.

Finally, using the horizontal bar plots, it is obvious that the R and D department is the most dangerous in the company (although not by any significant margins) and that if you are in management you are likely to have been at the company for at least 4 years.

Overall, with the manipulation and visualization of this data, employers can gain valuable knowledge about their workplace and their employees to help retain talent and improve their companies.
