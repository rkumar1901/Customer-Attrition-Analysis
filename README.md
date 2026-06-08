# Customer-Attrition-Analysis
Here's a concise description of the **Attrition Analysis** project:

This is a **research project** focused on predicting customer churn in the **telecom industry**, with the goal of helping businesses retain customers by identifying *who* is at risk and *when* to intervene.

### Problem
Rather than just predicting whether a customer will leave, the project goes further by predicting the **timing** of churn — giving businesses a window to act before losing a customer.

### Dataset
5,000 customer records from an Iranian Telecom Company (sourced from the UC Irvine repository), with 21 attributes covering call usage, charges, and service plans across day, evening, night, and international calls.

### Approach
The model combines two techniques in a novel pipeline:
- **XGBoost** (ensemble boosting) for predictive power
- **Cox Proportional Hazards model** (survival analysis) to estimate churn risk over time for each individual customer

### Key Results
The best-performing model used **Recursive Feature Elimination (RFE)** for feature selection, achieving a **Concordance Index of 0.76** and a **Brier Score of 0.23** — both strong scores. As a bonus, the model doubles as a binary classifier with **93% accuracy** and an impressive **AUC of 0.98**.

### Additional Outputs
- **Customer segmentation** via K-Means clustering based on risk scores
- **Churn timing insight**: risk is highest between days 80–102 of a customer's tenure
- A deployable Python pipeline ready for cloud integration

### Business Impact
The project enables targeted retention strategies, cost savings on acquisition, upsell/cross-sell opportunities, and overall improvement in brand loyalty and revenue.
