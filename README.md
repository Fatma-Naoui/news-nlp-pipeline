# News NLP Pipeline

A classic NLP pipeline for processing and analyzing news articles. This project demonstrates **text cleaning, tokenization, lemmatization, embeddings (CBOW, Skip-gram, BERT), and similarity analysis** on a real-world news dataset.

---

## Overview

This repository provides a step-by-step **NLP workflow** for news articles. The pipeline handles:

- Cleaning raw text (removing URLs, emails, emojis, hashtags, social media artifacts, and other noise)
- Tokenization and lemmatization
- POS tagging and Named Entity Recognition (NER)
- Generating word embeddings using CBOW, Skip-gram, and BERT
- Similarity analysis between words and articles

---

## Dataset

We use the **Al Jazeera News Dataset** from Kaggle:  
[https://www.kaggle.com/datasets/oumaymael/aljazeera-news-dataset/](https://www.kaggle.com/datasets/oumaymael/aljazeera-news-dataset/)

The dataset contains:

- `category`: news category (Economy, Science & Technology, Sports)  
- `title`: news article title  
- `article_content`: main body of the article  

---

## Data Understanding

- Number of articles: 4439  
- Categories distribution: Economy (1532), Science & Technology (1493), Sports (1413)  
- Article length statistics: Mean 590 words, Min 16, Max 4738 words  
- Title length statistics: Mean 58 characters, Min 13, Max 68 characters  

Exploratory analysis includes category distribution, article length, and duplicate detection/removal.

---

## Pipeline

1. **Text Cleaning:** Remove HTML, URLs, emails, hashtags, emojis, and promotional phrases.  
2. **Tokenization:** Split articles into meaningful words.  
3. **Lemmatization:** Convert tokens to their base forms using spaCy.  
4. **Stemming:** Optional stemming using NLTK’s Porter Stemmer.  
5. **POS Tagging:** Identify parts of speech.  
6. **NER:** Extract named entities.  
7. **Embedding Generation:** Prepare corpus for CBOW, Skip-gram, and BERT embeddings.  
8. **Similarity Analysis:** Compare word embeddings across models.

---

## Embedding Models

- **CBOW (Continuous Bag of Words):** Predicts a word given its surrounding context, efficient for frequent words.  
- **Skip-gram:** Predicts surrounding words given a word, better for rare words.  
- **BERT:** Contextual embeddings capturing semantics from entire sentences and their context.

---

## Results

- Word similarity examples highlight differences: Skip-gram captures rare words, BERT captures contextual meaning, CBOW is faster for common words.  
- Overall, contextual embeddings (BERT) provide richer semantic relationships than traditional Word2Vec models.

