# Starbucks_Udacity_Capstone_Project

### Table of contents
1. [Installtion](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project#installation)
2. [Required Libraries](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project#required-libraries)
3. [Project Motivation](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project#project-motivation)
4. [File Description](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project#file-description)
5. [Model Observation](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project#model-observations)
6. [Conclusion](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project#conclusion)
7. [Medium Blog Post](https://medium.com/@adityananda14/data-science-project-analysis-of-starbucks-promotional-offers-b20d895fed7e)
8. [Referrence](https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project/blob/master/README.md#referrence)
 
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

1. RandomForestClassifier model accuracy: 0.913
2. XGBoost Classifier model accuracy: 0.912
3. LogisticRegression model accuracy: 0.877
4. Naive predictor accuracy: 0.472

Model ranking based on training data F1-score

1.RandomForestClassifier model accuracy: 0.911
2. XGBoost Classifier model accuracy: 0.910
3. LogisticRegression model accuracy: 0.865
4. Naive predictor accuracy: 0.641

Results suggest that the random forest model has the best training data accuracy and F1-score

### Conclusion

We have chosen two questions to answer in this project:

1. What are the main drivers of offer effectiveness?
2. Explore if we can predict whether a user would take up an offer?

We have performed many steps to answer the above questions but most crucial steps was to analysing the data, combining the dataframes( portfolio, offer_df, transaction_df and profile), building the model and assessing our model with the help of metrics that is accuracy and f1 score.

To answer the first question we have used Heat map which provided us the effective drivers which are played a vital role in our model prediction. Those effective drivers are given below.

1. Offer difficulty
2. Offer duration
3. Offer reward
4. Type of offer

To answer the 2nd question we have used machine learning models like Naive Predictor, Logestic Regression, RandomForest Classifier and XGBoost classifier. From the analysis we come to know that random forrest clasifier has the slightly better acuuracy but f1 score is same for both models. However, Random Forest took 30 minutes to compute the results so as a alternative I have use XGBoost model to predict the result with almost same accuracy and f1score. We have pridicted the result of test set with the accuracy and f1 score of 91% which suggest that our model is not over fitted.

However there is always a room for improvement since the most of the effective drivers are related to offers hence those who wants to improve the model can use different features like succes rate vs difficulty ratio or difficulty vs duration of offers to improve Randomforest model.

### Blog_Post

I have also written a blog post which gives you a breif summary about my project.
https://github.com/AdityarNarayan/Starbucks_Udacity_Capstone_Project

### Referrence

I took some refference from this blog post for my project and have immprove the model accuracy score from 76% to 91%.
https://medium.com/@susmitha.gudapati/starbucks-capstone-challenge-7dd19432c481
