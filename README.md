# student_performance_dataset

Student Performance Analysis
📊 Study Hours vs Final Exam Score
This project is created using Python (Jupyter Notebook) to analyze student performance. We generated a scatter plot to visualize the relationship between study hours per week and final exam scores.

🔍 Plot Explanation:
The graph demonstrates that students who spend more study hours per week tend to achieve higher final exam scores.

X-axis: Total study hours per week
Y-axis: Final exam score
Colorbar: Indicates score intensity (darker colors represent higher scores)
📂 Files Included:
student_performance_dataset.csv → Dataset of student performance
study_vs_exam_score.png → Generated scatter plot
analysis.ipynb → Python Jupyter Notebook code
🚀 Technologies Used:
Python
Pandas
Matplotlib
Jupyter Notebook
📌 This analysis helps us understand how study habits impact academic performance. 🚀
# code is :

import pandas as pd
import matplotlib.pyplot as plt

# Load dataset
df = pd.read_csv("student_performance_dataset.csv")

# Create scatter plot
plt.figure(figsize=(9, 6))
plt.scatter(df['Study_Hours_per_Week'], df['Final_Exam_Score'], c=df['Final_Exam_Score'], cmap='coolwarm', s=100, alpha=0.7)

# Add labels and title
plt.xlabel("Study Hours per Week", fontsize=12)
plt.ylabel("Final Exam Score", fontsize=12)
plt.title("Impact of Study Hours on Final Exam Score", fontsize=14)
plt.colorbar(label="Final Exam Score")  # Color bar for reference
plt.grid(True)

# Show plot
plt.show()

# question was :
How does the number of study hours per week affect a student's final exam score?

# code
