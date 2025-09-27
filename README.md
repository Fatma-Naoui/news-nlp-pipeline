# News NLP Pipeline

A classic NLP pipeline applied to news articles, covering **text preprocessing, tokenization, lemmatization, embeddings, and semantic analysis**. This project demonstrates how traditional NLP models like CBOW and Skip-gram compare with modern contextual embeddings like BERT.

---

## Dataset

The dataset used is the [Al Jazeera News Dataset](https://www.kaggle.com/datasets/oumaymael/aljazeera-news-dataset/), which contains news articles across multiple categories, including Economy, Science & Technology, and Sports.

---

## Project Pipeline

### 1. Data Understanding
- Load and inspect the dataset  
- Check for duplicates and missing values  
- Explore categories, titles, and article content  
- Perform initial exploratory analysis to guide preprocessing

### 2. Data Preprocessing
- Clean text by removing noise such as URLs, emails, emojis, hashtags, and promotional content  
- Tokenization and lemmatization of article text  
- POS tagging and Named Entity Recognition (NER) for additional insights

### 3. Embedding Generation
- Generate embeddings using:
  - **CBOW (Continuous Bag of Words)**  
  - **Skip-gram**  
  - **BERT**

### 4. Analysis
- Compare semantic similarity of words across embeddings  
- Evaluate differences between traditional and contextual embeddings  
- Highlight strengths and weaknesses of each approach

---
