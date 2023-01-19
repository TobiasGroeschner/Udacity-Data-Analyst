# Udacity data analyst Project-3: Analyze A/B Test Results

## Table of Contents
 * [Necessary packages](#necessary-packages)
 * [Project Motivation](#project-motivation)
 * [File Description](#file-description)
 * [How to Interact With Project](#how-to-interact-with-project)
 * [Conclusion](#conclusion)
  *  * [Part I-Probability](#part-i-probability)


## Necessary packages

- pandas
- numpy
- random
- matplotlib

## Project Motivation

This project is analysing the results of an A/B test run by an e-commerce website. The goal of this project is to decide if the company should implement the new internet site or keep the old one.

This project covered three parts:

- Part I - Probability(#Part-I---Probability)
- Part II - A/B Test
- Part III - Regression

## File Description

Analyze_ab_test_results_notebook.ipynb: Jupyter notebook with all the analysis
Analyze_ab_test_results_notebook.html: the Jupyter notebook as an .html file
countries.csv: tells us where the users are from
ab_data.csv: data of the control and treatment group

## How to interact with this project

Just clone the project and play around with the Notebook.

`git clone https://github.com/TobiasGroeschner/Udacity-Data-Analyst.git`

## Conclusion:

### Part I-Probability

The proportion of users converted no matter on what page they landed (control vs treatment) was 0.1196.
If we calculate these values for both groups indivually, the conversion rate of the control group is 0.1204. The converstion rate of the treatment group is 0.1188. 
Here, you can already see that the difference is negleccatable (0.0016). First indication that it does not make sense to not implement the new site.

### Part II - A/B Test

In Part II, we performed sampling distribution for the difference in converted individuals between the two pages. We did that for 10.000 iterations,

$n_{new}$ = 145310

$n_{old}$ = 145274

p = 0.11959708724499628

This resulted in a new_page converted ($p_{new}$) = 0.12057669809373064 and old_page_converted ($p_{old}$) = 0.12057669809373064. The difference between these two is 0.0012022745905573284. 
When we simulate  this calulation 10.000 times and  analyze the proportion of p_diffs that are greater then what we actually obsered, the proportion is tiny. Namely = -0.0015782389853555567. Again, it strongly suggests that the new page shall not be implemented.

### Part III - Regression

In Part III, we saw see that the result we achieved in the previous A/B test can also be acheived by performing regression. We first analysed if the landing page had any influence on the conversion rate. The P>|z| from the column ab_page (dummy column of landing page) turned out to be 0.190. Values ≥ 0.1 indicating insufficient evidence for rejectinig the $H_{0}$.

Then, we added country-information to our Dataframe. The countries did not show any linear correlation with the conversion rate. 

Finally,  we added columns of higher order (CA_new, UK_new, US_new) and correlated them. Again, no correlation with the conversion rate.

We can clearly state that The new_page should not be implemented.
