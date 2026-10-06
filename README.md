IBM Excel Basics for Data Analysis - Final Assignment
This repository contains the completed project files, datasets, and documentation for the Final Assignment of the Excel Basics for Data Analysis course (part of the IBM Data Analyst Professional Certificate).

📁 Repository Structure
Plaintext
├── Montgomery_Fleet_Equipment_Inventory_FA_PART_1_START.csv   # Initial raw dataset
├── Montgomery_Fleet_Equipment_Inventory_FA_PART_1_END.xlsx     # Cleaned dataset (Part 1 final output)
├── Montgomery_Fleet_Equipment_Inventory_FA_PART_2_END.xlsx     # Analyzed workbook with Pivot Tables (Part 2 final output)
└── README.md                                                  # Project documentation
📑 Project Workflow & Deliverables
Part 1: Data Cleaning & Preprocessing
The raw dataset (Montgomery_Fleet_Equipment_Inventory_FA_PART_1_START.csv) contained inconsistent entries, empty rows, duplicate records, and formatting issues. The following cleaning procedures were performed:

Workbook Conversion: Imported the raw CSV file into Excel and converted it to native .xlsx workbook format.

Column Width Adjustment: Auto-fitted all column widths so that header and cell values are completely legible.

Blank Row Removal: Filtered for and eliminated empty rows from the dataset.

Duplicate Record Removal: Identified and deduplicated redundant records across all columns.

Spelling Correction: Corrected typographical errors in departmental fields:

Enviromnental → Environmental

Rehabilltation → Rehabilitation

Recsue → Rescue

Servcies → Services

Whitespace Normalization: Removed double/extra whitespace characters across textual fields.

Column Unification: Merged split department name columns into a standardized single column using Flash Fill, subsequently removing redundant columns.

Final Export: Saved the clean output as Montgomery_Fleet_Equipment_Inventory_FA_PART_1_END.xlsx.

Part 2: Data Analysis & Pivot Tables
Using the cleaned dataset in Montgomery_Fleet_Equipment_Inventory_FA_PART_2_END.xlsx, data analysis tasks were carried out to organize and summarize fleet counts:

Table Formatting: Converted the data range (A1:C50) into a structured Excel Table with banded rows.

Summary Statistics (AutoSum): Computed core statistical measures for the Equipment Count column:

SUM: 1582

AVERAGE: 32.29 (approx. 32.2857)

MIN: 1

MAX: 379

COUNT: 49

Pivot Table 1 (Pivot Table 1):

Rows: Department

Values: Sum of Equipment Count

Ordering: Sorted in descending order by equipment count (top department: Transportation at 1,221).

Pivot Table 2 (Pivot Table 2):

Rows: Department (primary) and Equipment Class (secondary)

Values: Sum of Equipment Count

Hierarchy: Collapsed all department categories except the top department (Transportation), which is fully expanded.

Pivot Table 3 (Pivot Table 3):

Rows: Equipment Class (primary) and Department (secondary)

Values: Sum of Equipment Count

Hierarchy: Collapsed all equipment classes except the first vehicle class (CUV), displaying its department-level distribution.

Sheet Ordering: Worksheets are organized in sequence:
Montgomery_Fleet_Equipment_Inve → Pivot Table 1 → Pivot Table 2 → Pivot Table 3.

🛠️ Software & Tools Used
Excel for the Web / Microsoft Excel: Data cleaning, text operations, table structuring, and pivot table analysis.

Python (pandas, openpyxl): Data processing, automated validation, and workbook generation.

👤 Author
MD. MOAZZEM HOSSAIN MAJUMDER
