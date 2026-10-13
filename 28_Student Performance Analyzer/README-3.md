# Student Performance Analyzer

A data analysis project that examines the academic performance of 50 students across five subjects and identifies which factors (attendance, study habits, assignments) influence results.

## Objectives

- Clean and prepare a real-world style dataset (including missing values)
- Calculate totals, averages, grades and pass/fail status
- Compare performance across subjects, sections and gender
- Discover relationships between study habits and exam results
- Identify at-risk students and recommend improvements

## Project Structure

```
student-performance-analyzer/
├── student_performance.csv      # Input dataset
├── analyzer.py                  # Analysis code (or analyzer.ipynb / workbook.xlsx)
├── charts/                      # Saved visualizations
│   ├── subject_averages.png
│   ├── grade_distribution.png
│   ├── section_boxplot.png
│   ├── study_vs_average.png
│   └── correlation_heatmap.png
├── report.pdf                   # One-page summary of findings
└── README.md
```

## Dataset

**File:** `student_performance.csv` (50 records, 12 columns)

| Column | Type | Description |
|---|---|---|
| StudentID | int | Unique ID (1001–1050) |
| Name | text | Student name |
| Gender | text | Male / Female |
| Section | text | A, B or C |
| Attendance_Pct | number | Attendance percentage |
| Study_Hours_PerDay | number | Average daily study hours |
| Assignment_Score | number | Assignment marks (out of 100) |
| Math, English, Science, Computer, Urdu | number | Exam marks (out of 100) |

> **Note:** The dataset intentionally contains 4 missing values (1 in `Attendance_Pct`, 3 in `Math`) that must be handled during cleaning.

## Requirements

- Python 3.8+
- Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`

Install with:

```bash
pip install pandas numpy matplotlib seaborn
```

Excel can be used instead of Python.

## Tasks

### Part 1: Data Preparation
1. Load the dataset
2. Inspect shape, data types and summary statistics
3. Detect and handle missing values (mean or median, with justification)

### Part 2: Calculations
4. Add `Total` and `Average` columns
5. Add a `Grade` column
6. Add a `Result` column (Pass/Fail)
7. Rank students by total marks

**Grading scale**

| Grade | Average |
|---|---|
| A | 80 and above |
| B | 70–79 |
| C | 60–69 |
| D | 50–59 |
| F | Below 50 |

Pass = average of 50 or more.

### Part 3: Analysis
8. Class average, highest and lowest mark per subject
9. Top 5 and bottom 5 students
10. Average performance by section and by gender
11. Grade distribution
12. Correlation of Attendance, Study Hours and Assignment Score with Average marks
13. Strongest and weakest subject overall
14. At-risk students (attendance below 65% **or** average below 50)

### Part 4: Visualization
15. Bar chart: average marks per subject
16. Pie chart: grade distribution
17. Box plot: marks by section
18. Scatter plot with trend line: study hours vs. average
19. Heatmap: correlation matrix

### Part 5: Report
20. One-page summary with key findings and three recommendations

## How to Run

```bash
python analyzer.py
```

The script should read `student_performance.csv`, print the analysis results to the console, and save charts to the `charts/` folder.

## Deliverables

| Item | Format |
|---|---|
| Code | `.py`, `.ipynb`, or Excel workbook with formulas |
| Charts | PNG images (minimum 5) |
| Report | 1-page PDF or DOCX |

## Evaluation Criteria

| Criteria | Weight |
|---|---|
| Data cleaning and handling of missing values | 15% |
| Correct calculations (totals, grades, ranks) | 20% |
| Analysis depth and accuracy | 25% |
| Visualizations (clarity and labeling) | 20% |
| Report quality and recommendations | 15% |
| Code quality and comments | 5% |

## Expected Insights (Examples)

- Students with higher attendance tend to score higher
- Study hours show a positive correlation with average marks
- Some sections or subjects may perform noticeably better than others
- A small group of students qualifies as at-risk and needs intervention

## Author

Name: ____________________
Roll No: ____________________
Date: ____________________
