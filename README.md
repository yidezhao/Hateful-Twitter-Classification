# Hateful-Twitter-Classification

# Introduction
This project works on the "users_neighborhood_anon.csv" dataset trying to answer the question about who is more likely to be a hateful user. Out of the 100k dataset, only 5k are labeled with either "hateful" or "normal". Thus, by successfully training a good model for the classification task, I will able to make good judgements and predictions for unlabeled data points. Note here that the data exists a class inbalance with way more normal users than hateful users. I use pure logistic regression, naive PCA with logistic regression, featured PCA with logistic regression (proposed in this paper) and decision tree as possible candidate models. Due to the class inbalance, F1 score (combination of recall and precision) and AUC for the ROC curve are used as evaluation method. By a conbination of both unsurpervised and supervised models, the paper aims to identify hateful users on Twitter and create a more harmonious environment. 

# Model
1. Logistic regression \\
2. Logistic regression with naive PCA \n
3. Logistic regression with featured PCA (BEST)
4. Decision Tree
5. XG-boost

# Conclusion
In this study, we examine the Twitter user dataset aiming to identify hateful users in the unlabeled data. Models are trained in a supervised setting with the 5k labeled data. The best model is the featured PCA with AUC being 0.9778 and F1 score being 0.71. I also testify the hypothesis that having a hateful neighbor is an important feature in predicting hateful Twitter users. Along the analysis, I also find many other interesting features like hearing_empath and furniture_empath. This study hope to use trained model to predict hateful users on Twitter and prevent the spread of inappropriate message at the earliest stage, creating a harmonious environment. 
