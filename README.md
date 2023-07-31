Algorithmic Trading

## Overview of the Analysis

The program aims to look at data from market performance and devise a automated strategy based on patterns, algorithms, and comparing short term and longterm returns. The program utilizes machine learning technonolgy to understand the existing patterns from the train models to predict the test model. The program also uses different supervized machine learning methods to predict buying and selling of equity.

### Purpose of the Exercise

- Implement an algorithmic trading strategy that uses machine learning to automate the trade decisions.

- Adjust the input parameters to optimize the trading algorithm.

- Train a new machine learning model and compare its performance to that of a baseline model.

### Data Used for the Analysis
Data availabe for this analaysis is included in the Resources folder (emerging_markets_ohlcv.csv). 
 - Fund's daily closing price
 - Simple Moving Averages are used (4 days and 100 days )
 - Daily returns are calculated and positive and negative returns are used as the label variable  


### Steps for Analysis

* Imported the data from the CSV
* Calculated the daily returns and the moving averages
* Calcluated the signal based on the daily returns
* Seperated the data into labels and features
* Data split by timeslate using dateoffset
* Scaled the data using the standard scaler
* Analysed the data using Support Vector Machine model and Decision Tree Classifier
* Measured the outcome using the classification report
* Backteted the data

## Results

* Machine Learning Model 1: Support Vector Machine
 * SVM Classification Report <br>
    <img title="SVM Classification Report" alt="Alt text" src="/Images/svm_classificationreport.png"> <br>
 * SVM Based Acutual vs Prediction Comparision <br>
    <img title="SVM Based Acutual vs Prediction Comparision" alt="Alt text" src="/Images/SVM_testing.png"> <br>

* Machine Learning Model 2: Decision Tree Classifier
 * Decision Tree Classification Report <br>
    <img title="Decision Tree Classification Report" alt="Alt text" src="/Images/dtree_classificationreport.png"> <br>
 * Decision Tree Based Acutual vs Prediction Comparision <br>
    <img title="Decision Tree Based Acutual vs Prediction Comparision" alt="Alt text" src="/Images/dtree_testing.png"> <br>


## Summary

Comparing the two models, the SVM model provided a more accurate results compared woth the Decision Tree Classifier model.