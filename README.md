# Module 12 Report Template

## Overview of the Analysis
  The intention of this analysis is to train and evaluate a machine learning model based on loan risk. The analysis is centered around the logistic regression
model with a secondary random forest test model. The dataset provided for the project contained loan application details such as loan size, borrower income, debt, etc. By utilizing machine learning models we attempted to predict whether a loan would be considered "low risk" or "high risk".
  Not only were we considering the whether a loan would be high risk or not, the goal is to determine whether a logistic regression model is an effective method of handling this task. One of the ways this can be achieved is by using the value_counts function to check the balance of the variables. This is an important step in the process to ensure the model is not biased or that the dataset is not imbalanced, which can lead to misleading model evaluation metrics. 
  Other important stages required for the completion of the analysis include splitting the data into training and testing sets, use the testing data to make predictions, calculate the accuracy score of the model and create a classification report using sklearn metrics' accuracy_score and classification_report functions. In addition to running the data set with the logistic regression model, I also used the random forest model to be able to compare. 
  
## Results

* Machine Learning Model 1: Logistic Regression Model
  * Accuracy: 0.99
  * Class 0 Precision: 1.00
  * Class 0 Recall: 0.99
  * Class 1 Precision: 0.85
  * Class 1 Recall: 0.91


* Machine Learning Model 2: Random Forest Model
  * Accuracy: 0.99
  * Class 0 Precision: 1.00
  * Class 0 Recall: 0.99
  * Class 1 Precision: 0.85
  * Class 1 Recall: 0.90

## Summary
  The results shown above prove that Logisitic Regression and Random Forest models are very similar on the surface when considering accuracy, precision and recall. This is likely due to the similarities between the two machine learning methods. Both logistic regression and random forest are supervised learning methods, which are typically used for classification problems such as this one. Both models can handle both categorical and numerical features like the ones in the lending_data.csv file used, and both models are scalable, making them capable of working with large datasets. Taking only the numbers into account both models are equally as efficient at identifying healthy loans, but logistic regression performed just slightly better than random forest at identifying high risk loans, returning a recall value 0.01 higher. 
  In conclusion, the logistic regression model is the best choice for this specific application. Although the Random Forest model could potentially perform better with a different larger dataset with more complex or noisy features. 
