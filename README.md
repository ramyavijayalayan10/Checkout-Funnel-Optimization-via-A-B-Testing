# 🧪 Checkout Funnel Optimization via A/B Testing

## 🎯 Hypothesis

Simplifying the e-commerce checkout funnel by reducing the number of steps will increase user conversion rate by **5% or more**.

![Python](https://img.shields.io/badge/Language-Python-3776AB?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Library-Pandas-yellow?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/Library-NumPy-blue?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Library-Matplotlib-green?logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Library-Seaborn-43B02A)
![SciPy](https://img.shields.io/badge/Library-SciPy-yellow?logo=scipy&logoColor=white)
[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC_BY--NC--ND_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

---

## ✏️ Project Summary

In this end-to-end A/B testing project, I designed a simulated, streamlined checkout funnel variant and tested its performance against a control group. Using Proportions Z-test and Chi-square segmentation, I found a **5.66% uplift** in conversion. My analysis demonstrates business-focused experimentation, behavioral segmentation, and strong statistical grounding.
>

---
## 🧱 Experimental Design

| Group     | Funnel Structure                                      |
|-----------|--------------------------------------------------------|
| Control   | Search → Cart → Bill and Personal Details → Payment Confirmation |
| Variant   | Streamlined Search → Unified Cart → Payment Confirmation |

- **Streamlined Search**: Fewer filters, smarter suggestions, faster browsing
- **Unified Cart**: Pre-saved personal details, coupon fields, and billing info to reduce friction

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

### Plots 
- [Funnel Comparison: Control vs Variant](./plot-results/Funnel%20Comparison%20Chart.png)  
- [Conversion Rates Across Funnel Groups](./plot-results/Conversion%20Rate%20Comparison%20Chart.png)  
- [Segmentation by Gender & Device](./plot-results/Segmentation%20Analysis%20by%20Gender%20and%20Device.png")  
> For Python scripts, refer to the **google drive** link in the **resume**
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
## 📐 Confidence Interval

```python
95% Confidence Interval for the Uplift is: [5.50%, 5.83%]
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

## 📂 Folder Structure

| File / Folder             | Description                                      |
|---------------------------|--------------------------------------------------|
| `notebooks/analysis.ipynb`| Main workflow with code, analysis and visuals    |
| `plot-results/`           | Charts and plots                                 |
| `README.md`               | Project summary                                      |
| `LICENSE.md`               | License info                                   |

---

## 📜 License & Usage

This project is licensed under the **Creative Commons Attribution–NonCommercial–NoDerivatives 4.0 International License**.

> ⚠️ This repository is for demonstration purposes only. No reuse, modification, or redistribution is permitted without **explicit permission**.

View full terms in [LICENSE.md](./LICENSE.md) or [on Creative Commons](https://creativecommons.org/licenses/by-nc-nd/4.0/).

© Ramya Vijayalayan, 2025

---
## 📬 Author & Contact Info

**Prepared by Ramya Vijayalayan on 14 Jun 2025**  

For project insights or review requests:

📧 [vrmya2510@gmail.com]  
🔗 [LinkedIn Profile](https://linkedin.com/in/ramya-vijayalayan-9a51b2289)
