# Patient-Feedback-Analysis-Using-NLP-and-LLMs
Analyzing patient feedback using NLP and LLMs to extract topics, detect sentiment, and generate actionable insights for healthcare management.

Analyze patient reviews to identify themes, sentiment, and actionable insights using **NLP topic modeling (BERTopic)** and **LLM-driven topic extraction (Falcon-7B-Instruct)**. Features data preprocessing, sentiment filtering, topic extraction, visualization, and AI-augmented summarization for healthcare decision-making.

## Project Overview

This project applies **advanced NLP and Large Language Models (LLMs)** to extract insights from patient feedback collected from Google and Trustpilot. It combines **unsupervised topic modeling (BERTopic)** with **instruction-based LLM topic extraction**, generating structured, human-readable themes from unstructured text. The analysis helps hospitals identify recurring issues, patient pain points, and areas for service improvement.

The project demonstrates skills in text preprocessing, sentiment analysis, topic modeling, LLM application, visualization, and actionable insights generation.

## Data

**The dataset includes 10,000 synthetic patient reviews (5,000 from Google, 5,000 from Trustpilot), with review text, star rating (1–5), and hospital location.**

**Negative reviews (<3 stars) are filtered for focused analysis.**

**All data is synthetic for demonstration purposes. No real hospitals or patients are represented.**

## Approach

### Data Preprocessing and Cleaning

* Remove missing or empty reviews
* Standardize text (lowercasing, punctuation removal)
* Remove stopwords and numbers
* Tokenize reviews for analysis
* Filter by sentiment and hospital location

### Topic Modeling with BERTopic

* Merge Google and Trustpilot negative reviews
* Apply BERTopic to extract unsupervised topics
* Visualize topic distributions, keywords, and inter-topic relationships
* Identify recurring location-specific concerns

### LLM-Driven Topic Extraction

* Use **Falcon-7B-Instruct** via Hugging Face Transformers
* Generate top 3 topics per review using instruction-based text generation
* Normalize topics into consistent categories (e.g., “Staff Behavior,” “Waiting Times”)
* Aggregate insights across hospitals to detect common pain points

### Classical Topic Modeling with Gensim

* Preprocess text using NLTK: stopword removal, tokenization, lemmatization
* Build a Gensim dictionary and corpus from negative patient reviews
* Train a Gensim LDA model to extract 10 baseline topics
* Analyze top words per topic to understand recurring patient concerns
* Provides a benchmark for comparing unsupervised BERTopic and LLM-driven topic extraction

### Visualization and Insights

* Topic frequency counts and heatmaps
* Location-specific analysis of recurring issues
* Structured summaries for decision-making

## Key Skills Demonstrated

* NLP for topic modeling and sentiment analysis (**BERTopic**, preprocessing, visualization)
* Large Language Model application for structured information extraction (**Falcon-7B-Instruct**)
* GPU-accelerated NLP processing and memory optimization
* Combining traditional NLP and LLM approaches for richer insights
* Translating unstructured text into actionable business intelligence for healthcare operations
