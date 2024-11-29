# CaseSummarizer

**CaseSummarizer** is a tool designed to preprocess legal or textual documents and generate concise summaries. This repository includes a sample input file, its pre-processed output, and the corresponding summary in the `sample` folder for reference.

---

## Features

1. **Preprocessing Documents**:
   - Tokenization
   - Lemmatization
   - Stopword removal

2. **Summarization**:
   - Generates summaries based on a provided dictionary and input text.
   - Allows flexible summary length as a fraction of the original text length.

---

## How to Use

### 1. Preprocess the Documents (Optional)

**Description**: Tokenizes the input text, performs lemmatization, and removes stopwords to prepare the data for summarization.

**Command**:
```bash
python preprocess.py path/to/input/folder/ path/to/output/folder/
## Generate Summaries

### a) Generate a Basic Summary
**Description**: Generates a summary using a provided dictionary file.

**Command**:
```bash
python summary.py path/to/input/folder/ path/to/output/folder/ path/to/dictionary.txt
### b) Generate a Length-Controlled Summary
**Description**: Creates a summary with a specified length as a fraction of the original text length.

**Command**:
```bash
python summary_length.py path/to/original/doc/folder/ path/to/summary/output/folder/ fraction/of/original/text/length
## Requirements

Ensure you have the following dependencies installed:

- Python 3.x
- Required libraries such as `nltk`, `pandas`, and others.

Install the dependencies using the following command:
```bash
pip install -r requirements.txt

