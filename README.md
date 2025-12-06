# **CDC-Diabetes-Health-Indicators**

## Description
This project aims to explore how feature variables contribute to the target outcome and analyze the relationships among variables, and further develops a predictive framework for classifying health states with improved accuracy.

## About Data 

#### **Diabetes Health Indicators Dataset**

The Diabetes Health Indicators dataset contains health-related survey responses from the CDC’s Behavioral Risk Factor Surveillance System (BRFSS), providing information on chronic conditions, lifestyle habits, and demographic factors. This project uses [Diabetes_012_health_indicators_BRFSS2015.csv](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset?select=diabetes_012_health_indicators_BRFSS2015.csv), a cleaned dataset from the year 2015.

- **Health states were labeled based:**
    - 0: no diabetes or only during pregnancy
    - 1: prediabetes
    - 2: diabetes

- **Dataset Summary**: 253,680 survey responses to the CDC's BRFSS2015 and 21 feature variables.

- **Imbalanced Class**: The non-diabetes class appears approximately five times larger than both the prediabetes and diabetes classes.

> **To download the data, you can download it from the following link: [here](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset)**

## Project Structure

| **File**         | **Description**                                  |
|------------------|--------------------------------------------------|
| diabetes.html    | HTML report of the project’s analysis and models |
| diabetes.pdf     | PDF version of the project report                |

## Pipeline

### **A/B testing**:

- **Qualitative variables**: testing for independence using a Resampling Method to overcome the limitation when the chi-square test has at least one expected frequency ($E_{ij}$) less than 5.


