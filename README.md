#  Algorithm selection for #SAT Model Counting

This project uses machine learning to predict the best solver for a given Boolean satisfiability counting (#SAT) instance using structural and statistical features of the problem. Includes preprocessing, feature engineering, PCA, hyperparameter tuning, and evaluation techniques.

##  Dataset
- Source: [train_data.csv](https://github.com/andvise/DM_Assignment/blob/main/train_data.csv)
- 1337 SAT instances, 72 numerical features
- Target: Optimal solver label (`gpmc`, `d4`, `ganak`, `addmc`, `sharpsat`)

##  Models Used
- k-Nearest Neighbors (k-NN)
- Support Vector Machine (SVM)

##  Techniques
- Feature scaling (StandardScaler, MinMaxScaler)
- Dimensionality reduction (PCA)
- Feature selection (SelectKBest, SelectPercentile)
- Hyperparameter tuning with GridSearchCV
- Evaluation with cross-validation and hold-out sets

##  Final Results
- Best Model: k-NN with MinMaxScaler + SelectKBest + GridSearchCV
- Accuracy on test set: 75.06%
- Cross-validation score: ~76%

##  Files
- `sat_model_classification.ipynb`: Full notebook with documentation and implementation
- `README.md`: This file

##  Keywords
#SAT, Machine Learning, k-NN, SVM, GridSearchCV, Algorithm Selection, Dimensionality Reduction

---
