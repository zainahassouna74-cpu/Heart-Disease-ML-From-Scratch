# Heart Disease Prediction Using Machine Learning

This project was completed as part of a Machine Learning course.

The main goal is to analyze the UCI Cleveland Heart Disease Dataset and implement Linear Regression and Logistic Regression from scratch using NumPy, then compare the results with scikit-learn models.

## Dataset

The project uses the UCI Cleveland Heart Disease Dataset.

Main file:

`processed.cleveland.data`

The dataset contains medical features such as:

- Age
- Sex
- Chest pain type
- Resting blood pressure
- Cholesterol
- Maximum heart rate
- Exercise-induced angina
- Oldpeak
- Heart disease diagnosis

## Project Tasks

1. Data preprocessing
2. Linear Regression from scratch
3. Logistic Regression from scratch
4. Model evaluation
5. Comparison with scikit-learn

## Data Preprocessing

The preprocessing steps include:

- Adding column headers
- Detecting missing values
- Median imputation
- Detecting outliers using the IQR method
- Converting the target into binary classes
- One-Hot Encoding for categorical features
- Avoiding the Dummy Variable Trap
- Train-test split
- Standardization
- Principal Component Analysis (PCA)

## Linear Regression

Linear Regression was implemented from scratch using NumPy and Gradient Descent.

The target used for this task is:

`thalach`

The models were evaluated using:

- MAE
- RMSE
- R² Score

### Best Linear Regression Result

The best result was achieved using Standardization and PCA.

| Metric | Result |
|---|---:|
| MAE | 15.8271 |
| RMSE | 19.6307 |
| R² Score | 0.3478 |

## Logistic Regression

Logistic Regression was implemented from scratch using:

- Sigmoid function
- Binary Cross-Entropy Loss
- Gradient Descent
- Probability prediction
- Binary classification

The target represents the presence or absence of heart disease.

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix

### Logistic Regression Results

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Baseline | 0.7705 | 0.7692 | 0.7143 | 0.7407 | 0.8074 |
| Standardization | 0.8525 | 0.8276 | 0.8571 | 0.8421 | 0.9545 |
| Standardization + PCA | 0.8525 | 0.8276 | 0.8571 | 0.8421 | 0.9416 |

The Standardization model achieved the highest ROC-AUC score.

## Comparison with Scikit-Learn

The custom implementations were compared with scikit-learn models to verify the correctness and performance of the implemented algorithms.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab

## Repository Files

- `ML_Project_Heart_Diseaseipynb.ipynb` — complete project notebook
- `processed.cleveland.data` — dataset used in the project
- `UCI Heart Disease.zip` — original dataset files

## How to Run

1. Download or clone this repository.
2. Open the notebook using Google Colab or Jupyter Notebook.
3. Make sure the dataset file is available.
4. Run the notebook cells in order.

## Conclusion

Data preprocessing significantly improved model performance.

For Logistic Regression, Standardization produced the best overall result, while PCA reduced the number of features without decreasing the classification accuracy.

The project demonstrates how Linear Regression and Logistic Regression can be implemented from scratch and compared with ready-made machine learning models.
