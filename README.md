# Workplace Diversity Analysis

## Project Overview

This project analyzes employee organizational structure, salary prediction, and potential gender pay disparities using Python, Pandas, and Scikit-learn.

The dataset contains 10,000 employee records across HR, Engineering, Marketing, and Sales.

## Technologies Used

- Python
- Pandas and NumPy
- Scikit-learn
- Random Forest Regressor
- Matplotlib
- Jupyter Notebook

## Project Workflow

### 1. Data Preparation and Employee Hierarchy

- Loaded and validated employee and company datasets.
- Identified organizational levels from CEO to Individual Contributor.
- Calculated direct and indirect employee reports.
- Merged organizational and salary data.
- Prepared numerical features using ordinal and one-hot encoding.

### 2. Machine Learning — Salary Prediction

- Split the modeling dataset into 80% training and 20% testing.
- Trained a Random Forest Regressor using 100 decision trees.
- Generated salary predictions for 2,000 test employees.
- Evaluated performance using MAE and R².

**Model Results:**

| Metric | Result |
|---|---|
| Mean Absolute Error | $59,730.60 |
| R² | 0.2917 |

The model captures some salary patterns but has limited predictive accuracy.

### 3. Feature Importance

The most influential model features were:

| Feature | Importance |
|---|---:|
| HR department indicator | 58.28% |
| Years of experience | 10.57% |
| Engineering department indicator | 10.46% |
| Number of reports | 7.08% |

These values represent model feature importance, not causal salary effects.

### 4. Gender Salary Analysis

Average annual salaries:

| Gender | Average Salary |
|---|---:|
| Male | $198,954.34 |
| Female | $171,314.52 |

The overall unadjusted difference was approximately $27,640 in favor of men.

Additional comparisons were conducted by department and organizational level. These revealed smaller and mixed differences across employee groups.

## Key Findings

- Organizational structure and management reporting relationships were successfully reconstructed.
- Department membership and years of experience were influential salary prediction features.
- The overall gender salary difference may partly reflect employee distribution across departments.
- Descriptive salary differences alone do not establish discrimination or pay equity.

## Recommendations

- Conduct more detailed salary comparisons within similar job roles.
- Incorporate job title, tenure, performance, and location into future analysis.
- Investigate unexplained pay differences using more rigorous statistical methods.
- Improve model accuracy through additional features and validation.

## Conclusion

This project demonstrates an end-to-end Python data analysis workflow combining data preparation, organizational hierarchy analysis, machine learning, and HR reporting.

The findings provide a foundation for further compensation analysis and data-driven HR decision-making.
