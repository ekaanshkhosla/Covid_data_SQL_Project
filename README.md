# SQL_Projects

This repository showcases hands-on SQL projects involving data cleaning and data analysis using real-world datasets. It demonstrates the use of SQL for transforming messy data into structured formats and deriving meaningful insights.

## 📂 Projects

### 1. Data Cleaning of Nashville Housing Data

**Objective**: Clean and preprocess a housing dataset using SQL.

**Techniques Used**:
- Date format conversion
- Address imputation using `JOIN`
- Address parsing with `SUBSTRING`, `CHARINDEX`, and `PARSENAME`
- Conditional updates (`CASE WHEN`)
- Duplicate removal using `ROW_NUMBER() OVER`
- Column deletion and schema optimization

**Key SQL Concepts**:
- `CONVERT`, `ISNULL`, `SUBSTRING`, `CHARINDEX`, `PARSENAME`
- `JOIN`, `ROW_NUMBER()`, `CASE`, `CTE`, `ALTER TABLE`

**Sample Tasks**:
- Fix `SaleDate` format to proper date
- Split `PropertyAddress` and `OwnerAddress` into street, city, and state
- Standardize 'Y'/'N' to 'Yes'/'No' in `SoldAsVacant` column
- Remove duplicate records using CTE
- Drop unnecessary columns like `TaxDistrict`, `OwnerAddress`

---

### 2. Data Analysis of COVID-19 Data

**Objective**: Analyze the global COVID-19 impact using SQL queries on deaths and vaccination data.

**Skills Demonstrated**:
- Joins and Common Table Expressions (CTEs)
- Aggregation and percentage calculations
- Time-series trend analysis
- View creation for reusable queries

**Key Analyses**:
- Total cases vs. total deaths (fatality rates)
- Highest infection and death rates by country and continent
- Vaccination progress vs. population
- Global death trends over time

**Highlights**:
- Used window functions (`SUM(...) OVER`) to track vaccination accumulation
- Created views for streamlined analysis
- Focused on real-world scenarios (e.g., Germany’s fatality trend)


