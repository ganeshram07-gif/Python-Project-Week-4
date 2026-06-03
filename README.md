# **Student Performance Analysis System**  
*Exploratory Data Analysis of Student Academic Performance Using Python*

***

## **Overview**
This Jupyter notebook analyzes synthetic student academic data to understand performance trends, identify top/low performers, and derive educational insights through EDA. It generates a 250-student dataset, preprocesses data, applies DSA concepts (heaps/sorting), performs group analysis, and creates comprehensive visualizations.

**Complete workflow**: Data generation → Cleaning → EDA → DSA analysis → Visualizations → CSV reports.

***

## **Dataset**
**Source**: Synthetic dataset (Faker + NumPy)  
**Size**: 250 students  
**Features**: StudentID, Name, Gender, Department (CSE/IT/ECE), Year (1st/2nd/3rd), Maths/Science/English marks, Attendance%, InternalMarks (0-25), TotalMarks, Average, Grade, OverallScore 
**Generated files**:
- `students.csv` - Complete dataset
- `report.csv` - Summary metrics  
- `edacharts.png` - All visualizations

***

## **Objectives**
1. ✅ Generate synthetic academic dataset (250 students) 
2. ✅ Data cleaning (missing values, derived metrics) 
3. ✅ Descriptive statistics (mean/std across subjects) 
4. ✅ Performance metrics (Total/Average/Grade/OverallScore) 
5. ✅ **DSA**: Max-heap (top 10 performers), sorting (low performers) 
6. ✅ Group analysis (Department/Gender/Year) 
7. ✅ Correlations (Attendance vs Performance)
8. ✅ 8 visualizations (histograms, pie charts, heatmaps) 
9. ✅ CSV reports generation 
***

## **Project Highlights**

### **1. Data Generation**
```python
# Cell 3: Creates realistic marks (Maths~75, Science~72, English~78)
# Departments: CSE(40%), IT(30%), ECE(30%)
df = pd.DataFrame(data)  # 250 students[file:1]
```

### **2. EDA & DSA**
- **Descriptive stats**: Subject-wise mean/std deviation
- **Max-heap**: Top 10 performers by OverallScore
- **Sorting**: Bottom 10 failing students 
- **Correlations**: Attendance strongly predicts performance 
### **3. Visualizations (3x3 Grid)**
| Chart | Analysis |
|-------|----------|
| Histogram | Average marks distribution |
| Pie chart | Grade distribution (Fail/Pass/Distinction)  |
| Bar chart | Department avg performance|
| Boxplot | Gender vs Average marks |
| Heatmap | Subject correlations  |
| Scatter | Attendance vs Performance |

### **4. Key Outputs**
```
Top 10 Performers (Heap): Student names + OverallScore
Low Performers (Sorted): Fail students by Average marks
Department Performance: Avg/Std/Distinctions count
Summary Report: Fail rate, Overall avg, Attendance corr
```

***

## **Tools & Technologies**
```
Python 3.x | Pandas | NumPy | Matplotlib | Seaborn | Faker
Jupyter/Colab | CSV exports | Heapq | Priority Queue
```

**Install**:
```bash
!pip install faker pandas numpy matplotlib seaborn
```

***

## **Usage**
1. Open `Student_Performance_Analysis.ipynb`
2. Run **Cell 1** (install dependencies)
3. Run **all cells sequentially** (generates data + analysis)
4. View `edacharts.png` + CSV files 

***

## **Key Findings**
- **Maths (75±15)**, **Science (72±16)**, **English (78±14)** averages 
- **Attendance** strongest performance predictor (correlation analysis)
- **CSE/IT/ECE** department performance benchmarking 
- **70% Pass**, **~20% Distinction**, **~10% Fail** distribution 

***

## **Visualisation **
<img width="751" height="687" alt="Screenshot 2026-06-03 093903" src="https://github.com/user-attachments/assets/cd7d535c-4a3e-44e5-af16-ed856ced9f32" />
<img width="802" height="664" alt="Screenshot 2026-06-03 093543" src="https://github.com/user-attachments/assets/ae85df7d-bb10-4188-96a6-5c01ccde93c8" />
<img width="636" height="667" alt="Screenshot 2026-06-03 093643" src="https://github.com/user-attachments/assets/7780f683-2a90-48a3-88a7-9ab1ec22be7b" />
<img width="803" height="667" alt="Screenshot 2026-06-03 093704" src="https://github.com/user-attachments/assets/ea77ca74-7395-4d5f-a47c-fbf442cf53c5" />
<img width="802" height="662" alt="Screenshot 2026-06-03 093719" src="https://github.com/user-attachments/assets/51145b85-5812-45bc-a9d9-652b78e425e1" />
<img width="801" height="663" alt="Screenshot 2026-06-03 093744" src="https://github.com/user-attachments/assets/364a9e09-469b-4279-9a16-23579c567d60" />
<img width="802" height="663" alt="Screenshot 2026-06-03 093757" src="https://github.com/user-attachments/assets/0fa4bdbb-6d36-4202-bbff-8b52684e4e77" />

***

## **Author**
**Ganesh Ram S**  
*Computer Science Student*  
Kamaraj College, Thoothukudi  
📧 [yesganesh2007@gmail.com] | 💻 GitHub: [ganeshram07-gif] 

***

**🎓 College project demonstrating Data Analysis + DSA + EDA visualization skills**

***

