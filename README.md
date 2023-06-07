# Regression

## Project Summary :
This dataset is a live dataset of Rossmann Stores. On analsysing this problem we observed that our goal is to predict the sales figures of Rossmann store. In this project we work Analysed the Dataset by using Exploratory Data Analysis , we used Exponential Moving Averages to analyse Trends and Seasonality in Rossmann dataset. we used the following for prediction analysis,

A. Linear Regression Analysis

B. Elastic Regression ( Lasso and Ridge Regression).

C. Random Forest Regression.

D. adaboost and Xgboost).

By applying above algorthim we find accuracy of 98% by Xgboost.

## Data Description :
Rossmann Stores Data.csv - historical data including Sales

store.csv - supplemental information about the store

Data fields Most of the fields are self-explanatory. The following are descriptions for those that aren't.

Id - an Id that represents a (Store, Date) duple within the test set

Store - a unique Id for each store

Sales - the turnover for any given day (this is what you are predicting)

Customers - the number of customers on a given day

Open - an indicator for whether the store was open: 0 = closed, 1 = open

StateHoliday - indicates a state holiday. Normally all stores, with few exceptions, are closed on state holidays. (Note that all schools are closed on public holidays and weekends. a = public holiday, b = Easter holiday, c = Christmas, 0 = None)

SchoolHoliday - indicates if the (Store, Date) was affected by the closure of public schools

StoreType - differentiates between 4 different store models: a, b, c, d

Assortment - describes an assortment level: a = basic, b = extra, c = extended

CompetitionDistance - distance in meters to the nearest competitor store

CompetitionOpenSince(Month/Year)- gives the approximate year and month of the time the nearest competitor was opened

Promo - indicates whether a store is running a promo on that day

Promo2 - Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not participating, 1 = store is participating

Promo2Since[Year/Week] - describes the year and calendar week when the store started participating in Promo2

PromoInterval - describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store

## Conclusion:
Sales column contains 172817 rows with 0 sale. new dataframe is created in which we removed 0 sales rows and tried to train our model. We used various algorithms and got accuracy score around 74%.

the curiousity was also about the total dataset(including Sales = 0 rows). So we trained another model using various algorithms and we got accuracy near about 98% which is far better than previous model.

So we came to conclusion that removing sales=0 rows actually removes lot of information from dataset as it has 172817 rows which is quite large and therefore we decided not to remove those values.We got our best rmpse score from Random Forest model,Graident boosting technique like adaboost ,Xgboost,we tried taking an optimum parameter so that our model doesnt overfit.
