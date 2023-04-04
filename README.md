# Table of Contents

* [Problem Statement](#problem-statement)
* [Objective](#objective)
* [Data Analysis](#data-analysis)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

<!-- You can include any other section that is pertinent to your problem -->

## Problem Statement

Lending Club is a platform that facilitates personal loans for consumers by
matching borrowers seeking loans with
investors looking to lend money and earn a return. Its focus is on lending
different types of loans to customers in
urban areas. The company evaluates loan applications based on the applicant's
profile to make loan approval decisions.

As with other lending companies, providing loans to "risky" borrowers is the
primary cause of financial loss, or credit
loss. Credit loss is the amount of money that lenders lose when borrowers fail
to repay or abscond with the money
borrowed. In other words, defaulting borrowers are the ones who cause the most
significant losses to lenders. Borrowers
labeled as "charged-off" are considered defaulters in this case.

The main objective is to minimize credit loss for the company. Two potential
sources of credit loss are:

1. Applicants who are likely to repay the loan, which can generate profits for
   the company through interest rates.
   Rejecting such applicants can result in a loss of business.
2. Applicants who are unlikely to repay the loan and may potentially default.
   Approving the loan for such applicants may
   lead to a financial loss for the company.

## Objective

The aim of this case study is to identify the applicants who pose a risk for
defaulting on their loans, in order to reduce the number of such loans and
minimize credit loss. This will be achieved by performing exploratory data
analysis (EDA) on the given dataset. Essentially, the company seeks to determine
the key driver variables that strongly indicate loan default, so that this
information can be used for risk assessment and managing their portfolio.

## Data Analysis

This sections groups the various fields or variables available in the data set
into relevant groups to understand the
data in a better way.

### Default History - Variables that might depict a history of default (Red)

- acc_now_delinq - The number of accounts on which the borrower is now
  delinquent.
- chargeoff_within_12_mths - A charge-off or chargeoff is a declaration by a
  creditor that an amount of debt is unlikely
  to be collected.
- collection_recovery_fee - levied if you do not pay your EMIs, your account
  goes into default, and the bank/lender has
  to take any action against you.
- delinq_2yrs - The number of 30+ days past-due incidences of delinquency in the
  borrower's credit file for the past 2
  years
- delinq_amnt - The past-due amount owed for the accounts on which the borrower
  is now delinquent.

### Income - Variables related to income and cash flow

- avg_cur_bal - Average current balance of all accounts
- open to buy - The difference between the credit limit assigned to a cardholder
  account and the present balance on the
  account.
- bc_util - Ratio of total current balance to high credit/credit limit for all
  bankcard accounts.
- annual_inc - The self-reported annual income provided by the borrower during
  registration.
- annual_inc_joint - The combined self-reported annual income provided by the
  co-borrowers during registration
- dti - A ratio calculated using the borrower’s total monthly debt payments on
  the total debt obligations, excluding
  mortgage and the requested LC loan, divided by the borrower’s self-reported
  monthly income.
- dti_joint (Calculate This) - A ratio calculated using the co-borrowers' total
  monthly payments on the total debt
  obligations, excluding
  mortgages and the requested LC loan, divided by the co-borrowers' combined
  self-reported monthly income
- emp_length - Employment length in years. Possible values are between 0 and 10
  where 0 means less than one year and 10
  means ten or more years.
- home_ownership - The home ownership status provided by the borrower during
  registration. Our values are: RENT, OWN,
  MORTGAGE, OTHER.
- verification_status - Indicates if income was verified by LC, not verified, or
  if the income source was verified

### Existing Loans Performance - Variables related to Loan Application

- application_type - Indicates whether the loan is an individual application or
  a joint application with two
  co-borrowers
- grade - Loan grading is a classification system that involves assigning a
  quality score to a loan based on a
  borrower's credit history, quality of the collateral, and the likelihood of
  repayment of the principal and interest.
- sub_grade - LC assigned loan subgrade
- loan_status - Current status of the loan
- purpose - A category provided by the borrower for the loan request.
- inq_last_6mths - The number of inquiries in past 6 months (excluding auto and
  mortgage inquiries)
- open_acc - The number of open credit lines in the borrower's credit file.
- pub_rec - Number of derogatory public records
- pub_rec_bankruptcies - Number of public record bankruptcies
- total_acc - The total number of credit lines currently in the borrower's
  credit file
- out_prncp - Remaining outstanding principal for total amount funded
- total_pymnt - Payments received to date for total amount funded
- total_pymnt_inv - Payments received to date for portion of total amount funded
  by investors
- total_rec_prncp - Principal received to date
- total_rec_int - Interest received to date
- total_rec_late_fee - Late fees received to date
- last_pymnt_d - Last month payment was received
- last_pymnt_amnt - Last total payment amount received
- next_pymnt_d - Next scheduled payment date
- last_credit_pull_d - The most recent month LC pulled credit for this loan.
  Sometimes these inquiries are referred to
  as “credit pulls” because you or any financial institution is pulling
  information about you from the credit Bureaus
  Files (Experian, Equifax, TransUnion – these are the three major credit
  bureaus from which the creditor or lenders
  request for borrowers credit report).

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Technologies Used

- python - 3.9.13
- seaborn - 0.11.2
- pandas - 1.4.4
- numpy - 1.21.5
- matplotlib - 3.5.2
- markdown - 3.3.4

# Conclusions

- Borrowers who take loans for a term of 60 months are more likely to default.
- Borrowers with less than 1 year of employment have a higher risk on
  defaulting.
- Borrowers with a "Verified" loan status who take high loan amounts with a
  60-month tenure have a higher risk of defaulting.
- Borrowers who have "Rent" and "Mortgage" as their home_ownership have a
  higher probability of defaulting.
- Borrowers who take loans for the purpose of debt consolidation are at a
  higher risk of defaulting.
- Borrowers who take loans for the purpose of small business have a higher
  probability of defaulting.
- Borrowers with loan amount 15K and above is at the highest risk.
- Borrowers who receive interest rates between 15% and higher are more likely
  to default.
- Borrowers with lower grades, i.e., E,F,G, are at a higher risk of defaulting.
- Borrowers from NV (Nevada) have a high risk of Charge Offs.
- Borrowers having bankruptcy record are at high risk of Charge Offs
- Borrowers with pub_rec_bankruptcies count of 2 and higher have even higher
  Charge Off ratio
- Borrowers with income range of 0-40K have the highest risk of Charge Offs

## Contact

Created by [@manikbajaj](https://github.com/manikbajaj) - feel free to contact
me!

