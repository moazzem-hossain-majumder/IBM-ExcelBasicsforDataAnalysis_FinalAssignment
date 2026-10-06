# IBM Excel Basics for Data Analysis – Final Assignment

This repository contains the completed project files, datasets, and documentation for the **Final Assignment** of the **IBM Excel Basics for Data Analysis** course, which is part of the **IBM Data Analyst Professional Certificate**.

The project focuses on **data cleaning, preprocessing, Excel table formatting, summary statistics, and Pivot Table analysis** using a Montgomery County fleet equipment inventory dataset.

---

## 📁 Repository Structure

```text
├── Montgomery_Fleet_Equipment_Inventory_FA_PART_1_START.csv
│   └── Initial raw dataset
│
├── Montgomery_Fleet_Equipment_Inventory_FA_PART_1_END.xlsx
│   └── Cleaned dataset – Part 1 final output
│
├── Montgomery_Fleet_Equipment_Inventory_FA_PART_2_END.xlsx
│   └── Analyzed workbook containing Pivot Tables – Part 2 final output
│
└── README.md
    └── Project documentation
```

---

# 📑 Project Workflow & Deliverables

## Part 1: Data Cleaning & Preprocessing

The original dataset contained **inconsistent entries, blank rows, duplicate records, spelling errors, formatting issues, and split department-name fields**.

The following data-cleaning procedures were performed.

### 1. Workbook Conversion

The raw CSV dataset was imported into Excel and converted into a native `.xlsx` workbook.

**Input:**

```text
Montgomery_Fleet_Equipment_Inventory_FA_PART_1_START.csv
```

**Output:**

```text
Montgomery_Fleet_Equipment_Inventory_FA_PART_1_END.xlsx
```

### 2. Column Width Adjustment

Column widths were automatically adjusted so that headers and cell values were fully visible and readable.

### 3. Blank Row Removal

The dataset was filtered to identify and remove empty rows that did not contain meaningful records.

### 4. Duplicate Record Removal

Duplicate records were identified and removed to ensure that each fleet equipment record appeared only once.

### 5. Spelling Correction

Typographical errors in departmental names were identified and corrected.

| Incorrect | Correct |
|---|---|
| `Enviromnental` | `Environmental` |
| `Rehabilltation` | `Rehabilitation` |
| `Recsue` | `Rescue` |
| `Servcies` | `Services` |

### 6. Whitespace Normalization

Extra and duplicate whitespace characters were removed from textual fields to improve consistency.

### 7. Column Unification

Split department-name columns were combined into a single standardized department column using **Flash Fill**.

Redundant columns were subsequently removed.

### 8. Final Export

The cleaned dataset was saved as:

```text
Montgomery_Fleet_Equipment_Inventory_FA_PART_1_END.xlsx
```

---

# 📊 Part 2: Data Analysis & Pivot Tables

The cleaned dataset was further analyzed to organize and summarize the fleet equipment inventory.

The final workbook is:

```text
Montgomery_Fleet_Equipment_Inventory_FA_PART_2_END.xlsx
```

## 1. Table Formatting

The dataset range:

```text
A1:C50
```

was converted into a structured Excel Table with **banded rows** for improved readability and organization.

---

## 2. Summary Statistics

Using Excel's **AutoSum** functionality, the following statistics were calculated for the **Equipment Count** column:

| Statistic | Result |
|---|---:|
| **SUM** | 1,582 |
| **AVERAGE** | 32.29 |
| **MIN** | 1 |
| **MAX** | 379 |
| **COUNT** | 49 |

> The exact average is approximately **32.2857**, which is displayed as **32.29** when rounded to two decimal places.

---

# 📌 Pivot Table Analysis

Three Pivot Tables were created to analyze the distribution of fleet equipment across departments and equipment classes.

## Pivot Table 1

**Purpose:** Summarize the total equipment count by department.

**Configuration:**

- **Rows:** Department
- **Values:** Sum of Equipment Count
- **Sorting:** Descending order by equipment count

The department with the highest equipment count was:

> **Transportation — 1,221 equipment units**

---

## Pivot Table 2

**Purpose:** Analyze equipment counts by department and equipment class.

**Configuration:**

- **Rows:** Department
- **Rows:** Equipment Class
- **Values:** Sum of Equipment Count

### Hierarchy

All department categories were collapsed except the department with the highest equipment count:

**Transportation**

The Transportation department was fully expanded to display its equipment-class distribution.

---

## Pivot Table 3

**Purpose:** Analyze equipment classes and their distribution across departments.

**Configuration:**

- **Rows:** Equipment Class
- **Rows:** Department
- **Values:** Sum of Equipment Count

### Hierarchy

All equipment classes were collapsed except the first vehicle class:

**CUV**

The CUV category was expanded to display its department-level distribution.

---

# 📑 Worksheet Organization

The final workbook organizes the worksheets in the following sequence:

```text
1. Montgomery_Fleet_Equipment_Inve
2. Pivot Table 1
3. Pivot Table 2
4. Pivot Table 3
```

This structure makes it easy to move from the cleaned source data to progressively detailed Pivot Table analysis.

---

# 🛠️ Software & Tools Used

### Microsoft Excel / Excel for the Web

Used for:

- Data cleaning
- Text manipulation
- Removing duplicates
- Removing blank rows
- Flash Fill
- Table formatting
- Summary statistics
- Pivot Table creation
- Data organization and analysis

### Python

The project workflow also used Python for data processing and validation.

Libraries used:

- **pandas** — Data manipulation and processing
- **openpyxl** — Excel workbook processing and generation

---

# 🎯 Key Skills Demonstrated

This project demonstrates practical skills in:

- Excel data cleaning
- Data preprocessing
- Data quality improvement
- Duplicate detection and removal
- Text and whitespace normalization
- Excel Flash Fill
- Structured Excel Tables
- Descriptive statistics
- Pivot Table creation
- Hierarchical data analysis
- Data summarization
- Spreadsheet organization
- Python-assisted data validation

---

# 📚 Course Information

**Course:** IBM Excel Basics for Data Analysis  
**Program:** IBM Data Analyst Professional Certificate  
**Assignment:** Final Assignment

---

# 👤 Author

**MD. MOAZZEM HOSSAIN MAJUMDER**

---

## ⭐ Project Purpose

This project demonstrates the practical application of **Microsoft Excel data-cleaning and analysis techniques** on a real-world fleet inventory dataset. It serves as part of a data analytics portfolio and demonstrates foundational skills required for **Data Analyst** roles.
