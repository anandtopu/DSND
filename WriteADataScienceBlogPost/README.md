<<<<<<< HEAD
# Analysis of the Stack Overflow Annual Developer Survey

## Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#file)
4. [Technical Details](#technical)
5. [Conclusions](#conclusions)
6. [Git Repo Link]
7. [Licensing and Acknowledgements](#licensing)
## Installation <a name="installation"></a>
The Jupyter notebook in this project is based on Python 3.7.1. You will need packages such as numpy, pandas, matplotlib, pycountry_convert, jupytab,seaborn to run this notebook. The package pycountry_convert is used to convert country names to continent names.<br>
After downloading the repository to your local machine, you will need to unzip the data.zip file before running the Stack_Overflow_survey_project.ipynb file. (I have to zip the dataset because it is too big.)
<br>
The file structure should be as follows:
> repository/  
&emsp;&emsp;Stack_Overflow_survey_project.ipynb  
&emsp;&emsp;data/  
&emsp;&emsp;stackoverflow_ide.twb  
&emsp;&emsp;stackoverflow_programming languages.twb  
&emsp;&emsp;IDE.xlsx  
&emsp;&emsp;language.xlsx  
&emsp;&emsp;Stack_Overflow_Survey_Analysis.html
&emsp;&emsp;README.md

## Project Motivation <a name="motivation"></a>
Based on stack overflow survey data few questions this project seeks to understand are:
 [Stack Overflow Annual Developer Survey](https://insights.stackoverflow.com/survey) dataset.
1. What is the most popular programming language in the past five years since 2015?
2. What is the most popular IDE for professional software developers in the past five years since 2015?  
3. How much does professional software developers make in the past five years since 2015? What is the salary increase rate?
4. Education degree and job satisfaction and salary/compension based on education level for 2019?

## File Descriptions <a name="file"></a>
1. Stack_Overflow_Survey_Analysis.ipynb: is the main file for data processing, analysis and visualization.
2. data.zip: contains Stack Overflow Annual Developer Survey dataset between Year 2015 and Year 2019. These datasets are used for this project. 
3. IDE.xlsx and stackoverflow_ide.twb: Tableau source files to generate the 'most popular IDE' figure.
4. language.xlsx and stackoverflow_programming languages.twb: Tableau source files to generate the 'most popular languages' figure.

## Technical details <a name="technical"></a>
###### Language and IDE data
To find out the most popular programming language, I used the survey data of the recent five years.</br>
To find out the most popular IDE, I only used the survey data of the recent four years. This is because the survey data in Year 2015 doesn't include information about IDE.</br>
To find out the relationship between higher education and salary I had used 2019 data only as the 
###### Salary 
The average salary calculation only includes full-time developers.</br>
The salary difference between countries is so big. It doesn't make sense to calculate the average salary of professional software developers for the whole world. Since we have data from more than 170 countries and dependent territories, it also does not make sense to calculate the average salary for every country. So I added a column named 'continent' and calculated the average salary based on different continents.</br>
###### Missing values
Because we have a very large dataset and only a small fraction of data has no salary information, so I removed the rows where salary information is missing.</br>
###### Incorrect values
When I examining the dataset in the data assessment step, I observed many full-time developers have a salary of 0, while others have a salary of 10^30 dollars! These are obviously incorrect. So I decided to only include salaries within 0.1 - 0.9 quantile range for the average salary calculation. I believe this is reasonable.</br>
###### Visualization
The two visuals related to salary is generated with matplotlib. The other visuals are generated using Tableau.

## Conclusions <a name="conclusions"></a>
1.The most popular programming languages are JavaScript, HTML/CSS and SQL.
2.The most popular IDEs are Visual Studio, Notepad++ and sublime.
3.North American developers have the highest average salary and relatively high salary increase rate. Asian Developers have highest increase in salary.
4.Professionals with advanced degrees are clearly earning more than those with only High School degree with the same years of Coding Experience However, as the years of experience increase, the difference becomes smaller. 

Blog [here](https://medium.com/@anand.goud.2020/stack-overflow-survey-analysis-db1c40602919).

###### Git repo link
https://github.com/anandtopu/udacity_data_scientist_nanodegree/

## Licensing and Acknowledgements <a name="Licensing"></a>
Thanks Stack Overflow for making the survey data
available to the general public.The code in this repository is released under the MIT license. 
=======
# udacity_data_scientist_nanodegree
This is git repo for udacity nanodegree submissions
>>>>>>> c2b5b5e80a9a8be13a93e6eb62fa3f9710477b93
