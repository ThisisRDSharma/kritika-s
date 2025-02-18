FICO employs a systematic approach to assess the sensitivity of model performance to variations in input data, as specified in the data specifications document. These analyses are conducted internally and shared with the model implementation team to ensure model robustness and reliability.

One key component of this process is the Blackout Analysis, which involves a structured evaluation of model performance across varying levels of data quality. Fields are tested individually by systematically blanking out values for different percentages of observations. By analyzing the degradation in model performance at each level of missing data, FICO identifies the fields that have the most significant impact on performance.

In addition to blackout analysis, FICO evaluates performance impacts resulting from invalid or inconsistent field values. This ensures the model is resilient to data discrepancies and continues to operate effectively under diverse conditions.

The results of these tests are measured using key performance indicators such as TDR (True Detection Rate), ADR (Alert Detection Rate), and RTVDR (Real-Time Verified Detection Rate). FICO has analyzed the performance impact when certain critical fields are randomly blanked out, providing insights into the expected model behavior under suboptimal data conditions.

Through these testing practices, FICO supports clients in maintaining high data quality standards, ensuring that the model remains reliable, interpretable, and well-aligned with the client's portfolio characteristics.
