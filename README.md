# PredictCustomerlifetimeValue

Notebook file 1: Data processing& exploration& customer_segmentation_RFM

#Purpose

Data expoloration for customer liftime value (CLV) prediction

A quick RFM analysis with clustering

# Content and result

Extracting data from Postgre SQL
Checking missing value, exclude orders without customerID (24.9% missing)
Delete duplicated records
Data interrogating and validation
( keep orders with negative value, keep all types of transaction (Normal sales, Return,Discount, Manual,Carriage,Postage and protection material,Bank charges). Delete 'return' transactions which have no previous transaction in the dataset )
Calulate 'Recency','Frequency' and 'Monetary' and score the values based on quartile values for clustering analysis
Cluster customers into 5 clusters using k-means (Elbow and Silhouette analysis)
Visualisation, analysis and summary

Clusters
Champions, Loyal/Potential Loyal, Promising, New Customers, About to Sleep/Churned

Libraries:
psycopg2
numpy,pandas,datetime,seaborn
mpl_toolkits,yellowbrick,sk-learn,plotly
Data :
http://archive.ics.uci.edu/ml/datasets/Online+Retail
