# Lab 10 Machine Translation (English to French)

An LSTM encoder decoder model that translates English sentences to French for an e-commerce use case

## Dataset
Kaggle Language Translation English-French downloaded with kagglehub
40,000 short sentence pairs were sampled after removing duplicates

## Model
Embedding with masking then a Bidirectional LSTM encoder then RepeatVector then an LSTM decoder with Dropout and a softmax output layer
Trained with Adam and EarlyStopping on validation loss

## Results
Test accuracy 0.68
The model gets the sentence structure right most of the time but still confuses some rare words

## How to run
Open the notebook in Colab and run all cells in order
