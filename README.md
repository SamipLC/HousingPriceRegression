```markdown
# Housing Price Regression 🏠

## Overview
This project simulates a housing dataset and builds a Ridge regression pipeline in Python.  
It showcases how **feature engineering**, **polynomial expansion**, **feature selection**, and **hyperparameter tuning** combine to produce a robust price predictor, achieving a ~15% reduction in prediction error.

---

## Project Structure
```

Housing\_Price\_Regression.ipynb    ← Colab notebook with full pipeline & visualizations
requirements.txt                  ← Python dependencies
README.md                         ← This file

````

---

## Requirements
- Python 3.7 or higher  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  

Install dependencies:
```bash
pip install -r requirements.txt
````

---

## Usage

1. Open `Housing_Price_Regression.ipynb` in Google Colab or Jupyter Notebook.
2. Run the cells in order:

   1. **Data Generation** – simulate 1,200 samples with 10 realistic housing features.
   2. **Baseline Model** – scale data and fit a Ridge regression model.
   3. **Advanced Pipeline** – add `PolynomialFeatures`, `SelectKBest`, scaling, and Ridge.
   4. **GridSearchCV** – tune `poly__degree`, `select__k`, and `ridge__alpha`.
   5. **Evaluation & Visualization** – compare MSE and plot actual vs. predicted & residuals.

---

## Techniques Used

* **Synthetic Data** generation with `make_regression`
* **Polynomial Feature Expansion** (`PolynomialFeatures`)
* **Feature Selection** (`SelectKBest` + `f_regression`)
* **Data Scaling** (`StandardScaler`)
* **Regression** using `Ridge`
* **Hyperparameter Tuning** via `GridSearchCV`
* **Cross-Validation** (5-fold CV)
* **Visualization** with `matplotlib`

---

## Results

* **Baseline MSE:** 5120.45
* **Optimized MSE:** 4352.10
* **Error Reduction:** \~15%
* **Best Hyperparameters:**

  * `poly__degree`: 2
  * `select__k`: 8
  * `ridge__alpha`: 1.0

---

## Next Steps

* Replace synthetic data with real-world housing datasets.
* Experiment with other regressors (Random Forest, XGBoost).
* Deploy the model as a REST API or integrate into a web dashboard.

---

## Author

**Samip Lamichhane**
Electrical Engineering @ UT Dallas | Break Through Tech AI Fellow
📫 [samiplc24@gmail.com](mailto:samiplc24@gmail.com)
[LinkedIn](https://www.linkedin.com/in/samiplamichhane/)

```
```
