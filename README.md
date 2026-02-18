# CA_03
Computer Assignment 03 Decision Tree

In this assignment, we built and evaluated a Decision Tree Classifier using Python and scikit-learn to predict an individual’s income category based on demographic and socioeconomic features.

The goal was to train a model, evaluate its performance, tune hyperparameters, interpret the decision tree, and use the final model to predict the income category of a new individual. 

First we prepared the data. It was filled with categorical features such as age_bin and msr_bin. We used hot one encoding as recommended by ChatGPT so the decision tree could interpret categorical variables numerically. We then split the data into:

- X_train, y_train → used to train the model
- X_test, y_test → used to evaluate performance

We used multiple evaluation methods to understand model behavior:
- Accuracy score
- Confusion matrix
- Precision, Recall, and F1-score
- Actual vs Predicted comparison

We trained a shallow tree (max_depth = 3) to see which features were important and to see the model work step-by-step

We did hypermater tuning to test out different parameters and their significance in accurcacy and other evaluation metrics. For example, we changed max depth and min_sample_leaf values. We also used tables and plots to evaluate them as well. 

Our final model had the following parameters:
- criterion = "entropy"
- max_depth = 10
- min_samples_leaf = 25
- max_features = 0.6
- random_state = 101

We then used our model to predict the income of a new individual based on information given to us.

