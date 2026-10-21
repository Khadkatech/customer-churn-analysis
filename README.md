# Customer Churn Analysis: Telecom Retention Case Study

## Business scenario
A telecom provider is losing a significant share of its customers, and the retention team has no clear view of who leaves or why. This project plays the role of a data analyst asked to answer three questions:

1. How big is the churn problem?
2. Which customers are most at risk?
3. What should the business do about it?

*The scenario is simulated. The analysis uses a public sample dataset, not data from a real company.*

## Dataset
- Public Telco customer churn sample dataset (Kaggle / IBM sample data)
- 7,043 customers, 50 variables covering contract type, monthly charges, satisfaction score, churn status and churn reason

## Approach
1. **Cleaned the data:** converted Total Charges to numeric, removed rows with missing values, and created a binary churn variable from the Churn Label column
2. **Measured overall churn** and compared churn rates across customer segments
3. **Visualised** churn by contract type, monthly charge, satisfaction score and churn category
4. **Translated the findings** into recommendations for the retention team

## Key findings

| Area | Finding |
|---|---|
| Overall churn | 26.5% of customers churned (1,869 of 7,043) |
| Contract type | Month-to-month churn is 45.8%, versus 10.7% for one-year and 2.5% for two-year contracts |
| Pricing | Churned customers paid a higher median monthly charge (79.65) than retained customers (64.43) |
| Satisfaction | All customers with a score of 1 or 2 churned; churn was 16.1% at score 3 and 0% at scores 4 and 5 |
| Reasons for leaving | Competitor (841, about 45%), Attitude (314), Dissatisfaction (303), Price (211), Other (200) |

## Recommendations
1. **Move month-to-month customers onto longer contracts.** This segment has by far the highest churn, so discounts or perks for switching to one- or two-year plans target the biggest risk.
2. **Trigger proactive outreach for low satisfaction scores.** Customers scoring 1 or 2 are very likely to leave, so a call, fix or retention offer should follow quickly.
3. **Review competitiveness for higher-paying customers.** Competitors are the top reason for leaving and churners pay more per month, so matched offers or bundles are worth testing.

## Limitations
- The satisfaction score may have been recorded after a customer decided to leave, so it shows a strong association, not proven cause.
- The analysis is descriptive. It shows where churn is highest but does not prove that the recommended actions would reduce it; an A/B test on a retention offer would be the next step.
- No predictive model has been built yet.

## Next steps
- Build a churn prediction model, excluding variables that leak the outcome (Churn Score, Customer Status, Churn Reason, Churn Category)
- Estimate the revenue at risk using CLTV and Total Revenue
- Build a dashboard for the retention team

## Tools
Python, pandas, matplotlib, seaborn, Google Colab

## Author
Bijay Khadka, MRes AI in Business | [LinkedIn] (https://www.linkedin.com/in/bijaykhadka-ai)
