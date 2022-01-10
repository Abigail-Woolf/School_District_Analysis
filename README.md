# School District Analysis
The task of this assignment is to prepare standardized test data from high schools and aggregate the data to inform duscussions at the school and district levels regarding budget allotment. I took a close look at individual students' math and reading scores between schools within the district and found answers to the key questions stated below. This is an introduction to Jupyter Notebooks (product of Anaconda, free open-source distribution software) and Pandas (library for data manipulation and analysis).

# Data Wrangling/ Data Munging
Using Jupyter Notebook and the Pandas library, I read raw data from CSV files, inspect and clean data, merge datasets, perform mathematical calculations, and visualize the data with charts and graphs to tell a story.
For practice, I created virtual environment for my python projects called PythonData using python 3.7. In Terminal, I wrote: conda create -n PythonData python=3.7 anaconda

## Challenge
While looking through the data, it was clear that the grades of nineth graders at Thomas High School were incorrect and needed to be removed from the data analysis. For this challenge, I was tasked with replacing the math and reading scores for Thomas High school without removing those nineth graders from the entire analysis. I did this by:
* duplicating the original, cleaned, Jupyter Notebook
* Replaced the reading and math scores for nineth grdaers at Thomas High with Nan using. I selected columns by condition with loc on the student_data_df. Using Numpy, I set certain columns equal to "NaN with np.nan for the reading and math scores.
* Next, I merged the clean student data with the school dataset
* Laslty, I recreated the district and school summary DataFrames and answered the questions below:

### How is the district summary affected?
![screenshot](https://github.com/Abigail-Woolf/School_District_Analysis/blob/master/Pre_edit_Summ_Stats.png)

![screenshot](https://github.com/Abigail-Woolf/School_District_Analysis/blob/master/Post_edit_Summ_Stats.png)
  The district summary is affected by the absence of THS data. All of the averages and scores decreased except for the Average Reading Score, which remained the same. The biggest change, however, occurred in the % Passing Reading with a 1.3 percent change.
#### How is the school summary affected?
  The school summary dataframe is affected because all of the data from Thomas High School was removed. All of the data from the other schools remained unchanged.

##### Recalculate the high- and low-performing schools.
  After recalculating which schools ranked in the top five, Thomas High School was removed and Wright High School was added as the fifth school. originally, THS was ranked second, so all the schools starting at rank two moved up. 
How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance, relative to the other schools? 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance, relative to the other schools?
Removing the math and reading scores from the nineth graders changed the THS ranking of bottom schools from 14 to 8. The removed scores of the nineth graders, brought the entire school's averages down, thus moving its rank towards the bottom of the list. 

### How does replacing the ninth-grade scores affect the following?
Math and Reading Scores by Grade - The math and reading scores by grade were not affected after dropping the THS nineth graders scores.
Scores by School Spending - no change
Scores by School Size - no change 
Scores by School Type - no change
