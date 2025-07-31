# Loan-Approval-prediction
A well-preprocessed dataset and proper imbalance handling (SMOTE) led to accurate and fair loan approval predictions, with logistic regression or decision tree showing the best performance.

📊 Project Objective:
Build a machine learning model to predict whether a loan application will be approved or rejected, using customer financial and personal information. The goal is to help automate loan approval decisions based on historical data patterns.

📦 Dataset:
A publicly available dataset (from Kaggle) with almost 4k+ loan applicant records, featuring both categorical and numerical variables. 

✅ Loan Status (Target: Approved/Rejected)

🛠 Process:
🔹 Data Preprocessing
Cleaned missing values using mode (categorical) and median (numerical)

Standardized column names for consistency

Encoded categorical variables (e.g., Yes/No to 1/0)

Scaled features using StandardScaler

🔹 Class Imbalance Handling
The dataset was imbalanced (more approved loans than rejections)

Applied SMOTE (Synthetic Minority Over-sampling Technique) to balance the classes

📊 Exploratory Data Analysis (EDA)
Checked feature distributions and missing data

Used correlation heatmaps to identify influential features

Found CIBIL score, income, and loan amount were strongly correlated with loan approval

🤖 Model Building & Evaluation
Two classification models were trained and compared:

🔍 Logistic Regression

Fast and interpretable

Achieved strong precision and recall after SMOTE

Best suited for linear decision boundaries

🌳 Decision Tree Classifier

Captured nonlinear relationships

Slightly more prone to overfitting

Easy to visualize and explain

Both models were evaluated using:

✅ Accuracy

🎯 Precision, Recall, and F1-score

📊 Confusion Matrix Visualization (Seaborn heatmap & normalized matrix)

📌 Key Insights Uncovered:
CIBIL Score and Annual Income were the most significant predictors of loan approval

Applicants with higher asset values (residential, bank) had higher approval rates

SMOTE effectively addressed class imbalance, improving recall and F1-score

Logistic Regression slightly outperformed Decision Tree in generalization and precision

🧠 Technologies Used:
🐍 Python

📊 Pandas, NumPy (Data handling)

🤖 Scikit-learn (Modeling & Evaluation)

🧠 Imbalanced-learn (SMOTE)

📈 Matplotlib & Seaborn (Data Visualization)
