Problem statement:
Analyze Airtel customer data to identify key drivers of churn and provide actionable insights to improve customer retention and protect revenue.

Steps:
- Analyzed churn behavior using customer service calls, plan types, and usage metrics.
- Segmented customers to understand churn drivers.
- Business recommendations to reduce churn.
- Tools Used: Python, Pandas, Feature Engineering

Key insights & conclusion:
- Those who have not taken the international plans , are retaining more as compared to those who have taken the international plain and churning more.
- Significant difference in average customer service calls for both the groups(churned & non-churned).
- Day charges are more as compared to evening & night charges.
- difference in total day minutes between churned and non-churned customers is EXTREMELY statistically significant.
- Customers making more than three calls exhibit churn rates above 50%, compared to only 11% for low-contact customers. This suggests that repeated service issues are a major churn driver, and early intervention after the third call could significantly reduce customer attrition.
- International calls have almost no effect here.

* Low international callers churn MORE than high callers.
* International calls affect churn differently by plan
* Biggest churn comes from unused international plans

Detailed analysis in the code attached in folder
