<div style="text-align: center;">
  <h1>Song-Popularity-Prediction</h1>
  <h2>UMC301 Kaggle Assignment - 1</h2>
</div>

This notebook is my submission for the **UMC301 Kaggle Assignment - 1**.  
Before running the code, please adjust the file paths as this notebook was originally executed on **Kaggle using GPU(P100)**.

---

### 🧠 Methodology

1. **Imputation:** Performed using **MICE (Multiple Imputation by Chained Equations)** on the train and test data **separately** to avoid data leakage.
2. I am using **XGB** for both regression and classification in MICE.
3. **Exploration:** Applied **t-SNE** and **Separability Scores** to visualize and assess feature separability.  
4. **Feature Engineering:** Used **GP-Learn** for **evolutionary feature construction and optimization**.  
5. **Modeling:** Tuned **XGBoost** and **LightGBM** models using **Optuna** for hyperparameter optimization.  
6. **Ensembling:** Averaged predictions from both models to generate the **final submission**.
