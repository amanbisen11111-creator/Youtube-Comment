# YouTube Comments Analysis

This repository contains Python scripts to analyze YouTube comments using **topic modeling**, **word cloud visualization**, and **n-gram frequency analysis**. The analysis helps to discover patterns, trends, and important topics from user comments.

---

## Features

1. **Topic Modeling**
   - Uses **TF-IDF Vectorization** and **NMF** to extract main topics.
   - Displays top words for each topic.
   - Works on large datasets of YouTube comments.

2. **Word Cloud Generation**
   - Generates word clouds for each discovered topic.
   - Visualizes the most important words in a clear, visual format.

3. **N-gram Analysis**
   - Calculates top **bigrams** (2-word sequences) and **trigrams** (3-word sequences).
   - Helps identify common patterns and repeated phrases in comments.

---

## Files

- `topic_modeling_wordcloud.py` – Performs topic modeling and generates word clouds.  
- `ngram_analysis.py` – Performs bigram and trigram frequency analysis.  
- `data/` – Folder to store your Excel files containing YouTube comments.

---

## How to Use

1. **Topic Modeling & Word Clouds**
   - Place your Excel file in the `data/` folder.
   - Update the `input_file_name` and `column_to_analyze` variables in the script.
   - Run the script:
     ```bash
     python topic_modeling_wordcloud.py
     ```
   - Output: console topics, bar plots, and word clouds.

2. **N-gram Analysis**
   - Place your Excel file with preprocessed text in the `data/` folder.
   - Update the file path and column name in the script.
   - Run the script:
     ```bash
     python ngram_analysis.py
     ```
   - Output: top 20 bigrams and trigrams.

---

## Requirements

- Python 3.9+
- Libraries:
```bash
pip install pandas matplotlib scikit-learn wordcloud openpyxl
