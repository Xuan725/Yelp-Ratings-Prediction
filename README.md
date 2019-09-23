# Yelp-Ratings-Prediction

![alt text](https://github.com/Taniesta/Yelp-Ratings-Prediction/blob/master/wordcloud.png)

Predict Yelp ratings using reviews and restaurants information
The project aims to combine information from restaurants and their reviews to predict whether the rating of a restaurant is greater than or equal to 4. Codes, slides and the paper are posted along with the data in this repository.

## Yelp Reviews EDA and Text Mining
This notebook is for Review EDA and feature extraction from reviews. Considering the large number of reviews from 2000 restaurants, we did sampling to get more than 60k reviews from the restaurants. The Wordcloud and LDA model were created, and then TF-IDF was used to extract features. Here we tried 2 types of features. The first one is using principal components based on 1000 keywords tf-idfs, while the second one contains features from 100 key words without PCA.

## Business Cleaning and EDA
In this notebook, business dataset was cleaned and joined with reviews features. EDA was conducted based on processed data.

## Modelling
This notebook is about creating models to predict restaurants' ratings based on information from business and reviews. The target is whether the rating is greater than or equal to 4. For the reviews, we tried PCs from 1000 words tfidf and tfidfs from 100 words without PCA. Logistic Regression and Gradient Boosting were built, and they achieved similar performances, with AUC around .90.

## paper
Details, results and insights of the projected can be found in the paper.

![alt text](https://github.com/Taniesta/Yelp-Ratings-Prediction/blob/master/auc.png)
