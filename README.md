# Predicting-Student-Exam-Success-Using-Multiple-Regression-and-Classification-Models
# Overview
This project aims to predict student success in writing exams based on various socio-demographic and academic variables. By utilizing multiple regression and classification models, we analyze how different factors influence student performance. The dataset includes information about 1,000 students and incorporates variables such as gender, parental education, economic status, recitation class attendance, and exam scores in math, reading, and writing.

The project's primary goal is to create predictive models for exam scores and classify student success using techniques such as Multiple Linear Regression, Logistic Regression, and Naïve Bayes.

# Dataset
Name: Students Performance in Exams
Number of Samples: 1,000
Variables:
Gender
Race/ethnicity
Parental education level
Lunch option (economic status indicator)
Recitation class attendance
Math score
Reading score
Writing score
The final prediction is focused on estimating the writing score and classifying the success in the writing exam.

# Methodology
Data Pre-processing:

The dataset is examined for correlations between variables.
Features with low correlation (e.g., parental education, race/ethnicity) are eliminated.
Gender, wealth, and recitation attendance are converted to binary indicators for modeling.
Data is normalized to ensure fair weight distribution across variables.
# Model Selection:

Multiple Linear Regression: Used to predict the writing score based on selected features.
Logistic Regression: Applied to classify whether a student will be successful or not (based on average performance).
Naïve Bayes: Used for letter grade classification (A, B, C, etc.) based on reading and math scores.
Implementation Details:

Multiple Linear Regression: Predicts the writing score using five independent variables: gender, wealth, recitation attendance, reading score, and math score.
Logistic Regression: Uses sigmoid activation to classify success as "above average" or "below average."
Naïve Bayes: Estimates letter grades based on Gaussian distribution for features.
# Results
# Multiple Linear Regression:

Achieved a reasonable prediction for writing scores, minimizing the cost function over 1,000 iterations.
The final model produced weights indicating how each variable contributes to writing success.
# Logistic Regression:

The initial gradient descent approach resulted in low accuracy.
Switching to Maximum Likelihood Estimation (MLE) significantly improved accuracy, reaching 74.1% on the test set.
# Naïve Bayes Classification:

Classifies students into letter grade categories (F to A).
Achieved an accuracy of 87.5% for letter grade prediction.
# Challenges
Pre-processing and analyzing the correlation between variables was complex due to data redundancy.
Implementing gradient descent from scratch for multiple regression and logistic regression required extensive research.
Optimizing logistic regression with MLE was crucial for improving accuracy.
Handling Naïve Bayes classification required restructuring the dataset and understanding Gaussian distribution.
