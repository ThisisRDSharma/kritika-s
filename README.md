# kritika-s
Kirtika


The Trulioo eIDV process relies on a set of controls to ensure proper operation, secure execution, and accuracy in the verification process. While this is a rule-based system rather than a statistical or machine learning model, key usage controls are implemented to verify inputs, confirm execution, and validate outputs.

Key Usage Controls:
Verification of Inputs:

Inputs such as name, address, date of birth, and government-issued documents are verified for validity and completeness before being processed.
Control Measures:
Ensuring input formats align with specifications (e.g., names in text format, dates in YYYY-MM-DD).
Validating document fields against predefined formats for national IDs, passports, and driver's licenses.
Rejecting incomplete or improperly formatted inputs and flagging them for correction or manual review.
Confirmation of Successful Model Execution:

Each step of the rule-based process is monitored to ensure that the system executes without errors during identity verification.
Control Measures:
System Logs: Detailed logs are maintained to track the progress of each identity check, recording the steps taken and whether they were successfully executed.
API Response Monitoring: API calls made to Trulioo’s system during identity verification return status codes to confirm successful execution or indicate errors. Any anomalies trigger alerts for resolution.
Validation of Outputs:

The outputs of the eIDV process (e.g., Verified, Not Verified, or Attention) are validated to ensure they align with the predefined rules and criteria.
Control Measures:
Outputs are reviewed against the matching thresholds and business logic applied during verification.
Any mismatched or ambiguous results are flagged for manual review by compliance teams to ensure accuracy.
Error Handling and Escalation:

If errors occur during input verification or system execution, the process includes controls to handle these errors and escalate unresolved cases.
Control Measures:
Real-time error detection triggers notifications to system administrators.
Escalation procedures ensure flagged cases are reviewed promptly by the appropriate teams (e.g., BSA officers).
Audit Trails:

Comprehensive audit logs are maintained to document the entire verification process, from input validation to final output.
These logs support compliance audits, allowing businesses to verify that the system was used correctly and consistently.





