
# Data Dictionary for Customer Churn Dataset

## Metadata
- **Source:** [Kaggle](https://www.kaggle.com/datasets/datazng/telecom-company-churn-rate-call-center-data)
- **Owner:** DataZng
- **Last Updated:** A year ago
- **Notes:** The orginal dataset has 23 features. We add another feature NumServices which is calculated based on PhoneService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies. We then created a star schema with a fact table and 3 dimension tables.

<!-- --- -->

## Original Dictionary

### Data Attributes
| Attribute Name    | Data Type       | Description                                           |
|-------------------|-----------------|-------------------------------------------------------|
| customerID        | VARCHAR(25)     | Unique identifier for the customer                    |
| gender            | VARCHAR(6)      | Customer's gender (Male/Female)                       |
| SeniorCitizen     | BOOL            | Indicates if the customer is a senior citizen (1 means senior citizen)         |
| Partner           | VARCHAR(3)      | Whether the customer is married/ in a live-in relationship (Yes/No) |
| Dependents        | VARCHAR(3)      | Whether the customer has dependents - children/ retired parents (Yes/No)                   |
| tenure            | INT             | Number of months the customer has stayed with the company |
| PhoneService      | VARCHAR(3)      | Whether the customer has a phone service (Yes/No)              |
| MultipleLines     | VARCHAR(25)     | Whether the customer has multiple lines (Yes/No/No phone service)               |
| InternetService   | VARCHAR(25)     | Customer's internet service type (DSL/Fiber optic/No)                      |
| OnlineSecurity    | VARCHAR(25)     | Whether the customer has online security (Yes/No/No internet service)              |
| OnlineBackup      | VARCHAR(25)     | Whether the customer has online backup (Yes/No/No internet service)                |
| DeviceProtection  | VARCHAR(25)     | Whether the customer has device protection (Yes/No/No internet service)            |
| TechSupport       | VARCHAR(25)     | Whether the customer has tech support (Yes/No/No internet service)                 |
| StreamingTV       | VARCHAR(25)     | Whether the customer has streaming TV (Yes/No/No internet service)                 |
| StreamingMovies   | VARCHAR(25)     | Whether the customer has streaming movies (Yes/No/No internet service)             |
| NumServices       | INT             | The number of services the customer is using from the telecom          |
| Contract          | VARCHAR(25)     | The term of the customer's contract (Month-to-month/One year/Two year)                   |
| PaperlessBilling  | VARCHAR(3)      | Whether the customer has paperless billing (Yes/No)            |
| PaymentMethod     | VARCHAR(25)     | The customer's payment method                         |
| MonthlyCharges    | DECIMAL(10, 2)  | The amount charged to the customer every month        |
| TotalCharges      | DECIMAL(10, 2)  | The total amount charged to the customer              |
| numAdminTickets   | INT             | Number of administrative tickets raised by the customer |
| numTechTickets    | INT             | Number of technical tickets raised by the customer    |
| Churn             | VARCHAR(3)      | Whether the customer has churned or not (Yes/No)               |

## StarSchema Dictionary

<!-- ### Data Attributes -->
The StarSchema organizes data into Fact and Dimension tables as follows:

#### FACT_CHURN
- Attributes and Key Types:
  - **customerID:** VARCHAR(25), Composite Primary Key, Foreign Key to DIM_CUSTOMER
  - **bundleID:** INT, Composite Primary Key, Foreign Key to DIM_BUNDLE
  - **contractID:** INT, Composite Primary Key, Foreign Key to DIM_CONTRACT
  - **MonthlyCharges:** DECIMAL(10, 2)
  - **TotalCharges:** DECIMAL(10, 2)
  - **numAdminTickets:** INT
  - **numTechTickets:** INT
  - **Churn:** VARCHAR(3)

#### DIM_CUSTOMER
- Attributes:
  - **customerID:** VARCHAR(25), Primary Key
  - **gender:** VARCHAR(6)
  - **SeniorCitizen:** BOOL
  - **Partner:** VARCHAR(3)
  - **Dependents:** VARCHAR(3)
  - **tenure:** INT

#### DIM_BUNDLE
- Attributes:
  - **bundleID:** INT, Primary Key
  - **PhoneService:** VARCHAR(3)
  - **MultipleLines:** VARCHAR(25)
  - **InternetService:** VARCHAR(25)
  - **OnlineSecurity:** VARCHAR(25)
  - **OnlineBackup:** VARCHAR(25)
  - **DeviceProtection:** VARCHAR(25)
  - **TechSupport:** VARCHAR(25)
  - **StreamingTV:** VARCHAR(25)
  - **StreamingMovies:** VARCHAR(25)
  - **NumServices:** INT

#### DIM_CONTRACT
- Attributes:
  - **contractID:** INT, Primary Key
  - **Contract:** VARCHAR(25)
  - **PaperlessBilling:** VARCHAR(3)
  - **PaymentMethod:** VARCHAR(25)