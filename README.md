# Covid Data SQL Project

This repository contains SQL-based data cleaning and analysis projects focusing on COVID-19 datasets. It demonstrates core SQL skills like joins, CTEs, window functions, views, and data transformation techniques.

## 📁 Repository Structure

- `Data-Cleaning-of-covid-data-in_SQL/`  
  SQL scripts for cleaning and preprocessing real estate transaction data.
  
- `Data-analysis-of-covid-data_in_SQL/`  
  SQL queries exploring COVID-19 cases, deaths, and vaccination data.

---

## 🧹 Data Cleaning Highlights (`Data-Cleaning-of-covid-data-in_SQL/`)

Tasks performed on the `NH` (Nashville Housing) dataset:

- **Date Standardization:** Converted `SaleDate` to SQL `Date` format.
- **Address Normalization:**  
  - Filled missing `PropertyAddress` using self-joins.
  - Split addresses into `Address`, `City`, and `State` using `SUBSTRING` and `PARSENAME`.
- **Vacancy Column Fix:** Replaced `Y/N` in `SoldAsVacant` with `Yes/No`.
- **Deduplication:** Removed duplicates using `ROW_NUMBER()` with CTE.
- **Cleanup:** Dropped unused columns like `TaxDistrict` and `OwnerAddress`.

---

## 📊 Data Analysis Highlights (`Data-analysis-of-covid-data_in_SQL/`)

Exploratory SQL analysis on two datasets: `Covid Deaths (CD)` and `Covid Vaccinations (CV)`.

- **Case Fatality Rate:**  
  Calculated `(total_deaths / total_cases) * 100` for different countries.
  
- **Infection Rate:**  
  Countries with the highest infection percentages relative to population.
  
- **Deaths by Continent:**  
  Aggregated death data to evaluate impact across continents.
  
- **Vaccination Progress:**  
  Used window functions (`SUM OVER PARTITION`) to compute cumulative vaccinations.
  
- **Global Metrics Over Time:**  
  Tracked global new cases and deaths by date.

- **Views & CTEs:**  
  Created a view (`PPV`) and used CTE (`PopvsVac`) for organized data reuse.

---

## 🛠️ Skills Demonstrated

- SQL Joins (Inner Join)
- Window Functions
- Common Table Expressions (CTEs)
- Aggregate Functions
- Data Type Conversion
- Data Cleaning & Formatting
- View Creation

---

## 📌 Note

This project is intended for SQL learning and practice. The datasets are anonymized and used for educational purposes only.

