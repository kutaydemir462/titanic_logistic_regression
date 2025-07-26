# Titanic Survival Prediction (Logistic Regression)

This project applies **Logistic Regression** to the classic Titanic dataset to predict which passengers survived based on various features such as age, gender, ticket class, and more.

---

## Dataset

- `train.csv`: Labeled data used for training and validation.

---

## Workflow

### 1. Data Cleaning
- Filled missing `Age` values with the **median**
- Dropped `Cabin` column due to excessive missing data
- Filled missing `Embarked` values with the **mode**

### 2. Feature and Label Selection
- Selected relevant features (e.g., `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`)
- Encoded categorical variables (`Sex`, `Embarked`) into numerical format
- Split data into training and validation sets

### 3. Model Training
- Used **Logistic Regression** with `sklearn`
- Trained on `X_train`, `y_train`

### 4. Evaluation
- Evaluated on `X_val`, `y_val`
- Achieved:
  - **Accuracy**: ~78%
  - **Precision/Recall/F1-score** via `classification_report`
  - **Confusion Matrix** for detailed insights

---

## Key Learnings
- How to handle missing data
- How to preprocess categorical variables
- Basics of Logistic Regression
- Model evaluation techniques: accuracy, classification report, confusion matrix


