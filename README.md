# ADS_508_Final_Project

## TalentIQ Employee Attrition Prediction
### Contributors: Stephanie Smith, Ramin Fazli
# Overview

TalentIQ Technologies is experiencing elevated employee attrition (~16%), resulting in significant costs. This project develops a machine learning pipeline to predict attrition risk, identify key drivers, and support proactive retention strategies.

The solution combines internal HR data with external labor market signals and is built using AWS cloud services.

# Business Objective
Predict which employees are at risk of leaving <br>
Identify key drivers of attrition <br>
Enable targeted, data-driven retention strategies <br>
Incorporate external job market trends into workforce planning <br>

# Data
## Internal HR Data
IBM HR dataset and synthetic employee data <br>
Includes demographics, job characteristics, compensation, satisfaction, and tenure <br>
## External Data
LinkedIn job postings (~33,000 records) <br>
Used to estimate job demand and salary benchmarks <br>
Serves as a proxy for external labor market conditions <br>

# Method
Algorithm: XGBoost (binary classification) <br>
Platform: AWS SageMaker built-in XGBoost container <br>
Hyperparameter tuning using SageMaker Automatic Model Tuning <br>
Training data stored and accessed from Amazon S3 <br>

# Key Findings
External job demand is the strongest predictor of attrition <br>
Overtime is strongly associated with higher attrition risk <br>
Compensation gaps increase likelihood of turnover <br>
Career stagnation and low satisfaction are key internal drivers <br>
