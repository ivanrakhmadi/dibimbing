# Telco Customer Churn
## Case Summary

Objective Statement:
- Get business insight about how many customer churn.
- Get business insight about factors that can make customer churn.
- To predict behavior to retain customers

Challenges:
- Large size of data, can not maintain by excel spreadsheet.

Methodology / Analytic Technique:
- Descriptive analysis
- Graph Analysis
 
 Business Benefit:
- Helping company  to analyze all relevant customer data and develop focused customer retention programs

Expected Outcome:
- Know how many how many customer churn.
- Know what factors that can make customer churn
- Customer analysis.

## Business Understanding
Churn is the percentage of customers that stopped using your company's product or service during a certain time frame. This case has some business question using the data:
- How many how many customer churn ?
- What factors that can make customer churn ?
- How about customer analysis ?

## Data Understanding
The Telco customer churn data contains information about a fictional telco company that provided home phone and Internet services to 7043 customers in California in Q3. It indicates which customers have left, stayed, or signed up for their service.
- Source data : https://www.kaggle.com/blastchar/telco-customer-churn

Data Dictionary
- Customer ID 
- Gender : Whether the customer is a male or a female
- SeniorCitizen : Whether the customer is a senior citizen or not (1, 0)
- Partner : Whether the customer has a partner or not (Yes, No)
- Dependents : Whether the customer has dependents or not (Yes, No)
- Tenure : Number of months the customer has stayed with the company
- PhoneService : Whether the customer has a phone service or not (Yes, No)
- MultipleLines : Whether the customer has multiple lines or not (Yes, No, No phone service)
- InternetService : Customer’s internet service provider (DSL, Fiber optic, No)
- OnlineSecurity : Whether the customer has online security or not (Yes, No, No internet service
- OnlineBackup : Whether the customer has online backup or not (Yes, No, No internet service)
- DeviceProtection : Whether the customer has device protection or not (Yes, No, No internet service)
- TechSupport : Whether the customer has tech support or not (Yes, No, No internet service)
- StreamingTV : Whether the customer has streaming TV or not (Yes, No, No internet service)
- StreamingMovies : Whether the customer has streaming movies or not (Yes, No, No internet service)
- Contract : The contract term of the customer (Month-to-month, One year, Two year)
- PaperlessBilling : Whether the customer has paperless billing or not (Yes, No)
- PaymentMethod : The customer’s payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))
- MonthlyCharges : The amount charged to the customer monthly
- TotalCharges : The total amount charged to the customer
- Churn : Whether the customer churned or not (Yes or No)\

## Data Preparation
- Code Used:
- Python Version: 3.7.12
- Packages: Pandas, Numpy, Matplotlib, and Seaborn

## Data Cleansing
- There are no missing value in this data
- The 'TotalCharge' value is still object, we need to change it to float first

## Exploratory Data Analysis
