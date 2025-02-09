# Social Network Ads - Random Forest Classification

This project demonstrates the use of a Random Forest Classifier to predict whether a user will purchase a product based on their age and estimated salary, using the "Social Network Ads" dataset.

## Table of Contents

1.  [Overview](#overview)
2.  [Dataset](#dataset)
3.  [Dependencies](#dependencies)
4.  [Installation](#installation)
5.  [Usage](#usage)
6.  [Model Evaluation](#model-evaluation)
7.  [Hyperparameter Tuning](#hyperparameter-tuning)
8.  [Feature Importance](#feature-importance)
9.  [Visualization](#visualization)
10. [Future Improvements](#future-improvements)
11. [License](#license)
12. [Author](#author)

## 1. Overview

This project aims to build a classification model that can predict whether a user will purchase a product advertised on a social network, based on their demographic information (age and estimated salary). The Random Forest algorithm is used for this classification task.

## 2. Dataset

The dataset used is "Social\_Network\_Ads.csv". It contains the following columns:

*   `User ID`: Unique identifier for each user (not used for training).
*   `Gender`: Gender of the user (not used for training).
*   `Age`: Age of the user.
*   `EstimatedSalary`: Estimated salary of the user.
*   `Purchased`: Whether the user purchased the product (0: No, 1: Yes).

The dataset is located in the `/content/drive/MyDrive/Machine Learning A-Z (Codes and Datasets)/Part 3 - Classification/Section 20 - Random Forest Classification/Python/` directory.  **(Make sure this path is correct for your environment)**

## 3. Dependencies

The following Python libraries are required:

*   `pandas`
*   `numpy`
*   `scikit-learn`
*   `matplotlib`

You can install these dependencies using pip:


## 4. Installation

1.  Clone this repository:

    ```
    git clone [your-repository-url]
    cd [your-repository-directory]
    ```

2.  Ensure you have the required dependencies installed (see section 3).

3.  Place the `Social_Network_Ads.csv` dataset in the specified directory (or update the path in the code accordingly).

## 5. Usage

Run the Python script `your_script_name.py` (replace with the actual name of your script):

This will:

*   Load the dataset.
*   Split the data into training and testing sets.
*   Scale the features using StandardScaler.
*   Train a Random Forest Classifier.
*   Predict the test set results.
*   Evaluate the model using a confusion matrix, accuracy score, and classification report.
*   Display feature importances.
*   Visualize the decision boundary of the classifier on the test set.

## 6. Model Evaluation

The model's performance is evaluated using the following metrics:

*   **Confusion Matrix:**  Provides a breakdown of true positives, true negatives, false positives, and false negatives.
*   **Accuracy:**  The overall accuracy of the model.
*   **Classification Report:** Includes precision, recall, and F1-score for each class.
*   **Feature Importances:** Indicates which features are most important for the prediction.

## 7. Hyperparameter Tuning

The `RandomForestClassifier` can be further optimized by tuning its hyperparameters.  Consider using `GridSearchCV` or `RandomizedSearchCV` from `scikit-learn` to find the best combination of parameters, such as:

*   `n_estimators`: Number of trees in the forest.
*   `max_depth`: Maximum depth of the trees.
*   `min_samples_split`: Minimum number of samples required to split an internal node.
*   `min_samples_leaf`: Minimum number of samples required to be at a leaf node.

An example of how to implement `GridSearchCV` is provided (commented out) in the code.

## 8. Feature Importance

The Random Forest algorithm provides a measure of feature importance, indicating the relative contribution of each feature to the model's predictive power.  The script calculates and displays these importances, allowing you to identify the most influential factors in predicting purchase behavior.  A visualization of the feature importances is also included.

## 9. Visualization

The project includes a visualization of the decision boundary of the trained Random Forest Classifier on the test set. This helps to understand how the model is separating the two classes (purchased vs. not purchased) based on age and estimated salary.

## 10. Future Improvements

*   **Hyperparameter Optimization:** Implement `GridSearchCV` or `RandomizedSearchCV` to fine-tune the model's hyperparameters.
*   **Cross-Validation:** Incorporate k-fold cross-validation to obtain a more robust estimate of the model's performance.
*   **Feature Engineering:** Explore potential new features that could improve the model's accuracy.
*   **Ensemble Methods:** Experiment with other ensemble methods like Gradient Boosting Machines (GBM) or XGBoost.
*   **More Detailed Analysis:**  Add more detailed data exploration and analysis (e.g., looking at the distribution of ages and salaries for purchasers vs. non-purchasers).

## 11. License

This project is licensed under the [MIT License](LICENSE) - see the `LICENSE` file for details.  (Optional: Create a LICENSE file in your repository with the MIT License text, or another license of your choice).

## 12. Author

[Your Name]
[Your Email Address]
[Your GitHub Profile URL (Optional)]

