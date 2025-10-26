# 🚗 AutoScout Car Price Prediction  
*Advanced Linear Regression with Regularisation*

---

## 📌 Scope
This project builds a **robust regression pipeline** to predict used car prices for a reseller platform.  

**Key tasks include:**  
- 🧹 **Data Preprocessing** → cleaning, encoding, handling imbalances, scaling  
- 📊 **Exploratory Analysis** → frequency distributions, correlation analysis, outlier detection  
- 🛠 **Feature Engineering** → one‑hot encoding, multilabel handling, VIF‑based pruning  
- 🤖 **Modeling** → Baseline Linear, VIF‑Pruned Linear, Ridge, and Lasso Regression  
- 📈 **Evaluation** → R², Adjusted R², MAE, MSE, RMSE, residual analysis, multicollinearity checks  
- 💡 **Business Insights** → identifying key drivers of car prices and actionable recommendations  

---

## 📊 Summary
- **Dataset**: 15,915 rows × 23 columns (mix of numerical + categorical predictors)  
- **Target (Price)**: Right‑skewed → normalized via log transformation  
- **Market Insights**:  
  - ~75% used cars dominate  
  - Sedans >50% of listings  
  - Benzine & Diesel ~99% of fuel types  
  - Audi models command premium; Opel/Renault models depress value  
  - Luxury features (leather, LED headlights, parking aids) consistently raise prices  

---

## ⚙️ Details

### 🔑 Key Insights
- 📉 **Depreciation**: Age & Mileage are strongest negative drivers  
- 🚀 **Performance**: Horsepower (Hp_kw) is the most influential positive driver  
- 🤝 **Trust Signals**: Single ownership & inspection status boost resale value  
- 💎 **Luxury & Comfort**: Leather upholstery, advanced lighting, infotainment add premiums  

---

### 📈 Model Performance

| Model                     | Train R² | Test R² | MAE   | RMSE  | Adjusted R² |
|----------------------------|----------|---------|-------|-------|-------------|
| **Linear Regression**      | 0.930    | 0.931   | 0.077 | 0.105 | 0.928       |
| **VIF‑Pruned Linear**      | 0.910    | 0.912   | 0.088 | 0.118 | 0.909       |
| **Ridge (α=1.5)**          | 0.930    | 0.931   | 0.077 | 0.105 | 0.928       |
| **Lasso (Best α)**         | 0.928    | 0.928   | 0.078 | 0.106 | 0.925       |

---

### 🚀 Features of High Impact
- **Positive Drivers**: Horsepower, Audi A3, Renault Espace, luxury features (Heads‑up display, LED headlights, parking camera)  
- **Negative Drivers**: Age, Mileage, Manual gearing, Opel Astra/Corsa, Renault Clio, “Other” makes  

---

### 💡 Use Cases
- **Pricing Strategy** → Position low‑age, low‑mileage, high‑performance cars with premium features as high‑value listings  
- **Trust Differentiation** → Market single‑owner, recently inspected cars as premium‑ready  
- **Segmentation** → Tailor pricing for sedans vs compact wagons to match buyer preferences  

---

## ✅ Conclusion
Car prices are driven by a **balance of depreciation (Age, Mileage)** and **performance (Horsepower, Weight)**, with **brand reputation, luxury features, and trust signals** acting as multipliers.  

- 🏭 **Ridge Regression** → Best for production (robust, stable)  
- 📊 **Lasso Regression** → Best for feature selection dashboards  
- 🗣 **VIF‑Pruned Linear** → Best for stakeholder storytelling  

---

### ✨ Footer
🚗 *AutoScout Car Price Prediction — Advanced Linear Regression with Regularisation*  
