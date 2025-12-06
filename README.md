# **CDC-Diabetes-Health-Indicators**

## Description
This project aims to explore how feature variables contribute to the target outcome, analyze inter-variable relationships, and further develops a predictive framework for classifying health states with improved accuracy.


## About Data 

#### **Diabetes Health Indicators Dataset**

The Diabetes Health Indicators dataset contains health-related survey responses from the CDC’s Behavioral Risk Factor Surveillance System (BRFSS), providing information on chronic conditions, lifestyle habits, and demographic factors. This project uses the cleaned 2015 dataset [Diabetes_012_health_indicators_BRFSS2015.csv](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset?select=diabetes_012_health_indicators_BRFSS2015.csv).

- **Health states were labeled by:**
    - 0: no diabetes or only during pregnancy
    - 1: prediabetes
    - 2: diabetes

- **Dataset Summary**: 253,680 survey responses to the CDC's BRFSS2015 with 21 feature variables.

- **Class Imbalance**: The non-diabetes class appears approximately five times larger than both the prediabetes and diabetes classes.

> **You can download the dataset from Kaggle: [here](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset)**


## Project Structure

| **File**         | **Description**                                  |
|------------------|--------------------------------------------------|
| diabetes.html    | HTML report summarizing the analysis and models |
| diabetes.pdf     | PDF version of the project report                |


## Workflow

### **Data Visualization**:

Visualizing the distribution of feature variables and the relationships among them before performing A/B testing.

### **A/B testing**:

- **Qualitative variables**:
  Testing for independence using a Resampling method to overcome the limitation when the Chi-square test has at least one expected frequency $E_{ij}$ less than 5.  
- **Quantitative variables**:
  Testing for differences between groups using the Resampling ANOVA method to address the limitations of traditional ANOVA

### **Dealing with imbalanced data**:

- Under Sampling
- Over Sampling  
- SMOTE  
- Class Weight  
- Under Sampling + SMOTE  
- Under Sampling + Over Sampling

### **Classification Modeling**: 

- 3-class classification
- 2-class classification (merging prediabetes and diabetes)




