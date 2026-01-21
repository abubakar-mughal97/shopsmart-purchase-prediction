# ShopSmart Purchase Prediction

## Problem Statement
Predict whether a visitor will complete a purchase based on session behavior.
The dataset is imbalanced, so model performance is evaluated using F1-score.

## Dataset
- 12,330 user sessions
- Mix of numerical and categorical features
- Target: Revenue (purchase / no purchase)

## Approach
1. Exploratory Data Analysis (EDA)
2. One-hot encoding for categorical variables
3. Train-test split with stratification
4. Decision Tree baseline model
5. Cost-complexity pruning to reduce overfitting
6. Evaluation using F1-score

## Results
| Model | Train F1 | Test F1 |
|-----|---------|--------|
| Unpruned Decision Tree | ~1.00 | Low |
| Pruned Decision Tree | Lower | ≥ 0.55 |

Pruning significantly improves generalization.

## Key Insight
PageValues is the most influential feature, indicating strong purchase intent.

## Tools
- Python
- pandas, numpy
- scikit-learn
- matplotlib


