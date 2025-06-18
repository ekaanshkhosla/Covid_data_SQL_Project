# SQL_Projects

This repository showcases hands-on SQL projects involving data cleaning and data analysis using real-world datasets. It demonstrates the use of SQL for transforming messy data into structured formats and deriving meaningful insights.

---

## 📂 Projects

### 1. Data Cleaning of Nashville Housing Data

**Objective**: Clean and preprocess a housing dataset using SQL.

**Techniques Used**:
- Standardizing and converting date formats
- Filling missing values via self joins
- Splitting composite address fields into meaningful components
- Standardizing categorical values (Y/N → Yes/No)
- Identifying and removing duplicates
- Dropping unnecessary columns

**Key SQL Concepts**:
- `CONVERT`, `ISNULL`, `SUBSTRING`, `CHARINDEX`, `PARSENAME`
- `JOIN`, `ROW_NUMBER()`, `CASE`, `CTE`, `ALTER TABLE`, `UPDATE`, `DROP COLUMN`

**Sample Tasks**:
- Convert `SaleDate` from text to date type
- Fill null `PropertyAddress` values using parcel matches
- Split `OwnerAddress` into street, city, and state
- Clean up `SoldAsVacant` values
- Remove duplicates using `ROW_NUMBER()` and a CTE
- Drop columns like `TaxDistrict` and `SaleDate`


---

### 2. Data Analysis of COVID-19 Data

**Objective**: Explore COVID-19 trends using SQL, including case counts, fatalities, and vaccination progress.

**Techniques Used**:
- Filtering and aggregating time-series data
- Calculating derived metrics (e.g., death %, infection rate)
- Joining multiple datasets
- Using CTEs and Window Functions
- Creating views for reusable analysis

**Key SQL Concepts**:
- `JOIN`, `GROUP BY`, `ORDER BY`, `WHERE`, `CAST`, `CONVERT`
- Window functions: `SUM(...) OVER (PARTITION BY...)`
- CTEs: `WITH ... AS (...)`
- Creating views: `CREATE VIEW`

**Sample Tasks**:
- Analyze death rate by country and by population
- Determine countries with the highest infection and fatality rates
- Track cumulative vaccinations using rolling sums
- Summarize death trends globally by date
- Use CTE to simplify vaccination-percentage queries
- Create a persistent view `PPV` for population vs. vaccination stats
