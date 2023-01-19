# Udacity data analyst Project-4: Wrangle and Analyze Data


## Table of Contents
 * [Necessary packages](#necessary-packages)
 * [Project Motivation](#project-motivation)
 * [File Description](#file-description)
 * [How to Interact With Project](#how-to-interact-with-project)
 * [Results](#results)

## Necessary packages

- requests
- numpy 
- os
- pandas
- tweepy
- json
- timer
- matplotlib
- seaborn

## Project Motivation

The motivation of this project is to get data via a twitter API and check for data tidiness and quality. The logic is always *define* the issue, fix the issue via *code* and *test* if the issue has been fixed. 

## File Description

- act_report.html
- tweet-json.txt: twitter data in case request via twitter API does not work
- twitter_archive_enhanced.csv: WeRateDogs Twitter archive
- twitter_archive_master.csv: output of data wrangling
- wrangle_act.html
- wrangle_act.ipynb: 
    - gathering data
    - accessing data
    - cleaning data
    - storing data
- wrangle_report.ipynb
    - results of wrangle_act.ipynb


## How to interact with this project

In principle, you can simply clone the project:

`git clone https://github.com/TobiasGroeschner/Udacity-Data-Analyst.git`

To interact with the twitter API, you would have to set up a developer account on developer.twitter.com.

You will have to generate these 4 things:

1. consumer_key = 'xxxx' #API Key - helps to verify who I am
2. consumer_secret = 'xxxx' #API Key secrect - like a password, verifies API key
3. access_token = 'xxxx-xxxx' 
4. access_secret = 'xxxx'

I recommend to just work with the twitter-json.txt file. This is the output of the twitter API request which can be tricky.

## Results: 

See wrangle_report.ipynb

## Acknowledgements:
- udacity & twitter for providing this project.