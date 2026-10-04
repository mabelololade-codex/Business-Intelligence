# Healthcare Performance and Patient Analysis Dashboard 

## Project Overview 

This project was developed as part of a business intelligence and data analytics portfolio project.

The goal is to transform this raw data into an interactive Power BI dashboard that helps management understand the healthcare organization's performance and make data driven decisions,to show:
• The healthcare organization performance.
• Patient's experience and, 
• Major areas that require attention.

## Business Problem

The management needs a clear and interactive way to monitor the healthcare performance, patient's experience and identify areas that require attention. The dashboard was designed to answer questions such as:

1. Which age group represents the largest number of patients?
2. Which diagnoses are most common?
3. Which states have the highest patient volume?
4. How many patients are returning?
5. What are the most common patient outcomes?
6. Which department receives the most patients?
7. Which department has the longest waiting time?
8. Which brand handles the most visits?
9. Which departments have lower satisfaction scores?
10. Are there operational areas management should investigate?
11. Which state generates the most revenue?
12. Which department generates the most profit?
13. Which services generate the most revenue?
14. Are states meeting their revenue targets?
15. Which areas require further financial investigation?
16. Which department has the highest satisfaction?
17. Which brand has the lowest satisfaction?
18. What is the relationship between waiting time and satisfaction?
19. Which patient outcomes occur most frequently?

## 🛠️ Tools Used

Microsoft Excel – Data cleaning and preparation
Power BI – Power Query, Star Schema, Drill through, Tooltips, Slicers, Data modelling, DAX calculations, visualization, and dashboard development
GitHub – Readme.md 

## 📁 Project Deliverables

* Cleaned dataset
* Power BI dashboard
* Data model
* DAX measures
* Business insights and recommendations
* Dashboard Screenshots
* Power BI file
* Presentation 

## Dataset

The dataset includes information about the healthcare performance and patient analysis:

1. Cost NGN
2. Revenue NGN
3. Insurance Type 
4. Payment Method 
5. Diagnosis 
6. Age/Age group
7. Waiting Time
8. Satisfaction Score
9. State
10. Date_Table
11. Branch
12. Department 
13. Service
14. Visit counts

## 🧹 Data Cleaning & Preparation

Before building the dashboard, the dataset was cleaned and prepared to ensure accurate analysis.

The cleaning process included:

Checking and removing duplicate records
Identifying and handling missing values
Correcting data types
Standardizing categories such as states, branches, departments, and diagnoses
Checking for inconsistent or incorrect entries
Reviewing numerical fields such as revenue, cost, waiting time, and satisfaction scores
Creating calculated columns where necessary
Ensuring dates were correctly formatted for time-based analysis

After cleaning, the data was loaded into Power BI for modelling and visualization.



## 🗂️ Data Model

The data model was structured to support analysis across different areas of the healthcare organization.

Key fields included:

* Patient ID
* Visit Date
* State
* Branch
* Department
* Gender
* Age
* Diagnosis
* Revenue
* Cost
* Revenue Target
* Waiting Time
* Satisfaction Score
* Patient Outcome

The model allows users to filter and analyze performance by date, state, branch, department, and gender.



## 📊 Key DAX Measures

Some of the key measures created for the dashboard include:

```DAX
Total Patients =
DISTINCTCOUNT('Patients_visit'[Patient_ID])
```

```DAX
Total Visits =
COUNTROWS('Patients_ visit’[Visit_ID])
```

```DAX
Total Revenue =
SUM('Patients_ visit’[Revenue NGN])
```

```DAX
Total Cost =
SUM('Patients_ visit’[Cost NGN])
```

```DAX
Total Profit =
[Total Revenue] - [Total Cost]
```

```DAX
Profit Margin % =
DIVIDE([Total Profit], [Total Revenue], 0)
```

```DAX
Revenue Variance =
[Total Revenue] - [Revenue Target]
```

```DAX
Revenue Achievement % =
DIVIDE([Total Revenue], [Revenue Target], 0)
```

Other measures were created to analyze average revenue per patient, average waiting time, average satisfaction score, patient volume, and revenue performance.


## 🔍 Key Insights

### Patient & Operational Performance

* The organization recorded 1,200 patients and over 3,000 visits.
* Pediatrics recorded the highest number of visits.
* Awka Branch handled the highest number of visits, with 210 visits.
* Pediatrics also recorded the highest waiting time.
* The relationship between waiting time and satisfaction showed that satisfaction generally decreases as waiting time increases, although the relationship varies across patients.
* Pediatrics recorded the highest satisfaction score based on the departmental analysis.
* Lekki Branch in Lagos recorded the lowest satisfaction score.
* Recovery was the most common patient outcome.

### Financial Performance

* The organization generated approximately ₦47.48 million in revenue.
* Rivers State generated the highest revenue.
* Pediatrics recorded the highest profit contribution at 22.22%.
* Most states performed below their revenue targets, with several achieving less than half of their target.
* The revenue target gaps indicate a need to investigate differences in performance across states.


## 💡 Recommendations

Based on the analysis, management should consider:

1. Improving Pediatrics capacity
Review staffing levels, equipment, and patient flow in Pediatrics due to its high patient demand and waiting time.

2. Reducing waiting time
Review appointment scheduling, patient flow, and staffing at branches with longer waiting times.

3. Improving low-performing branches
Investigate the factors contributing to the low satisfaction score at Lekki Branch.

4. Investigating revenue target gaps
Review why several states are significantly below their revenue targets and identify the factors affecting revenue generation.

5. Reviewing cost efficiency
Compare revenue, costs, and profit across states and departments to identify areas where resources can be used more efficiently.

6. Evaluate investment opportunities
Assess whether additional staffing and equipment in high-demand departments could improve patient capacity, waiting time, satisfaction, and financial performance.


## 📝 Conclusion

The analysis provides an overview of the organization's operational, financial, and patient performance.

The organization recorded strong patient activity and positive recovery outcomes, but the analysis also identified areas requiring further attention, particularly waiting time, patient satisfaction, Pediatrics capacity, and revenue target performance across states.

The dashboard can help management monitor these areas, identify performance gaps, and make more informed decisions about staffing, equipment, resource allocation, and financial performance.

### 👩🏽‍💻 Author

Mabel Ololade Fadare
B.Sc Mathematics(Hons)
IFEXA Certified Data Analysis 
Google Data Analysis Certified - Coursera


