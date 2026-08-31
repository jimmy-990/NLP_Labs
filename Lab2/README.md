# Lab 2: Text Pre-processing & Regular Expressions

## Tasks
- **Task 1** – Count all hashtags in the Apple tweets dataset and print the top 10 (`re.findall(r"#\w+")` + `Counter.most_common`).
- **Task 2** – Use `re.compile()` to compile a digit pattern, print its type, replace 2021 with 2022.
- **Task 3** – Use `re.split()` to split a string on digits.
- **Task 4** – Tokenize a sentence with spaCy and compare to NLTK's `word_tokenize`.

## Dataset (Task 1)
Loaded from Kaggle via kagglehub:
```python
path = kagglehub.dataset_download("seriousran/appletwittersentimenttexts")
df = pd.read_csv(os.path.join(path, "apple-twitter-sentiment-texts.csv"))
```

## Notes
- New NLTK versions need `punkt_tab` and `wordnet` — download them or you'll get a `LookupError`.
- If `spacy.load` fails, run the spaCy download line, then Restart Kernel.
- Use `.discard()` instead of `.remove()` on stop-word sets to avoid `KeyError`.
