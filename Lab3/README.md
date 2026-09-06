# N-Gram Tweet Generation Lab

This lab builds a **Bigram Maximum Likelihood Estimation (MLE) language model** using tweets from Pakistan.

## Dataset

Kaggle dataset:

`adizafar/large-random-tweets-from-pakistan`

The dataset is loaded using **KaggleHub**.

## Preprocessing

The tweets are cleaned by removing:

- Hashtags
- RT
- URLs
- Mentions
- Emojis

The text is also converted to lowercase.

## Model

The cleaned tweets are tokenized and used to train a **Bigram MLE model** using NLTK.

Padding is added using:

`padded_everygram_pipeline()`

## Tasks

- Load and clean the dataset
- Build a Bigram MLE model
- Generate a tweet
- Evaluate the model using perplexity
- Calculate the probability of `(pakistan is)`
- Calculate the perplexity of `pakistan`

## Libraries

- `pandas`
- `nltk`
- `emoji`
- `kagglehub`

## Note

MLE does not use smoothing, so unseen bigrams may have probability `0`, which can result in infinite perplexity (`inf`).
