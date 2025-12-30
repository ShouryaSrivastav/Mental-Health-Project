# 🚀 Mental Health & Productivity Insights Dashboard

🔗 **Interactive Dashboard:** [View Live Dashboard](https://app.powerbi.com/view?r=eyJrIjoiYzc4ODlkNjgtZTMwOS00Y2JkLWE0ZTUtNzViNjc3NTIzMTMxIiwidCI6IjZiNGQwNDQ4LTc5MGMtNGQ5MS1iZjY3LTg5ZDk1NmJlNDEwYSJ9&pageName=8e5244683906612e0b36)
(View In Landscape Mode On Phone)

---

## 📌 Problem Statement

This dashboard provides a comprehensive analysis of mental health, lifestyle, work environment, and productivity across different **age groups, genders, and employment statuses**. By evaluating stress, sleep, productivity, and mental health risk, it enables stakeholders to:

- Understand patterns of **mental health risk** across employment categories and age groups.
- Monitor the correlation between **work environment, lifestyle, and productivity**.
- Identify high-risk groups to **inform mental health interventions and organizational strategies**.
- Visualize key trends for decision-making regarding **wellness programs and support initiatives**.

---

## 📊 Key Metrics (KPIs)

The dashboard tracks key indicators such as:

- **Total Respondents**: Number of survey participants
- **Stress Level**: Average stress level across groups
- **Sleep Hours**: Average sleep duration
- **Productivity Score**: Average productivity by demographics
- **Mental Health Risk**: Categorized risk based on anxiety & depression scores
- **Seeks Treatment**: Percentage of participants who sought mental health support

---

## 🎯 Business Requirements

- Age-wise and gender-wise **mental health trends**
- **Employment status and work environment** analysis for stress, sleep, and productivity
- Visual identification of **high-risk groups** for mental health support
- Comparisons across **lifestyle and productivity metrics** to identify patterns and correlations
- Interactive filtering with **slicers** to enable exploratory analysis

---

## 🔧 Workflow & Technical Steps

### 1️⃣ Data Acquisition

- Downloaded **Mental Health & Lifestyle dataset** covering multiple employment statuses (employed, unemployed, student, self-employed) and work environments (on-site, hybrid, remote)

---

### 2️⃣ Database Connection & Verification

- Imported dataset into **SQL Server (SSMS)**
- Performed **data verification**: checked column structure, row counts, and missing/invalid values
- Ensured **data integrity and consistency** for Power BI analysis
- SQL queries for verification and cleaning are available in a separate file (`SQL_Queries.sql`)

---

### 3️⃣ Data Cleaning & Transformation (Power Query Editor)

Performed all transformations in **Power Query Editor** for a clean and standardized dataset:

- **Column Management:** Changed types, added index column, reordered, and renamed columns
- **Value Standardization:** Replaced blanks, N/A, and unknowns for key fields
- **Conditional Columns:**
  - **Age Group:** 18–30 → *Young Adult*, 31–48 → *Adult*, 49–65 → *Elder*
  - **Work Environment:** Set *“Not Applicable”* for unemployed respondents
  - **Employment Status:** Updated *Student* → *Intern*
  - **Gender:** Non-binary and variants → *Others/Non-Binary*
- **Boolean Conversion:** True/False → Yes/No in *Seeks Treatment* and *Mental Health History*
- **Custom Columns & Filters:** Added derived metrics, filtered rows, and removed unnecessary columns

---

### 4️⃣ Power BI Dashboard Setup

- Connected cleaned dataset to **Power BI Desktop**
- Selected a **professional background** and **color palette**
- Designed **three interactive pages**: Overview, Mental Health Trends, and Lifestyle & Productivity
- Added **slicers** for Age Group, Employment Status, and Seeks Treatment to enable dynamic filtering

---

### 5️⃣ Advanced DAX Measures

- Total Respondents
- Average Stress, Sleep, and Productivity Scores
- Age Group & Gender-specific aggregations
- Mental Health Risk summaries
- Seeks Treatment & Mental Health History analysis

---

## 📊 Dashboard Preview & Insights

### 📄 Page 1 — Overview

**Visuals:** KPI Cards for Total Respondents, Stress, Sleep, Productivity

**Key Insights:** Provides a high-level snapshot of mental health and productivity trends.

![Page 1 — Overview](https://github.com/ShouryaSrivastav/Mental-Health-Project/blob/0a0aba6984c3243be2cad123a26e3748539df9eb/Page%201%20-%20Overview.png
)

---

### 📄 Page 2 — Mental Health Trends

**Visuals:** Clustered & stacked bar charts:
- Employment Status by Age Group
- Mental Health History by Age Group
- Mental Health Risk by Age Group
- Stress, Sleep, Productivity by Age & Gender

**Key Insights:** Highlights age and employment-specific trends in mental health risk and productivity.

![Page 2 — Mental Health Trends](https://github.com/ShouryaSrivastav/Mental-Health-Project/blob/0a0aba6984c3243be2cad123a26e3748539df9eb/Page%202%20-%20Mental%20Health%20Trends.png)

---

### 📄 Page 3 — Lifestyle & Productivity

**Visuals:**
- Combo charts & clustered bars: Productivity vs Stress, Sleep, Work Environment
- Lifestyle & Productivity by Gender
- Health Risk by Anxiety & Depression Scores

**Key Insights:** Shows correlation between lifestyle factors, work environment, and mental health risk. Student work environment updated to *Intern*.

![Page 3 — Lifestyle & Productivity](https://github.com/ShouryaSrivastav/Mental-Health-Project/blob/1ff507efbdadaaf4b16540661a17d150f7111724/Page%203%20-%20Productivity%20And%20Health%20Risk.png)

---

## 🛠️ Tools & Technologies

- **SQL Server (SSMS):** Data verification, integrity checks, preprocessing
- **Power Query Editor:** Data cleaning, conditional columns, type conversions
- **Power BI Desktop:** Dashboard design, interactive visualizations, DAX measures
- **Microsoft Excel:** Minor data transformations and exploration

---

## ✅ Conclusion

The **Mental Health & Productivity Insights Dashboard** demonstrates a full end-to-end analytics workflow:

1. Raw data acquisition → SQL verification
2. Data cleaning & transformation via Power Query
3. Interactive visualization and storytelling in Power BI

It converts messy survey data into actionable insights on mental health, lifestyle, and productivity, providing organizations a clear roadmap to support employee wellness and improve productivity outcomes.

---
