# <h1 align="center">Udacity - Data Scientist Nanodegree Program</h1>
<h2 align="center">Project 4: Starbucks Capstone Project</h2>

## Table of Contents
- Udacity - Data Scientist Nanodegree Program
  1. [Table of Contents](#table-of-contents)
  2. [Medium Blog](#Blog-)
  3. [Project Summary](#Summary-)
  4. [Requirement Technical](#technical-)
  5. [Input Datasets](#Datasets-)
  6. [Project File Description](#description-)
  7. [Analysis Results](#Results-)
  8. [License, Acknowledgements](#Acknowledgements-)


## ii. Medium Blog <a name="Blog"></a>
More detail of my works are in the link

## iii. Project Summary <a name="Summary"></a>
This project analyzes simulated data that represents customer behavior on the Starbucks rewards mobile app. Starbucks periodically sends out offers to app users, which can be advertisements or actual offers like discounts or buy one get one free (BOGO) deals. The challenge is to determine which demographic groups respond best to different offer types.

The data includes transactional, demographic, and offer information. Each offer has a validity period, and the data also tracks when users view and complete offers. The goal is to combine this data and identify the demographic groups that have the highest response rates to specific offer types.

By understanding customer behavior and preferences, Starbucks can personalize offers and improve the effectiveness of their mobile app marketing campaigns. 

And through that, I will try to find out how well Starbucks customers use the current management application and incentive system. And from there, propose which customers will need more attention through their needs and behaviors from data taken from app users.

## iv. Requirement Technical <a name="technical"></a>
You need to have enough of these libraries installed in the Jupyter Notebook for working this project:

Python (version 3.x)
Data and Machine Learning Libraries:
* Pandas
* numpy
* datetime
* matplotlib
* seaborn
* Scikit-learn (sklearn)

## v. Input Datasets <a name="Datasets"></a>
For this project, the data sets are provided by Starbucks through Udacity in 3 JSON files below. These contains contains data which about customer behavior on the Starbucks rewards (offers) mobile app.
The data is contained in three files:

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

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


## vi. Project File Description <a name="description"></a>

Starbucks_Capstone_notebook.ipynb: The Jupyter Notebook which contains all of my works from examination and analysis the datasets above.

## vii. Analysis Results <a name="Results"></a>

1. If considered monthly, revenue will almost increase month by month. This is interesting, because when we detect an increase, we will have appropriate incentive policies to keep regular customers. As in the graph, we pay attention to the months June and July every 2 years will be the months with the highest increase in the number of users.

2. Based on the ratio, I discovered that male customers receive offers and the number of transactions is about **~3%** more than female customers. However, female customers will have a higher offer completion rate than male customers, **~13%**. The type of offer that male customers receive "loses" to female customers is bogo with about ~1%, the rest are similar and not much different.

3. Between transaction data, we get data about offer received. We can see that almost 70-78% of offers will be seen by customers and customers will use 50-55% of those viewed offers. Number of completed promotion for '**bogo**' and '**discount**' doesn't different much.

4. After separated the age to age group and show the statistic on the chart above. I found that almost Starbucks customers came from Adult, and just a small number of Teenager care about those drinks. I think those such low figures are due to the fact that teenagers often do not have enough money to pay for expensive drinks.

5. In terms of gender, completing an offer will not have a big change between the average time when male customers take 381 hours and female customers take 380 hours. But when considering age groups, Teenagers will tend to complete offers faster than other age groups. But it's not much of a difference when the time difference is about 4~10 hours.

Thereby, I think that because female customers tend to favor offers more and they have quite high incomes, focusing on increasing the number of promotions on female customers will probably be the right decision to increase the number of customers. salable goods.

In addition, although it is unknown about the offer completion rate of customers by age group, the statistical time to complete an offer seems to be much higher than the remaining age groups. This is also a business and promotion opportunity.


## viii. License, Acknowledgements <a name="Acknowledgements"></a>

The data for coding this project was given by Starbucks and Udacity









