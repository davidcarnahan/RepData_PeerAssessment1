===========================================
  REPRODUCIBLE RESEARCH
  Johns Hopkins Data Science Course
===========================================  

The purpose of this assignment is to use the knitr package to create an R markdown file
for a routine analysis to demonstrate how to produce reproducible research.


Data:
The data can be found here: https://d396qusza40orc.cloudfront.net/repdata%2Fdata%2Factivity.zip

This dataset represents the self quantified movement spawned from devices like nike+, 
fitbit, and jawbone.

It contains the number of steps in five minute intervals on a specified date, and has 
a little more than 17k observations. 

=======================
  Data Prep
=======================

Like real world data science, there is quite a bit of data prep required to answer the 
questions below. I did some up front data prep, but was required to do more as I went 
along. 

My initial steps for data prep prior to answering the questions were as follows:
1. Load the data and evaluate for load success.
2. Transform the data from a numeric to a date.
3. Create a subset that eliminates observations with missing data.  

=======================
  Questions
=======================

1. What is mean/median total number of steps taken per day?

The steps I took to answer this question were as follows:
a. Reshaped the data by using the melt function.
b. Create a summary dataset that gives the total steps per day.
c. Graph a histogram that shows total steps per day.
d. Graph a rug underneath the histogram as a little garnish.
e. Determine mean/median.

2. What is the average daily activity pattern?

The steps I took to answer this question were as follows:
a. Modify above dataset by adding back interval to the dataset.
b. Create a summary dataset that gives the average no. steps by interval.
c. Plot a line graph that shows average steps by interval.
d. Determine the interval with the max no. of steps.

3. What is the impact of imputing data for the missing observations?

The steps I took to answer this question were as follows:
a. Determine the no. of observations with missing data.
b. Use the mean no. steps for each interval to impute steps data for missing observations.
c. Create summary dataset for coming graph.
d. Regraph histogram to determine the potential impact of missing data.
e. Determine mean/median and compare to previous results in question 1.

4. Are there differences in activity patterns between weekdays and weekends?

The steps I took to answer this question were as follows:
a. Add a new factor variable (weekend) in order to allow for split graphs using facet.
b. Create a summary dataset around interval and weekend levels.
c. Plot a second line graph that splits out average steps by interval according to
weekend level (weekdays versus weekend).

=======================
  Submission
=======================

There are three requirements:
1. README file
2. R Markdown File (rmd)
2. HTML file from R Markdown File (html)

** Note -- when I submitted the files to github, it tells me the 1.2 MB HTML file is too
large. However, there is a little screen icon that will allow you to open in your desktop
github, which would allow you to see it as it is in its final form.