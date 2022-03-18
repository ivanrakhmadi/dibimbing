# Exploratory Data Analysis - Telco Customer Churn
## Case Summary

Objective Statement:
- Get business insight about how many customer churn.
- Get business insight about potential factors that can make customer churn.


Challenges:
- Large size of data, can not maintain by excel spreadsheet.

Methodology / Analytic Technique:
- Univariate analysis
- Multivariate analysis
 
 Business Benefit:
- Helping company  to analyze all relevant customer data and develop focused customer retention programs

Expected Outcome:
- Know how many how many customer churn.
- Know what  potential factors that can make customer churn.


## Business Understanding
Churn is the percentage of customers that stopped using your company's product or service during a certain time frame. This case has some business question using the data:
- How many how many customer churn ?
- What potential factors that can make customer churn ?

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
How many how many customer churn ?

![Screenshot (10)](https://user-images.githubusercontent.com/101379389/158145637-8853412b-baf9-4089-9bc7-518fd77c78e0.png)

- According from data above, the customer churn is below 2000 customer from total 7043 customer which is good because company didn't lose much customer. For the next step company will know what steps to do to keep customers to use their services.

What is the potential factors that can make customer churn ?

- We try to add 'gender' as a potential factor for customer churn

![Screenshot (11)](https://user-images.githubusercontent.com/101379389/158149389-a8fcc122-5766-400f-b932-30ea21d5b1cc.png)

- The result from data above shows male and female customers that churn have same result while the male customer that didn't churn have slightly more amount than the female customer that didn't churn


- For the second try, we try to compare some categories to see if there any correlation between one to another (correlation heatmap)
![Screenshot (13)](https://user-images.githubusercontent.com/101379389/158218777-14a614b1-c82f-414a-89e0-130fe5b212f0.png)

- Based on result above, we can see that 'TotalCharges' and 'tenure' are highly correlated each other

- Last, we are using pairplot  to look the correlation between the categories

![Screenshot (15)](https://user-images.githubusercontent.com/101379389/158223557-33e0aa18-52bb-4996-8318-3fc9d844e7f8.png)

- The results from using pairplot are :
- Customer who belong to SeniorCitizen did not churn
- Customer with higher tenure tend to more loyal (did not churn)
- Customer that did not Churn have more MonthlyCharges
- Customer that did not Churn have more TotalCharges



