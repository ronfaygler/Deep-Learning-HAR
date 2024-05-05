# deep-learning-HAR
**Human Activity Recognition**
This project focuses on predicting user actions based on sensor data collected from a smartwatch. The dataset consists of CSV files containing sequences of points on the x/y/z axes for various actions performed by users. The goal is to develop models that can accurately classify these actions.

**Data Preprocessing**
* Identified and processed CSV files to understand the data distribution.
Focused on actions performed on the hand due to majority distribution.
Applied padding to ensure uniform sequence length.
Utilized data from a single sensor for simplicity and consistency.
**Model Development**
Baseline Model: Employed a Random Forest classifier for initial performance evaluation.
1D CNN Model: Designed a Convolutional Neural Network to capture spatial dependencies in the data.
LSTM Model: Implemented a Long Short-Term Memory network to handle the time-series nature of the data.
**Additional Techniques**
User Validation: Split the training set to create a validation set that included users not present in the original training set. This ensured a more comprehensive evaluation of the model's generalization ability to new users.
Self-Supervised Learning: Introduced a method (predict the last 500 rows of sensor data), to help the model learn patterns for better generalization.
**Kaggle Competition**
This project was part of a competition among class students on Kaggle, where the goal was to achieve the highest accuracy in predicting user actions based on smartwatch sensor data.
