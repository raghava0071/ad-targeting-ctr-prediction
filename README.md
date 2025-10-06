# Ad Targeting: Click-Through Prediction (Logistic Regression)

**Author:** Raghavendra Karanam  
**Program:** NSDC Data Science Projects – Ad Targeting

## 📌 Project Summary
Predict whether a user will click an advertisement and identify the levers that drive engagement.

- **Model:** Logistic Regression (balanced)
- **Test Metrics:** Accuracy ~0.93, Precision ~0.97, Recall ~0.89, F1 ~0.93, ROC-AUC ~0.98
- **Top Signals:** Lower daily internet usage & less time-on-site ↑ click odds; Age ↑ clicks; Area Income ↓ clicks
- **Actionable:** Daypart bids toward higher-CTR hours, native/less intrusive creatives for heavy-usage cohorts, age-tailored messaging

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

## Results (Test Set)
- Accuracy: 0.931
- Precision: 0.968
- Recall: 0.891
- F1: 0.928
- ROC-AUC: 0.982
