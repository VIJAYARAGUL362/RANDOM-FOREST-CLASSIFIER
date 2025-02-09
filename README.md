# Social Network Ads Classification

A machine learning project that predicts whether a user will purchase a product based on their age and estimated salary using Random Forest Classification.

## Overview

This project implements a Random Forest Classifier to analyze social network advertising data and predict customer purchasing behavior. The model uses demographic information (age and salary) to predict whether a user will purchase a product after seeing an advertisement.

## Features

- Data preprocessing and scaling
- Random Forest Classification model
- Comprehensive model evaluation metrics
- Visual analysis including:
  - Feature importance plots
  - Decision boundary visualization
  - Confusion matrix heatmap
- Hyperparameter tuning capabilities
- Object-oriented implementation for easy reuse and modification

## Prerequisites

- Python 3.8+
- Required packages:
  ```
  numpy>=1.19.2
  pandas>=1.2.0
  scikit-learn>=0.24.0
  matplotlib>=3.3.0
  seaborn>=0.11.0
  ```

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/social-network-ads.git
   cd social-network-ads
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Prepare your data:
   - Ensure your dataset is in CSV format
   - Required columns: 'Age', 'EstimatedSalary', 'Purchased'
   - Place the CSV file in the project directory

2. Run the classifier:
   ```python
   from social_network_ads_classifier import SocialNetworkAdsClassifier
   
   # Initialize and run the classifier
   classifier = SocialNetworkAdsClassifier('Social_Network_Ads.csv')
   
   # Run the complete pipeline
   (classifier
       .load_data()
       .split_and_scale()
       .train()
       .evaluate()
       .plot_feature_importance()
       .plot_decision_boundary())
   ```

3. Optional: Perform hyperparameter tuning:
   ```python
   # Define custom parameter grid if needed
   param_grid = {
       'n_estimators': [10, 50, 100, 200],
       'max_depth': [None, 10, 20, 30],
       'min_samples_split': [2, 5, 10],
       'min_samples_leaf': [1, 2, 4]
   }
   
   # Run grid search
   best_model = classifier.perform_grid_search(param_grid)
   ```

## Model Evaluation

The classifier provides several evaluation metrics:
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)
- Overall Accuracy Score
- Feature Importance Analysis

## Output Examples

The model generates several visualizations:
1. Confusion Matrix Heatmap: Shows true positives, false positives, true negatives, and false negatives
2. Feature Importance Plot: Displays the relative importance of age and salary in predictions
3. Decision Boundary Plot: Visualizes how the model separates different classes in the feature space

## Project Structure

```
social-network-ads/
├── README.md
├── requirements.txt
├── social_network_ads_classifier.py
├── data/
│   └── Social_Network_Ads.csv
└── examples/
    └── example_usage.py
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

Your Name - S.VIJAYARAGUL

EMAIL Link: vijayaragul2005@gmail.com

## Acknowledgments

- Social Network Ads dataset providers
- The scikit-learn team for their excellent machine learning library
- Contributors and maintainers of the dependencies used in this project
