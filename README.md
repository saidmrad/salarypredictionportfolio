# salarypredictionportfolio
Salary Prediction Project (Python)
This repository contains the python code for a salary prediction project. Details of the project can be read in the notebook.

### Introduction

Salary structures are a necessary part of effective management. They help make sure that the pay levels are externally competitive and internally fair. Salary structures also allow companies to reward performance and development while controlling cost.

### Data supplied

- train_features.csv: This file contains one million observations, each row is an individual record of job posting. Each column describes features of the job posting. We have the companyId, the job Type, the degree, the industry, the miles from the metropolis and the years of Experience. We have 1 million entries.
- train_salaries.csv: Each row associates a “jobId” with a “salary”, the same job_id as train_features is used and we can thus assign a salary to each job dexription above
- test_features.csv: This file contains one million observations, similar to train_features.csv with the same features, but used for our ultimate prediction. 

### Define the Problem

Project Goal: The goal of this project is to analyze a dataset of job listings with posted salaries and predict the salaries of job listings that neglected to post a salary.

Use Case: This type of model could be utilized by either recruiting firms or individual companies attempting to remain competitive in the job market.

Tools: The problem has been approached using Python 3 with machine learning algorithms/estimators from sklearn

### Data Exploration
- Import useful libraries and load the dataset.
- Take a rough look at the three data. Each of them has one million records and mixed data types(numerical+categorical).
- Data Cleaning:
  - There are no missing or duplicated values in the data.
  - Check and inspect potential outliers based on IQR rule and removed the five records of data with salary zero.
