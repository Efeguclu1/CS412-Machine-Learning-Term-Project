# CS412-Machine-Learning-Term-Project


# User Content Classification and Engagement Prediction

## Project Overview

This machine learning project focuses on two key tasks:
1. Predicting the number of likes for user-generated content
2. Classifying user accounts into specific categories

### Key Features
- Regression task: Predict like counts using LightGBM
- Classification task: Categorize accounts using a Voting Classifier
- Advanced preprocessing and feature engineering techniques
- Handling of imbalanced datasets

## Project Structure

### Regression Task
- **Objective**: Predict the number of likes for a post
- **Model**: LightGBM Regressor
- **Key Features**:
  - Historical user engagement metrics
  - Post characteristics (comment count, caption length, media type)
  - Logarithmic transformation of target variable

### Classification Task
- **Objective**: Categorize user accounts into domains
- **Model**: Voting Classifier
  - Logistic Regression
  - Support Vector Classifier
  - XGBoost
- **Preprocessing Techniques**:
  - Text preprocessing (URL removal, lowercasing)
  - TF-IDF Vectorization
  - SMOTE for handling class imbalance

## Performance Metrics

### Regression Results
- **Log Mean Squared Error**: 0.078
- **Prediction Range**: 0 to 1,327,989 likes
- **Zero Predictions**: 534 out of total samples

### Classification Results
| Category | Precision | Recall | F1-Score |
|----------|-----------|--------|----------|
| Art | 0.23 | 0.08 | 0.12 |
| Fashion | 0.53 | 0.72 | 0.61 |
| Sports | 0.80 | 0.70 | 0.74 |

## Key Challenges and Solutions

### Data Preprocessing
- Handled missing values
- Applied feature scaling
- Addressed class imbalance using SMOTE

### Feature Engineering
- Extracted user-specific trends
- Created combined features from posts and profiles
- Used TF-IDF for text feature representation

## Future Work
- Implement advanced NLP techniques
- Explore deep learning models
- Conduct extensive hyperparameter tuning
- Improve handling of imbalanced classes

## Technologies Used
- Python
- Scikit-learn
- LightGBM
- XGBoost
- Pandas
- NumPy


## Contributors
- Efe Güçlü
- Irmak Sözen
- Bora Sacır
- Murat Ozan Aybak
- Janset Tunca
