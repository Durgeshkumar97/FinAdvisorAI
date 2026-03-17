# FinAdvisorAI: Generative AI for Personalized Financial Advising and Investment Strategies

![Python](https://img.shields.io/badge/Python-3.10-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow)
![Finance](https://img.shields.io/badge/Domain-Quantitative_Finance-darkgreen)
![XAI](https://img.shields.io/badge/Explainability-SHAP%20%7C%20LIME-red)

> A research-grade AI framework for stock trend forecasting, transformer-based financial reasoning, and explainable investment insight generation.

---

## Project Overview

**FinAdvisorAI** is an AI-driven financial intelligence system designed to combine:

* market forecasting
* transformer-based NLP
* explainable machine learning
* statistical feature diagnostics

to generate transparent and interpretable financial insights.

The project explores how modern AI architectures can support **personalized financial advisory systems** using structured market data and financial language modeling.

---

## Core Capabilities

| Capability              | Description                                                              |
| ----------------------- | ------------------------------------------------------------------------ |
| Multi-Model Pipeline    | LightGBM, XGBoost, Transformer regressors and classifiers                |
| Tabular-to-Text NLP     | Converts financial indicators into transformer-readable narratives       |
| Transformer Fine-Tuning | DistilBERT and DistilRoBERTa for financial classification and regression |
| Explainable AI          | SHAP and LIME feature attribution for transparent predictions            |
| Statistical Layer       | Granger causality and correlation analysis for feature influence         |
| Insight Generation      | Human-readable investment interpretation layer                           |

---

## Use Cases

* Retail investor signal dashboards
* Robo-advisory intelligence systems
* Financial research and experimentation
* Wealth-tech prototype development
* Explainable AI demonstrations in finance

---

## Tech Stack

### Language

* Python 3.10+

### Libraries

* pandas
* numpy
* scikit-learn
* matplotlib
* shap
* lime
* transformers
* keras
* xgboost
* lightgbm
* yfinance

### Models

* DistilBERT
* DistilRoBERTa
* Custom Transformer Encoder (Keras)

### Data

* NIFTY50 market data
* engineered technical indicators

---

## Repository Structure

```bash id="k9w3es"
FinAdvisorAI/
│
├── FinalThesisModeljune.ipynb               # Main notebook: model training and evaluation
├── Final_thesis_Durgesh_kumar_citaions.pdf  # Full thesis documentation
├── requirements.txt                         # Environment dependencies
├── README.md                                # Project documentation
```

---

## Model Architecture Highlights

### Feature Engineering

Technical indicators include:

* RSI
* MACD
* EMA
* Bollinger Bands
* Momentum
* VWAP
* Volume dynamics

### Tabular-to-Text Conversion

Structured market signals are transformed into textual financial narratives such as:

> "RSI is elevated, MACD indicates bullish crossover, and volume is increasing."

This allows transformer models to learn market states through language representations.

### Transformer Layer

Implemented using custom Keras transformer components with:

* positional encoding
* multi-head attention
* feed-forward blocks

### Explainability Layer

Predictions are accompanied by:

* SHAP global feature importance
* LIME local decision explanations

---

## Example Output

```text id="jfrx7q"
The model predicts a bullish move with 83% confidence.
Primary drivers: MACD crossover, low RSI, increasing volume.
SHAP identifies MACD and Bollinger Band width as dominant features.
```

---

## Performance Summary

| Model               | Task           | Metric                 | Notes                                                              |
| ------------------- | -------------- | ---------------------- | ------------------------------------------------------------------ |
| LightGBM            | Regression     | R² = 0.996             | Engineered feature benchmark using highly correlated market inputs |
| Transformer (Keras) | Regression     | R² = 0.987             | Sequence-based regression on temporal financial features           |
| DistilBERT          | Classification | F1 = 0.75 / AUC = 0.83 | Binary directional classification on generated financial text      |
| DistilBERT          | Regression     | R² = 0.952             | Regression using textualized financial indicator representation    |
| SHAP / LIME         | Explainability | Feature attribution    | Used for model transparency                                        |

> Metrics are reported on held-out evaluation data within the current experimental setup.

---

## Research Contributions

* Financial transformer adaptation for structured and textual signals
* Explainable AI integration for model transparency
* Tabular-to-text financial encoding pipeline
* Statistical feature dependency analysis

---

## Current Limitations

* Focused on NIFTY50 market environment
* Limited external sentiment integration
* Regulatory deployment layer not yet implemented
* Future evaluation should include stricter time-series validation

---

## Future Development

* Real-time news sentiment ingestion
* Social signal integration
* user-profile aware advisory engine
* multi-objective portfolio reasoning
* Streamlit / Flask deployment layer
* broader market coverage (US equities, ETFs, macro assets)

---

## How to Run

### Clone repository

```bash id="czj4al"
git clone https://github.com/Durgeshkumar97/FinAdvisorAI.git
cd FinAdvisorAI
```

### Create environment

```bash id="kg8qjk"
python -m venv venv
```

### Activate environment

**Linux / Mac**

```bash id="r1wzhu"
source venv/bin/activate
```

**Windows**

```bash id="8aq89n"
venv\Scripts\activate
```

### Install dependencies

```bash id="lx6l6e"
pip install -r requirements.txt
```

### Launch notebook

```bash id="9e2yhe"
jupyter notebook FinalThesisModeljune.ipynb
```

---

## Author

**Durgesh Kumar**
Independent Researcher — AI, Quantitative Finance, Financial Intelligence Systems

LinkedIn: https://www.linkedin.com/in/durgeshkumar3/
Email: [12duklan.durgesh@gmail.com](mailto:12duklan.durgesh@gmail.com)

---

## License

MIT License

---

## Research Reference

This repository is based on:

**Generative AI for Personalized Financial Advising and Investment Strategies**

---

If this work is useful in your research or development, a star is appreciated.


---

If this work is useful in your research or development, a star is appreciated.
