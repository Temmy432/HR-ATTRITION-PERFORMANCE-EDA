# HR-ATTRITION-PERFORMANCE-EDA
Exploratory Data Analysis (EDA) of IBM HR Analytics Employee Attrition & Performance dataset to uncover key drivers of employee turnover, performance trends, and actionable HR insights.

---
Exploratory Data Analysis (EDA) Report

IBM HR Analytics: Employee Attrition & Performance

1. Introduction

Employee attrition remains a critical concern for organizations striving to retain skilled talent, maintain productivity, and manage operational costs. This analysis leverages the IBM HR Analytics Employee Attrition & Performance dataset to explore patterns behind employee turnover, job satisfaction, and performance within a corporate environment.

The dataset includes comprehensive information on employee demographics, compensation, job roles, performance metrics, and work-life balance indicators. The objective is to extract actionable insights that can inform human resource (HR) strategies, improve employee retention, and drive organizational effectiveness.

2. Executive Summary

This EDA investigates the key factors influencing employee attrition and performance within the IBM HR Analytics dataset. With attrition impacting stability and increasing organizational costs, it is vital to identify underlying causes and address them strategically.

The dataset comprises 1,470 employee records, capturing a broad range of attributes such as salary, satisfaction levels, overtime status, tenure, and performance ratings. The analysis uncovered the following insights:

Overtime, early career stage, and specific job roles (e.g., Sales Representative, Lab Technician) are strongly associated with higher attrition.

Job satisfaction shows weak correlation with financial metrics, highlighting the influence of intrinsic and environmental factors.

Salary hikes are strictly aligned with performance ratings, with a clear gap between ratings 3 and 4.

Higher monthly income tends to correlate with retention, but income alone does not drive satisfaction or loyalty.

These findings emphasize the need for holistic HR strategies that go beyond compensation to include employee engagement, career development, and work-life balance.

3. Objectives

This analysis aims to:

Examine employee demographics and satisfaction levels

Analyze income distribution by gender, education, department, performance, and attrition

Identify key drivers of attrition, such as overtime, experience, job role, and commute distance

Evaluate the link between salary hikes and performance ratings

Determine the most influential factors contributing to turnover

Recommend strategies to improve employee engagement and reduce attrition

4. Data Source

The dataset was sourced from Kaggle and includes:

1,470 employee records

35 features, covering demographics, job details, compensation, performance, and satisfaction metrics

The data is structured in CSV format and serves as a valuable case study for applying analytics in real-world HR contexts.

5. Data Overview

Key data categories:

Demographics: Age, Gender, Education, Marital Status

Job Attributes: Department, Job Role, Business Travel, Distance from Home

Compensation: Monthly Income, Percent Salary Hike, Stock Options

Work-Life Balance: Overtime, Work-Life Balance Score, Job Satisfaction

Experience: Total Working Years, Years at Company, Training Times Last Year

6. Data Preprocessing

To ensure analytical accuracy and consistency, the following steps were taken:

Loaded and validated the dataset using Pandas

Confirmed no missing/null values

Applied label encoding and one-hot encoding for categorical variables

Standardized data types and formats

Created derived features (e.g., income brackets, age groups)

Removed redundant or non-informative columns

7. Key Analysis & Findings

7.1 Gender Distribution

60% Male, 40% Female

7.2 Job Satisfaction

61% report moderate to high satisfaction (Levels 3–4)

39% report low satisfaction (Levels 1–2)
![](Images/Screenshot%202025-07-22%20170122.png)      

7.3 Monthly Income Patterns

By Gender: Females slightly out-earn males ($6,687 vs. $6,381 average)

By Education: Higher education leads to higher income

By Department: R&D leads in income; HR ranks lowest

7.4 Distance from Home by Role

Sales Executives and Research Scientists have the longest commutes

HR staff typically live closer to work

7.5 Attrition Trends

Overall attrition: 16% (237 employees)

Overtime: 54% of those who left were working overtime

Experience: Highest attrition in 0–6 years of experience

Job Role: Sales Reps and Lab Technicians show higher turnover; Managers and Directors show stability

7.6 Performance Rating vs. Salary Hike

Rating 4 employees receive 20%–25% hikes

Rating 3 employees receive 11%–19% hikes

Clear, categorical differentiation in hike structure

7.7 Average Salary Hike

Rating 3: 14.0%

Rating 4: 21.8%

7.8% differential favoring higher performers

7.8 Monthly Income vs. Attrition

Employees who stayed had higher and more varied income

Those who left had lower, concentrated income

7.9 Correlation with Job Satisfaction

Weak correlations found:

Positive:

Attrition (0.103)

DailyRate (0.031)

PercentSalaryHike (0.020)

Negative:

HourlyRate (-0.071)

NumCompaniesWorked (-0.056)

Compensation-related factors have minimal effect on satisfaction

8. Key Insights

Overtime is a strong predictor of attrition — indicating potential burnout

Younger, less experienced employees are more likely to leave

Job-specific attrition: Sales Reps and Lab Technicians are at higher risk

Job satisfaction is likely influenced by non-monetary factors

Salary hikes are well-aligned with performance but may not directly boost retention

Monthly income is not a standalone predictor of attrition

9. Recommendations

Monitor Overtime Patterns: Reduce excessive workloads and avoid burnout through policy changes and automation tools

Support Early-Career Employees: Implement mentorship, career growth programs, and regular recognition

Tailor Interventions by Job Role: Develop role-specific retention strategies for Sales and Technical roles

Focus Beyond Compensation: Invest in leadership development, team cohesion, and meaningful work experiences

Develop Early-Warning Systems: Combine overtime, satisfaction, income, and tenure data to identify at-risk employees

10. Conclusion

This analysis underscores the multifaceted nature of employee attrition. While compensation and performance evaluation play a role, they are not sufficient alone to retain talent.

Overtime demands, job roles, and early career dynamics are more prominent drivers of turnover. Organizations should adopt a data-driven, holistic HR strategy that prioritizes employee experience, growth opportunities, and workload balance.

Doing so can enhance employee engagement, reduce attrition rates, and create a more resilient and motivated workforce.
