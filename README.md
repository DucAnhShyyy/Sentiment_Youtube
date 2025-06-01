# 📊 YouTube Comment Sentiment Analysis (Vietnamese Channel)

This project aims to analyze and predict the sentiment of comments from YouTube viewers on a Vietnamese video. It serves three key purposes:

- **For users**: Helping them choose suitable content to watch.  
- **For content creators**: Providing insights to improve video quality and attract more viewers.  
- **For YouTube platform**: Assisting in detecting potentially problematic channels or videos.

> **Note**: The entire project was developed in a Jupyter Notebook (`.ipynb`) format.

---

## 🔍 Project Overview

- **Scope**: Focused on Natural Language Processing (NLP) and sentiment prediction techniques.
- **Data Source**: Comments were collected from **one video**, not the entire channel (but the framework is customizable).
- **Duration**: **2 weeks** — from data collection to model evaluation and insights generation.
- **Role**: A solo project, fully executed by myself, covering all technical and analytical aspects including planning, data collection, preprocessing, EDA, model building, and summary comparison.

---

## 🛠️ Tools & Methodologies

- **Programming Language**: Python  
- **Libraries**: `scikit-learn`, `NLTK`, `pandas`, `matplotlib`, `Gemini API`  
- **NLP Techniques**:
  - Text cleaning (removing emojis, stopwords, converting numbers to words)
  - Tokenization
  - Lemmatization
  - Vectorization
- **Sentiment Analysis Methods**:
  - Lexicon-based approach
  - Machine Learning models (Naive Bayes, SVM, Decision Tree, Random Forest)
  - LLM-based sentiment prediction using Gemini API (prompt-based only)

---

## 📈 The Approach and Process

### 1. **Data Collection**
- Utilized YouTube Data API via Google Cloud Console.
- Extracted `video ID`, `comment text`, and `author` using Python.
- Data saved in CSV format.
- Tested auto-refresh by setting a 2-minute timer to simulate updates.

### 2. **Exploratory Data Analysis**
- Analyzed average comment length, most common words, and N-grams.
- Helped identify key repeated terms and phrases used by viewers.

### 3. **Preprocessing & Feature Engineering**
- **Tokenization**: Splitting text into basic units (tokens).
- **Lemmatization**: Reducing words to their base/dictionary form.
- **Vectorization**: Converting text into numeric vectors for ML models.

### 4. **Machine Learning Modeling**
- On a small test dataset (~100 comments), SVM underperformed.
- On the real dataset, SVM surprisingly performed well.
- Tree-based models like **Random Forest** and **Decision Tree** consistently achieved high accuracy.
- **Naive Bayes** performed fairly but struggled with slang and abbreviations.

### 5. **LLM Integration**
- Used Gemini API (Google’s Large Language Model) for prediction.
- Crafted prompts to get desired outputs — no fine-tuning involved.
- Showed strong capability in handling informal and freestyle text data.

### 6. **Lexicon-Based Approach**
- Implemented rule-based sentiment prediction using sentiment dictionaries.
- Did not perform well due to the unpredictable nature of YouTube comment language.

---

## ✅ End Results and Recommendations

### Strategic Recommendations
- Lexicon-based approaches are limited for unstructured, informal comments.
- Machine Learning and LLMs are more effective but may lack interpretability.
- Always assess the text format and context before selecting an analysis method.

### Outcomes
- Confirmed that modern sentiment analysis tools can understand context well.
- Built a flexible pipeline that can scale to more videos or entire channels.

---

## 🚀 Future Development

- Automate rule generation and data labeling processes.
- Fine-tune pre-trained transformer models like **BERT** for Vietnamese.
- Use data augmentation methods such as back-translation for training.

---

## 📎 Repository Access

To explore the code, data, and notebook in detail, visit the GitHub repo:  
👉 [GitHub Repository](https://github.com/DucAnhShyyy/Sentiment_Youtube)

---
