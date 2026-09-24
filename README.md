# Climate Risk & Health Prediction Challenge

Binary classifier predicting whether a recorded death in Uganda falls into a
climate-sensitive category, using demographic, geographic, and climate data.
Built for a Zindi competition; scored on a 0.6×F1 + 0.4×ROC-AUC blend.

**Best leaderboard score: 0.84562**

## Progression

| Notebook | What changed | Score |
|---|---|---|
| `baseline.ipynb` | Logistic Regression only, no external climate data | 0.793 |
| `feature-engineered.ipynb` | 5-model comparison (LR, RF, Extra Trees, GB, XGBoost) | 0.818 |
| `fe-hpt.ipynb` | Hyperparameter search across tree-based models | 0.836 |
| `hpt-eda-updated.ipynb` | Correlation review to refine categorical encoding | 0.8362 |
| `fe-updated.ipynb` | Added interaction features | 0.83908 |
| `fe-catboost.ipynb` | Introduced CatBoost | 0.84463 |
| `catboost-climate-features.ipynb` | Merged `climate_features.csv`, target-mean encoding | **0.84562** |

Full writeup: `Climate_Risk_Project_Report.docx`.

## Repo structure

```
data-exploration/
  eda-1.ipynb
notebooks/
  baseline.ipynb
  climate-risk-health-prediction-feature-engineered.ipynb
  climate-risk-health-prediction-fe-hpt.ipynb
  climate-risk-health-prediction-hpt-eda-updated.ipynb
  climate-risk-health-prediction-fe-updated.ipynb
  climate-risk-health-prediction-fe-catboost.ipynb
  climate-risk-health-prediction-catboost-climate-features.ipynb
```

## Stack

Python · pandas · scikit-learn · XGBoost · LightGBM · CatBoost

## License

See `LICENSE`.
