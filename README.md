🚗 AutoScout Car Price Prediction
Using Advanced Linear Regression with Regularisation

📌 Scope
This project develops a robust regression pipeline to predict used car prices for a reseller platform. The scope includes:

Data preprocessing: cleaning, encoding, handling imbalances, and scaling.

Exploratory analysis: frequency distributions, correlation analysis, and outlier detection.

Feature engineering: one‑hot encoding, multilabel handling, and VIF‑based pruning.

Modeling: Baseline Linear Regression, VIF‑pruned Linear Regression, Ridge Regression, and Lasso Regression.

Evaluation: R², Adjusted R², MAE, MSE, RMSE, residual analysis, and multicollinearity checks.

Business insights: identification of key drivers of car prices and actionable recommendations.

📊 Summary
Dataset: 15,915 rows × 23 columns (mix of numerical and categorical predictors).

Target variable (Price): Right‑skewed, normalized via log transformation.

Market insights:

~75% used cars, sedans dominate (>50%), Benzine & Diesel ~99%.

Audi models command premium; Opel/Renault models depress resale value.

Luxury features (leather, LED headlights, parking aids) consistently raise prices.

Model results:

Baseline Linear Regression: R² ~0.93, strong generalization.

VIF‑Pruned Regression: Slight accuracy dip, improved interpretability.

Ridge Regression (α=1.5): Matches baseline, adds coefficient stability.

Lasso Regression: Slightly lower R², but highlights strongest predictors.

⚙️ Details
🔑 Key Insights
Depreciation: Age & Mileage are strongest negative drivers.

Performance: Horsepower (Hp_kw) is the most influential positive driver.

Trust signals: Single ownership and inspection status boost resale value.

Luxury & comfort: Leather upholstery, advanced lighting, and infotainment systems add premiums.

📈 Important Metrics
Model	Train R²	Test R²	MAE	RMSE	Adjusted R²
Linear Regression	0.930	0.931	0.077	0.105	0.928
VIF‑Pruned Linear	0.910	0.912	0.088	0.118	0.909
Ridge (α=1.5)	0.930	0.931	0.077	0.105	0.928
Lasso (Best α)	0.928	0.928	0.078	0.106	0.925
🚀 Features of High Impact
Positive: Horsepower, Audi A3, Renault Espace, luxury features (Heads‑up display, LED headlights, parking camera).

Negative: Age, Mileage, Manual gearing, Opel Astra/Corsa, Renault Clio, “Other” makes.

💡 Use Cases
Pricing strategy: Position low‑age, low‑mileage, high‑performance cars with premium features as high‑value listings.

Trust differentiation: Market single‑owner, recently inspected cars as premium‑ready.

Segmentation: Tailor pricing for sedans vs compact wagons to match buyer preferences.

✅ Conclusion
Car prices are driven by a balance of depreciation (Age, Mileage) and performance (Horsepower, Weight), with brand reputation, luxury features, and trust signals acting as multipliers.

Ridge Regression → Best for production (robust, stable).

Lasso Regression → Best for feature selection dashboards.

VIF‑Pruned Linear → Best for stakeholder storytelling.
