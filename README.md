# Employee Salary Analysis and Recommendation  
**Course**: ADS 575 - Applied Testing for Data Science  
**Student**: Şeyma Gülşen Akkuş  
**Date**: 28.05.2025  

---

## Project Description

This project presents a comprehensive salary analysis for a dataset provided by Monsanto (acquired by Bayer), on behalf of ICL Group. The goal is to understand:

- What factors influence salaries the most?
- Are there disparities across departments, professions, or demographic groups?
- Are there any signs of bias or unfair pay structure?
- What recommendations can be made to improve salary policies?

The dataset contains detailed employee records from multiple departments and professions, including salary, demographics, education, and company tenure for 250,000 employees.

---

## Key Objectives

- Determine key drivers of employee salary using statistical and machine learning methods.
- Analyze salary distribution across departments, jobs, and professions.
- Evaluate fairness with respect to gender, marital status, and other demographic features.
- Provide HR-oriented, data-driven policy recommendations.

---

##  Methodology

### 1. **Data Preprocessing**
- Removed irrelevant columns (e.g., `id`)
- Renamed misspelled columns (e.g., `Profesion` → `Profession`)
- Encoded categorical features
- Created derived features (e.g., Age from Birth Year)

### 2. **Exploratory Data Analysis (EDA)**
- Salary distribution and quantiles
- Group-wise salary analysis by:
  - Gender
  - Marital Status
  - Degree
  - Profession
  - Job
  - Department

### 3. **Statistical Testing**
- ANOVA, Kruskal-Wallis, Chi-Square for group comparisons
- Shapiro-Wilk for normality testing
- Correlation matrices (Pearson, Spearman, Kendall)

### 4. **Modeling**
- Linear Regression for feature importance
- StandardScaler for numerical features
- R² and RMSE for model performance evaluation

---

## Key Findings

- **Strongest Influencers**:  
  -  `Years of Education` and `Years in the Company` are the most significant predictors of salary.
  - Their effect is both statistically and practically significant.

- **Demographics**:  
  - Sex and Marital Status have no meaningful impact on salary.
  - Minor differences observed are not practically significant.

- **Job and Department**:  
  - Salary is consistent across jobs and departments when adjusted for sample imbalance.
  - No job or department is favored in terms of compensation.

- **Professions**:  
  - No profession shows salary privilege; distribution is uniform and fair.

---

## Fairness and Bias Assessment

- ✅ No evidence of systemic discrimination in salary.
- ❌ Minor statistical differences exist in combinations like `Sex × Department`, but require HR follow-up to confirm cause.
- ✔️ Consistent salary progression observed with education and tenure (supports internal fairness).

---

## Recommendations

- Prioritize **education and experience** in compensation models.
- Continue using structured, tenure-based salary progression.
- Increase **transparency** of salary policy to build employee trust.
- Monitor minor disparities in subgroup intersections (e.g., age × department).
- Conduct periodic fairness audits to maintain equality in compensation.

---

## 🛠Technologies Used

| Category            | Tools/Libraries                         |
|---------------------|------------------------------------------|
| Data Processing     | `pandas`, `numpy`                        |
| Visualization       | `seaborn`, `matplotlib`, `plotly`       |
| Modeling            | `sklearn`, `statsmodels`                |
| Statistical Tests   | `scipy.stats`, `kruskal`, `shapiro`     |


---

## Author

**Şeyma Gülşen Akkuş**  
Graduate Student, Applied Data Science  
TED University


