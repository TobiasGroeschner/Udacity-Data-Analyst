# Udacity data analyst Project-5: ProsperLoan Data Exploration

## Table of Contents
 * [Necessary packages](#necessary-packages)
 * [Project Motivation](#project-motivation)
 * [File Description](#file-description)
 * [How to Interact With Project](#how-to-interact-with-project)
 * [Conclusion](#conclusion)

## Necessary packages:

- numpy
- pandas
- matplotlib
- seaborn


## Project Motivation

The project motivation is to explore meaningful variables of the dataset.

The jupyter notebook performs:

- basic data exploration
- univariate exploration
- bivariate exploration

## File description

- Explanatory_visualization_Slide_Deck.html
- Explanatory_visualization_Slide_Deck.ipynb
- Explanatory_visualization.ipynb
- Explanatory_visualization.html
- [prosperLoanData.csv](https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv&sa=D&ust=1547699802003000)]
    - The columns are explained in the [data dictionary](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit?usp=sharing) 

## How to Interact With Project

Just clone the project and play around with the Notebook.

`git clone https://github.com/TobiasGroeschner/Udacity-Data-Analyst.git`

## Conclusion

* **EmploymentStatus:** majority of people work full time
* **IncomeRange:** 31% of people earn $50000-74999 dollars
* **ProsperScore:** normal distribution
* **StatedMonthlyIncome:**: Monthly Income is right skewed: very few people be have a higher salary. Majority of the borrowers are having a salary with less than 10000 USD and, peak is observed at 5000 USD
* **LoanOriginalAmount:** Right skewed with multiple peaks observed around 4000 USD, 10000 USD and 17000 USD.
* **Investors:** Majority of the investors are between 0 and 100

Columns which have a positive correlation are for example:

- **Borrower APR** (annual percentage rate) & **Borrower Rate** have a positve correlation
- **Borrower APR** & EstimatedEffectedYield have a positive correlation

Columns which have a negative correlation are for example:

**Borrower APR** and **ProsperRating_Numeric**


## Key Insights for Presentation

For the presentation, I focused mainly on features that are impactful for approval of loan status.
The major insights obtained is: **The loan approval status is heavily dependent on the applicant's information on Income Range, Homeowner status and employment status.**
