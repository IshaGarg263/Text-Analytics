# 📰 Sentiment Analysis & Stock Prediction Dashboard

An interactive Streamlit dashboard covering sentiment analysis, stock return prediction, and a four-way model comparison: ARIMA, SARIMA, Regression (price-only), and Regression with sentiment features. Built for the **Global MBA (GMBA)** program at **SP Jain School of Global Management**.

[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://your-app-name.streamlit.app)

---

## Overview

This dashboard demonstrates how text sentiment from financial news can be quantified and used alongside time series and regression models for stock return prediction. All data is synthetic and generated automatically — no setup, API keys, or external files required.

---

## Sections

| # | Section | Description |
|---|---------|-------------|
| 1 | **Home & Overview** | Workflow, dataset preview, key statistics |
| 2 | **Sentiment Analysis Theory** | Lexicon-based, VADER, and ML approaches with examples |
| 3 | **Dataset Exploration** | Candlestick chart, return distribution, news headlines browser |
| 4 | **Sentiment Scoring Demo** | Type any text and see Lexicon, VADER, and TextBlob scores with word-level matching |
| 5 | **Sentiment Visualizations** | Sentiment over time, distribution, scatter vs returns, rolling averages |
| 6 | **Stock Prediction — Without Sentiment** | Regression model using only price-based technical features |
| 7 | **Stock Prediction — With Sentiment** | Same model with sentiment features added (with look-ahead bias prevention) |
| 8 | **ARIMA/SARIMA on Stock Data** | Interactive p,d,q and P,D,Q,s parameter selection; ACF/PACF analysis; stationarity testing |
| 9 | **Head-to-Head: All Models** | Four-way comparison — ARIMA vs SARIMA vs Regression vs Reg+Sentiment — metrics, charts, verdict |
| 10 | **Summary & Takeaways** | Concept reference, method comparison, evaluation metrics, limitations |

---

## Getting Started

### Run Locally

```bash
git clone https://github.com/your-username/sentiment-stock-dashboard.git
cd sentiment-stock-dashboard

pip install -r requirements.txt
python -c "import nltk; nltk.download('vader_lexicon')"

streamlit run sentiment_dashboard.py
```

### Deploy on Streamlit Cloud

1. Push this repo to GitHub
2. Go to [share.streamlit.io](https://share.streamlit.io) → sign in → **New app**
3. Select repo → set main file to `sentiment_dashboard.py` → **Deploy**

---

## Repository Structure

```
sentiment-stock-dashboard/
├── sentiment_dashboard.py   # Streamlit application
├── requirements.txt         # Python dependencies
├── nltk.txt                 # Auto-downloads VADER lexicon on Streamlit Cloud
└── README.md
```

---

## Dependencies

| Package | Purpose |
|---------|---------|
| `streamlit` | Dashboard framework |
| `pandas` / `numpy` | Data manipulation |
| `plotly` | Interactive charts |
| `statsmodels` | ARIMA, SARIMA, ACF/PACF, ADF test |
| `scikit-learn` | Regression models and accuracy metrics |
| `scipy` | Statistical analysis |
| `nltk` | VADER sentiment analysis |
| `textblob` | Alternative sentiment scoring |

---

## Author

**Dr. Anshul Gupta**
Associate Professor & Area Head — Technology Management
SP Jain School of Global Management

---

<p align="center">
  <em>Built with ❤️ for the Global MBA Program</em>
</p>
