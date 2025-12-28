# ML Project — Classification & Linear Regression

This repository contains notebooks and dataset(s) for two machine-learning tasks:

- `Classification/Classification.ipynb` — student dropout classification pipeline (exploration, preprocessing, models, evaluation)
- `LR.ipynb` — step-by-step Linear Regression (synthetic examples, Normal Equation, SVD/pseudoinverse, scikit-learn, house-price pipeline)

**Datasets**

- Student dropout: `Classification/students_dropout_academic_success.csv`
- Houses (engineered): `Linear-Regression/houses_data_eng.csv`

**Project Structure**

```
Project ML/
├── Classification/
│   ├── students_dropout_academic_success.csv
│   └── Classification.ipynb
├── Linear-Regression/
│   ├── houses_data_eng.csv
│   └── (helper files, if any)
├── LR.ipynb
├── Classification.ipynb
└── README.md
```

**Quick Start**

1. Create and activate a virtual environment (recommended):

```powershell
python -m venv .venv
.\.venv\Scripts\Activate
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Launch Jupyter and open notebooks:

```bash
jupyter notebook
# then open `LR.ipynb` or `Classification.ipynb` in the browser
```

**Notebook Highlights**

- `LR.ipynb`:

  - Synthetic data generation and visualization
  - Closed-form Normal Equation and numerical alternatives (lstsq, pseudoinverse)
  - Scikit-Learn `LinearRegression` implementation, evaluation (MSE, RMSE, R²), visualizations
  - Computational complexity demo and edge-case handling (singular matrices, multicollinearity)
  - `linear_regression_pipeline()` helper function for train/test split, scaling, training, and evaluation

- `Classification.ipynb`:
  - Full classification workflow: preprocessing, model training, cross-validation, metrics (precision/recall/F1), ROC/PR analysis, and visualization

**Notes & Tips**

- The computational-complexity demo in `LR.ipynb` generates large random matrices and may be slow; reduce `m_instances` or `n_features_list` to speed it up.
- Ensure the datasets listed above are present in the repository before running the related cells.
- If running on Windows, use PowerShell commands shown in the Quick Start.

**Dependencies**
See `requirements.txt` for the core Python packages used across the notebooks.

**Contributing & Version Control**

- Use feature branches and open a pull request to merge into `main`.
- Commit notebook checkpoints selectively; consider using `git-lfs` for large notebooks if needed.

If you want, I can commit and push this updated README for you — tell me to proceed.

---

# ML-StudentDropout-Classification-HousePricesPrediction-Linear-Regression

Machine Learning project containing:

- **Student Dropout Classification**: Complete classification pipeline following MNIST methodology
- **House Prices Prediction**: Linear regression analysis

## Project Structure

```
Project ML/
├── Classification/
│   ├── students_dropout_academic_success.csv
│   └── Classification.ipynb (16 comprehensive steps)
├── Linear-Regression/
│   └── houses_data_eng.csv
└── README.md
```

## Classification Notebook

The classification notebook covers:

1. Data loading and exploration
2. Train/test splitting
3. Binary classification (Dropout detector)
4. Cross-validation evaluation
5. Confusion matrix analysis
6. Precision, Recall, F1 metrics
7. Precision-Recall trade-off
8. ROC curve analysis
9. Multiclass classification
10. Feature scaling
11. Error analysis
12. Final model evaluation
13. Multilabel classification
14. Model comparison
15. Hyperparameter tuning
16. Visualization (2D projection)

## Dataset

- **Student Dropout Dataset**: 4424 samples, 36 features, 3 classes (Dropout, Enrolled, Graduate)
- **House Prices Dataset**: Housing data for linear regression analysis

## Technologies

- Python
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
