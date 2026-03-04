Problem statement:
Analyze Airtel customer data to identify key drivers of churn and provide actionable insights to improve customer retention and protect revenue.

Steps:
- Analyzed churn behavior using customer service calls, plan types, and usage metrics.
- Segmented customers to understand churn drivers.
- Business recommendations to reduce churn.
- Tools Used: Python, Pandas, Feature Engineering

Key insights :
- Those who have not taken the international plans , are retaining more as compared to those who have taken the international plain and churning more.
- Significant difference in average customer service calls for both the groups(churned & non-churned).
- Day charges are more as compared to evening & night charges.
- difference in total day minutes between churned and non-churned customers is EXTREMELY statistically significant.
- Customers making more than three calls exhibit churn rates above 50%, compared to only 11% for low-contact customers. This suggests that repeated service issues are a major churn driver, and early intervention after the third call could significantly reduce customer attrition.
- International calls have almost no effect here.

* Low international callers churn MORE than high callers.
* International calls affect churn differently by plan
* Biggest churn comes from unused international plans

Challenges Faced :
- Imbalanced target variable required careful aggregation to avoid misleading conclusions.
- Raw numerical features needed binning and segmentation to extract meaningful patterns
- Customer behavior metrics were highly skewed, requiring threshold-based analysis.
- Understanding churn drivers required combining multiple dimensions (plan type, calls, usage) instead of relying on single variables.

Recommendations :
 Customer Experience
- Proactively flag customers with >3 service calls for retention outreach.
- Improve first-call resolution to reduce repeated support interactions.
- Implement customer satisfaction checks after multiple support contacts.

International Plan Strategy :
- Review pricing and service quality for international plans.
- Offer personalized retention offers to high international-usage customers.
- Monitor churn separately for international vs non-international segments.

Retention Strategy
- Build an early-warning churn system using:
    * Service call count
    * International plan usage
    * High monthly charges




Target high-risk customers with loyalty incentives before churn occurs.
Detailed analysis in  code attached in the folder

SQL:
create database TelecommChurnAnalysis
--drop table PorterdataAnalysis
create table TelecommChurn(state1 varchar(10), account_length int, area_code varchar(100), international_plan varchar(4),
       voice_mail_plan varchar(4), number_vmail_messages float, total_day_minutes float,
       total_day_calls float, total_day_charge float, total_eve_minutes float,
       total_eve_calls float, total_eve_charge float, total_night_minutes float,
       total_night_calls float, total_night_charge float, total_intl_minutes float,
       total_intl_calls float, total_intl_charge float,
       number_customer_service_calls float, churn varchar(4)
)

--truncate table  hospitaladmissionanalysis
select * from TelecommChurn;



Skills Demonstrated :

Data Cleaning & Preprocessing
Exploratory Data Analysis (EDA)
Statistical Analysis
Data Visualization
Business Insight Generation
power bi Dashboard Development
Problem Solving

Tools & Technologies :

Python
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook
