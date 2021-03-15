# Starbucks Capstone Project
## Table of contents
1. [Introduction](https://github.com/aparna-git-swe/Starbucks/blob/master/README.md#introduction)
2. [Project Overview](https://github.com/aparna-git-swe/Starbucks/blob/master/README.md#project-overview)
3. [Dataset Description](https://github.com/aparna-git-swe/Starbucks/blob/master/README.md#dataset-description)
4. [libraries](https://github.com/aparna-git-swe/Starbucks/blob/master/README.md#libraries)
5. [Process](https://github.com/aparna-git-swe/Starbucks/blob/master/README.md#process)
6. [Analysis Summary](https://github.com/aparna-git-swe/Starbucks/blob/master/README.md#analysis-summary)

## Introduction
This project is Capstone project  of the Udacity's Data Scientist Nanodegree Program .<br/>
This project is underlying to only one product ,where as Starbucks sells dozens of products.<br/>
My task is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type.

## Project Overview
Customer satisfaction drives business success and data analytics provides insight into what customers think. For example, the phrase "360-degree customer view" refers to aggregating data describing a customer's purchases and customer service interactions.<br/>

The Starbucks Udacity Data Scientist Nanodegree Capstone challenge data set is a simulation of customer behavior on the Starbucks rewards mobile application. Periodically, Starbucks sends offers to users that may be an advertisement, discount, or buy one get on free (BOGO). An important characteristic regarding this dataset is that not all users receive the same offer.<br/>

This data set contains three files. The first file describes the characteristics of each offer, including its duration and the amount a customer needs to spend to complete it (difficulty). The second file contains customer demographic data including their age, gender, income, and when they created an account on the Starbucks rewards mobile application. The third file describes customer purchases and when they received, viewed, and completed an offer. An offer is only successful when a customer both views an offer and meets or exceeds its difficulty within the offer's duration.<br/>

### Business Objective

The business problem that I would like to solve is how to get more customers to complete the offers and how we can reward the customer that make purchases during the promotional period for their loyalty.

## Dataset Description:

The data is contained in three files:<br/>

 .portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.).<br/>
 .profile.json - demographic data for each customer.<br/>
 .transcript.json - records for transactions, offers received, offers viewed, and offers completed.<br/>
Here is the schema and explanation of each variable in the files:<br/>

#### Data is contained in three files:

**portfolio.json**- containing offer ids and metadata about each offer (duration, type, etc.) <br/>
id (string) - offer id<br/>

offer_type (string) - type of offer ie BOGO, discount, informational<br/>

difficulty (int) - minimum required spend to complete an offer<br/>

reward (int) - reward given for completing an offer<br/>

duration (int) - time for offer to be open, in days<br/>

channels (list of strings)<br/>

**profile.json** - demographic data for each customer<br/>
age (int) - age of the customer<br/>

became_member_on (int) - date when customer created an app account<br/>

gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)<br/>

id (str) - customer id<br/>

income (float) - customer's income<br/>

**transcript.json** - records for transactions, offers received, offers viewed, and offers complete <br/>
event (str) - record description (ie transaction, offer received, offer viewed, etc.)<br/>

person (str) - customer id<br/>

time (int) - time in hours since start of test. The data begins at time t=0<br/>

value - (dict of strings) - either an offer id or transaction amount depending on the record<br/>

### libraries
Following Libraries was used to complete this project

pandas<br/>

numpy<br/>

math<br/>

json<br/>

datetime

matplotlib.pyplot as plt

seaborn as sns

sns.set()

%matplotlib inline

from sklearn.preprocessing import MinMaxScaler<br/>

from sklearn.model_selection import train_test_split, GridSearchCV<br/>

from sklearn.tree import DecisionTreeClassifier<br/>

from sklearn.naive_bayes import GaussianNB<br/>

from sklearn.neighbors import KNeighborsClassifier<br/>

from sklearn.linear_model import LogisticRegression<br/>

from sklearn.ensemble import RandomForestRegressor<br/>

### Process
The Process used to complete this project<br/>

Business Objective<br/>
Analyze business problem with visuals, data exploration understand which features and algorithm will be best.<br/>
Implement algorithm<br/>
Present result and write blog post about my findings.<br/>

### Analysis Summary:
Analysis complete summary is present [here](https://bantuaparna.medium.com/starbucks-rewards-b8c1f0c22e9a) in a Medium Post.
