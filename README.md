# This Repository's Purpose
This repository is publicly available as part of my final code submission for my thesis research.

Please note that the original development was done in a private repository to protect sensitive information. The dataset used contains credentialed data from a commercial greenhouse, and I am committed to maintaining the privacy and confidentiality of the greenhouse owner.

#Previouse Git History


---

# Crop Yield Prediction in Cambodian Greenhouses using ML & DL

This project implements machine learning and deep learning models to predict crop yield in semi-controlled greenhouse environments in Cambodia. It is part of my undergraduate thesis at the Royal University of Phnom Penh (2021–2025), focusing on bok choy and curly cabbage under nethouse systems in specific study at Prey Kdouch Farm, Takeo.

---
## 01. Overview
* There are 31 total features after feature engineering and merged with quiried dataset:
- Crop & Cycle Identifiers: `nethouse_id`, `crop_type`, `cycle_number`, `transplant_date`, `plant_care_date`, `harvest_date`, `Day_to_harvest`
- Fertilizer & Pesticide Usage: `fertilizer_A`, `fertilizer_B`, `fertilizer_C`, `fertilizer_D`, `insecticide`, `fungicide`, `pesticide_A`, `pesticide_B`
- Weather Conditions: `temperature_2m`, `relative_humidity_2m`, `rain`, `temperature_80m`, `temperature_120m`, `temperature_180m`
- Soil Temperature: `soil_temperature_0cm`, `soil_temperature_6cm`, `soil_temperature_18cm`, `soil_temperature_54cm`
- Soil Moisture: `soil_moisture_0_to_1cm`, `soil_moisture_1_to_3cm`, `soil_moisture_3_to_9cm`, `soil_moisture_9_to_27cm`, `soil_moisture_27_to_81cm`
- Target: `yield_kg_per_m2`

On top of that, to find out more insight there's an another summplementaty dataset to find the key insight.
## 02. Repository Structure

```
.
├── data/                   # Processed datasets and feature sets
├── notebooks/             # Jupyter notebooks for preprocessing, modeling, and evaluation
├── models/                # Saved model weights or configurations
├── reports/               # Exported results, plots, and analysis
├── utils/                 # Custom Python scripts (e.g., feature engineering, metrics)
└── README.md              # Project overview (you’re here!)
```
 
However, this original github repository have to put the visibility as private of dataset credentiality.

---

## 02. Project Highlights

- **Feature Engineering**: VIF filtering, correlation reduction, domain-informed manual sets
- **Models Used**: Linear Regression, Random Forest, SVR, Gradient Boost, LSTM
- **Experimentation**: Trained on multiple feature subsets with evaluation via R², MAE, RMSE, and MAPE
- **Visualization**: Power BI dashboard with SHAP plots, yield trends, and decomposition trees

---

## 03. Requirements

- Python 3.10+
- `pandas`, `numpy`, `scikit-learn`, `catboost`, `xgboost`
- `seaborn`, `matplotlib`
- `keras`, `tensorflow` (for LSTM models)
- Jupyter Notebook or VS Code

```bash
pip install -r requirements.txt
```

---

## 04. How to Reproduce

1. Clone the repository:
```bash
git clone git@github.com:Pheak02/Agri-Analytics.git
```

2. Navigate to the notebook:
```bash
cd notebooks/
```

3. Run preprocessing and modeling notebooks in order.

---

## 05. Thesis Reference

> **Title**: Crop Yield Prediction of Greenhouse Field Study in Cambodia Using Machine Learning and Deep Learning  
> **Author**: Sopheak Saing  
> **University**: Royal University of Phnom Penh  
> **Advisor**: Mr. Chap Chanpiseth  
> **Date**: June 2025

---

## Sample Output


---

## License

This research is submitted in partial fulfillment of a bachelor's degree. Please contact me for permission before reuse.

---

## Acknowledgments

Thanks to my advisor, colleague, and greenhouse data providers. See full acknowledgments in the thesis document.

