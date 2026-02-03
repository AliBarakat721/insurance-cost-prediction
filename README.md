# 🏥 Medical Insurance Cost Prediction

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.2%2B-orange?logo=scikit-learn)
![License](https://img.shields.io/badge/License-MIT-green)

Predict medical insurance charges using demographic and health-related features with 87.7% accuracy.

## 📌 Problem Statement
Accurate prediction of medical insurance costs helps:
- Insurance companies price policies fairly
- Individuals understand factors influencing their medical expenses
- Healthcare providers allocate resources efficiently

## 🔑 Key Features Used
| Feature | Type | Description |
|---------|------|-------------|
| `age` | Numerical | Age of primary beneficiary |
| `bmi` | Numerical | Body Mass Index |
| `children` | Numerical | Number of children covered |
| `smoker` | Categorical | Smoking status (yes/no) |
| `sex` | Categorical | Gender (male/female) |
| `region` | Categorical | Residential area in US |

## 📊 Model Performance

| Model | R² Score | MAE | RMSE | Overfitting? |
|-------|----------|-----|------|--------------|
| Linear Regression | 0.784 | $4,181 | $5,796 | Moderate |
| **Random Forest** | **0.877** | **$2,475** | **$4,368** | **Minimal** ✅ |

✅ **Key Insight**: Smoking status is the #1 factor affecting insurance costs (confirmed by feature importance analysis).

## 🚀 How to Run
```bash
# 1. Clone repository
git clone https://github.com/AliBarakat721/insurance-cost-prediction.git
cd insurance-cost-prediction

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run Jupyter Notebook
jupyter notebook insurance_cost_prediction.ipynb
