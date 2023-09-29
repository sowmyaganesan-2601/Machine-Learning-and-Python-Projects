
# EDA, Customer Segmentation using RFM and KMeans

# Customer Segmentation
Segmentation means grouping entities together based on similar properties. Entities could be customers, products, and so on.
Customer segmentation is important for businesses to understand their target audience. Different advertisements can be curated and sent to different audience segments based on their demographic profile, interests, and affluence level.
It is the segmentation of customers on the basis of their similar characteristics, behavior, and needs. This will eventually help the company in many ways. Like, they can launch the product or enhance the features accordingly. They can also target a particular sector as per their behaviors. All of these lead to an enhancement in the overall market value of the company.

# Segmentation Factors

The most common ways in which businesses segment their customer base are:

Demographic information, such as gender, age, familial and marital status, income, education, and occupation.
Geographical information, which differs depending on the scope of the company. For localized businesses, this info might pertain to specific towns or counties. For larger companies, it might mean a customer’s city, state, or even country of residence.
Psychographics, such as social class, lifestyle, and personality traits.
Behavioral data, such as spending and consumption habits, product/service usage, and desired benefits.

# Advantages of Customer Segmentation
1) Determine appropriate product pricing.
2) Develop customized marketing campaigns.
3) Design an optimal distribution strategy.
4) Choose specific product features for deployment.
5) Prioritize new product development efforts.


# Libraries Required
1) Pandas – This library helps to load the data frame in a 2D array format.
2) Numpy – Numpy arrays are very fast and can perform large computations.
3) Matplotlib / Seaborn – This library is used to draw visualizations.
4) Sklearn – This module contains multiple libraries having pre-implemented functions to perform tasks from data preprocessing to model development and evaluation.

# Data
This project is based on Online Retail II data set containing all the transactions occurring for a UK-based and registered, non-store online retail between 01/12/2009 and 09/12/2011.The company mainly sells unique all-occasion gift-ware. Many customers of the company are wholesalers.

# Methodology

In this dataset we only have features that demonstrate Purchasing habits and Spending habits (Behavioural) factors. We perform RFM Modelling and KMeans Clustering on this dataset to segment customers.

# KMeans and RFM Analysis
1) RFM Model Analysis
RFM is a method used to analyze customer value. RFM stands for RECENCY, Frequency, and Monetary.

RECENCY: How recently did the customer visit our website or how recently did a customer purchase?

Frequency: How often do they visit or how often do they purchase?

Monetary: How much revenue we get from their visit or how much do they spend when they purchase?

The RFM Analysis helps the businesses to segment their customer base into different homogenous groups so that they can engage with each group with different targeted marketing strategies.

2) KMeans
K means clustering is one of the most popular clustering algorithms and usually the first thing practitioners apply when solving clustering tasks to get an idea of the structure of the dataset. The goal of K means is to group data points into distinct non-overlapping subgroups. One of the major application of K means clustering is segmentation of customers to get a better understanding of them which in turn could be used to increase the revenue of the company.

