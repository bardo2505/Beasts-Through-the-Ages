# Beasts-Through-the-Ages
# 📚 Literary Animal Mentions Analysis

This project analyzes the historical and semantic representation of animals in literature using large-scale digitized text corpora.  
By combining temporal trends, sentiment analysis, and semantic embeddings, we explore how animals have been portrayed and how their symbolic and cultural roles have evolved over time.

---

## 📜 Data Sources

Our dataset integrates information from three complementary digital libraries:

1. **Google Books Ngram Viewer**  
   - Provides historical frequency data for individual animal terms from 1700 to 2000.
   - Used to filter and prioritize animals with sufficient historical coverage.

2. **Project Gutenberg**  
   - Offers full-text public domain books.
   - Extracted sentence-level context for animal mentions, with metadata such as title and publication year.

3. **Internet Archive**  
   - Provides additional English-language fiction texts beyond Gutenberg.
   - Supplemented the corpus with a broader variety of styles, dates, and contexts.
     

---

## 🐾 Animals Analyzed

The study focuses on **20 selected animals**, chosen for their historical prominence and diversity of symbolic meaning:

lion, eagle, raven, owl, cat, dog, snake,
deer, bat, rabbit, whale, shark, tiger,
panther, crocodile, monkey, wolf, fox, horse, dolphin



---

## 🧠 Methodology

### 1. Temporal Trends  
- Historical frequency trends from **Google Books Ngram Viewer** (1700–2000).  
- Identified broad patterns and anomalies in cultural prominence.

### 2. Sentiment Analysis  
- Used `cardiffnlp/twitter-roberta-base-sentiment` for fine-grained sentiment scoring (-1 to +1).  
- Measured affective framing of animals over time.

### 3. Sentence Embeddings  
- Generated semantic embeddings using **SBERT** (`all-MiniLM-L6-v2`, 384-dim).  
- Aggregated by `(animal, decade)` for diachronic analysis.

### 4. Clustering & Visualization  
- Applied **KMeans** (k=6) to detect semantic groupings.  
- Reduced dimensionality with **UMAP** for visualization.

---

## 📊 Key Insights
- Temporal spikes in mentions often correspond to historical or cultural shifts.
- Some animals (e.g., *dog*) maintain consistently positive sentiment.
- Others (e.g., *wolf*, *snake*) exhibit more negative sentiment trends.
- Clustering reveals thematic groupings of animals with similar symbolic roles.





