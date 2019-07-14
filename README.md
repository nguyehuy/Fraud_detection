# Fraud_detection
This is a simple solution for dectecting the fraud transaction
# Goal
E-commerce websites often transact huge amounts of money. And whenever a huge amount of money is
moved, there is a high risk of users performing fraudulent activities, e.g. using stolen credit cards, doing
money laundry, et .

Machine Learning really excels at identifying fraudulent activities. Any website where you put your credit
card information has a risk team in charge of avoiding frauds via machine learning.

The goal of this challenge is to build a machine learning model that predicts the probability that the first
transaction of a new user is fraudulent.

# Challenge Description
Build a model to predict whether an activity is fraudulent or not. Explain how different assumptions about
the cost of false positives vs false negatives would impact the model.

# Data Information

## Fraud_Data: -infomation about each user first transaction
### Columns:
 User_Id:Id of the user. Unique by user
 
 Signup_time: the time when the user created her account (GMT time)
 
 Purchase_time: The time when the user bought the item (GMT time)
  
 Purchase_value: The cost of the item purchased (USD)
 
 Device_id: The device id. Yopu can asume that it is unique by device, I.e, 2 transactions with the same device ID means that the same physical device was used to buy
 
 Source: User markerting channnel: ads, SEO, Direct (i.e came to site by directly typing the site address on the browser)
 
 Browser: The browser used bt the user
 
 Sex: user sex: Male / Female
 
 Age: User age
 
 Ip address: User numeric ip address
 
 Class: This is what we are trying to prdict: Whether the activity was fraudulent(1) or not (0)
 
 ## IpAddress_to_Country: -mapping tyhe numeric ip address to its country. For each country, it gives the range. If the numberic ip address falls within the range, then the ip address belongs to the corresponding country.
 
 ### Columns:
 
  lowe_bound_ip_address: the lower bound of the numberic ip address for that country
  
  upper_bound_ip_address: the upper bound if the numeric ip address for that country
  
  country: the corresponding country. If a user has an ip address whose value is within the upper and lower bound, the he/she is based in this country
