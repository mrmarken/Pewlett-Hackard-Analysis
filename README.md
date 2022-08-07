# **Pewlett Hackard Analysis**

## Overview of Project

### Summary ### 
The objective of this project is to utilize PGAdmin to dissect data from SQL databases to assess retirement eligibility for a large part of the Pewlett Hackard workforce.
The goals are to provide:
* The number of retiring employees by title
* A list of employees eligible for the mentorship program
* A written report on the employee database analysis


### Data Sources
The data sources to complete this project are outlined below:
* SQL Database from 6 csv files
* retirement_titles.csv
* unique_titles.csv
* retiring_titles.csv
* mentorship_eligibilty.csv

### Software Used
pgAdmin: "PostgreSQL 14.4 on x86_64-apple-darwin20.6.0, compiled by Apple clang version 12.0.0 (clang-1200.0.32.29), 64-bit"
Visual Studio: v. 1.69.2 (Universal), Commit: 3b889b090b5ad5793f524b5d1d39fda662b96a2a

## Results 
The following observations were made by examining the newly formed tables:
* The largest group of workers eligible for retirement (29,414) are Senior Engineers
* The next largest group (28,254) are employees in a “Senior Leadership” role.
* As per [mentorship_eligibilty.csv](https://github.com/mrmarken/Pewlett-Hackard-Analysis/blob/main/Data/mentorship_eligibilty.csv), there are a total of 56,859 possible mentors in the retiring group. 
* There are only two managers in the group that are retiring
![Figure 1. Total employees eligible for mentorship](https://github.com/mrmarken/Pewlett-Hackard-Analysis/blob/main/Total%20employees%20eligible%20for%20mentorship.png) 



 
## Summary
As the baby boomer population reaches the retirement age, Pewlett Hackard (PH) faces a tremendous task with replacing that aging workforce in an event that can be described as an upcoming "silver tsunami."  This report contains various data tables for the executives to make appropriate plans to replace the retiring workforce. Further analysis can be provided as the company begins to format a strategy.

### How many roles will need to be filled as the "silver tsunami" begins to make an impact?
From our query and [unique_titles.csv table](https://github.com/mrmarken/Pewlett-Hackard-Analysis/blob/main/Data/unique_titles.csv), there are 90,398 currently hired people that will be able to retire in the next 1-3 years, assuming people will retire at 65 years old. 
PH will need to strategize a plan to replace this large set of the workforce with an emphasis on mentoring younger employees.  A query to breakdown the departments affected and the number of employees in the retirement age should aid PH in preparing for this mass exodus. 
### Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
At the rate the eligible mentors will be retiring over the next few years, it is essential that PH begins a mentorship program as soon as possible.  The data can be further broken up and analyzed to provide an overview of the eligible mentoring population by department so that the company can prioritize a plan for the mentorship program.  A simple query (lines 62-66 of [Employee_Database_challenge.sql](https://github.com/mrmarken/Pewlett-Hackard-Analysis/blob/main/Employee_Database_challenge.sql): 

![Figure 2. additional_query.png](https://github.com/mrmarken/Pewlett-Hackard-Analysis/blob/main/additional_query.png) 
