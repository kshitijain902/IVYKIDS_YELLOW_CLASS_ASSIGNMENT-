# IVYKIDS_YELLOW_CLASS_ASSIGNMENT
# Introduction
Here we are exploring Customer Chunk Dataset to analyze the proportion of customer which are at higher risk of Churn and what changes need to be done to reduce the proportion.
# Exploring the Data
It help us in understanding the data like shape of data_set(7043, 21), various attributes and how we have to change our working potential in order to reduce the Churn .
# Visualising for missing values
First we will convert TotalCharges to numeric from float in order to find the missing values.
We are creating a DataFrame that store rows where TotalCharges is Nan  and replacing it will mean value of TotalCharges column.
We will remove the column where Tenure is equal to 0 as only 11 missing values are there which can be removed
Mapping the value of Senior Citizen to numeric values
# Visualising the dataset using libraries like Matplotlib.pyplot ,seaborn etc to find the relation between the attributes.
First we represent the relation between Gender and Churn Values to estimate which gender is likely to become Churn.
when we created a plot between Contract and Churn we come to conclusion that poeple who opted for monthly payment are more likely to contribute to Churn and people with 1 year contract are less likely to contribute to Churn.
we found that male customers contribute more to Churn than female customers.
We found that customer using using Electronic check contribute to Churn.
Creating Covariance Matrix to find the relation between the attributes|
# Data Preprocessing
First we are doing LabelEncoding to deal with categorical values.
We will take the help of covariance matrix and will choose features in x dataset that contribute to improve the accuracy of output and will drop the features that will reduce the accuracy.
After that we define the x dataset and y dataset and defined x_train,x_test,y_train,y_test.
With the help of covariance matrix we have choosen three features for comparision.
# Model Training and Evaluation
After normalizing the dataset we apply different Training Model on it like Logistic Regression,Knn Classifier,RandomForest
We found that Logistic Regression gives the best accuracy score according to evaluation matrix among the other model.
# Recommendations
The gender, contract type, and payment method are found as significant factors affecting  churn and factors like Contract,DeviceProtection,StreamingTV are dropped as tjey were reducing model accuracy.
# Conclusion
This model help us in predicting customers that are at high risk of churn and analyzing  the changes that can be made in order to reduce the churn rate among the customers.
