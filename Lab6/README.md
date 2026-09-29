LAB 6 - Deep Learning for NLP (Yelp Sentiment)
 
Run: !pip install gensim, then run all cells top to bottom.
 
Task 1: Word2Vec (vector_size=200, window=5, min_count=1, sg=1, epochs=100)
        trained on train reviews; each review = average of its word vectors.
Task 2: 200 -> 128 -> 64 -> 32 -> 1, ReLU, BCEWithLogitsLoss,
        Adam lr=0.001, 15 epochs.
 
Result: about 62-66% test accuracy (TF-IDF baseline: 75.5%).
Low because full-batch training with 15 epochs gives only 15 updates,
and 800 reviews is too little data for Word2Vec.
 
Fixes: added optimizer.zero_grad(); applied preprocess_text when tokenizing.
