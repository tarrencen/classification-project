### classification-project
This repository holds the work for my Codeup Data Science (Innis Cohort) ML Classification project.

The goal for this project is to build an ML model that will predict churn in the Telco telecommunication company's customer base. A report of this model's findings, including (but not limited to) recommendations to reduce churn,  will be presented to stakeholders in the company's business leadership.

Initial analytical explorations of the data indicates that a driver of churn may be dissatisfaction with either price or service among customers who used Telco's fiber internet service. 70% of customers who churned (1297 of 1869) were fiber internet subscribers. 52% of these churned customers streamed TV or movies. Another driver of churn may be associated with the paperless billing program; nearly 75% of customers who churned used paperless billing, yet only 12% had automatic billing.

# Data Dictionary:
'senior_citizen': whether or not the customer is a senior citizen (1-true, 0-false)

'tenure': time, in months, as customer

'internet_service_type_id': identifier for internet service type(1-DSL, 2-Fiber, 3-None)

'contract_type_id': identifier for contract type (1-month to month, 2-one year, 3-two year)

'payment_type_id': payment identifier (1-electronic check, 2-mailed check, 3-bank transfer[automatic], 4-credit card[automatic]) 

'monthly_charges': amount in USD

'total_charges': total paid during time as customer, in USD

'gender_Male': gender (1-male, 0-female)

'partner_Yes': whether customer has a significant other (1-true, 0-false)

'dependents_Yes': whether customer has dependents (1-true, 0-false)

'phone_service_Yes': (1-true, 0-false)

'multiple_lines_No phone service: (1-true, 0-false)

'multiple_lines_Yes': (1-true, 0-false)

'online_security_No internet service': (1-true, 0-false)

'online_security_Yes': (1-true, 0-false)

'online_backup_No internet service': (1-true, 0-false)

'online_backup_Yes': (1-true, 0-false)

'device_protection_No internet service': (1-true, 0-false)

'device_protection_Yes': (1-true, 0-false)

'tech_support_No internet service': (1-true, 0-false)

'tech_support_Yes': (1-true, 0-false)

'streaming_tv_No internet service'(1-true, 0-false)

'streaming_tv_Yes': (1-true, 0-false)

'streaming_movies_No internet service': (1-true, 0-false)

'streaming_movies_Yes': (1-true, 0-false)

'paperless_billing_Yes': (1-true, 0-false)

'contract_type_One year': (1-true, 0-false)

'contract_type_Two year: (1-true, 0-false)

'payment_type_Credit card (automatic)': (1-true, 0-false)

'payment_type_Electronic check': (1-true, 0-false)

'payment_type_Mailed check': (1-true, 0-false)

'internet_service_type_Fiber optic': (1-true, 0-false)

'internet_service_type_None': (1-true, 0-false)

### Planning:
- Data is to be acquired via pandas-read SQL query from acquire.py module, cleaned and prepped with prep.py for analysis and modeling.
- Data will then be explored and analyzed to identify possible drivers of churn, with accompanying visualizations
- Findings from exploration will be taken into consideration during construction and training of ML models
- Once models are built, they will be validated and tested. Evaluation of models to be conducted at each stage.
- Predictions and prediction probabilities from highest scoring models are to be exported to .csv files.

### Conclusions:
Customers who used fiber optic internet and paperless billing were found to be the most likely to churn. Recommendations are to promote automated billing solutions for the customer who used paperless billing and to ensure, to the extent possible, that fiber optic internet service is reliable, with promised bandwidth and upload/download speed at least on par with competitors. 
