
# Credit Card Transaction Fraud Detection

### Overview

The problem statement is regarding Fraud detection on credit card transactions.

A sequential Deep Learning ANN model has been created to perform the binary classification between genuine and fraudulent transactions

This project was assigned by BITS Pilani during the third semester of M.Tech Data Science & Engineering.

## Group Members

This project was done by a group of 3 members including:

 - Nipun Gupta
 - Aiswarya S Parvathi
 - Vengadesh S
 
## About the dataset

Link: https://www.kaggle.com/datasets/dermisfit/fraud-transactions-dataset

This dataset is fictional and is trying to simulate real life details. Any similarity to real life cases is purely coincidental. It has the following columns.

trans_date_trans_time: The date and time of the transaction.

cc_num: credit card number.

merchant: Merchant who was getting paid.

category: In what area does that merchant deal.

amt: Amount of money in American Dollars.

first: first name of the card holder.

last: last name of the card holder.

gender: Gender of the cardholder.Just male and female

street:Street of card holder residence

city:city of card holder residence

state:state of card holder residence

zip:ZIP code of card holder residence

lat:latitude of card holder

long:longitude of card holder

city_pop:Population of the city

job:trade of the card holder

dob:Date of birth of the card holder

trans_num: Transaction ID

unix_time: Unix time which is the time calculated since 1970 to today.

merch_lat: latitude of the merchant

merch_long:longitude of the merchant

is_fraud: Whether the transaction is fraud(1) or not(0)

## Libraries Used

The libraries that we used to build this project are:

 #### numpy
  ![numpy](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Screenshots/Numpy.png?raw=true)
 #### pandas
 ![pandas](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Screenshots/Pandas.png?raw=true)
 #### matplotlib
 ![matplotlib](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Screenshots/Matplotlib.png?raw=true)
 #### seaborn
 ![seaborn](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Screenshots/Seaborn.png?raw=true)
 #### sklearn
 ![skleanr](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Screenshots/Sklearn.png?raw=true)
 #### keras
 ![seaborn](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Screenshots/Keras.png?raw=true)
 
## Steps performed

- Downloaded the dataset
- Read the dataset as a dataframe
- Exploratory Data Analysis
- Data Preprocessing and data cleaning
- Feature Engineering
- Feature importance
- Feature selection
- Feature scaling
- Model Building
- Model compiling
- Model training and testing
- Training vs Validation accuracy and loss comparison
- Model evaluation
- Hyperparameter tuning

## Plots

Countplot

![countplot](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Plots/Countplot.png?raw=true)

Countplot

![countplot](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Plots/Countplot1.png?raw=true)

Boxplot

![boxplot](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Plots/Boxplot.png?raw=true)

Heatmap

![heatmap](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Plots/Heatmap.png?raw=true)

Feature Importance

![Feature Importance](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Plots/Feature%20Importance.png?raw=true)

Histogram

![Histogram](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Plots/Histogram.png?raw=true)

Training vs Validation accuracy

![Training vs Validation accuracy](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Plots/Training%20vs%20Validation%20Accuracy.png?raw=true)

Training vs Validation loss

![Training vs Validation loss](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Plots/Training%20vs%20Validation%20Loss.png?raw=true)

Confusion matrix - ANN Sequential model

![Confusion matrix](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Plots/Confusion%20Matrix%20ANN%20Model.png?raw=true)

Confusion matrix - RandomizedSearchCV model

![Confusion matrix](https://github.com/nipun1992/Credit-card-transaction-fraud-detection/blob/master/Plots/Confusion%20Matrix%20Hyperparameter%20tuned%20ANN%20model.png?raw=true)

## Model Performance

- The ANN model is yielding an accuracy score of 91.21% on the test data. The model has predicted 1919 true negatives and 226 false positives out of 2145 fraudulent transactions resulting a recall score of 0.89 for the fraudulent class transactions. This model has predicted 504956 true positives and 48618 false negatives out of 553574 genuine transactions resulting a precision score of 1.00 and a recall score of 0.91 for the genuine class transactions.


- The ANN model hyperparameter tuned using RandomizedSearchCV is yielding an accuracy of 90.71% on the test data. This model has predicted 1909 true negatives and 236 false positives out of 2145 fraudulent transactions resulting a recall score of 0.89 for the fraudulent class transactions. This model has predicted 502186 true positives and 51388 false negatives out of 553574 genuine transactions resulting a precision score of 1.00 and a recall score of 0.91 for the genuine class transactions.
## Files and Folders

- **Plots** folder consists of the plots that were plotted in the project

- **Screenshots** folder consists of the online pictures depicting the libraries used in the project

- **DL_Assignment_Template.ipynb** file is the template that has been referred to for the project

- **Deep Learning - Fraud Detection.ipynb** file is the jupyer notebook that contains the project code

- **README.md** is the README File

- **ANN model.h5** is the saved ANN model
- **RandomizedSearchCV model.h5** is the saved hyperparameter tuned model