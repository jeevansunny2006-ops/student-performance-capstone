Student Performance Prediction – Capstone Project
👩‍💻 Project Overview
This project aims to analyze and predict student performance based on demographic, educational, and behavioral attributes. The goal is to use machine learning models to predict the final outcome of students as Pass, Fail, Withdrawn, or Distinction.

📁 Dataset
File: studentInfo.csv

Source: Open University Learning Analytics Dataset

Total Records: 32,593 students

Features Used:

gender

region

highest_education

imd_band

age_band

num_of_prev_attempts

studied_credits

disability

final_result (Target)

🔧 Project Stages
📌 1. Data Preprocessing
Handled missing values

Performed value counts on the target column

Encoded categorical variables using LabelEncoder

Split data into features (X) and target (y)

Scaled numerical features using StandardScaler

📌 2. Model Building
One model was trained and evaluated (you can add more later):

📦 Model	✅ Accuracy Score
Random Forest Classifier (or whichever you used)	38%

🔍 Additional metrics:

Macro Avg F1-score: 0.31

Weighted Avg F1-score: 0.36

📉 Confusion Matrix
python
Copy
Edit
from sklearn.metrics import confusion_matrix, ConfusionMatrixDisplay
cm = confusion_matrix(y_test, y_pred)
ConfusionMatrixDisplay(cm).plot()
True \ Predicted	0	1	2	3
0 (Fail)	307	500	617	71
1 (Withdrawn)	323	837	744	69
2 (Pass)	395	656	1206	201
3 (Distinction)	76	151	315	51

🛠️ Technologies Used
Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

📁 Files in Repository
model building (1).ipynb: Full code and output

README.md: Summary of the project
