# Heart Disease Prediction

## Overview
The Heart Disease Prediction Project aims to predict the likelihood of a patient having heart disease based on various medical parameters. Using a dataset of 303 patients, machine learning models were trained and evaluated to make these predictions, achieving high accuracy scores.

## Dataset
The dataset contains 303 entries with 14 attributes:

1. `age`: Age in years
2. `sex`: Sex (1 = male, 0 = female)
3. `cp`: Chest pain type
4. `trestbps`: Resting blood pressure
5. `chol`: Serum cholesterol in mg/dl
6. `fbs`: Fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
7. `restecg`: Resting electrocardiographic results
8. `thalach`: Maximum heart rate achieved
9. `exang`: Exercise-induced angina (1 = yes, 0 = no)
10. `oldpeak`: ST depression induced by exercise relative to rest
11. `slope`: Slope of the peak exercise ST segment
12. `ca`: Number of major vessels colored by fluoroscopy
13. `thal`: Thalassemia type
14. `target`: Heart disease (1 = yes, 0 = no)

## Methodology
1. **Data Exploration and Cleaning**: Initial data exploration was performed to understand the dataset's structure and check for missing values.
2. **Visualization**: High-dimensional data was visualized in 2D space to detect clusters or patterns.
3. **Feature Engineering**: Relevant features were selected, and data imputation was performed as necessary.
4. **Model Training**: Various machine learning models were trained, including Logistic Regression, Random Forest, XGBoost, and Support Vector Classifier (SVC).
5. **Hyperparameter Tuning**: Grid search was employed to fine-tune model parameters for optimal performance.
6. **Model Evaluation**: Models were evaluated based on accuracy, precision, recall, and F1-score. Confusion matrices were also generated for a more detailed performance view.
7. **Data Balancing**: The Synthetic Minority Over-sampling Technique (SMOTE) was utilized to balance the dataset, ensuring equal representation of both target classes.

## Tools and Libraries
- **Python**: Primary programming language
- **pandas and numpy**: Data manipulation and analysis
- **matplotlib and seaborn**: Data visualization
- **Scikit-learn**: Model training, evaluation, and hyperparameter tuning
- **XGBoost**: Gradient boosting framework
- **imblearn**: Handling class imbalance

## Results
The models achieved high accuracy scores, with Random Forest and XGBoost outperforming others. After balancing the dataset, the models were refitted, achieving comparable performance.

## Future Work
Further refinement can be performed by incorporating more advanced feature engineering techniques, experimenting with ensemble methods, or using deep learning models.
