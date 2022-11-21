
# Introduction

This repository contains examples of code for building recommendation system within CIND820 D1H - Big Data Analytics Project - F2022. 

There are five key tasks:
* Prepare Data: Preparing and loading data for each recommender algorithm
* Explore Data: Perform Exploratory Data Analysis
* Model: Building models using different recommender algorithms such as Association Rules, Content Based, Collaborative Filtering (Matrix Factorization), Hybrid.
* Evaluate: Evaluating algorithms with offline metrics
* Model Select and Optimize: Tuning and optimizing hyperparameters for recommender models


# Prepare Data
Dataset: Brazilian E-Commerce Public Dataset by Olist - https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce
1. Merge all 9 tables into 1 Master table
2. Filter Master table: to Delivered orders (to have final review score) and with at least 2 products per customer (not necesseraly within 1 order) to have the ability to run performance metrics 

Explore Data: 
1. Check data for null values and duplicates and remove if any
2. Check numerical and categorical data distribution and correlation




# References

1.	Deepjyoti Roy, Mala Dutta (2022), “A systematic review and research perspective on recommender systems”, Journal of Big Data, Springer Open, https://journalofbigdata.springeropen.com/articles/10.1186/s40537-022-00592-5 
2.	Le Nguyen HoaiNam (2022), “Towards comprehensive approaches for the rating prediction phase in memory-based collaborative filtering recommender systems”, https://www.sciencedirect.com/science/article/abs/pii/S002002552101344X?via%3Dihub
3.	Nassar, N., Jafar, A., Rahhal, Y. (2020), “Multi-criteria collaborative filtering recommender by fusing deep neural network and matrix factorization”, https://journalofbigdata.springeropen.com/articles/10.1186/s40537-020-00309-6 
4.	P. M. Alamdari, N. J. Navimipour, M. Hosseinzadeh, A. A. Safaei and A. Darwesh, "A Systematic Study on the Recommender Systems in the E-Commerce," in IEEE Access, vol. 8, pp. 115694-115716, 2020, doi: 10.1109/ACCESS.2020.3002803, https://ieeexplore.ieee.org/abstract/document/9118884 
5.	Faxin Qi, Xiangrong Tong, Lei Yu, Yingjie Wang (2019) “Personalized project recommendations: using reinforcement learning”, https://jwcn-eurasipjournals.springeropen.com/articles/10.1186/s13638-019-1619-6 
6.	Mingang Chena, Pan Liu (2017), “Performance Evaluation of Recommender Systems”, http://www.ijpe-online.com/EN/abstract/abstract3798.shtml
7.	Francesco Ricci, Lior Rokach, Bracha Shapira, Paul B. Kantor (2011), “Recommender Systems Handbook”, Springer Science Business Media.

