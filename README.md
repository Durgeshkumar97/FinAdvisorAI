# FinAdvisorAI: Generative AI for Personalized Financial Advisory and Stock Trend Prediction

![Python](https://img.shields.io/badge/Python-3.10-blue)
![License](https://img.shields.io/badge/License-MIT-green)

> A cutting-edge AI system that combines deep learning, generative AI, and explainable ML to deliver **transparent, personalized investment insights** based on market trends and financial indicators.
> 
## Project Overview
**FinAdvisorAI** is a research-grade intelligent system designed to:
- Predict **stock market trends** using deep learning (NIFTY50 index as base)
- Generate **natural language investment insights** using tabular-to-text + transformer models (BERT, RoBERTa)
- Ensure **interpretability** using SHAP & LIME explanations
- Lay the foundation for **personalized, AI-powered financial advisory tools**
  
## Core Features

| Feature                                 | Description                                                            |
|-----------------------------------------|------------------------------------------------------------------------|
|  **Multi-Model Pipeline**            | LightGBM, XGBoost, RNNs, Transformer regressors and classifiers        |
|  **Tabular-to-Text NLP**             | Converts financial indicators to textual summaries for LLM fine-tuning |
|  **Transformer Fine-Tuning**         | Uses DistilBERT & RoBERTa for classification and regression on text    |
|  **Explainable AI (XAI)**            | SHAP and LIME explanations for transparent predictions                 |
|  **Business Insights Layer**         | Generates human-readable investment suggestions                        |
|  **Granger Causality + Correlation** | Statistically detects influential indicators                           |

##  Use Cases:
-  **Retail Investor Dashboard** (e.g. signal strength, risk alerts)
-  **Robo-Advisory Tools** (personalized advice for goal-based investing)
-  **B2B Integrations** (plug into wealth management platforms)
-  **Academic / Research Tool** (for finance + AI studies)

## Tech Stack:
- **Language:** Python 3.10+
- **Libraries:** 'pandas', 'numpy', 'scikit-learn', 'matplotlib', 'shap', 'lime', 'transformers', 'keras', 'xgboost', 'lightgbm', 'yfinance'.
- **Models:** DistilBERT, DistilRoBERTa, Transformer encoder from scratch
- **Data Sources:** NIFTY50 stock data + financial indicators

## How to Run:

### 1. Clone this repo:
bash
git clone https://github.com/Durgeshkumar97/LJMU_Research1.git
cd LJMU_Research1

### 2. Install dependencies:
bash
pip install -r requirements.txt

-> You may want to create a virtual environment:
bash
python -m venv venv
source venv/bin/activate  
# or venv\Scripts\activate on Windows

### 3. Launch the notebook:
bash
jupyter notebook FinalThesisModeljune.ipynb

## File Structure:

LJMU_Research1/

├── FinalThesisModeljune.ipynb               # Main Jupyter notebook model training and evaluation

├── Final_thesis_Durgesh_kumar_citaions.pdf  # Full research thesis with citations

├── requirements.txt                         # Python dependencies for full environment setup

├── README.md                                # Project overview and documentation (this file)

## Model Architecture Highlights:
* **Tabular Feature Extraction**: RSI, MACD, EMA, Bollinger Bands, Momentum
* **Transformer Encoder**: Built using Keras with Positional Encoding & Multi-Head Attention
* **DistilBERT Fine-Tuning**: Textual input created from features like:
  *"RSI is high, MACD shows bullish crossover..."*
* **XAI Layer**: SHAP values and LIME interpretations output alongside each prediction

## Sample Output:
Example:
> *The model predicts a bullish move with 83% confidence.*
> *Reason: MACD crossover, low RSI, and increasing volume.*
> *Explanation: SHAP indicates MACD and Bollinger Band width as top drivers.*

## Performance Summary:
| Model               | Task           | Accuracy / R² | AUC / F1 | Notes                 |
| ------------------- | -------------- | ------------- | -------- | --------------------- |
| LightGBM            | Regression     | 0.996         | -        | Strong baseline       |
| Transformer (Keras) | Regression     | 0.987         | -        | Custom encoder model  |
| DistilBERT          | Classification | 0.75 (F1)     | 0.83 AUC | Fine-tuned on text    |
| DistilBERT          | Regression     | 0.952 (R²)    | -        | Text-to-price mapping |
| SHAP / LIME         | XAI            | -             | -        | Used for transparency |

## Limitations:
* Focused on NIFTY50 data for now
* Ethical / regulatory integration pending (e.g., KYC compliance)

## Future Plans:
* Integrate real-time news sentiment + social signals
* Add user profile input + multi-objective planning (risk, goals, time horizon)
* Deploy Streamlit/Flask front-end for demo
* Train on broader market datasets (international ETFs, US market)
* Collaborate with financial institutions for real-world testing

## Contributing:
I am open to collaboration!
If you're passionate about AI, finance, and ethical automation — let’s talk.

## License
This project is licensed under the MIT License.

## About the Author
**Durgesh Kumar**
Master's Researcher in AI x Finance
LinkedIn: https://www.linkedin.com/in/durgeshkumar3/ | Email: 12duklan.durgesh@gmail.com

## If this repo helps you, consider giving it a star!

> *Let’s make AI-driven financial intelligence more transparent, ethical, and accessible.*

## Extra Resources:

DataSet Used in This Project is NIFTY50_all (2000-2021)

https://www.kaggle.com/datasets/rohanrao/nifty50-stock-market-data
