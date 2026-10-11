# Lab 9 – Named Entity Recognition (NER)

Entity detection and classification using spaCy.

- **Task 1:** Takes a sentence from the user and prints each entity with its label, start/end position, and explanation.
- **Task 2:** Fixed the missed and wrongly detected entities ("Abc & Co.", "Bcd LLC" as ORG), counted PERSON (1) and ORG (2), and visualized the result.
- **Task 3:** Fine-tuned `en_core_web_sm` on a custom example for 20 iterations, saved it as `custom_ner_model`, then loaded it to tag new sentences.

**Requirements:** `spacy`, `en_core_web_sm`

**Note:** Run Task 3 before the visualization cell that loads `custom_ner_model`.
