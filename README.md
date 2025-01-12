

# CS412 Machine Learning Project: Turkish Instagram Influencers


## Overview of the Repository
This repository contains the following key components for the machine learning project:

- `CS412_Project_Report.pdf`: A comprehensive report detailing the project's objectives, data description, methodology, results, and future work.
- `classification_task.ipynb`: A Jupyter Notebook implementing the classification task to categorize user accounts into different domains.
- `regression_task.ipynb`: A Jupyter Notebook implementing the regression task to predict the number of likes for user-generated content.


## Methodology
The project tackles two main machine learning problems:

1. **Regression Task**: Predicting the number of likes for user-generated content using LightGBM.
   - Key features include historical user engagement metrics, post characteristics, and logarithmic transformation of the target variable.
   - The model demonstrated effective performance with a low Log Mean Squared Error.

2. **Classification Task**: Categorizing user accounts into domains using a Voting Classifier.
   - Preprocessing techniques include text cleaning, TF-IDF vectorization, and handling class imbalance with SMOTE.
   - The ensemble model, combining Logistic Regression, SVC, and XGBoost, achieved robust classification performance across various categories.


## Results
### Regression Task
- Log Mean Squared Error: 0.078
- Prediction range: 0 to 1,327,989 likes
- Number of zero predictions: 534 out of total samples

### Classification Results
| Category | Precision | Recall | F1-Score |
|----------|-----------|--------|----------|
| Art | 0.23 | 0.08 | 0.12 |
| Entertainment | 0.45 | 0.40 | 0.42 |
| Fashion | 0.53 | 0.72 | 0.61 |
| Food | 0.86 | 0.87 | 0.87 |
| Gaming | 0.00 | 0.00 | 0.00 |
| Health and Lifestyle | 0.62 | 0.79 | 0.70 |
| Mom and Children | 0.71 | 0.40 | 0.51 |
| Sports | 0.80 | 0.70 | 0.74 |
| Tech | 0.71 | 0.75 | 0.73 |
| Travel | 0.67 | 0.64 | 0.66 |

**Note**: The model performs well for categories like Food, Sports, and Tech, while struggling with smaller or more niche categories like Gaming and Art.

Finally, let's add the team contributions:

## Team Contributions
- Efe Güçlü
- Irmak Sözen
- Bora Sacır
- Murat Ozan Aybak
- Janset Tunca

