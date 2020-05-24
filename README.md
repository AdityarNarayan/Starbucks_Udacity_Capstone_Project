# Starbucks_Udacity_Capstone_Project

### Table of contents
1. [Installtion](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project#installation)
2. [Required Libraries](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project#required-libraries)
3. [Project Motivation](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project#project-motivation)
4. [File Description](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project#file-description)
5. [Model Observation](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project#model-observations)
6. [Conclusion](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project#conclusion)
7. [Medium Blog Post](https://medium.com/@adityananda14/data-science-project-analysis-of-starbucks-promotional-offers-b20d895fed7e)
 
### Installation
For running this project you need to install progressbar2 and XGBoost in your IDE terminal.

### Required Libraries
* Pandas
* Nampy
* Math
* Json
* Seaborn
* Progressbar2
* Matplotlib
* Sklearn
### Project Motivation
This project is the Capstone project of my Data Scientist nanodegree with Udacity. As students in the nanodegree, we have the option to take part in the Starbucks Capstone Challenge. For the challenge, Udacity provided simulated data that mimics customer behavior on the Starbucks rewards mobile app.

In this project, I use the data to answer 2 business questions:

1.  What are the main drivers of an effective offer on the Starbucks app?
2.  Could the data provided, namely offer characteristics and user demographics, predict whether a user would take up an offer or not?

### File Description
* Starbucks_Capstone_notebook.ipynb- Contains all the code related to this project
* Data- This contain the raw data portfolio(contains offer details), profile(Demographic information) and trasncript(contains transaction and offer events)
Note:- Above file are in json format
* transaction_offer_analysis.csv - Combined data of transaction , offers, profile and portfolio.

### Model Observations
Observations of the Model

Model ranking based on training data accuracy

1. RandomForestClassifier model accuracy: 0.944
2. XGBoost Classifier model accuracy: 0.916
3. LogisticRegression model accuracy: 0.877
4. Naive predictor accuracy: 0.472

Model ranking based on training data F1-score

1.RandomForestClassifier model accuracy: 0.942
2. XGBoost Classifier model accuracy: 0.913
3. LogisticRegression model accuracy: 0.865
4. Naive predictor accuracy: 0.641

Results suggest that the random forest model has the best training data accuracy and F1-score

### Conclusion

The problem that we have chose to solve was to build a model that predicts whether a customer will respond to an offer. Our strategy for solving this problem has mainly two steps. First, we combined offer portfolio, customer profile, and transaction data. Second, we assessed the accuracy and F1-score of a naive model that assumes all offers were successful. Third, we have compared the performance of logistic regression , random forest models and XGBoost Model. This analysis suggests that a random forest model has the best training data accuracy and F1-score. Analysis suggests that random forest model has a training data accuracy of 0.944 and an F1-score of 0.942. The test data set accuracy of 0.914 and F1-score of 0.910 suggests that the random forest model that we have constructed did not overfit the training data.

"Feature importance" refers to a numerical value that describes a feature's contribution to building a model that maximizes its evaluation metric. A random forest classifier is an example of a model that estimates feature importance during training. My analysis of the Starbucks Capstone Challenge customer offer effectiveness training data suggests that the top five features based on their importance are:

Offer difficulty (how much money a customer must spend to complete an offer)
Offer duration
Offer reward
Type of offer

### Blog_Post

I have also written a blog post which gives you a breif summary about my project.
https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project
