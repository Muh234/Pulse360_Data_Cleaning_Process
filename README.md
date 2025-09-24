# Data Cleaning with Excel – Pulse360 Advertising Case Study

## 📌 Project Overview
This project demonstrates **data cleaning using Excel** for Pulse360 Advertising, a full-service advertising firm.  
The dataset contained over **99,000 rows** with quality issues such as duplicates, missing values, inconsistent formats, and erroneous entries.  

The goal of this project was to **transform the raw marketing campaign dataset into a clean, analysis-ready format**.

---

## ⚙️ Data Cleaning Process

The cleaning was performed in Excel **column by column**, with the **process file** showing dirty values beside the cleaned results.  

### Examples of Cleaning Performed:
- **Company Column** → Removed extra spaces using `=TRIM()`.
- **Campaign_Type** → Standardized inconsistent categories (e.g., “SM (socail media)” → “Social Media”).
- **Target_Audience** → Split into two columns (age group & gender) using `=LEFT()`, `=RIGHT()`, and `=TEXTSPLIT()`. Replaced “All” with “Men & Women” and standardized to “All Ages”.
- **Channels_Used** → Fixed naming inconsistencies (“Google AD’s” → “Google Ads”).
- **Acquisition_Cost & ROI** → Removed `$` symbol and converted text to numeric values using `=VALUE()`.
- **Date** → Standardized into `MM/DD/YYYY` format using `=TEXT()`.
- **Missing Values** → Replaced blanks with default values where applicable (`=IF(ISBLANK(cell), 0, cell)`)

---

## ✅ Final Result
- A **process dataset** (`pulse360_cleaning_process.xlsx`) showing dirty vs cleaned columns side by side.  
- A **final cleaned dataset** (`pulse360_cleaned.xlsx`) containing only the clean values, ready for analysis and reporting.  

---

## 📂 Repository Structure
- `pulse360_Advertising_cleaning_process.xlsx` → Excel file with dirty + cleaned data side by side.  
- `Cleaned_Pulse360_advertising_data.xlsx` → Final cleaned dataset (values only).  

---

## 🛠️ Tools Used
- **Microsoft Excel**  
  - Functions: `TRIM`, `SUBSTITUTE`, `TEXTSPLIT`, `VALUE`, `IF`, `PROPER`, `TEXT`.    
  - Data validation and formatting.

---

## 🎯 Conclusion
This project transformed a **messy, inconsistent dataset** into a **structured, reliable dataset**.  
By cleaning missing values, duplicates, inconsistent formats, and outliers, the dataset is now **ready for accurate analysis and reporting**.
