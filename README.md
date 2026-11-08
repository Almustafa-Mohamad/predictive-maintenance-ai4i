# Predictive Maintenance - AI4I 2020

Exploratory data analysis and feature engineering on the AI4I 2020 Predictive Maintenance dataset (10,000 machines, 14 columns).

## Key findings
- Severe class imbalance: only 3.39% of machines fail (339 of 10,000).
- Linear correlation between raw sensors and failure is weak (max 0.19, Torque).
- Engineered feature `power` (torque x angular speed) shows failures at both extremes (very low and very high power), a U-shaped pattern that linear correlation misses.
- Tree-based models are a better fit than linear models for this data.

## Files
- `eda_01.ipynb`: exploratory analysis
- `data/ai4i2020.csv`: dataset (Matzka, 2020)

## Next steps
Model training, class imbalance handling, evaluation with recall and F1.
