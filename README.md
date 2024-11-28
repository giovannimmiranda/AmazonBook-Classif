# Amazon Book Reviews Classifier

## Project Overview

This project involves the analysis of a dataset containing Amazon book reviews to develop a model capable of:
	1.	Predicting book ratings (1–5 stars) based on textual reviews.
	2.	Performing sentiment analysis as a multi-class text classification task.

Using advanced Natural Language Processing (NLP) techniques and deep learning models, the goal was to reliably classify reviews into their corresponding rating categories.

## Dataset

- Source: [Kaggle - Amazon Book Reviews Dataset](https://www.kaggle.com/datasets/mohamedbakhet/amazon-books-reviews).
- Size: 3,000,000 rows and 10 features.
- Key features used:
  - review/text: Textual content of reviews.
	- review/score: Numerical ratings (1–5 stars).

## Challenges:

- Imbalanced data with a predominance of 5-star reviews.
- Addressed via undersampling to balance classes.

## Methodology

- Data Preprocessing
- Model Architecture:
  - Bidirectional LSTM for capturing sequential patterns in text.
	- Embedding layer for text vectorization.
  - Dropout layers to reduce overfitting.
	- Fully connected layers for classification.
- Training Details:
  - Loss Function: Cross-Entropy.
	- Optimizer: Adam with a custom learning rate scheduler.
  - Regularization: Dropout with a 0.5 rate.
  - Early stopping to prevent overfitting.

## Results

- Achieved robust accuracy on training and validation sets.
- Early stopping at optimal epoch prevented overfitting.
- Confusion matrix analysis highlighted minor misclassification errors, primarily within adjacent rating classes.

## Conclusion

The project demonstrates the potential of deep learning for sentiment analysis and multi-class classification. Despite challenges like dataset imbalance and ambiguous human-labeled reviews, the model achieved satisfactory results, providing a foundation for future improvements.
