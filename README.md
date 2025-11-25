# 📘 Tableau-HR-Dashboard-Project

<img width="1200" height="650" alt="HR  Dashboard" src="https://github.com/user-attachments/assets/47a7a9bc-2ceb-42ce-9f74-4df72f4f4d46" />

## 1. **Project Overview and Objective**



The HR Dashboard is designed to provide a comprehensive view of workforce performance, demographics, and compensation across the organization. It enables HR leaders to monitor key metrics such as headcount, hiring and termination trends, salary distribution, and employee performance.

**Primary Objective:**
To help HR teams **identify workforce trends**, **improve employee retention**, **ensure compensation fairness**, and **support strategic workforce planning** through data-driven insights.

---

## 2. **Data Source and Preparation**

### **Dataset Used**

* **Filename:** `dataset.csv`
  (*uploaded and processed together with the dashboard*)

### **Key Columns Utilized**

The dashboard is built using the following major fields from the dataset:

* `Employee_ID`
* `Gender`
* `State`
* `City`
* `Education Level`
* `Department`
* `Job Title`
* `Salary`
* `Performance Rating`

### **Data Preparation Steps**

Several transformations were likely performed to prepare the dataset for visualization:

* **Age Calculation**
  Derived from `Birthdate` → *Age = Today – Birthdate*
* **Tenure Calculation**
  Derived from `Hiredate` → *Tenure = Today – Hiredate*
* **Turnover Rate Calculation**
  Using `Termdate` and `Employee_ID` to identify terminated employees
* **Standardization of categories**
  (e.g., normalizing Education Level labels)
* **Salary aggregation**
  for averages by Department and Job Title
* **Geographical grouping**
  to analyze workforce distribution by State or City

---

## 3. **Key Dashboard Components (Parameters)**

The Tableau HR Dashboard contains multiple analytical components. Based on the dataset and visuals, the key parameters and KPIs include:

### **A. Workforce Demographics**

* Gender distribution (Male vs. Female)
* Education level breakdown (High School, Bachelor’s, Master’s, PhD)
* Geographic distribution by `State` and `City`
* Department-level headcount

### **B. Compensation Analysis**

* Average salary by:

  * Department
  * Job Title
  * Education level
  * Gender (pay equity check)
* Salary distribution across age groups

### **C. Performance Metrics**

* Distribution of `Performance Rating` across the workforce
* Cross-analysis:

  * Education Level × Performance
  * Department × Performance
  * Manager-level performance patterns

### **D. Stability and Turnover**

* Total active employees
* Employee hires vs. terminations
* Tenure analysis
* Turnover rate (derived from termination count & active headcount)

---

## 4. **Key Insights & Business Recommendations**

Using common HR analytic patterns and the column structures, the following business recommendations are generated:

### **Recommendation 1 — Compensation & Performance**

If analysis shows that employees with *Excellent* or *Good* performance ratings earn salaries similar to or lower than *Satisfactory* performers, **a compensation equity review is recommended**.
➡️ *Adjust pay bands or performance-based incentives to ensure high performers are recognized and retained.*

---

### **Recommendation 2 — Retention & Turnover**

If certain departments (e.g., Customer Service, Sales, or IT) show higher termination rates or shorter average tenure, HR should **conduct stay interviews and exit-pattern analysis**.
➡️ *Identifying root causes—such as workload, manager relationships, or unclear career progression—can directly reduce attrition.*

---

### **Recommendation 3 — Workforce Planning & Diversity**

If demographic analysis reveals underrepresented groups (e.g., gender imbalance in IT or lack of PhD-level employees in R&D), HR should **adjust recruitment strategies**.
➡️ *Target hiring in specific cities/states, partner with universities, or create internal upskilling programs to improve role readiness and diversity.*

---
