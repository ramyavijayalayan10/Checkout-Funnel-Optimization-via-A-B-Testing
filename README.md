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
