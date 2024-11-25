# Near-Earth Object (NEO) Close Approaches Analysis

An analysis of factors influencing NEO close approaches to Earth using machine learning classification models.

## Overview

This study analyzes NASA CNEOS data to predict and classify the rarity of near-Earth object close approaches, focusing on encounters within 10 lunar distances (LD). The project leverages machine learning to identify key factors influencing close approach rarity and develop accurate classification models.

## Research Questions

1. What factors most significantly influence NEO close approach rarity?
2. How effectively can machine learning models predict NEO close approach rarity?
3. Which classification models perform best for NEO encounter prediction?

## Methodology

### Data Processing
- Source: NASA CNEOS dataset
- Features: Velocity, distance, absolute magnitude
- Target Variable: Rarity classification
- Preprocessing: Missing value handling, outlier treatment via winsorization
- Feature Engineering: Diameter range analysis

### Model Development & Performance

#### Individual Models
- Decision Tree: Accuracy 0.99, F1-score 0.99
- KNN: Accuracy 0.97, F1-score 0.97
- Neural Network (Model 1): Accuracy 0.95, F1-score 0.94
- Neural Network (Model 2): Accuracy 0.93, F1-score 0.92
- Logistic Regression: Accuracy 0.89, F1-score 0.88

#### Ensemble Methods
- Stacking Classifier: Accuracy 0.97, F1-score 0.97
- Voting Classifier: Accuracy 0.91, F1-score 0.91

Evaluation Metrics: Accuracy, precision, recall, F1-score

## Key Findings

- Absolute magnitude and diameter significantly influence NEO approach rarity
- Decision Tree classifier achieved highest performance (F1-score: 0.99)
- Stacking ensemble outperformed voting ensemble due to weak learner composition
- Strong correlations identified between rarity and velocity/distance metrics

## Project Structure

```
├── NEO Earth Close Approaches.csv    # Dataset
├── A_Raju_FinalProject.ipynb        # Analysis notebook
└── README.md                        # Project documentation
```

## Requirements

- Python 3.x
- Key Libraries:
  - pandas
  - numpy
  - scikit-learn
  - tensorflow
  - matplotlib
  - seaborn

## Future Improvements

- Expand dataset with additional hazard-related characteristics
- Implement more sophisticated feature engineering
- Explore advanced ensemble techniques
- Incorporate orbital dynamics parameters

## Contributors

- Aravind Raju
- Surya Suresh Sriraman
- Nivetha Sivakumar

