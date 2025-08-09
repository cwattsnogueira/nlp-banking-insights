# Banking Complaints – Sentiment Insights

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![NLP](https://img.shields.io/badge/NLP-VADER%20%7C%20TFIDF-orange.svg)]()
[![Status](https://img.shields.io/badge/Project-Completed-brightgreen.svg)]()

This project applies Natural Language Processing (NLP) and sentiment analysis to over **7,000 banking complaints** submitted in 2023. The goal is to help financial institutions identify pain points, product issues, and regional trends through data-driven insights.

## Objectives

- Clean and preprocess complaint text for semantic analysis
- Classify banking products using supervised models
- Apply sentiment analysis using VADER
- Generate interactive dashboards and exportable reports
- Deliver actionable insights for business stakeholders

## Technologies Used

- **Python**: pandas, numpy, scikit-learn, nltk, matplotlib, seaborn, plotly
- **Sentiment Analysis**: VADER (Valence Aware Dictionary and sEntiment Reasoner)
- **Text Vectorization**: TF-IDF
- **Modeling**: Naive Bayes, Logistic Regression
- **Visualization**: matplotlib, seaborn, plotly
- **Export**: HTML, PDF (via WeasyPrint)


## Project Structure

```
data/
├── banking_complaints_2023.csv

data_clean/
├── banking_complaints_2023_sentiment.csv

models/
├── nb_model.pkl
├── NLProcessingCourseEndProject.ipynb and nlprocessingcourseendproject.py

ploty_html/
├── (HTML visualizations)

png_html_pdf/
├── (Exported PNGs, HTMLs, PDFs)
```

## Pipeline Overview

### 1. Data Preparation

- Fill missing values in `State` and `ZIP`
- Tokenize, remove stopwords, lemmatize
- Convert text to TF-IDF matrix

### 2. Modeling

- Predict banking product using:
  - Naive Bayes (~56% accuracy)
  - Logistic Regression (~70% accuracy, handles imbalance)

### 3. Sentiment Analysis

- VADER applied to raw complaint descriptions
- Sentiment categories:
  - **Positive** (≥ 0.05)
  - **Negative** (≤ -0.05)
  - **Neutral** (between -0.05 and 0.05)

### 4. Business Insights

- Products with high negative sentiment
- Products with more praise than criticism
- States with elevated complaint rates
- Monthly sentiment trends

### 5. Visualizations

- Static charts (.png)
- Interactive dashboards (.html via Plotly)
- Exportable HTML and PDF reports

## Sample Visuals

- Sentiment Distribution by Product
- Negative Complaints by State
- Product Risk Bubble Chart
- Monthly Complaint Volume
- Sentiment Trends Over Time

## Key Insights

- **Checking accounts** and **Credit cards** show high complaint volume and negativity
- **Student loans** receive more positive than negative feedback
- States like **California** and **Florida** show elevated dissatisfaction
- Monthly spikes may reflect seasonal or regulatory changes

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/cwattsnogueira/nlp-banking-insights.git
   cd nlp-banking-insights


## Author
Carllos Watts-Nogueira, focused on transforming raw feedback into actionable insights.
Data Scientist 

• 	GitHub: @cwattsnogueira

• 	LinkedIn: linkedin.com/in/carlloswattsnogueira


