**Model Description**

This model is made to predict customer churn by identifying customers who are likely to cancel a service or subscription given the features below.

**Input Features**

| Input Features | Description                                                                              |
|----------------|------------------------------------------------------------------------------------------|
| bundleID       | A concatenation of each unique combination of services (322)                             |
| contractID     | A concatenation of each unique combination of contract, billing, and payment method (24) |
| gender         | Is customer is male or female                                                            |
| SeniorCitizen  | If customer is a senior citizen or not (Yes or No)                                       |
| Partner        | If customer has a partner or not (Yes or No)                                             |
| Dependents     | If customer has dependents or not (Yes or No)                                            |
| tenure         | How long the customer has been with the company                                          |
| MonthlyCharges | The amount charged to customer each month for services used                              |

**Output Interpretation**

The model’s output is binary prediction where ‘No’ for customers predicted not to churn and ‘Yes’ for customers predicted to churn.

In the context of business problem, understanding who is likely to churn enables the business to take proactive measures to retain these those customers, maybe by addressing service issues.

**Performance Metrics**

The performance metrics used to evaluate the model are below

-   Accuracy: Proportion of all predictions that were correct
-   Precision: Proportion of positive identifications that were actually correct
-   Recall: Proportional of actual positives that were identified correctly
-   F1 Score: Harmonic mean of precision and recall, a balance between the two
-   AUC: Measure of the ability of the classifier to distinguish between classes
-   ROC Curve: Graph showing the performance of a classification model at all classification thresholds

**Instructions On How To Use The Model**

Preprocessing: Choose the relevant columns through SQL query.

Feature engineering: If new data is collected, encoding should also be applied to both the training and testing data.

Making predictions: With the data preprocessed and encoded, predictions can be made by calling the model’s ‘predict’ method.

Interpreting Predictions: The output should be interpreted as the probability of a customer churning versus not churning. A threshold can also be set according to business requirements to classify a customer as at-risk of churning.
