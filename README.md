# Ad Targeting: Click-Through Prediction (Logistic Regression)

**Author:** Raghavendra Karanam  
**Program:** NSDC Data Science Projects – Ad Targeting

# Ad Targeting: Click-Through Prediction (NSDC Project)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/raghava0071/ad-targeting-ctr-prediction/blob/main/Raghavendra_Karanam_Ad_Targeting.ipynb)
![Python](https://img.shields.io/badge/Python-3.10-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Summary
Predict whether a user will click an advertisement and identify the levers that drive engagement.

- **Model:** Logistic Regression (balanced)
- **Test Metrics:** Accuracy ~0.93, Precision ~0.97, Recall ~0.89, F1 ~0.93, ROC-AUC ~0.98
- **Top Signals:** Lower daily internet usage & less time-on-site ↑ click odds; Age ↑ clicks; Area Income ↓ clicks
- **Actionable:** Daypart bids toward higher-CTR hours, native/less intrusive creatives for heavy-usage cohorts, age-tailored messaging

## 🧠 About this Project

This project was completed as part of the **National Student Data Corps (NSDC)** initiative.
It explores the behavioral and demographic patterns influencing online ad engagement and develops an interpretable predictive model.

**Key Steps**
- Data Cleaning and Imputation (Mean & “Unknown” fill)
- Feature Engineering (Hour, Day, Month from Timestamp)
- Exploratory Data Analysis (Seaborn + Matplotlib)
- Model Training (Logistic Regression)
- Performance Evaluation (Precision, Recall, F1, ROC-AUC)
- Feature Importance & Business Insights

**Core Insight:**  
Users with lower daily internet usage and less time spent on the site are *more likely to click* on ads — suggesting fatigue in heavy users and opportunity in moderate-usage cohorts.

## 🗂️ Repository
- `Ad_Targeting.ipynb` – full EDA → modeling pipeline (Milestones 1–3)
- `reports/figures` – ROC, PR, Confusion Matrix, Feature Importance
- `models/` – trained logistic model + scaler (joblib)
- `requirements.txt` – environment

## 🔍 Highlights
- Clean handling of missing values (mean + “Unknown” buckets)
- Clear EDA visuals: distributions, box/violin plots, faceted histograms
- Threshold tuning & business interpretation
- Ethical notes: contextual/time targeting over sensitive proxies

## 🧰 Built With
- 🐍 Python (pandas, numpy, scikit-learn)
- 📊 Seaborn & Matplotlib for visualization
- 🧮 Logistic Regression for prediction
- ☁️ Google Colab for experimentation

## 🚀 Quick Start
```bash
# clone
git clone https://github.com/<your-username>/ad-targeting-ctr-prediction.git
cd ad-targeting-ctr-prediction

# setup
python -m venv .venv && source .venv/bin/activate   # (Windows: .venv\Scripts\activate)
pip install -r requirements.txt

# open notebook
jupyter notebook Ad_Targeting.ipynb

 Results (Test Set) 
- Accuracy: 0.931
- Precision: 0.968
- Recall: 0.891
- F1: 0.928
- ROC-AUC: 0.982

## 📈 Visual Highlights

| Metric | Visualization |
|--------|----------------|
| ROC & Precision-Recall Curve | ![ROC Curve](reports/figures/roc_curve.png) |
| Confusion Matrix | ![Confusion Matrix](reports/figures/confusion_matrix.png) |
| Feature Importance | ![Feature Importance](reports/figures/feature_importance.png) |
| Age vs Clicked on Ad (Boxplot) | ![Boxplot](reports/figures/age_vs_click.png) |


 Next Steps 
Cross-validation & model calibration
Top-K bucketing for high-cardinality categories
A/B tests for dayparting and creatives


---

📜 **Author:** [Raghavendra Karanam](https://github.com/raghava0071)  
🎓 M.S. Data Science & Analytics, Florida Atlantic University  
💬 Let’s connect on [LinkedIn](https://linkedin.com/in/raghavendra-karanam)
