#### **Determine Business Objectives**

-   **Background**
    -   The subscription video on demand (SVOD) landscape is consistently becoming more competitive as more SVOD companies emerge to gain market share. In 2021, 85% of US households subscribed to a SVOD service, and 35% were estimated to churn ([As The World Churns: The Streaming Wars Go Global \| Deloitte, 2021](https://www.deloitte.com/global/en/our-thinking/insights/industry/technology/technology-media-and-telecom-predictions/2022/streaming-video-churn-svod.html)). Customer churn is a critical problem among SVOD services as it is costly to acquire new customers and even more expensive to re-acquire churned customers, especially as the SVOD competition increases ([As The World Churns: The Streaming Wars Go Global \| Deloitte, 2021](https://www.deloitte.com/global/en/our-thinking/insights/industry/technology/technology-media-and-telecom-predictions/2022/streaming-video-churn-svod.html)). Disney’s SVOD service is one of the market leaders, and it is paramount for Disney to reduce consumer churn. In 2023, Disney+ bundle’s consumer churn rate was allegedly around 2%, which was lowest consumer churn in the SVOD industry ([Redirecting, 2023](https://www.indiewire.com/news/analysis/disney-bundle-cost-churn-rate-netflix-1234876494/)). However, in Q1 of 2024, Disney+ bundle’s churn rate was around 4% and they did no longer have the lowest consumer churn in the SVOD industry ([Hurff, 2024](https://churnkey.co/blog/churn-rates-for-streaming-services/)).
    -   The primary aim of this project is to reduce consumer churn for a telecommunication company that offers a bundle package by identifying predictive churn behavior. Identifying predictive churn behavior allows us to get a better understanding of the main causes of consumer churn and target at-risk consumers who may churn. The target-industry of this project is the telecommunication industry, in which we analyze consumer behavior and churn rates based on a Telecom Churn Rate dataset. We believe that our approach and methodology can be translated and applicable to other industries that offer bundle packages, such as the media-consumer-technology industry (i.e., Disney+). We justify our secondary aim by identifying the similarities and overlap between the bundle packages offered in the Telecommunication industry and Disney+ bundle package (see Table 1).

| **Similarities Between Telecom and Disney+ Bundles** |             |             |
|------------------------------------------------------|-------------|-------------|
|                                                      | **Telecom** | **Disney+** |
| **Offer individual services**                        | ✓           | ✓           |
| **Offer bundle services**                            | ✓           | ✓           |
| **Products require high engineering power**          | ✓           | ✓           |
| **Churn is the prominent issue**                     | ✓           | ✓           |

-   **Business Activity Category**
    -   **Based on the Data Periodic Table**
    -   **Can be more than one**
    -   **Focus on one business area (sales, marketing, finance, accounting, HR, operations, IT, customer service, legal, etc.)**
    -   A06. Improved customer retention
    -   A10. Increased loyalty/customer satisfaction
    -   D04. Improved understanding of the impact of emerging customer behavior
    -   All of these focus in the customer service business area
-   **OKR (Objectives and Key Results)**
    -   **Objective / CRISP-DM's Business Objective / Data Periodic Table's Business Activity**
    -   **SMART Key Results / CRISP-DM's Business Success Criteria**
    -   Objective: Reduce the monthly churn rate
    -   Key results:
        -   Decrease the monthly churn rate from 27% to 17% (i.e., 10%) within 6 months (around 1.67% reduction per month)
    -   KPI:
        -   Reduce the number of monthly tech tickets by 20% within 6 months (around 3.33% reduction per month)
            -   Justification: This KPI is the most impactful and correlated metric related to consumer churn
        -   Achieve 80% recall score of the churn prediction model
            -   Justification: This KPI aims to successfully predict and identify churning consumers. By doing so, we’re able to take immediate actions toward the said customer and prevent them from churning.
        -   Achieve 75% F1-score of the churn prediction model
            -   Justification: This KPI aims to successfully predict and identify churning consumers. By doing so, we’re able to take immediate actions toward the said customer and prevent them from churning.
-   **OKR Initiatives**
    -   **List the project’s deliverables**
    -   Develop and implement descriptive and diagnostic analytics dashboards.
    -   Establish an automated data pipeline
    -   Create and refine a predictive model for churn

#### **Assess Situation**

-   **Inventory of Resources**
    -   **Personnel**
        -   List each member's name and their job title for the project (data analyst, data engineer, data scientist, etc.)
            -   Valentin: Product owner - business analyst
            -   Minh: Scrum Master - data scientist
            -   Kevin: Developer - data engineer
            -   Mason: Developer - data engineer
            -   Rachel: Developer - data engineer
    -   **Data**
        -   Telecom Company Churn Rate Dataset
    -   **Computing Resources**
        -   Cloud computing platforms
    -   **Software**
        -   Analytics tools, data processing softwares
            -   Excel
            -   Tableau
            -   Python
-   **Requirements, Assumptions, and Constraints**
    -   Data is accurate and complete
    -   Data is timely recorded
    -   We assume that churn rate does not solely depend on internal factors (e.g., improving customer experience) but that it is also impacted by the competitive landscape (e.g., competitor launches an innovative product or competitor launches low pricing campaigns).
    -   The Telecom Churn dataset is acquired legally through Kaggle.com
    -   The monthly churn rate is not provided in the Telecom Churn dataset and has to be calculated
-   **Risks and Contingencies**
    -   Data inaccuracy and loss
    -   External factors negatively impact consumer churn rates (e.g., competitor gains an unusual rate of market share in short-period of time)
-   **Terminology**
    -   OMTM: one metric that matters
    -   Our OMTM: monthly churn rate
    -   NRR: net recurring revenue
-   **Costs and Benefits**
    -   **Costs based on a typical hourly rate for each role identified under personnel and the expected hours required to complete the project**
        -   The total budget allocated to this project is \$6,000 and the expected completion time is 75 hours. See the breakdown of budget and time below.

| **Contractor Salary Breakdown**                     |                     |                                                |                |
|-----------------------------------------------------|---------------------|------------------------------------------------|----------------|
| Salary                                              | Data Analyst        | Data Engineer                                  | Data Scientist |
| \# of Employees                                     | 1                   | 3                                              | 1              |
| Hourly rate                                         | \$57                | \$72                                           | \$81           |
| Total hourly rate                                   | \$57                | \$216                                          | \$81           |
| Annual rate                                         | \$120,000           | \$150,000                                      | \$170,000      |
| Total annual rate                                   | \$120,000           | \$450,000                                      | \$170,000      |
|                                                     |                     |                                                |                |
| **Total Budget and Hours Allocated To The Project** |                     |                                                |                |
| Hours to complete the project                       | Total employee cost | Additional Comments                            |                |
| 75                                                  | \$37,170            | Each employee spends 105 hours on this project |                |

-   **Benefits based on the Data Periodic Table's Business Activity Categories. Try to quantify as best as you can, i.e. for labor hours saved. If you cannot quantify the benefit, still identify the benefit.**
    -   Costs:
    -   Benefits: Reduction in customer churn, improved customer retention, and better resource allocation.
    -   *In Telecom’s latest month, 27% of customers churned. As a result, they lost out on \$139,130.85. If 17% would have churned instead of 27% (i.e., 10% less), then Telecom would have earned an additional \$13,913.09 in revenue. Considering the effort along with the project budget being \$37,170, the additional \$13,913.09 might not look like an attractive gain. However, the \$13,913.09 gain only reflects one month. By reducing consumer churn by 10%, the additional annual revenue would result in \$166,957.02. Thus, the ROI of this project is estimated to be a 3.5X after one year of implementation.*

#### **Determine Data Mining Goals**

-   **Data Mining Goals aka Enabling Activities aka Data Activities**
    -   **Identify ALL relevant data activities from the Data Periodic Table**
    -   F02. Increased use of internal data
    -   F06. Improved quality of customer data
    -   F07. Increased use of structured data
    -   F11. Increased understanding and insight of customers
    -   F14. Improved use of historical dialogue customer data
    -   F15. Improved modeling accuracy
    -   F17. Improved use of data science models
    -   F19. Improved analytics tools
    -   F20. Real-time streaming data architecture
    -   F23. Improved use of machine learning
-   **Data Mining Success Criteria**
    -   Achieve a **specified** accuracy in churn prediction, and identify significant churn predictors.
    -   *Achieve 80% recall score and 75% F1-score in the churn prediction model*

#### **Produce Project Plan**

-   **Initial Assessment of Tools (Technology) and Techniques (Analytics)**
-   **Data Toolkit Items**
    -   Dashboards, machine learning, and reports.
-   **Project Plan**
    -   To keep the project on schedule, we will use the Scrum Agile project management framework.
    -   Work will be documented in [Trello](https://trello.com/b/4zCHAuvB/bsan-6080-02-project-disconnected-unveiling-patterns-in-telecom-churn)
