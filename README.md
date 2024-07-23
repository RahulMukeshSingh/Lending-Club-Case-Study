# Project Name : Lending Club Case Study

## Table of Contents

- [General Info](#general-information)
- [Objectives](#objectives)
- [Approach](#approach)
- [Technologies Used](#technologies-used)
- [Conclusions](#conclusions)
- [Team](#team)

## General Information

This project is a case study to use Exploratory Data Analysis (EDA) to understand how consumer attributes and loan attributes influence the tendency of default. The aim is to identify patterns that indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of the loan, or lending (to risky applicants) at a higher interest rate.

- Background: The company specializes in lending various types of loans to urban customers. When a loan application is received, the company must decide whether to approve the loan based on the applicant's profile. Approving a loan for an applicant likely to default leads to financial loss, while not approving a loan for an applicant likely to repay results in lost business opportunities.
- Business Problem: The project aims to mitigate financial losses by identifying high-risk loan applicants using historical loan data, thereby enhancing the company's loan approval process and risk assessment strategies.
- Dataset: The dataset contains historical information about past loan applicants, including whether they defaulted. Key variables include loan amount, interest rate, loan grade, employment length, annual income, debt-to-income ratio, and more.

## Objectives

The Goal is to use Exploratory Data Analysis (EDA) to understand how consumer attributes and loan attributes influence the tendency to default. The objective is to To analyze loan application data to identify patterns indicating whether an applicant is likely to default. The outcome of this analysis will provide the company with a better understanding of the factors influencing loan defaults, enabling more accurate and profitable lending decisions.

## Approach

- Data Understanding
- Data Handling & Cleaning
  - Identify columns with blank values which need to be imputed
  - Dropping Columns based on EDA and Domain Knowledge
  - Handling Incorrect Data Types
  - Handling Outliers
- Sanity Check
  - Analysis of the dataset post cleanup
- Analysis
  - Univariate Analysis
  - Segmented Analysis
  - Bivariate Analysis
  - Derived Metrics Analysis
- Conclusions Insigts
- Business Recommendations

## Technologies Used

- Python - 3.12.3
- Pandas - version 2.2.2
- Numpy - version 1.26.4
- Matplotlib - 3.7.1
- Seaborn - version 0.13.2

## Conclusions

- Loan Amount and Default Risk: Higher loan amounts are associated with an increased likelihood of default, especially loans exceeding $15000.
- Annual Income and Default Risk: Consumers in lower annual income groups are more likely to default on their loans.
- Income Ratio and Default Risk: A higher loan amount-to-income ratio significantly increases the likelihood of default.
- Installment Amount and Default Risk: Consumers with higher installment amounts as a percentage of their monthly income are more prone to default.
- Loan Term and Default Risk: Loans with shorter terms have a lower chance of being charged off, while loans with longer terms have a higher chance of defaulting.
- Credit History: Longer credit histories are associated with a higher likelihood of fully paying loans. Borrowers with more inquiries in the last 6 months are associated with a higher chance of defaulting.
- Interest Rates: Higher interest rates (above 10%) are linked to higher default rates.
- Debt-to-Income (DTI) Ratio: Higher DTI ratios are correlated with higher default rates. Lower DTI ratios are associated with a higher likelihood of fully paying the loan.

<!-- ## Acknowledgements

Give credit here.

- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com). -->

## Team

Created by:

- [Rahul Singh](https://github.com/RahulMukeshSingh)
- [Raja Kalavala](https://github.com/RajaKalavala)

<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
