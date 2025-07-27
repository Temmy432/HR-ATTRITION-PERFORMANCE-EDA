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

![](Images/Screenshot%202025-07-26%20000509.png)      

7.2 Job Satisfaction

The bar chart shows how employees are distributed across different job satisfaction levels (on a scale of 1 to 4):

•	Level 4 (Very Satisfied): 459 employees

•	Level 3 (Satisfied): 442 employees

•	Level 2 (Somewhat Dissatisfied): 280 employees

•	Level 1 (Dissatisfied): 289 employeees

•	A majority of employees report moderate to high job satisfaction, with over 60% falling under levels 3 and 4.

•	However, nearly 40% (levels 1 and 2 combined) still experience some level of dissatisfaction, which is significant enough to warrant attention


![](Images/Screenshot%202025-07-22%20170122.png)      


7.3 Monthly Income Patterns

By Gender:

• Females: $6,687

•  Males: $6,381

•  This shows that females earn approximately $306 more per month on average than males.


![](Images/Screenshot%202025-07-22%20232646.png)     


By Education

This analysis shows that monthly income increases with education level, rising from $5,641 to $8,278. The highest education group earns significantly more, with greater income variation. This suggests that

higher education leads to better-paying and more diverse job opportunities.

![](Images/Screenshot%202025-07-22%20233905.png)

By Department

The chart shows that Research & Development has the highest total monthly income at $6,036,284, followed by Sales with $3,103,791, while Human Resources earns the least at $419,234. This indicates that Research & 

Development contributes the most financially among all departments.



![](Images/Screenshot%202025-07-23%201612411.png)  




7.4 Distance from Home by Role

•	Sales Executives have the highest distance from home at 3,149 units.

•	Research Scientists follow closely with 2,632 units.

•	Laboratory Technicians also live far, with 2,437 units distance.

•	Human Resources employees live closest to work, with just 425 units distance.

•	Managers and Research Directors have moderate distances of 819 and 675 units, respectively.

•	This indicates that job roles like Sales and Research often require commuting from longer distances, possibly due to job location constraints or role-specific demands.

![](Images/Screenshot%202025-07-23%20161543.png) 


7.5 Attrition Trends

Employee Attrition

This analysis compares the number of employees who left the company (Attrition = Yes) vs. those who stayed (Attrition = No).

•	Only 237 employees left the company.

•	1,233 employees stayed.

•	Majority of the workforce (~84%) did not leave.

•	Around 16% attrition rate (237 / 1470 total employees).

![](Images/Screenshot%202025-07-23%20161758.png) 

Attrition by Overtime Status

•  Employees who work overtime are more likely to leave:

•	127 employees who left the company had OverTime = Yes.

•	Only 110 who left had OverTime = No.

•	Among those who left: 54% (127 out of 237) worked overtime.

•	Among those who stayed: only 289 out of 1,233 worked overtime (~23%).

•	944 employees stayed and did not work overtime — that's over 76% of the retained workforce.


![](Images/Screenshot%202025-07-24%20143406.png) 


Attrition by Total working Years

•  Employees who left the company had fewer total working years than those who stayed.

•  Most employees who left had around 3 to 6 years of experience.

•  Employees who stayed had around 10 years of experience on average.

•  Those with more working years (above 15) were less likely to leave.

•  Attrition is higher among less experienced employees.

•  Some employees left very early, even with 0–2 years of experience

![](Images/Screenshot%202025-07-24%20162624.png)  

Attrition by Job Role

•  Laboratory Technicians had the highest number of employees who left (62).

•  Sales Executives (57) and Research Scientists (47) also had high attrition.

•  Sales Representatives had a high attrition rate compared to the total in that role (33 out of 83).

•  Managers, Healthcare Reps, and Research Directors had the lowest attrition counts.

•  Most job roles show a much higher number of employees staying than leaving.

•  Roles like Manufacturing Director and Research Director show very low attrition, suggesting better retention in leadership or specialized roles

` Sales Reps and Lab Technicians show higher turnover; Managers and Directors show stability

![](Images/Screenshot%202025-07-24%20163244.png) 

7.6 Performance Rating vs. Salary Hike

Two distinct clusters:

•	One cluster of data points is at Performance Rating = 3

•	Another cluster is at Performance Rating = 4

Salary hike is higher for employees rated 4:

•	Employees with Performance Rating = 4 received a higher Percent Salary Hike (mostly between 20% and 25%).

•	Employees with Performance Rating = 3 received a lower Percent Salary Hike (mostly between 11% and 19%).

 No overlapping in ratings:

•	No employee with a performance rating of 3 got a salary hike of 20% or above.

•	No employee with a performance rating of 4 got a salary hike below 20%.

No gradual progression:

•	The relationship between PercentSalaryHike and PerformanceRating appears categorical rather than continuous—no midpoints or mixed values.


![](Images/Screenshot%202025-07-24%20163715.png)   


7.7 Average Salary Hike

•	Employees with Performance Rating of 4 receive a significantly higher average salary hike than those rated 3.

•	Employees rated 4 get an average of 7.8% more salary hike than those rated 3.

•	The company appears to reward higher-rated employees more generously,

![](Images/Screenshot%202025-07-24%20164427.png)


7.8 Monthly Income vs. Attrition

Employees who stayed had higher and more varied income

Those who left had lower, concentrated income

![](Images/Screenshot%202025-07-24%20164954.png)  

7.9 Correlation with Job Satisfaction

Positive Correlations

Attrition (0.103) shows the highest positive link to job satisfaction — people may leave for reasons other than dissatisfaction.

BusinessTravel (0.034), Gender (0.033), DailyRate (0.031), and SalaryHike (0.020) show slight positive links.

Weak Influencers

StockOptionLevel (0.011), PerformanceRating (0.002), and most pay factors (e.g., MonthlyIncome) have little effect.

EnvironmentSatisfaction and Training are negligible.

Negative Correlations

HourlyRate (-0.071) shows the strongest negative link.

NumCompaniesWorked (-0.056) and EducationField (-0.055) also relate to lower satisfaction.

Other weak negatives: OverTime, JobRole, WorkLifeBalance, etc.

Observation

Pay, performance, and recognition don’t strongly drive satisfaction.

Those who leave may not be unhappy — they might just be ready to move on.

![](Images/Screenshot%202025-07-25%20164355.png) 



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
