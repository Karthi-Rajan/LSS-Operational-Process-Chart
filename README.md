# LSS-Operational-Process-Chart

# 🏭 LSS Operational Process Dashboard with Pareto Analysis (Power BI)

This project is a **Lean Six Sigma (LSS) Operational Process Dashboard** built in **Power BI** to identify and visualize **wastes (VA, NVA, SVA)** in a process, with a strong emphasis on **Pareto Analysis** to prioritize key issues.

---

## ✅ Project Objective

- Identify and categorize operational activities into:
  - ✅ **VA** – Value-Added
  - ⚠️ **NVA** – Non-Value-Added
  - 🟡 **SVA** – Sub-Value-Added
- Highlight bottlenecks and inefficiencies using **Pareto Charts**
- Enable stakeholders to **prioritize improvements** using 80/20 rule

---

## 📦 Project Workflow

### 1. 🔄 Data Loading & Preparation

- **Data Sources**: 6 Process Tables from Excel
- **Loading Tool**: Power BI (Excel Import)
- **Data Structure**: Each sheet contains columns like:
  - `Process Step`
  - `Description`
  - `Duration (Decimal)`
  - `Category` (VA/NVA/SVA)
- **Merged into a Unified Table** using Power Query with a new column for `Source Table Name`

---

### 2. 🧮 Calculated Columns & Measures

**Key Columns Created:**
- `Total Duration (sec)` = Decimal minutes converted to duration (hh:mm:ss)
- `Category` classification VA/NVA/SVA based on activity type
- `Source Table Name` to differentiate between process sheets

**DAX Measures:**
- `Total VA Time`
- `Total NVA Time`
- `Total SVA Time`
- `% of NVA`
- `Cumulative % for Pareto`

---

## 📊 Dashboard Pages & Visuals

### 📄 1. Overall Operational Efficiency

**Visuals:**
- **Pie Chart**: Share of VA, NVA, SVA
- **KPI Cards**:
  - Total Duration
  - VA Time
  - NVA Time
  - % NVA
- **Stacked Column Chart**: Duration by Category per Process
- **Slicers**: Sheet Name, Category, Process Step

![image](https://github.com/user-attachments/assets/9bb48845-fc2e-4a9e-8327-83356a348f9a)

---

### 📄 2. Pareto Analysis

**Visuals:**
- **Pareto Chart** (Bar + Line Combo):
  - X-axis: Top Process Descriptions
  - Left Y-axis: Count of Occurrences
  - Right Y-axis: Cumulative Percentage
- **Card**: Top 3 contributing problems
- **Slicer**: Category (VA, NVA, SVA), Sheet Name


![image](https://github.com/user-attachments/assets/677f76c5-87d2-4a51-99b7-f4cca2f42f3b)

---

### 📄 3. Sheet-Level Analysis

**Visuals:**
- **Table View**: Process Step, Description, Time, Category
- **Bar Chart**: Category-Wise Waste by Sheet
- **Filter**: Individual sheet slicer to drill down

![image](https://github.com/user-attachments/assets/285776a4-83dd-4631-9df4-f58ecdab8dd8)


---

## 🛠️ Tools & Technologies Used

| Tool        | Purpose                               |
|-------------|----------------------------------------|
| Power BI    | Data analysis and dashboarding         |
| Power Query | Data transformation and merge          |
| DAX         | Custom measures and KPIs               |
| Excel       | Source of operational data             |

---

## 📁 Suggested Folder Structure

