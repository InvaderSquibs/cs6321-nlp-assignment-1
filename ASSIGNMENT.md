# CS-6321 Natural Language Processing — Assignment 1: Text Preprocessing

**Student:** Zach Walton

## Overview

Modify in-class regex text cleaning and adapt a text-preprocessing pipeline. Starter code is from `inclass_lecture2_cs6321nlp_utahtechuniversity.py`. Submit as an individual `.py` or Jupyter notebook named `walton.py` / `walton.ipynb`.

## Requirements

### 1. Modify `remove_sp_char` (5 points)

Starting code (also in the in-class lecture file):

```python
import re

def remove_sp_char(text):
    pattern = r"[^a-zA-Z\s]"
    text = re.sub(pattern, "", text)
    return text
```

Modify the above code to:

- **a.** Allow an input parameter such as `keep_digits=True` or `keep_digits=False` (default `keep_digits=True`) and return the appropriate output.
- **b.** Process and return the correct output whether the input text is a **string** or a **list of strings**.

### 2. Modify the text preprocessing pipeline (5 points)

Review the Text Preprocessing code from the course materials / download. Modify the code to:

- **a.** Preprocess the **entire list of strings** instead of just one string (line).
- **b.** Use the output from (1) — the modified regex — to remove special characters and punctuation instead of `string.punctuation`.
- **c.** Do **spell correction before tokenization**.
- **d.** Use the **NLTK** library instead of spaCy:
  - `word_tokenize` from `nltk.tokenize` for tokens
  - WordNet Lemmatizer and stopwords from `nltk.corpus`

## Deliverables

- [ ] `walton.py` **or** `walton.ipynb` (well annotated)
- [ ] Acknowledge use of any AI coding assistant

## Notes / constraints

- Individual assignment.
- Test using the provided `sample_corpus` (also in the Text Preprocessing Python download).
- Default AI acknowledgment in the notebook: AI (Cursor) converted the assignment prompt into Jupyter scaffolding; graded work is the student’s unless noted.

## Source

Prompt captured for scaffolding. Student completes all graded work in the notebook.
