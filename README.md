# Incident_Management_Analysis
This repository contains analysis of Incident management held at IT firm. The analysis has been done using Pyspark in Databricks Community edition.
There is one ipynb file each for Dataframe and SQL operations, for Data Analysis.

Inside the dataset folder are two files:

1.	incident_event_log.csv which contains the full data (This is the file used on all the ipynb files)
2.	incident_event_log_reduced.csv which contains data that is reduced to one record per incident 

Inside the Machine Learning Models folder are 5 files:

1.	Incident_Management_Spark_ML_Decision_Tree.ipynb
	The best performing model out of all the models created in terms of accuracy
	Has an accuracy of around 93%

2.	Incident_Management_Spark_ML_KMeans_Clustering.ipynb
	An attempt at clustering the data into 4 categories, keeping 4 different priority levels in mind, proved to be 
quite successful as the model's predictions were close enough to match our data

3.	Incident_Management_Spark_ML_Linear_Regression.ipynb
	The linear regression model to predict the duration to resolve an incident had a high root mean squared error 
and a poor R-squared value.

4.	Incident_Management_Spark_ML_Linear_SVC.ipynb
	It had a lower accuracy of 63% in predicting whether an incident met SLA as compared to Logistic Regression's 76%
	The process to scale the data took nearly half an hour to execute

5.	Incident_Management_Spark_ML_Logistic_Regression.ipynb
	The One Hot encoded data enabled the model to fit well on the training data and produced better performances 
compared to the Linear SVC

