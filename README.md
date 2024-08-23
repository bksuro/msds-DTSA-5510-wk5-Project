# msds-DTSA-5510-wk5-Project

## Description
This project was taken from Kaggle, this involves predicting the type of vehicle.

Details:
The dataset has 846 observations/samples. 
The dataset was divided training set (719 observations - vehicle_train.csv) and testing set (127 observations – vehicle_test.csv). 
There are 18 numerical variables/features. 
Training set actual class labels are provided in the “vehicle_training_label.csv” file 
(0 –bus, 1 – Opel Manta, 2 – Saab, 3 – Van).

During EDA, 'ID' column was dropped.

Correlation matrix showed that data is highly correlated.

## PCA Analysis
PCA analysis was done to figure out how many features are needed, played and tested with 5, 10, and 15.

10 and 15 provided the same output.

Using StandardScaler with PCA, data was transformed and the output using the non transformed data and transformed data didnt show much difference in this dataset.

Using GridSearch to find the best parameters provided two such combinations.

-  {'C': 10, 'kernel': 'rbf'}
-   {'C': 0.01, 'kernel': 'linear'}

## SVC Model
SVC model is used to predict the data but not much luck.

## Agglomerative Clustering
Used the AG from the class homework which provided a littler better output but not much

## KMeans
Used KMeans to check if we get and better output but no luck.


Accuracy scores
- SVC - 23.62%
- AG - 45.34%
- KMeans - 35.04%
