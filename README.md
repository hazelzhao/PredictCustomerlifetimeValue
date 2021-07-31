# PredictCustomerlifetimeValue

Data :
http://archive.ics.uci.edu/ml/datasets/Online+Retail

## Notebook file 1: Data processing& exploration& customer_segmentation_RFM

### Purpose

Data expoloration for customer liftime value (CLV) prediction.
A quick clustering analysis based on RFM model.

### Result 

https://public.tableau.com/app/profile/hazel4114/viz/CustomerSegmentation_16276652316260/Dashboard1

Clusters: Champions, Loyal/Potential Loyal, Promising, New Customers, About to Sleep/Churned.

### Content 

Extracting data from Postgre SQL.

Checking missing value, exclude orders without customerID (24.9% missing).

Delete duplicated records.

Data interrogating and validation. 
keep orders with negative value, keep all types of transaction (Normal sales, Return,Discount, Manual,Carriage,Postage and protection material,Bank charges). Delete 'return' transactions which have no previous transaction in the dataset.

Calulate 'Recency','Frequency' and 'Monetary' and score the values based on quartile values for clustering analysis.

Cluster customers into 5 clusters using k-means (Elbow and Silhouette analysis).

Visualisation, analysis and summary.

## Notebook file 2: Models 

Baseline model: linear regression /Sequential Neuron Network /Wide and Deep /BG/NBD-GammaGamma / Hybrid model (BG/NBD-GammaGamma + linear regression)/ XGBoost

### Result

https://public.tableau.com/app/profile/hazel4114/viz/models_16276636191700/Dashboard2

Wide and Deep model has the lowest value of root mean squared error, mean absolute error can be accessed depends on bussiness purpose

Monetary value during feature period has dominant power in prediction, recency and average busket size have negative effect.

Evaluated performance over different clusters, different models have different performance for each clusters, therefore it is possible to improve performance if different group of customers have different models.


## SQL 

data cleaning and generate features and target accrdoing to threshold date

## Tableau















