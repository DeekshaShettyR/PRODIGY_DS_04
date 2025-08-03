# Task 4: Sentiment Analysis on Twitter Data 🐦

This project performs sentiment analysis on tweets using the **VADER (Valence Aware Dictionary and sEntiment Reasoner)** model from NLTK. The goal is to understand public opinion and attitudes toward various entities by analyzing the tone of tweets.

---

## 📁 Dataset

- **Name:** `twitter_training.csv`
- **Source:** [Prodigy InfoTech GitHub - Task 4](https://github.com/Prodigy-InfoTech/data-science-datasets/tree/main/Task%204)
- **Columns:**
  - `tweet_id` – Unique ID for each tweet
  - `entity` – Subject/brand the tweet is about
  - `sentiment` – Original labeled sentiment (not used in scoring)
  - `content` – Actual tweet text

---

## 📊 Key Tasks Performed

### 🔹 1. Preprocessing
- Removed nulls
- Ensured all content is string

### 🔹 2. Sentiment Scoring
- Used `nltk.sentiment.vader.SentimentIntensityAnalyzer` to get compound scores
- Classified sentiment as:
  - **Positive** (compound ≥ 0.05)
  - **Negative** (compound ≤ -0.05)
  - **Neutral** (otherwise)

### 🔹 3. Visualization (saved in `charts/` folder)

| Chart                           | Description                               |
|--------------------------------|-------------------------------------------|
| `sentiment_distribution.png`   | Bar chart of predicted sentiment labels   |
| `sentiment_by_entity.png`      | Top 5 entities and their sentiment spread |
| `compound_score_distribution.png` | Histogram of sentiment scores         |

---

## 📁 Folder Structure

