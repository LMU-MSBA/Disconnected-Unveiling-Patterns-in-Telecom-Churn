# User Churn Dashboard
## Purpose
The purpose of this dashboard is to provide a high-level overview of the user churning behavior amongst different characteristics. It is intended to empower stakeholders by providing them with a comprehensive overview of (1) their consumer’s churn and (2) the key metrics that influence consumer churn. This dashboard is designed to be used by onboarding managers and product support teams to monitor the effectiveness of the user onboarding process and provide customer support as needed.

## Access
This dashboard can be accessed by the Tableau server. The link will be updated as the project nears completion

# Data Sources
This dashboard is powered by data from a kaggle dataset about a telecommunication company. The dataset contains information about customer demographics, services, and churn rates.

The data is publicly available and can be accessed [here](https://www.kaggle.com/datasets/datazng/telecom-company-churn-rate-call-center-data).

# Key Metrics
The key metrics displayed on this dashboard include:

- **Churn Rate**: The percentage of customers who have stopped using the service from the past month.
- **Support Tickets**: The number of support tickets opened by customers from the last month.
- **Charges**: The charges summary from past accounts each month
-**Number of Services Distribution**: The distribution of customers based on the number of services they are enrolled in

# How to use the dashboard
The dashboard is a 1 month rolling basis of customer information and can be used to identify customer groups that needs more product support.

# How to refresh the data
Upon completion of the ETL Pipeline, the dashboard will be refreshed at 12pm on the 1st of every month. The data will be updated to reflect the previous month's data.
