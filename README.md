# 📊 HR Analytics Dashboard – Power BI Portfolio Project

## 🎯 Project Objective

To create a comprehensive and interactive **HR Analytics Dashboard** in Power BI that provides **actionable insights into employee attrition patterns**, aiming to:

- Improve employee retention  
- Streamline recruitment strategies  
- Elevate workforce satisfaction and performance  

---

## 🔧 Tools Used

- **Power BI Desktop**  
- **Power Query Editor**  
- **DAX (Data Analysis Expressions)**  

---

## 🧩 Project Workflow Overview

### 1️⃣ Data Collection

The dataset was sourced from the **HR Management System**, comprising the following details:

- Employee demographics  
- Job roles  
- Education  
- Salary  
- Tenure  
- Attrition data  

---

### 2️⃣ Data Cleaning & Preparation (Power Query)

All preprocessing was performed in **Power BI's Power Query Editor**, including:

- Removed irrelevant and duplicate records  
- Renamed ambiguous columns for better clarity  
- Converted data types:
  - Age → Whole Number  
  - Salary → Decimal Number  
- Created derived columns:
  - **Salary Slabs** (e.g., Up to ₹5K, ₹5K–10K, etc.)  
  - **Age Groups** (e.g., 18–25, 26–35, etc.)  
  - **Years at Company Buckets**

---

### 3️⃣ Data Modeling & DAX Calculations

Custom DAX measures and columns were created to support **dynamic KPIs**:

```dax
Total Employees = DISTINCTCOUNT(Employee[EmployeeID])

Attrition Count = COUNTROWS(FILTER(Employee, Employee[Attrition] = "Yes"))

Attrition Rate = DIVIDE([Attrition Count], [Total Employees], 0)

Average Salary = AVERAGE(Employee[Salary])

Average Age = AVERAGE(Employee[Age])

Years at Company = AVERAGE(Employee[YearsAtCompany])


## 📈 Dashboard Design

### 🔹 Dashboard Highlights

- Professional and clean color theme for executive readability  
- Interactive **Department Filter**: HR, Research & Development, Sales  
- Uniform chart formatting with **tooltips for additional insights**

---

### 🔹 Key KPIs (Top Summary Tiles)

| Metric             | Value    |
|--------------------|----------|
| Total Employees    | 1,473    |
| Attrition Count    | 237      |
| Attrition Rate     | 16.1%    |
| Average Age        | 37 years |
| Average Salary     | ₹6.5K    |
| Avg. Tenure        | 7 years  |

---

## 📊 Visualizations Used

| Visual Type        | Description                                      |
|--------------------|--------------------------------------------------|
| Bar Charts         | Attrition by Age, Salary Slab, Job Role          |
| Donut Chart        | Attrition by Education                           |
| Line Chart         | Attrition by Years at Company                    |
| Clustered Column   | Attrition by Gender                              |
| Matrix Table       | Attrition by Job Role & Tenure Period            |
| Slicer Buttons     | Department-wise interactive filtering            |

---

## 🔍 Insights & Analysis

### ✳️ General Attrition Trends

- Highest attrition occurred in the **26–35 age group** (116 employees)  
- Employees with **Life Sciences education** (38%) showed highest attrition  
- **Salary bracket up to ₹5K** had the most attrition cases (163 employees)  
- Employees typically left after **1 year of service** (59 cases)  
- **Male attrition (140)** was higher than **female attrition (79)**  

---

### ✳️ Job Role Insights

| Job Role               | Attrition Count |
|------------------------|-----------------|
| Laboratory Technician  | 62              |
| Sales Executive        | 57              |
| Research Scientist     | 47              |

---

## 🎯 Recommendations for HR Strategy

- **Career Development Programs**: Especially for the 26–35 age group  
- **Salary Review**: Enhance pay structure for employees under ₹5K  
- **Retention Programs**: Focus on onboarding and first-year experience  
- **High-Attrition Roles**: Create initiatives for Sales Executives & Lab Technicians  
- **Gender-Specific Interventions**: Explore factors behind higher male attrition  
- **Flexible Work Policies**: Support new or single employees better  

---

## 🚧 Challenges Faced

| Area              | Description                                                  |
|-------------------|--------------------------------------------------------------|
| Data Quality      | Incomplete or inconsistent records required heavy cleaning   |
| DAX Complexity    | Designing custom KPIs and conditional metrics was complex    |
| Clarity in Visuals| Balancing multiple filters, departments, and metrics cleanly |

---

## ✅ Key Skills Demonstrated

- **Power BI**: Data Import, Modeling, Visualization  
- **Power Query**: Data Cleaning, M Code Transformation  
- **DAX**: Measure & Column Creation, Time Intelligence Functions  
- **Dashboard UX**: Filters, Slicers, Tooltips, Interactivity  
- **Insight Generation**: Business-driven insights and recommendations  

---

## 📷 Dashboard Preview

> ![Dashboard Preview](images/hr-dashboard-preview.png)
