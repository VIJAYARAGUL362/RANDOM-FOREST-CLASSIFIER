# Social Network Ads - Random Forest Classification

This project uses a Random Forest Classifier to predict product purchase based on age and salary from the "Social Network Ads" dataset.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Model Evaluation](#model-evaluation)
- [Hyperparameter Tuning](#hyperparameter-tuning)
- [Feature Importance](#feature-importance)
- [Visualization](#visualization)
- [Future Improvements](#future-improvements)
- [License](#license)
- [Author](#author)

## 1. Overview

This project builds a classification model predicting product purchase based on user demographics (age and salary) using the Random Forest algorithm.

## 2. Dataset

"Social_Network_Ads.csv" (located at `/content/drive/MyDrive/Machine Learning A-Z (Codes and Datasets)/Part 3 - Classification/Section 20 - Random Forest Classification/Python/` - adjust path if needed). Columns: User ID, Gender, Age, EstimatedSalary, Purchased (0: No, 1: Yes).  User ID and Gender are not used in training.

## 3. Dependencies

Python libraries: pandas, numpy, scikit-learn, matplotlib. Install: `pip install pandas numpy scikit-learn matplotlib`

## 4. Installation

1. Clone: `git clone [your-repository-url]`
2. Navigate: `cd [your-repository-directory]`
3. Install dependencies (see section 3).
4. Place `Social_Network_Ads.csv` in the specified directory.

## 5. Usage

Run `your_script_name.py`: This loads data, splits into train/test, scales features, trains Random Forest, predicts, evaluates (confusion matrix, accuracy, classification report), displays feature importances, and visualizes the decision boundary.

## 6. Model Evaluation

Metrics: Confusion Matrix, Accuracy, Classification Report (precision, recall, F1-score), Feature Importances.

## 7. Hyperparameter Tuning

Use `GridSearchCV` or `RandomizedSearchCV` (example commented out in code) to tune `n_estimators`, `max_depth`, `min_samples_split`, `min_samples_leaf`, etc.

## 8. Feature Importance

Calculates and displays feature importances, visualizing influential factors.

## 9. Visualization

Visualizes the decision boundary on the test set.

## 10. Future Improvements

- Hyperparameter Optimization (GridSearchCV/RandomizedSearchCV)
- Cross-Validation (k-fold)
- Feature Engineering
- Ensemble Methods (GBM, XGBoost)
- More Detailed Analysis

## 11. License

MIT License (see LICENSE file).

## 12. Author

S.VIJAYARAGUL EMAIL:- vijayaragul2005@gmail.com 
