# EDA-Projects
# 📈 Mutual Fund EDA – India

[![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

This project explores a comprehensive dataset of Indian mutual funds with the goal of performing insightful Exploratory Data Analysis (EDA), classifying funds into market cap segments (Large, Mid, Small), and generating actionable insights for investors and analysts.

---

## 📂 Files Included

- `comprehensive_mutual_funds_data.csv`: Raw dataset used for analysis.
- `INDIAN_MutualFund_EDA.ipynb`: First version with flawed classification logic.
- `INDIAN_MutualFund_EDA-Fixed.ipynb`: Final notebook with corrected classification and refined analysis.

---
### 🔄 Steps Followed in EDA

1. **Loading and understanding the dataset**  
   - Inspected columns, datatypes, and missing values  
   - Understood key fields: NAV, 1Y/3Y returns, fund categories

2. **Preprocessing and cleaning**  
   - Standardized column names  
   - Removed duplicates
   - median imputation for Null values

3. **Derived new columns**  
   - Return metrics (CAGR over time)  
   - Asset-based classification (Large/Mid/Small cap)  
   - Consolidated fund types and schemes

4. **Segmentation and grouping**  
   - Grouped funds by category, AUM brackets, and cap size  
   - Compared performance across fund types

5. **Visualization**  
   - Used `matplotlib` and `seaborn` for bar plots, boxplots, scatter plots, and heatmaps

---

### ❓ Questions This EDA Tries to Answer

- 📊 What is the distribution of mutual funds across categories?
- 📈 Which categories perform better in 1Y and 3Y return windows?
- 💰 How does AUM size relate to performance and risk?
- ⚖️ Are small-cap funds really higher risk and higher return?
- 🥇 Are there consistently top-performing funds over time?
- 🧠 Can funds be segmented by return-risk profiles for better comparison?

---



## ⚠️ What Went Wrong Initially

In the first notebook, fund categories were incorrectly derived from a misleading column, causing:
- Incorrect segmentation into Large/Mid/Small cap.
- Misleading insights and visualizations.
- Skewed return/risk comparison.

---

## ✅ What Was Fixed

The second notebook applies a more robust classification approach:
- **Combined multiple columns**: category name, fund family, and fund type.
- **Manual validation** of classification.
- **Re-run of all downstream analysis**, including:
  - Category-level return and risk distribution
  - AUM-based segmentation
  - Visualization of return trends
  - Better fund filtering logic

---

## 📊 Key Analyses & Visuals

The final notebook (`INDIAN_MutualFund_EDA-Fixed.ipynb`) includes:

- 📌 **Category Distribution Plot**
- 💹 **Risk vs Return scatter plots**
- 📈 **Top performing funds by AUM and CAGR**
- 🧮 **Boxplots & histograms** for returns and volatility
- 🧠 (Optional) **Clustering or heatmaps**, depending on further exploration

> _The visuals are generated using `Matplotlib` and `Seaborn` libraries._

---

## 🛠️ Tech Stack

- **Languages**: Python (v3.8+)
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn
- **Tools**: Jupyter Notebook

---

## ▶️ Getting Started

1. Clone this repository.
2. Open the `.ipynb` notebooks using Jupyter.
3. Make sure `comprehensive_mutual_funds_data.csv` is in the same directory.
4. **Run `INDIAN_MutualFund_EDA-Fixed.ipynb`** for the latest, validated insights.

---

## ✍️ Author Notes

This project showcases how:
- EDA requires domain knowledge + correct feature engineering.
- One incorrect assumption can mislead all visualizations.
- It's vital to **validate preprocessing logic** before deeper analysis.

---

## 📬 Contact

If you have questions, suggestions, or want to collaborate:

**Sai Akshay Y**  
📧 [ysaiakshay.y@gmail.com]  
🔗 [LinkedIn](https://www.linkedin.com/in/saiakshayy/) 

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
