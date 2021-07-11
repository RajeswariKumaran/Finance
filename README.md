# Finance

DESCRIPTION

Problem Statement

Finance Industry is the biggest consumer of Data Scientists. It faces constant attack by fraudsters, who try to trick the system. Correctly identifying fraudulent transactions is often compared with finding needle in a haystack because of the low event rate. 
It is important that credit card companies are able to recognize fraudulent credit card transactions so that the customers are not charged for items that they did not purchase.
You are required to try various techniques such as supervised models with oversampling, unsupervised anomaly detection, and heuristics to get good accuracy at fraud detection.
Dataset Snapshot

The datasets contain transactions made by credit cards in September 2013 by European cardholders. This dataset represents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

<img width="1299" alt="1566546571_cap 2" src="https://user-images.githubusercontent.com/52888997/125187447-54eb5480-e24d-11eb-9a93-a859943b3b2d.png">
 



 

It contains only numerical input variables which are the result of a PCA transformation. 
Features V1, V2, ... V28 are the principal components obtained with PCA. 
The only features which have not been transformed with PCA are 'Time' and 'Amount'

 

Project Task: Week 1

Exploratory Data Analysis (EDA):

1.    Perform an EDA on the Dataset.
       a)    Check all the latent features and parameters with their mean and standard deviation. Value are close to 0 centered (mean)
              with unit standard deviation
       b)    Find if there is any connection between Time, Amount, and the transaction being fraudulent.
2.    Check the class count for each class. It’s a class Imbalance problem.
3.    Use techniques like undersampling or oversampling before running Naïve Bayes, Logistic Regression or SVM.
       a.    Oversampling or undersampling can be used to tackle the class imbalance problem
       b.    Oversampling increases the prior probability of imbalanced class and in case of other classifiers, error gets multiplied as the 
              low-proportionate class is mimicked multiple times.
4     Following are the matrices for evaluating the model performance: Precision, Recall, F1-Score, AUC-ROC curve. Use F1-Score as
       the evaluation criteria for this project.

Project Task: Week 2

Modeling Techniques:

Try out models like Naive Bayes, Logistic Regression or SVM. Find out which one performs the best
Use different Tree-based classifiers like Random Forest and XGBoost. 
       a.    Remember Tree-based classifiers work on two ideologies: Bagging or Boosting
       b.    Tree-based classifiers have fine-tuning parameters which takes care of the imbalanced class. Random-Forest and XGBboost.
Compare the results of 1 with 2 and check if there is any incremental gain.

Project Task: Week 3

Applying ANN:

Use ANN (Artificial Neural Network) to identify fradulent and non-fradulent.
       a)    Fine-tune number of layers
       b)    Number of Neurons in each layers
       c)    Experiment in batch-size
       d)    Experiment with number of epochs. Check the observations in loss and accuracy
       e)    Play with different Learning Rate variants of Gradient Descent like Adam, SGD, RMS-prop
       f)    Find out which activation performs best for this use case and why?
       g)    Check Confusion Matrix, Precision, Recall and F1-Score
2.    Try out Dropout for ANN. How is it performed? Compare model performance with the traditional ML based prediction models from
       above. 
3.    Find the best setting of neural net that can be best classified as fraudulent and non-fraudulent transactions. Use
       techniques like Grid Search, Cross-Validation and Random search.

Anomaly Detection:

4.     Implement anomaly detection algorithms.
        a)    Assume that the data is coming from a single or a combination of multivariate Gaussian
        b)    Formalize a scoring criterion, which gives a scoring probability for the given data point whether it belongs to the
              multivariate Gaussian or Normal Distribution fitted in a)
Project Task: Week 4

Inference and Observations:

Visualize the scores for Fraudulent and Non-Fraudulent transactions.
Find out the threshold value for marking or reporting a transaction as fraudulent in your anomaly detection system.
Can this score be used as an engineered feature in the models developed previously? Are there any incremental gains in F1-Score? Why or Why not?
Be as creative as possible in finding other interesting insights.
