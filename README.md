# 🧪 Checkout Funnel Optimization via A/B Testing

## 🎯 Hypothesis

Simplifying the e-commerce checkout funnel by reducing the number of steps will increase user conversion rate by **5% or more**.

---

## 🧱 Experimental Design

| Group     | Funnel Structure                                      |
|-----------|--------------------------------------------------------|
| Control   | Search → Cart → Bill and Personal Details → Payment Confirmation |
| Variant   | Streamlined Search → Unified Cart → Payment Confirmation |

- **Streamlined Search**: Fewer filters, smarter suggestions, faster browsing
- **Unified Cart**: Pre-saved personal details, coupon fields, and billing info to reduce friction

---

## 🛠️ Technologies & Tools

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/Matplotlib-20232A?style=for-the-badge&logo=matplotlib&logoColor=white"/>
  <img src="https://img.shields.io/badge/Seaborn-43B02A?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white"/>
</p>

---

## 📂 Data Preparation

### ✔️ Merged Multi-Source Data

- Joined five page-level datasets into a unified `control_df`
- Simulated `variant_users_df` by modifying funnel steps
- Created unified cart structure, removed details page
- Final conversion defined as:  
  ```python
  ab_data_df['converted'] = ab_data_df['payment_confirmation']
  ```
---
## 📈 Visualizations

**Saved Images (link if hosted):**
- `funnel_comparison.png`
- `conversion_rate_chart.png`
- `segmentation_analysis.png`

### 📌 Highlights
- Funnel Comparison: Control vs Variant  
- Conversion Rates Across Funnel Groups  
- Segmentation by Gender & Device  

---

## 📊 Key Performance Metrics

- 🔄 **Conversion Rate - Control Group**: 0.50%  
- 🚀 **Conversion Rate - Variant Group**: 6.16%  
- 🎯 **Uplift from Variant**: +5.66 percentage points  

---

## 📐 Proportions Z-Test

```python
Z-statistic ≈ 67.09  
P-value ≈ 0.0000
```
---

## ✅ Conclusion

Statistically significant improvement.  
The streamlined funnel increases conversions by **5.66 percentage points**, validating the hypothesis.

---

## 🧠 Behavioral Segmentation via Chi-Square Tests

### Gender vs. Conversion

| Gender | Conversion Rate |
|--------|------------------|
| Female | 3.45%            |
| Male   | 3.21%            |

📊 **Chi-square = 7.8393**  
🧪 **p-value = 0.0051** → **Significant difference**

---

### Device vs. Conversion

| Device  | Conversion Rate |
|---------|------------------|
| Mobile  | 5.14%            |
| Desktop | 2.42%            |

📊 **Chi-square = 922.2552**  
🧪 **p-value ≈ 0.0000** → **Highly significant difference**

---

## 🏁 Final Takeaways

- ✅ Hypothesis confirmed — simplified funnel yields **+5.67% conversion gain**
- 📱 Mobile-first design crucial: Mobile converts **>2×** better than desktop
- 👩 Gender shows subtle conversion differences
- 🎯 Streamlining steps leads to tangible business impact

---

## ✏️ Portfolio Summary

> *In this end-to-end A/B testing project, I designed a simulated checkout funnel variant and tested its performance against a control group. Using proportions z-test and chi-square segmentation, I found a 5.66% uplift in conversion. My analysis demonstrates business-focused experimentation, behavioral segmentation, and strong statistical grounding.*

---

## 📂 File Guide

| File / Folder             | Description                                      |
|---------------------------|--------------------------------------------------|
| `notebooks/analysis.ipynb` | Main workflow with code, analysis and visuals     |
| `data/`                   | Cleaned data files                                |
| `images/`                 | Charts and plots                                  |
| `README.md`               | Project summary                                   |

---

## 📌 Author & Date

**Prepared by Ramya Vijayalayan on 14 Jun 2025**
