# Project Name

This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of
medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface.

If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount
of credit loss. Identification of such applicants using EDA is the aim of this case study.

In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the
variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk
assessment.

## Table of Contents

* [General Info](#general-information)
* [Data Analysis](#data-analysis)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

- Provide general information about your project here.
- What is the background of your project?
- What is the business probem that your project is trying to solve?
- What is the dataset that is being used?

## Data Analysis

This sections groups the various fields or variables available in the data set into relevant groups to understand the
data in a better way.

### Default History - Variables that might depict a history of default (Red)

- acc_now_delinq - The number of accounts on which the borrower is now delinquent.
- chargeoff_within_12_mths - A charge-off or chargeoff is a declaration by a creditor that an amount of debt is unlikely
  to be collected.
- collection_recovery_fee - levied if you do not pay your EMIs, your account goes into default, and the bank/lender has
  to take any action against you.
- delinq_2yrs - The number of 30+ days past-due incidences of delinquency in the borrower's credit file for the past 2
  years
- delinq_amnt - The past-due amount owed for the accounts on which the borrower is now delinquent.

### Income - Variables related to income and cash flow

- avg_cur_bal - Average current balance of all accounts
- open to buy - The difference between the credit limit assigned to a cardholder account and the present balance on the
  account.
- bc_util - Ratio of total current balance to high credit/credit limit for all bankcard accounts.
- annual_inc - The self-reported annual income provided by the borrower during registration.
- annual_inc_joint - The combined self-reported annual income provided by the co-borrowers during registration
- dti - A ratio calculated using the borrower’s total monthly debt payments on the total debt obligations, excluding
  mortgage and the requested LC loan, divided by the borrower’s self-reported monthly income.
- dti_joint (Calculate This) - A ratio calculated using the co-borrowers' total monthly payments on the total debt
  obligations, excluding
  mortgages and the requested LC loan, divided by the co-borrowers' combined self-reported monthly income
- emp_length - Employment length in years. Possible values are between 0 and 10 where 0 means less than one year and 10
  means ten or more years.
- home_ownership - The home ownership status provided by the borrower during registration. Our values are: RENT, OWN,
  MORTGAGE, OTHER.
- verification_status - Indicates if income was verified by LC, not verified, or if the income source was verified

### Existing Loans Performance - Variables related to Loan Application

- application_type - Indicates whether the loan is an individual application or a joint application with two
  co-borrowers
- grade - Loan grading is a classification system that involves assigning a quality score to a loan based on a
  borrower's credit history, quality of the collateral, and the likelihood of repayment of the principal and interest.
- sub_grade - LC assigned loan subgrade
- loan_status - Current status of the loan
- purpose - A category provided by the borrower for the loan request.
- inq_last_6mths - The number of inquiries in past 6 months (excluding auto and mortgage inquiries)
- open_acc - The number of open credit lines in the borrower's credit file.
- pub_rec - Number of derogatory public records
- pub_rec_bankruptcies - Number of public record bankruptcies
- total_acc - The total number of credit lines currently in the borrower's credit file
- out_prncp - Remaining outstanding principal for total amount funded
- total_pymnt - Payments received to date for total amount funded
- total_pymnt_inv - Payments received to date for portion of total amount funded by investors
- total_rec_prncp - Principal received to date
- total_rec_int - Interest received to date
- total_rec_late_fee - Late fees received to date
- last_pymnt_d - Last month payment was received
- last_pymnt_amnt - Last total payment amount received
- next_pymnt_d - Next scheduled payment date
- last_credit_pull_d - The most recent month LC pulled credit for this loan. Sometimes these inquiries are referred to
  as “credit pulls” because you or any financial institution is pulling information about you from the credit Bureaus
  Files (Experian, Equifax, TransUnion – these are the three major credit bureaus from which the creditor or lenders
  request for borrowers credit report).

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Technologies Used

- library - version 1.0
- library - version 2.0
- library - version 3.0

## Acknowledgements

Give credit here.

- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).

## Contact

Created by [@githubusername] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->