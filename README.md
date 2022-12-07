# Capstone-Project
## Starbucks Capstone Challenge

## Introduction

This is a capstone project of Udacity Machine Learning Engineer Nanodegree. The main task of this project is to come up 
with a marketing strategy which determine what kind of reward will be more appropriate for a certain customer.

## Data

Starbucks has provided this experimental dataset on 
[kaggle](https://www.kaggle.com/datasets/blacktile/starbucks-app-customer-reward-program-data). 
The dataset contains 3 json files:
* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

The schema and explanation of each variable in the files:

**portfolio.json**
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

**profile.json**
* age (int) - age of the customer 
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

**transcript.json**
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record


## Files of Repository

* data
  * portfolio.json
  * profile.json
  * transcript.json
* Proposal
  * proposal.tex - tex file of proposal
  * proposal.pdf - proposal of this project
  * Udacity Reviews.pdf - reviews of proposal including some links
* Data.ipynb - notebook of data processing and data visualization
* model.ipynb - notebook of training model and evaluation
* profile.csv - processed data used in model.ipynb
* Report.pdf - report of this project
* Udacity Reviews.pdf - reviews of project
* report.tex - tex file of report
* README.md

## Library

This project is developed in Python 3.9.

The following libraries are used in this project:

* numpy 1.22.3
* pandas 1.5.1
* matplotlib 3.5.3
* scipy 1.7.3
* xgboost 1.7.1
* scikit-learn 1.0.2
* tensorflow 2.9.1
