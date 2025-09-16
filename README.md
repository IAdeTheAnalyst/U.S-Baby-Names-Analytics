# 👶 Baby Names Analytics — MySQL Data Analysis

This project explores historical trends in U.S. baby names using the Social Security dataset. By analyzing naming patterns across years, states, regions, and genders in **MySQL 8 (Workbench)**, the project uncovers cultural influences, shifts in popularity, and long-term demographic trends.

## 🧠 Key Business Questions
1. What are the top 10 most popular baby names for boys and girls in each year?
2. How have naming trends changed over decades, and which names stayed consistently popular?
3. Which states or regions share similar naming patterns, and where do differences stand out?
4. Which names show sharp spikes/declines in popularity, and what eras do they align with?
5. How does name diversity (unique names per year) change over time?
6. Are there gender-specific trends in name length or “traditional vs. modern” styles?
7. Which names hold a **top-3** rank the longest across years or decades?
8. How does popularity differ across regions (e.g., New England vs. South vs. West)?
9. Which states drive the most births for the most popular names?

## 📊 Tools Used
- **SQL (MySQL 8+)** with **MySQL Workbench**
- **Common Table Expressions (CTEs)**
- **Aggregate Functions (SUM, COUNT, AVG)**
- **JOINs & Subqueries**
- **CASE Expressions**
- **Window Functions** (`ROW_NUMBER`, `RANK`, `DENSE_RANK`)
- **Data Cleaning/Standardization** (region normalization, state mapping)

## 📂 Dataset Overview
Tables used:
- **`names`** — `year`, `state`, `name`, `gender`, `births`
- **`regions`** — `state`, `region` (e.g., New England, Midwest, South, West, etc.)

> Note: Michigan (`MI`) is standardized to the **Midwest**. “New England” is normalized to `New_England` for consistent labeling.

## 🚀 Quick Start
1. Import CSVs into MySQL (Workbench → *Table Data Import Wizard*) or via `LOAD DATA INFILE`.
2. Ensure **MySQL 8+** (CTEs & window functions required).
3. (Optional) Add helpful indexes:
   ```sql
   CREATE INDEX idx_names_year_gender ON names(year, gender);
   CREATE INDEX idx_names_state ON names(state);
   CREATE INDEX idx_names_name_year ON names(name, year);
   CREATE INDEX idx_regions_state ON regions(state);
