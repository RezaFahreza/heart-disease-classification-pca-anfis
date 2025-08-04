# Heart Disease Classification using PCA-Based Feature Selection and ANFIS

This project combines **Principal Component Analysis (PCA)** for feature selection and dimensionality reduction with an **Adaptive Neuro-Fuzzy Inference System (ANFIS)** for heart disease classification.

## 🗃️ Dataset & Feature Reduction

- Dataset: 303 records, 14 attributes  
- Source: UCI Heart Disease Dataset  
- PCA was used to reduce dimensionality and select the most relevant features to improve performance and reduce complexity.

## 🧠 ANFIS Model & Optimization

Grid Search was applied to tune hyperparameters:

- `n_memb` (number of membership functions): 2, 3, 4, 5, 6  
- `memb_func` (type of membership function): Gaussian, Generalized Bell, Sigmoid  

**Best configuration:**

- `n_memb = 5`  
- `memb_func = Gaussian`

## 📊 Results

- **Accuracy**: 83%  
- **F1-Score**: 80%

This result shows that PCA + ANFIS is a promising approach for classifying heart disease in an efficient and interpretable way.
