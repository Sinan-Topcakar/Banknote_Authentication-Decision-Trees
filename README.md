# Banknote Authentication using Decision Tree

This repository contains a Decision Tree classification project for detecting counterfeit banknotes using the **Banknote Authentication Dataset** from the UCI Machine Learning Repository.

The implementation was done in Python using **Google Colab** and libraries such as `scikit-learn`, `pandas`, `seaborn`, and `matplotlib`.

---

## 📁 Files

- `ELE_489HW2.ipynb`: The main Colab notebook containing:
  - Data loading and exploration
  - Visualization of the statistical features
  - Decision tree model implementation and tuning
  - Evaluation metrics and visualizations
  - Final interpretation of results
- `README.md`: This file.

---

## 📊 Dataset Description

- **Dataset**: Banknote Authentication (UCI)
- **Instances**: 1372
- **Features**:
  - `variance`: Variability in wavelet-transformed image
  - `skewness`: Asymmetry of the distribution
  - `kurtosis`: Tailedness of the distribution
  - `entropy`: Randomness in the image
- **Target**: Binary label (0 = Fake, 1 = Authentic)

---

## 🧪 Methodology

1. **Exploratory Data Analysis (EDA)**  
   Feature pairs were plotted to understand separability.

2. **Train-Test Split**  
   Dataset was split into 80% training and 20% testing.

3. **Model Training**  
   A DecisionTreeClassifier was trained with different hyperparameters:
   - `max_depth`: 2 to None
   - `min_samples_split`: 2, 10
   - `criterion`: `"gini"` and `"entropy"`

4. **Model Evaluation**  
   The models were evaluated using:
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - Confusion Matrix

5. **Best Model**  
   The highest performing model used:
   - `criterion = "entropy"`
   - `max_depth = 2`
   - `min_samples_split = 10`

6. **Feature Importance**  
   - `variance` was the most important feature.
   - `skewness` and `kurtosis` had moderate impact.
   - `entropy` had minimal contribution.

7. **Interpretability**  
   The tree structure was visualized using `plot_tree()` for insights on decision paths.

---

## 🧠 Conclusion

The Decision Tree model was found to be both **accurate and interpretable** for this classification task. Its performance, coupled with its simplicity, makes it a suitable model for banknote authentication based on image statistics.

---

## ▶️ How to Run

1. Open the notebook `ELE_489HW2.ipynb` in **Google Colab**.
2. Run the notebook sequentially to see results and visualizations.
3. Ensure required libraries are installed:  
   `scikit-learn`, `pandas`, `numpy`, `seaborn`, `matplotlib`

---

## 🔗 Project Link

> Add your GitHub repository link here before submission.

---

