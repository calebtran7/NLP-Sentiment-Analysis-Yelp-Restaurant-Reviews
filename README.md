# NLP-Sentiment-Analysis-Yelp-Restaurant-Reviews

This NLP project aims to automatically analyze the sentiment of restaurant reviews from Yelp using two different approaches: the VADER Bag of Words approach and a pre-trained RoBERTa model from Hugging Face. I also incorporate a Naive Bayes Model to classify the reviews as either positive or negative.

### Table of Contents
1. Introduction
2. Data Collection
3. Data Preprocessing
4. VADER Bag of Words Approach
5. Naive Bayes Classification Model
6. RoBERTa Pretrained Model
7. The Transformers Pipeline
8. Conclusion

### 1. Introduction
Yelp is a popular platform where users can share their experiences and opinions about various restaurants. This project focuses on sentiment analysis, which involves determining whether a restaurant review conveys positive, negative, or neutral sentiments. The goal is to provide valuable insights to restaurant owners and potential customers based on the sentiment analysis of the reviews.

### 2. Data Collection
Link to dataset: https://www.kaggle.com/datasets/farukalam/yelp-restaurant-reviews

The dataset includes reviews, ratings, and other relevant information. Note that the dataset used for this project has been anonymized and doesn't contain any identifiable user information.

### 3. Data Preprocessing
Before applying sentiment analysis, the raw data is preprocessed to handle noise, remove irrelevant information, tokenize the text, and perform other necessary tasks to prepare it for the models' input format.

### 4. VADER Bag of Words Approach
The VADER (Valence Aware Dictionary and sEntiment Reasoner) Bag of Words approach is a lexicon-based sentiment analysis method. It uses a pre-built sentiment lexicon to score each word in the review and aggregate the scores to predict the overall sentiment of the text.
VADER Results plotted:
![image](https://github.com/calebtran7/NLP-Sentiment-Analysis-Yelp-Restaurant-Reviews/assets/121086856/736d41cb-7420-410b-a626-834f3703e0f8)

### 5. Naive Bayes Classification Model
I developed and implemented a Naive Bayes model that classifies the reviews as either positive or negative, according to their VADER compound score. 
The NB model ultimately achieved an accuracy of 0.86. 

### 6. RoBERTa Pretrained Model
RoBERTa, developed by Facebook AI, is a powerful transformer-based language model. I leveraged a pre-trained RoBERTa model from Hugging Face's transformers library, fine-tuned on our Yelp restaurant review dataset for sentiment analysis.

### 7. The Transformers Pipeline
The Transformers Pipeline is a powerful and user-friendly feature provided by Hugging Face's transformers library, which simplifies the process of using pre-trained language models for various NLP tasks, including sentiment analysis. By specifying the task as "sentiment-analysis," the pipeline automatically tokenizes the input text, feeds it to the RoBERTa model, and generates sentiment predictions for each review.

### 8. Conclusion
The Yelp Restaurant Review Sentiment Analysis project provides valuable insights into the sentiments expressed in restaurant reviews using two different approaches. Users can choose between the VADER Bag of Words approach, which is computationally efficient and lexicon-based, or the more sophisticated RoBERTa pretrained model, which may yield more accurate results at the cost of increased computational requirements.
