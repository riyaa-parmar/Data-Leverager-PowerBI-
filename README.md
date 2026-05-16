# 📊 Power Query Data Transformation Project

## 📌 Overview
This project demonstrates data transformation and preparation using Power Query in Power BI. It includes combining multiple files, cleaning data, and performing advanced transformations.

## 📂 Data Sources
- Sales Data (Jan–Apr Excel files from folder)
- Employee Data (Excel file)
- Product Category Sales Data (for Pivot/Unpivot)
- Web Source: Wikipedia (Country-wise population)
- Folder-based source using parameter (FolderPath)

## ⚙️ Transformations Performed

### 🔹 Data Cleaning
- Removed unnecessary columns
- Renamed columns
- Trimmed and formatted text
- Fixed date format using Change Type with Locale

### 🔹 Date Transformations
- Extracted Year, Month, Day, Quarter
- Created Fiscal Month (April–March financial year)

### 🔹 Custom Columns
- Created Full Name column
- Created Sales Category:
  - High (≥ 10000)
  - Medium (5000–9999)
  - Low (< 5000)

### 🔹 Indexing
- Added 0-based and 1-based index columns

### 🔹 Pivot & Unpivot
- Unpivoted regional data
- Pivoted data for analysis

### 🔹 Merging & Appending
- Merged Sales Data with Employee Data using Region
- Appended monthly files (Jan–Apr)

### 🔹 Aggregation
- Grouped by Region
- Calculated:
  - Total Sales
  - Average Sales
  - Total Transactions

### 🔹 Parameters
- Created FolderPath parameter
- Used dynamic loading:
  Folder.Files(FolderPath)

### 🔹 Refresh Simulation
- Added new file (Sales_Apr.xlsx)
- Refreshed query
- Verified automatic data update

## 🚧 Challenges & Solutions
- Date format issues → fixed using Locale
- Binary/Text errors → corrected query steps
- Wrong parameter type → changed to Text
- Missing columns → rebuilt query properly

## ✅ Final Outcome
- Automated data loading using parameters
- Dynamic refresh with new files
- Clean and structured dataset
- Complete ETL process using Power Query

## 🛠 Tools Used
- Microsoft Excel
- Power BI (Power Query Editor)

## 📎 Files Included
- .pbix file
- Excel datasets
- Project Report (PDF)

## 📬 Author
Riya Parmar
