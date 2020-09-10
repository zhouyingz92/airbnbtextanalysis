# Airbnb-Review-Analysis

## 1 Data Description

### 1.1 Data Source

Gathered the data from http://insideairbnb.com/get-the-data.html, which is sourced from publicly available information from the Airbnb site. Boston was chosen as the main target for analysis. 
The data was by August, 31, 2020, which has been already cleansed and aggregated where appropriate to facilitate this project.


### 1.2 Data Prepossessing Needs
(1) Mixed languages and content problem: Some reviews from the dataset are not in English. Also, some reviews are attached with pictures, which may cause difficulty for analysis.


(2) Selection bias: the recorded data are collected from customers who are willing to give online reviews. Those who don’t have the habit of giving reviews online or even those who don’t have the access to the internet are omitted from selection sample.


(3) Ambiguous attribute: The available information within the sub-dataset calendar.csv does not differentiate between a booked night vs an unavailable night, both have been counted as "unavailable", which seems ambiguous and thus understate the Availability metric. 


(4) Noisy information: Spamming reviews are not blocked by Airbnb, which may generate unnecessary noisy information for analysis. 


### 1.3 Dimensions
The whole datasets consist three subsets, including calendar.csv, listings.csv and reviews.csv. The calendar.csv is the detailed listings data for Boston, with 7 attributes and 2,610,115 records. 

The attributes include listing_id, date, available, price, adjusted_price, minimum_nights, maximum_nights. The listings.csv has a shape of 7151 rows and 106 columns, which comprehensively shows the information of each listed room, include its url, name, summary, space, description, etc. The reviews.csv has 311,277 records with 6 attributes, including listing_id, id, date, review_id, review_name, and comments. 


## 2 Project Objectives

### 2.1 Insights Plan to Get
(1) What amenities drive high guests’ satisfactions?


(2) Which are popular neighbourhoods in Boston?


(3) The price range of housing within the neighbourhood and compare ranges at the neighbourhood level.

### 2.2 Insights Application
(1) Host: Hosts can have a sense about which parts they should improve to meet customers’ needs and increase their housing rating based on these insights. 


(2) Customer: insights provide detailed and useful benchmarks for potential customers to make housing choices. 
