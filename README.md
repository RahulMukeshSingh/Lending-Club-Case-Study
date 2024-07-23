# Project Name : Lending Club Case Study

## Table of Contents

- [General Info](#general-information)
- [Objectives](#objectives)
- [Approach](#approach)
- [Technologies Used](#technologies-used)
- [Key Conclusions](#key-conclusions-summary)
- [Next Business Steps](#next-business-steps)
- [Acknowledgements](#acknowledgements)
- [Team](#team)

## General Information

This project is a case study to use Exploratory Data Analysis (EDA) to understand how consumer attributes and loan attributes influence the tendency of default. The aim is to identify patterns that indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of the loan, or lending (to risky applicants) at a higher interest rate.

- **Background**: The company specializes in lending various types of loans to urban customers. When a loan application is received, the company must decide whether to approve the loan based on the applicant's profile. Approving a loan for an applicant likely to default leads to financial loss, while not approving a loan for an applicant likely to repay results in lost business opportunities.
- **Business Problem**: The project aims to mitigate financial losses by identifying high-risk loan applicants using historical loan data, thereby enhancing the company's loan approval process and risk assessment strategies.
- **Dataset**: The dataset contains historical information about past loan applicants, including whether they defaulted. Key variables include loan amount, interest rate, loan grade, employment length, annual income, debt-to-income ratio, and more.

## Objectives

The Goal is to use Exploratory Data Analysis (EDA) to understand how consumer attributes and loan attributes influence the tendency to default. The objective is to To analyze loan application data to identify patterns indicating whether an applicant is likely to default. The outcome of this analysis will provide the company with a better understanding of the factors influencing loan defaults, enabling more accurate and profitable lending decisions.

## Approach

* Data Understanding
* Initial Steps
    * Import Required Libraries and Configure Default Settings
    * Read the dataset
* Data Cleaning and Manipulation
    * Analyse empty values in each column
    * Remove completely empty columns
    * Check for single valued columns
    * Analyse remaining columns
    * Remove general information columns
    * Remove post-approval columns not useful for pre-approval risk assessment
    * Removing ongoing loans
    * Taking care of remaining columns with empty values
        * The number of months since the last public record and borrower's last delinquency
        * Employment length
        * Number of public record bankruptcies
        * Revolving line utilization rate
    * Handling Incorrect Data Types 
        * Checking Data Types
        * Term (Convert to Numerical)
        * Interest rate (Convert to Numerical)
        * Employment Length (Convert to Numerical)
        * Revolving line utilization rate (Convert to Numerical)
        * Loan issue date (Convert to Date)
        * Earliest reported credit line (Convert to Date)
    * Check and remove any duplicate rows
    * Outlier Handling
        * Finding outlier columns
        * Finding outlier threshold
        * Remove outliers above threshold
        * Check distribution after removing outliers
    * Sanity Checks
        * Range Check for Numerical and Date Columns
        * Earliest Credit Line Date Cannot Be More Than Issue Date
        * Loan Amount matches the calculation of Term, Installment and Interest Rate
        * Any columns with string value as NaN, None or Null
    * Shape of dataframe after data cleaning and manipulation
* Analysis
    * Derived Metrics
        * Annual Income (Data-driven Derived Metrics)
        * Loan Issue Date (Type driven Derived Metrics)
        * Earliest credit line (Business driven Derived Metrics)
        * Loan Amount (Data and Business driven Derived Metrics) 
        * Installments (Business driven Derived Metrics)
        * DTI (Data driven Derived Metrics) 
        * Revolving utilization rate (Data driven Derived Metrics)
* Analysis of Target Variable
* Visual Analysis (Univariate, Segmented Univariate, Bivariate, Multivariate Analysis)
    * Common Functions for plotting
    * Correlation between each numerical variable against Loan Status (Target Variable)
    * Loan Amount
    * Annual Income
    * Loan Amount to Income Ratio
    * Installment
    * Monthly Installment as percent of Income
    * Installment to loan ratio
    * DTI
    * Term
    * Revolving Utilization
    * Interest Rate
    * Issue Date
    * Earliest Credit Line
    * Grade and Sub Grade
    * Verification Status
    * Purpose
    * Employment Length
    * Home Ownership
    * State (Address)
    * Remaining columns/variables:
        * Inquiries in the last 6 months (inq_last_6mths)
        * The number of open accounts (open_acc)
        * Revolving Balance (revol_bal)
        * The total number of credit line accounts (total_acc)
        * Number of 30+ days past-due incidences for the past 2 years (delinq_2yrs)
        * Number of derogatory public records (pub_rec)
        * Number of public record bankruptcies (pub_rec_bankruptcies)
* Summary of Key Conclusions
* Next Business Steps

## Technologies Used

- Python - version 3.12.3
- Pandas - version 2.2.2
- Numpy - version 1.26.4
- Matplotlib - version 3.7.1
- Seaborn - version 0.13.2

## Key Conclusions Summary

- **Loan Amount and Default Risk:** Higher loan amounts are associated with an increased likelihood of default, especially loans exceeding $15000.
- **Annual Income and Default Risk:** Consumers in lower annual income groups are more likely to default on their loans.
- **Income Ratio and Default Risk:** A higher loan amount-to-income ratio significantly increases the likelihood of default.
- **Installment Amount and Default Risk:** Consumers with higher installment amounts as a percentage of their monthly income are more prone to default.
- **Loan Term and Default Risk:** Loans with shorter terms have a lower chance of being charged off, while loans with longer terms have a higher chance of defaulting.
- **Credit History:** Longer credit histories are associated with a higher likelihood of fully paying loans. Borrowers with more inquiries in the last 6 months are associated with a higher chance of defaulting.
- **Interest Rates:** Higher interest rates (above 10%) are linked to higher default rates.
- **Debt-to-Income (DTI) Ratio:** Higher DTI ratios are correlated with higher default rates. Lower DTI ratios are associated with a higher likelihood of fully paying the loan.
- **Public Record**: Consumers with no public records have better repayment history.

## Next Business Steps

- Consider capping loan amounts for borrowers with lower incomes to reduce the risk of default.
- Set higher interest rates or stricter approval criteria for high risk borrowers (e.g., those with high revolving utilization and low incomes)
- Focus marketing efforts on low-risk borrower segments (high income, low DTI, good credit history).
- Develop more robust credit scoring models that account for employment length, credit history length, and loan purpose.
- Be cautious with loans for high-risk purposes (e.g., debt consolidation, renewable energy) and implement additional checks.


## Acknowledgements

- This project was inspired by IIITB and Upgrad's Lecture on EDA
- References:
  - [Seaborn Documentation](https://seaborn.pydata.org/)

## Team

- [Rahul Singh](https://github.com/RahulMukeshSingh)
- [Raja Kalavala](https://github.com/RajaKalavala)
