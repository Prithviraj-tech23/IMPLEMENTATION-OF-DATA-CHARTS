Student Performance Visualization (R)

**Name:** P S S Prithivi Raj  
**Roll No:** 23BAD088  

This repository contains an R script that performs basic analysis on a *student performance* dataset and generates three visualizations using **ggplot2** and **dplyr**:

1. **Subject-wise Average Marks** (Bar Chart)  
2. **Performance Trend Across Tests** (Line Chart)  
3. **Final Grade Distribution** (Pie Chart)

---

## Requirements
- R (4.0 or above recommended)
- R packages:
  - `ggplot2`
  - `dplyr`

Install packages:
install.packages(c("ggplot2", "dplyr"))

## Dataset

The script reads the dataset from:

`/home/danteprithiviraj/Documents/student_performance.csv`



##  Expected CSV Columns

Your `student_performance.csv` must contain these columns:

* `Subject`
* `Internal_Test1`
* `Internal_Test2`
* `Assignment_Marks`
* `Final_Grade`

Example format:

| Subject | Internal_Test1 | Internal_Test2 | Assignment_Marks | Final_Grade |
| ------- | -------------- | -------------- | ---------------- | ----------- |
| Maths   | 18             | 20             | 15               | A           |

---

##  How to Run

1. Clone the repository or download the files.
2. Open the script in **RStudio** (or run in R).
3. Run:

source("EDA ASSIGNMENT 1.R")

> Replace `student_performance_analysis.R` with your script filename if different.


## What the Script Does

### 1) Data Cleaning

* Removes missing values:
student_performance <- na.omit(student_performance)

### 2) Total Marks Calculation

Creates a new column:

* `Total_Marks = Internal_Test1 + Internal_Test2 + Assignment_Marks`

### 3) Subject-wise Average Marks

* Groups by `Subject`
* Calculates mean `Total_Marks`
* Plots bar chart

### 4) Performance Trend Across Tests

* Calculates average marks of:

  * Internal Test 1
  * Internal Test 2
  * Assignment
* Plots line chart

### 5) Final Grade Distribution

* Counts students per grade (`Final_Grade`)
* Displays a pie chart

---

##  Output

Running the script displays **three plots** in the R plot window.
(You can save them using `ggsave()` if required.)
the result of this is in the repo as a screenshot
---

##  Author

**P S S Prithivi Raj**
**23BAD088**

