# Healthcare Analysis
![istockphoto-1373659740-612x612](https://github.com/Babatunde-Oduwole/Healthcare-Analytics/assets/167521089/30ea3d7a-101f-4b34-82ac-55238289e6c4)


## Table of Contents


- [Project Introduction](#Project-Introduction)
- [Data Source](#Data-Source)
- [Tools](#Tools)
- [Data Cleaning/Preparation](#Data-Cleaning/Preparation)
- [Exploratory Data Analysis (EDA)](#Exploratory-Data-Analysis (EDA))
- [Data Analysis](#Data-Analysis)
- [Findings](#Findings)
- [Recommendations](#Recommendations)
- [Limitations](#Limitations)

### Project Introduction


This project focuses on analyzing healthcare data to identify trends, patterns, and insights that can be used to improve patient outcomes and operational efficiency. The visualization techniques used aim to transform complex datasets into meaningful insights for stakeholders in the healthcare industry.

### Data Source

The data for this project was gotten from kaggle.com, it contains informations such as patient names, blood type, hospitals, insurance provider, and admission types, among others. These datasets offer comprehensive information on patient care, and healthcare resource utilization.

### Tools

1. PostgreSQL - Data Analysis
2. Power BI - Data cleaning and Visualization

### Data Cleaning/Preparation

Data cleaning and preparation involved multiple steps.
1. Handled missing values using techniques like deletion of non-informative rows.
2. Standardized categorical variables to ensure consistency across datasets.
3. Created new features based on existing data to improve the quality of analysis.

### Exploratory Data Analysis (EDA)

EDA involved exploring the sales data to answer key questions, such as:

1. What was the total number of patients?
2. What was the total number of doctors?
3. What was the total amount of billing per month?
4. What was the total amount of insurance provider by gender?
5. What was the total categories of blood group by gender?
6. What was the admission type by gender?
7. What was the medical condition by gender?
8. What was the total number of patients by medical condition?
9. What was the total number of doctors by admission type?
10. What was the average age of patients by medical condition?

### Data Analysis

Some of the interesting code/features worked with include:

```sql
SELECT 
    gender, 
    medical_condition, 
FROM 
    healthcare_dataset
GROUP BY 
    gender, 
    medical_condition;
```

```sql
SELECT department, COUNT(*) AS patient_count 
FROM admissions 
GROUP BY department;
```

### Findings
Below are some of the finding discovered after analysis:
1. The female gender constitutes the highest number of patients across all types of admission.
2. The medical condition with highest number of patient are Asthma and cancer, this has continue to remain the same a period of 6 years.

### Recommendations

Based on the analysis, the following recommendations are suggested for actions:

1. More resources should be allocated to medical conditions with consistently high patient volumes.
2. Further analysis is needed to determine the reason the females having the most number of patients across all types of admission.
3. Further analysis is also needed to determine the reason for the high rate of patients with asthma, and cancer over the years (6 years) 


### Limitations

1. Some datasets had missing or incomplete information, affecting the quality of analysis.
2. The analysis did not consider external factors such as socioeconomic status, which could impact healthcare outcomes.


