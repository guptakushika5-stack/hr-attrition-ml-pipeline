# HR Employee Attrition Prediction

A beginner-friendly Machine Learning project that demonstrates an end-to-end pipeline for predicting employee attrition using synthetic HR data. Developed as a hands-on learning exercise for data preprocessing, exploratory data analysis, classification, and model evaluation.

## 🎯 Project Objective

The objective is to build and compare machine learning models that predict whether a fictional employee will resign within the following year. The project demonstrates how predictive analytics can support HR analysis and retention planning.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Imbalanced-learn
- Joblib
- Jupyter Notebook / Google Colab

## 📊 Dataset

The notebook automatically generates a synthetic dataset containing 1,000 fictional employee records, with missing values and duplicate rows introduced for data-cleaning practice.

Features include:

- EmployeeID
- Department
- WorkMode
- ExperienceYears
- MonthlySalary
- SatisfactionScore
- OvertimeHours
- Absences

**Target variable:** `Resigned`

- `0` — Employee stayed
- `1` — Employee resigned within the following year

EmployeeID is excluded from model training because it is an identifier rather than a predictive feature.

## 🔄 Project Workflow

1. Install and import the required libraries.
2. Generate and load the synthetic HR dataset.
3. Inspect data types, missing values, and duplicate records.
4. Clean duplicate rows and validate feature ranges.
5. Separate input features and the target variable.
6. Split data into training and testing sets using an 80:20 ratio.
7. Perform exploratory data analysis using statistical summaries and visualizations.
8. Impute missing numerical and categorical values.
9. Scale numerical features using StandardScaler.
10. Apply SMOTENC to address class imbalance in the training data.
11. Encode categorical features using one-hot encoding.
12. Train baseline and SMOTENC Logistic Regression models.
13. Evaluate both models using classification metrics and confusion matrices.
14. Predict attrition for a new fictional employee.
15. Save the trained model components and evaluation outputs.

## 🤖 Models

### 1. Baseline Logistic Regression
Trained using the original training data without oversampling.

### 2. SMOTENC Logistic Regression
Trained using the training data after applying SMOTENC to generate synthetic minority-class examples for mixed numerical and categorical features.

Both models are evaluated on the same held-out test dataset to support a fair comparison.

## 📈 Evaluation Metrics

The notebook evaluates model performance using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Classification report

Run the notebook to obtain the actual results. Compare the metrics for both models rather than assuming that oversampling will always improve performance.

## 🚀 How to Run the Project

1. Clone or download this repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Upload `HR_Attrition_Monday_Complete_Pipeline.ipynb`.
4. Run the notebook cells sequentially.
5. Review the data analysis, model comparison, confusion matrices, and predictions.
6. Download the generated output files if required.

The dataset is generated within the notebook, so no external dataset download is necessary.

## 📁 Expected Project Files

- `HR_Attrition_Monday_Complete_Pipeline.ipynb` — Complete project notebook.
- `hr_attrition_raw.csv` — Generated synthetic dataset.
- `hr_attrition_cleaned.csv` — Cleaned dataset.
- `model_comparison.csv` — Model evaluation results.
- `hr_attrition_teaching_model.joblib` — Saved model and preprocessing components.

The output files are generated when the relevant notebook cells are executed.

## 💡 Key Learning Outcomes

- Data cleaning and missing-value handling.
- Exploratory data analysis and visualization.
- Training-test splitting and prevention of data leakage.
- Numerical feature scaling and categorical encoding.
- Handling class imbalance with SMOTENC.
- Logistic Regression classification.
- Model evaluation and confusion matrix interpretation.
- Saving reusable machine learning components.

## ⚠️ Limitations and Responsible Use

- The dataset is synthetic and does not represent real employee behavior.
- The model is intended for educational purposes and has not been validated for real-world HR use.
- SMOTENC does not guarantee improved model performance.
- Predictions and model coefficients do not establish the causes of employee attrition.
- The model should not be used to make hiring, promotion, or termination decisions.

## 👩‍💻 Project Type

Machine Learning | HR Analytics | Classification | Python | Beginner Project
