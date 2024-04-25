# User Churn Dashboard
## Purpose
This diagnostic dashboard is designed to provide a deep dive into user churn behaviors and service-related issues, enabling onboarding managers and product support teams to pinpoint inefficiencies and improve customer retention. It specifically helps in understanding the underlying causes of churn and the impact of service delivery on customer satisfaction.

## Access
This dashboard can be accessed by the Tableau server. The link will be updated as the project nears completion

# Data Sources
This dashboard is powered by data from a AWS RDS database set up by our initial Sprint 1. We connect the dashboard with the appropriate credentials of the database

# Key Metrics
The key metrics displayed on this dashboard include:

- **Churn Rate**: The percentage of customers who have stopped using the service from the past month.
- **Ticket Volume by Service Category**: Evaluates the number of support tickets within each service category to identify high-risk areas.
- **Ticket Volume by Service Count**: Evaluates the nuber of support tickets within each group of service count the customers are enrolled in.

# How to use the dashboard
- **Interactive Filters**: Users can apply filters to analyze specific customer segments, compare different service categories, or focus on particular time frames.
- **Dynamic Visualization**: Provides real-time updates that reflect changes based on user-selected parameters, offering tailored diagnostic insights.

# How to refresh the data
Upon completion of the ETL Pipeline, the dashboard will be refreshed at 12pm on the 1st of every month. The data will be updated to reflect the previous month's data.
