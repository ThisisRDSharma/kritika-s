# kritika-s
Kirtika


Reduced Accuracy:
Limited consortium data or data sources may result in a narrow view of fraud patterns, reducing the model's ability to generalize effectively to emerging or rare fraud schemes.

Overfitting to Local Data:
The model may overly rely on institution-specific data, making it less effective in detecting global or novel fraud trend

Remediation:
Strengthen the feedback loop with Falcon to continuously improve fraud pattern detection by incorporating its global fraud insights.



Applicability Risk:

The model may underperform or produce inaccurate results if applied to data outside its training scope (e.g., new geographies, product types, or transaction types).
Portfolio Drift Risk:

Changes in portfolio characteristics (e.g., shift in customer demographics, transaction patterns) may lead to reduced model accuracy and higher false positives or negatives.

rEMEDIATION:
Regularly review the population characteristics (product types, geographies, and transaction types) to ensure alignment with the training data.
Implement a portfolio drift monitoring framework to track changes in customer demographics, transaction behaviors, and other key features over time.
