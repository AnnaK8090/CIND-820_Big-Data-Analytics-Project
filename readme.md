
# Introduction

This repository contains examples of code for building recommendation system within CIND820 D1H - Big Data Analytics Project - F2022. 

There are five key tasks:
* Prepare Data: Preparing and loading data for each recommender algorithm
* Explore and Transform Data: Perform Exploratory Data Analysis and data structures transfrmation
* Model: Building models using different recommender algorithms such as Association Rules, Collaborative Filtering (Matrix Factorization), Content Based, Hybrid.
* Evaluate: Evaluating algorithms with offline metrics
* Model Select and Optimize: Tuning and optimizing hyperparameters for recommender models


# Prepare Data 
1. The initial dataset: Brazilian E-Commerce Public Dataset by Olist - https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce
2. Upload 9 tables to the notebook and merge into 1 Master table according to Data Schema

# Explore and Transform Data: 
1. Check data for null values and duplicates and remove if any.
2. Check values for correlation and distribution. 
3. Transform Master table: 
 * filter by order_status = Delivered - to have final review score as there are orders with multiple reviews
 * filter by at least 3 products per customer (not necesseraly within 1 order)  - mainly to reduce processing time 
 4. Extract Features: 
 * Product features - there is only 1 feature - "product category" that will be taken into account. Other product attributes (like weight, length, height, width) are not of interest. 
 * Customer features - the dataset does not provide any personal characteristics (like age, gender, occupation, interests). The only customer data is related to geography (state, city, zipcode), which might be used for "customer cold start" problem - for a new customer with zero purchases, recommender system might offer "the most popular items in your region". 
 5. Define response variable - review_score (1-5). 
 Link to the result of Data Preparation, Analysis and Transformation - https://github.com/AnnaK8090/CIND-820_Big-Data-Analytics-Project/blob/main/1_basic_transformations.ipynb

# Build Models: 
1. Matrix Factorization - https://github.com/AnnaK8090/CIND-820_Big-Data-Analytics-Project/blob/main/2_Collaborative_Filtering_Matrix_Factorization.ipynb
2. Association Rules - https://github.com/AnnaK8090/CIND-820_Big-Data-Analytics-Project/blob/main/3_ASSOCIATION_RULES.ipynb
3. Content Based - TBD
4. Hybrid - TBD
5. Compare the results of 4 models (run performance metrics). 



# References

1.	Deepjyoti Roy, Mala Dutta (2022), “A systematic review and research perspective on recommender systems”, Journal of Big Data, Springer Open, https://journalofbigdata.springeropen.com/articles/10.1186/s40537-022-00592-5 
2.	Le Nguyen HoaiNam (2022), “Towards comprehensive approaches for the rating prediction phase in memory-based collaborative filtering recommender systems”, https://www.sciencedirect.com/science/article/abs/pii/S002002552101344X?via%3Dihub
3.	Nassar, N., Jafar, A., Rahhal, Y. (2020), “Multi-criteria collaborative filtering recommender by fusing deep neural network and matrix factorization”, https://journalofbigdata.springeropen.com/articles/10.1186/s40537-020-00309-6 
4.	P. M. Alamdari, N. J. Navimipour, M. Hosseinzadeh, A. A. Safaei and A. Darwesh, "A Systematic Study on the Recommender Systems in the E-Commerce," in IEEE Access, vol. 8, pp. 115694-115716, 2020, doi: 10.1109/ACCESS.2020.3002803, https://ieeexplore.ieee.org/abstract/document/9118884 
5.	Faxin Qi, Xiangrong Tong, Lei Yu, Yingjie Wang (2019) “Personalized project recommendations: using reinforcement learning”, https://jwcn-eurasipjournals.springeropen.com/articles/10.1186/s13638-019-1619-6 
6.	Mingang Chena, Pan Liu (2017), “Performance Evaluation of Recommender Systems”, http://www.ijpe-online.com/EN/abstract/abstract3798.shtml
7.	Francesco Ricci, Lior Rokach, Bracha Shapira, Paul B. Kantor (2011), “Recommender Systems Handbook”, Springer Science Business Media.

