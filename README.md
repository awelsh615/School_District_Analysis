# School District Analysis

## Overview of District Analysis
### Purpose of Analysis
The purpose of this analysis was to analyze and review student funding and standardized testing data for a specific school district containing 15 schools.  The data needed to be first cleaned, and then organized to showcase trends in school  performance.  The final analysis is intended for the school board, and other school administration to help inform decisions about school budget allotments.  Specifically for this analysis, the following information was aggregated from the data:
- District Summary
- School Summary
- Top and Bottom 5 Schools based on overall passing rate
- Average Math and Reading scores by grade level for each school
- Scores by School Spending, School Size, and School Type

### Resources
- Data Sources: schools_complete.csv, students_complete_csv
- Software: Python 3.8.8, Jupyter notebook 6.4.0, Jupyter lab 3.0.16
- Python libraries: numpy, pandas

## School District Summary
### Summary
The following is the Summary by School for the complete set of data.

### Data Cleaning
The original students_complete.csv file included several Prefixes and Suffixes that made it difficult to work with the given data.  I employed many different methods to quantify the following list of prefixes and suffixes, and the code below to remove those from the Series of Student Names.

```
prefixes_suffixes = ["Dr. ", "Mr. ","Ms. ", "Mrs. ", "Miss ", " MD", " DDS", " DVM", " PhD"]

for word in prefixes_suffixes:
    student_data_df["student_name"] = student_data_df["student_name"].str.replace(word,"")
```

### Thomas High School



### Challenges of this Project
