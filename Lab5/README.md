# Lab 5 — Text Representation

TF-IDF, cosine similarity, and Word2Vec (Skip-gram) embeddings.

## Tasks

| # | Task | Method |
|---|---|---|
| 1 | Cosine similarity between 4 sentences | `TfidfVectorizer` + `cosine_similarity` |
| 2 | Find important words in 3 sentences | `TfidfVectorizer` |
| 3 | Clean Simpsons dialogue, train embeddings | `gensim.Word2Vec(sg=1)` |
| 4 | Words similar to homer, marge, bart | `wv.most_similar()` |
| 5 | Odd one out in 3 character groups | `wv.doesnt_match()` |

## Notes

- Sentences 1 and 4 in Task 1 score 1.000 — punctuation and casing are stripped, so both become the same bag of words.
- `data` gets a low weight in Task 2 because it appears in every document.
- Word2Vec output varies per run; a `KeyError` means the word is below the vocabulary threshold.
