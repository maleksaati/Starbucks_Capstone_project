
# Starbucks Capstone Project

# Overview

Starbucks is the world’s largest coffeehouse chain, with over 33,833 stores in 80 countries, Starbucks has kindly provided a simulated dataset that mimics customer behavior on their rewards mobile app.

A detailed report of analysis for this project is available [here](https://medium.com/@maleksaati/starbucks-capstone-challenge-db8a5b6e1daa).

## **Datasets and Inputs**

the data is contained in three files:

portfolio.json — containing offer ids and metadata about each offer (duration, type, etc.).

profile.json — demographic data for each customer.

transcript.json — records for transactions, offers received, offers viewed, and offers complete.

Here is the schema and explanation of each variable in the files:

**portfolio.json**

-   id (string) - offer id
-   offer_type (string) - type of offer ie BOGO, discount, informational
-   difficulty (int) - minimum required spend to complete an offer
-   reward (int) - reward given for completing an offer
-   duration (int) - time for offer to be open, in days
-   channels (list of strings)

**profile.json**

-   age (int) - age of the customer
-   became_member_on (int) - date when customer created an app account
-   gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
-   id (str) - customer id
-   income (float) - customer's income

**transcript.json**

-   event (str) - record description (ie transaction, offer received, offer viewed, etc.)
-   person (str) - customer id
-   time (int) - time in hours since start of test. The data begins at time t=0
-   value - (dict of strings) - either an offer id or transaction amount depending on the record
