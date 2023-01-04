![Amazon Product](https://drive.google.com/uc?export=view&id=13b8hPFhv7eYy1EVTNuj5xFd9YDJaCD9a)
# Sentiment Analysis Case Study on Amazon Reviews

This is a case study on sentiment analysis of Amazon reviews using three different approaches:
1. Bags of words approach with VADER (Valence Aware Dictionary and sEntiment Reasoner)
2. Huggingface's RoBERTa (Robustly Optimized BERT) pretrained model
3. Transformers library

The case study compares the results of these approaches and discusses their strengths and weaknesses.

## Requirements
The case study requires the following dependencies:
- pandas
- nltk
- vaderSentiment
- transformers
- torch

## Data
The Amazon review data used in this case study is a sample of 500 reviews taken from the [Amazon Fine Food Reviews](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews) dataset on Kaggle. The data consists of the following columns:
- Id: Row Id
- ProductId: The product id
- UserId: The user id
- ProfileName: Profile name of the user
- HelpfulnessNumerator: Number of users who found the review helpful
- HelpfulnessDenominator: Number of users who indicated whether they found the review helpful or not
- Score: The rating given by the user (1-5)
- Time: Timestamp of the review
- Summary: Brief simmary of the review
- Text: The review text

## Conclusion
<br>The Transformers approach performed the best, followed by RoBERTa and then VADER. However, all three approaches had similar performance, with the differences being small.<br/>

One limitation of the VADER approach is that it is based on a pre-defined dictionary of sentiment-laden words, which may not always accurately capture the sentiment of a review. The RoBERTa and Transformers approaches, on the other hand, are able to capture the context and syntax of the review, which may give them an advantage in accurately classifying the sentiment.
