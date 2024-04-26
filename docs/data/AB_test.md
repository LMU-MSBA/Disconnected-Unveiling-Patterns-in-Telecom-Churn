## **The A/B Tests for Sprint 2**
 
**Metrics:** Monthly consumer churn rate

**Hypotheses**
Based on data, we assume that reducing technical support tickets will lead to fewer customer churn. We further assume that educating our customers with a 4-minute educational video will lead to fewer technical support tickets. These assumptions led us to our null and alternative hypothesis.

**H0:** Subscribers that viewed the video will not exhibit a significant difference in monthly churn rate compared to subscribers that did not view the video.

**HA:** Subscribers that viewed the video will exhibit a significant difference in monthly churn rate compared to subscribers that did not view the video.

![pic1](https://github.com/LMU-MSBA/Disconnected-Unveiling-Patterns-in-Telecom-Churn/assets/144483962/a542d4fb-3d42-4496-a402-194b9f8754bc)

**Experimental Design**
The company has 7,043 customers. We do not want to A/B test with all of our customers as our A/B test could back fire, which could result in many customers churning. Therefore, we will segment the control and experimental group into a sample size that we deem (1) appropriate in regards to risk and (2) large enough in regards to statistical power.
3,168 customers are on an annual or bi-annual payment contract whereas 3,875 of our customers are on a month-to-month contract. We decided to only segment our experimental and control group with customers who are on a month-to-month. Moreover, to reduce the risk of loosing consumers due to our A/B test backfiring, we further segmented the month-to-month contractors by only including 930 (24%) of our total month-to-month contractors. Lastly, we split our 930 month-to-month contractors in half and funneled them into a control and experimental group.

![pic2](https://github.com/LMU-MSBA/Disconnected-Unveiling-Patterns-in-Telecom-Churn/assets/144483962/51e75516-42a6-47a5-aad2-eaaba7aaf5c1)

The randomization process consists of: (1) randomly assigning all of our month-to-month contractors a unique number between 1 and 3,875 in our CRM system; (2) sort our month-to-month contractors based on the randomly generated number in an ascending order; (3) selecting the first 465 customers as our control group and the consecutive 465 customers as our experimental group; (4) discard the remaining customers for this A/B test.
The experiment will last for 2 months. The description of the control and experimental groups can be viewed under table 2.

![pic3](https://github.com/LMU-MSBA/Disconnected-Unveiling-Patterns-in-Telecom-Churn/assets/144483962/9a0821fe-382e-4437-bcf4-a13d0f1b7974)

**Implementation Plan**
We plan to educate our users in the experimental group with a 4-minute educational video that explains (1) the most frequently asked technical questions and (2) how to avoid potential technical problems. Thus, our implementation plan is in the following order:
* Hire an ad agency to produce a high quality 4-minute video. This will cost around $28,000.
* Generate a new list inside of our CRM that tags all members in our experimental and control group (see example below).
  
![pic4](https://github.com/LMU-MSBA/Disconnected-Unveiling-Patterns-in-Telecom-Churn/assets/144483962/30b282fb-753e-45df-a313-39c2b9c142b2)

* Set up a 2-week email cadence. The initial email will send the educational video to members in the experimental group. If the customer does not open the email, or click the video, then the email cadence will automatically follow-up with them every 2 days.
* Track and compare the (1) number of monthly support tickets from the experimental and control group along with their (2) churn rate.

**Data Collection and Analysis**
The members in our experimental and control group are tracked in our CRM and backend. As a result, we are capable of tracking and comparing the (1) number of monthly support tickets from the experimental and control group along with their (2) churn rate. We can visualize the results using dashboards. Moreover, we will apply a t-test to identify whether there is statistically significant different between the two groups.

![pic5](https://github.com/LMU-MSBA/Disconnected-Unveiling-Patterns-in-Telecom-Churn/assets/144483962/9a3b2bbc-13c6-44aa-8fb6-34d4988a0cbd)
