# ProsperLoan Data Exploration

## Dataset

This [data set](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1547699802003000)
contains 113,937 loans with 81 variables on each loan, including loan amount,
borrower rate (or interest rate), current loan status, borrower income, and many others.
This [data dictionary](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit?usp=sharing) explains the
variables in the data set.
The project objective is not expected to explore all of the variables in the dataset but focus on a few meaningful.

## Summary of Findings


# Conclusions

* **EmploymentStatus** majority of people work full time
* **IncomeRange**: 31% of people earn $50000-74999 dollars
* **ProsperScore**: normal distribution

* **StatedMonthlyIncome:**
 Monthly Income is right skewed: very few people be have a higher salary. Majority of the borrowers are having a salary with less than 10000 USD and, peak is observed at 5000 USD

* **LoanOriginalAmount:** Right skewed with multiple peaks observed around 4000 USD, 10000 USD and 17000 USD.

* **Investors:** Majority of the investors are between 0 and 100

Columns which have a positive correlation are for example:

- Borrower APR (annual percentage rate) & Borrower Rate have a positve correlation
- Borrower APR & EstimatedEffectedYield have a positive correlation


Borrower APR and ProsperRating_Numeric have a negative correlation. Borrower APR & ListCategory Numeric do not seem to correlate.


## Key Insights for Presentation

For the presentation, I focused mainly on features that are impactful for approval of loan status
I performed univariate, bivariate and
multivariate analysis on the selected variables.

The major insights obtained is :


The loan approval status is heavily dependent on the applicant's information on Income Range, Homeowner status and employment status.
