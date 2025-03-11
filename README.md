1️⃣ Load Rules – Retrieves fraud detection rules, including overdraft limits, customer-tier restrictions, and wire transfer rules.
2️⃣ Execute Rules – Runs the transaction against these rules using Cosmos DB.
3️⃣ Calculate Risk Score – Assigns a risk score based on fraud patterns; transactions exceeding the threshold are flagged.
4️⃣ Determine Action – Aggregates risk scores to decide whether to approve, flag, or recommend further review.

This process ensures efficient fraud detection by leveraging rule-based assessments and risk scoring.
