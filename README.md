# 🌍 Global Disease Burden Analyzer  

A comprehensive, interactive Python application designed to explore the relationship between disease burden (measured in **Disability-Adjusted Life Years – DALYs**) and socioeconomic indicators such as income, education, urbanization, and healthcare infrastructure. This project provides both a **CLI** and **GUI** for data visualization, statistical analysis, and policy-relevant insights.  

---

## 📖 Background & Motivation  
Global disparities in disease burden remain a pressing challenge. Despite advances in healthcare, low-income countries consistently face higher DALYs compared to wealthier nations. Understanding how **socioeconomic indicators** interact with disease outcomes is critical for shaping effective interventions and promoting equity.  

---

## 🛠 Project Objective  
- Investigate how socioeconomic factors (income, education, urbanization) correlate with global disease burden.  
- Analyze disparities by **age, gender, and disease category**.  
- Explore the role of healthcare infrastructure (beds, doctors, access).  
- Provide evidence-based insights to inform public health and policy decisions.  

---

## ❓ Research Questions  
- How strongly do socioeconomic factors correlate with disease burden?  
- Are certain demographics (age, gender) more affected?  
- Do these correlations vary across **infectious vs. non-communicable diseases**?  
- How has disease burden changed over time across **income groups**?  

---

## ✨ Features  
- **Interactive GUI** with PyQt5 and Matplotlib  
- **CLI mode** for automated analysis and export  
- 15+ visualizations including:  
  - DALYs by gender, age group, disease category, treatment type  
  - Correlation matrix of socioeconomic features  
  - DALYs vs. income, education, urbanization, healthcare access  
  - Time trends (2000–2025) and country rankings  
- Automatic export of:  
  - Cleaned datasets  
  - Regression and correlation reports  
  - Visualizations to the `assets/` folder  

---

## 📂 Repository Contents  
- `DS8007_Final_projectreport_Das_Sharmi.pdf` – Final report with methods, results & discussion  
- `Das_Sharmi_proposal.pdf` – Original project proposal  
- `DS8007_Final_projectfiles_Das_Sharmi.zip` – Supporting code and figures  
- `README_DATAVIZFINAL.md` – This documentation  

---

## 🛠 Methodology  
1. **Data Preprocessing**  
   - Missing values handled (median imputation, row removal for critical fields)  
   - Outlier detection with IQR (none found for DALYs)  
   - Normalization with z-scores  
   - Feature engineering: disease type (infectious vs. NCD), income groups  

2. **Exploratory Data Analysis (EDA)**  
   - DALYs distribution across demographics and categories  
   - Infectious vs. NCD comparisons  

3. **Statistical Analysis**  
   - Multiple Linear Regression (income, education, urbanization)  
   - Pearson Correlation (healthcare access, hospital beds, physician density)  
   - Summary tables of socioeconomic relationships  

4. **Visualization**  
   - PyQt5 interactive modules  
   - Static charts: scatter plots, correlation matrices, boxplots, time series  

---

## 📊 Key Findings  
- **No significant correlation** between DALYs and income, education, or urbanization.  
- Healthcare infrastructure (hospital beds, doctors, access %) did **not reduce DALYs** significantly.  
- **Persistent disparities**: low-income countries maintain ~30 higher DALYs than high-income countries (2000–2025).  
- **Infectious diseases** cluster in resource-limited settings, while **chronic conditions** appear across all income groups.  
- COVID-19 created a visible DALY spike post-2020.  

---

## 🌐 Dataset  
- **Global Health Statistics Dataset** (Kaggle)  
  👉 [Access here](https://www.kaggle.com/datasets/malaiarasugraj/global-health-statistics/data)  

---

## 🎯 Policy Implications  
- Healthcare access and physical infrastructure alone are **necessary but insufficient** to reduce disease burden.  
- Global strategies should:  
  - Strengthen **preventive care** (vaccinations, screenings)  
  - Improve **quality and equity** in services  
  - Tailor interventions to **regional disease profiles** (e.g., malaria in tropics, diabetes in aging populations)  

---

## 🚀 Getting Started  

### Prerequisites  
Install dependencies:  
```bash
pip install -r requirements.txt
```  

### Run the CLI  
```bash
python main.py --cli
```  

### Run the GUI  
```bash
python main.py --gui
```  

---

## 📂 Project Structure  
```
Global Disease Burden Analyzer
├── main.py                 # CLI/GUI entry point
├── gui.py                  # PyQt5 GUI logic
├── eda.py                  # Exploratory Data Analysis visuals
├── visualization.py        # Advanced statistical plots and regressions
├── preprocessing.py        # Data cleaning and feature engineering
├── data/
│   ├── Global Health Statistics.csv   # Raw dataset
│   └── cleaned_data.csv               # Output after preprocessing
├── assets/                 # Exported plots and reports
```

---

## 👩‍💻 Authors  
- **Sharmi Das** – MSc Data Science & Analytics, Toronto Metropolitan University  
- **Jenny Huang** – MSc Data Science & Analytics, Toronto Metropolitan University  
