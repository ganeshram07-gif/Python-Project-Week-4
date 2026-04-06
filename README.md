Student Performance Analysis System
Exploratory Data Analysis of Student Academic Performance Using Python

Overview
This Jupyter notebook analyzes synthetic student academic data to understand performance trends, identify top/low performers, and derive educational insights through EDA. It generates a 250-student dataset, preprocesses data, applies DSA concepts (heaps/sorting), performs group analysis, and creates comprehensive visualizations.

Complete workflow: Data generation → Cleaning → EDA → DSA analysis → Visualizations → CSV reports.

Dataset
Source: Synthetic dataset (Faker + NumPy)
Size: 250 students
Features: StudentID, Name, Gender, Department (CSE/IT/ECE), Year (1st/2nd/3rd), Maths/Science/English marks, Attendance%, InternalMarks (0-25), TotalMarks, Average, Grade, OverallScore

Generated files:

students.csv - Complete dataset

report.csv - Summary metrics

edacharts.png - All visualizations

Objectives
✅ Generate synthetic academic dataset (250 students)

✅ Data cleaning (missing values, derived metrics)

✅ Descriptive statistics (mean/std across subjects)

✅ Performance metrics (Total/Average/Grade/OverallScore)

✅ DSA: Max-heap (top 10 performers), sorting (low performers)

✅ Group analysis (Department/Gender/Year)

✅ Correlations (Attendance vs Performance)

✅ 8 visualizations (histograms, pie charts, heatmaps)

✅ CSV reports generation

Project Highlights
1. Data Generation
python
# Cell 3: Creates realistic marks (Maths~75, Science~72, English~78)
# Departments: CSE(40%), IT(30%), ECE(30%)
df = pd.DataFrame(data)  # 250 students[file:1]
2. EDA & DSA
Descriptive stats: Subject-wise mean/std deviation

Max-heap: Top 10 performers by OverallScore

Sorting: Bottom 10 failing students

Correlations: Attendance strongly predicts performance

3. Visualizations (3x3 Grid)
Chart	Analysis
Histogram	Average marks distribution
Pie chart	Grade distribution (Fail/Pass/Distinction)
Bar chart	Department avg performance
Boxplot	Gender vs Average marks
Heatmap	Subject correlations
Scatter	Attendance vs Performance
4. Key Outputs
text
Top 10 Performers (Heap): Student names + OverallScore
Low Performers (Sorted): Fail students by Average marks
Department Performance: Avg/Std/Distinctions count
Summary Report: Fail rate, Overall avg, Attendance corr
Tools & Technologies
text
Python 3.x | Pandas | NumPy | Matplotlib | Seaborn | Faker
Jupyter/Colab | CSV exports | Heapq | Priority Queue
Install:

bash
!pip install faker pandas numpy matplotlib seaborn
Usage
Open Student_Performance_Analysis.ipynb

Run Cell 1 (install dependencies)

Run all cells sequentially (generates data + analysis)

View edacharts.png + CSV files

Key Findings
Maths (75±15), Science (72±16), English (78±14) averages

Attendance strongest performance predictor (correlation analysis)

CSE/IT/ECE department performance benchmarking

70% Pass, ~20% Distinction, ~10% Fail distribution

Author
Ganesh Ram S
Computer Science Student
Kamaraj College, Thoothukudi

🎓 College project demonstrating Data Analysis + DSA + EDA visualization skills

