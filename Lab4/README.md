# Lab 4 — Classification and Evaluation in NLP

Sentiment analysis on text reviews: turn star ratings into positive/negative/neutral labels, then train and evaluate a classifier.

## Contents
- **Disney example** — TF-IDF + SVM on Disneyland reviews (worked through in class).
- **Amazon use case** — 6 tasks on Amazon unlocked-phone reviews: preprocess, split, TF-IDF, Naive Bayes, evaluate, confusion matrix.

## Data
Loaded via `kagglehub` (no manual download):
`kagglehub.dataset_download("PromptCloudHQ/amazon-reviews-unlocked-mobile-phones")`

## Run
Open in Colab and run cells top to bottom. If needed: `!pip install -q kagglehub nltk`.
