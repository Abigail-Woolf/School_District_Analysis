# School District Analysis
Introduction to Jupyter Notebooks (product of Anaconda, free open-source distribution software) and Pandas (library for data manipulation and analysis) 
data wrangling/ data munging
Using Jupyter Notebook and the Pandas library, you’ll read raw data from CSV files, inspect and clean data, merge datasets, perform mathematical calculations, and visualize the data with charts and graphs to tell a story.
Python3 and Anaconda
create virtual environment for python projects called PythonData python 3.7
conda create -n PythonData python=3.7 anaconda
to check all conda environments: conda info --envs
A Pandas Series is a one-dimensional, labeled array capable of holding any data type. This means the data is linear and has an index that acts as a key in a dictionary.

Here is the list of deliverables for the analysis of the school district: 

A high-level snapshot of the district's key metrics, presented in a table format
An overview of the key metrics for each school, presented in a table format
Tables presenting each of the following metrics:
Top 5 and bottom 5 performing schools, based on the overall passing rate
The average math score received by students in each grade level at each school
The average reading score received by students in each grade level at each school
School performance based on the budget per student
School performance based on the school size 
School performance based on the type of school

prepare standarize test data and funding
aggregat data and showcase trends in students performances

## Challenge
The grades of nineth graders at Thomas High School were incorrect and needed to be removed from the data analysis. Once that was complete, there were some changes to the results.

### How is the district summary affected?
![screenshot](https://github.com/Abigail-Woolf/School_District_Analysis/blob/master/Pre_edit_Summ_Stats.png)

![screenshot](https://github.com/Abigail-Woolf/School_District_Analysis/blob/master/Post_edit_Summ_Stats.png)
  The district summary is affected by the absence of THS data. All of the averages and scores decreased except for the Average Reading Score, which remained the same. The biggest change, however, occurred in the % Passing Reading with a 1.3 percent change.
#### How is the school summary affected?
  The school summary dataframe is affected because all of the data from Thomas High School was removed. All of the data from the other schools remained unchanged.

Recalculate the high- and low-performing schools.
  After recalculating which schools ranked in the top five, Thomas High School was removed and Wright High School was added as the fifth school. originally, THS was ranked second, so all the schools starting at rank two moved up. 
How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance, relative to the other schools? 
### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance, relative to the other schools?
### How does replacing the ninth-grade scores affect the following?
Math and Reading Scores by Grade
Scores by School Spending
Scores by School Size
Scores by School Type
  Removing the math and reading scores from the nineth graders changed the THS ranking of bottom schools from 14 to 8. The removed scores of the nineth graders, brought the entire school's averages down, thus moving its rank towards the bottom of the list. 
  
Recalculate the scores by grade, scores by school spending, scores by school size, and scores by school type.
How does replacing the ninth-grade scores affect the following?
Math and Reading Scores by Grade

  The math and reading scores by grade were not affected after dropping the THS nineth graders scores.
  
Scores by School Spending- no change

Scores by School Size- no change

Scores by School Type- no change
