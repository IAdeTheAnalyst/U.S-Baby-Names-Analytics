# Baby Names Analytics — MySQL Data Analysis

In this project, I analyzed historical U.S. baby name data from the Social Security Administration using MySQL 8 (Workbench). My goal was to identify long-term naming trends, regional differences, and shifts in popularity over time by applying advanced SQL techniques to a large, multi-decade dataset.

Through structured querying and data transformation, I uncovered patterns that reflect cultural influences, demographic shifts, and evolving naming preferences across states, regions, and genders.

## Project Objectives
In this analysis, I aimed to answer the following business questions:

1. What are the top 10 most popular baby names for boys and girls in each year?
2. How have naming trends changed over decades, and which names stayed consistently popular?
3. Which states or regions share similar naming patterns, and where do differences stand out?
4. Which names show sharp spikes/declines in popularity, and what eras do they align with?
5. How does name diversity (unique names per year) change over time?
6. Are there gender-specific trends in name length or “traditional vs. modern” styles?
7. Which names hold a **top-3** rank the longest across years or decades?
8. How does popularity differ across regions (e.g., New England vs. South vs. West)?
9. Which states drive the most births for the most popular names?

## Tools & Technical Approach
In this project, I used:

- **SQL (MySQL 8+)** with **MySQL Workbench**
- **Common Table Expressions (CTEs)**
- **Aggregate Functions (SUM, COUNT, AVG)**
- **JOINs & Subqueries**
- **CASE Expressions**
- **Window Functions** (`ROW_NUMBER`, `RANK`, `DENSE_RANK`)
- **Data Cleaning/Standardization** (region normalization, state mapping)

## What I Learned
Through this project, I strengthened my ability to:

- Use window functions to rank and compare entities over time
- Structure complex queries using CTEs for clarity and scalability
- Translate raw data into meaningful business insights
- Identify long-term trend stability versus short-term volatility
- Analyze geographic segmentation and its impact on popularity patterns

I also gained a deeper understanding of how cultural and regional factors influence measurable demographic outcomes.

## Challenges I Encountered
One challenge I faced was managing performance when ranking names across many years and states. I addressed this by restructuring queries using CTEs and optimizing aggregation logic.

Another challenge involved cleaning and standardizing region classifications to ensure consistent geographic comparisons. This required careful validation and normalization of state-to-region mappings.

Additionally, interpreting trend volatility required thoughtful query design to distinguish between short-term spikes and sustained popularity.

## Dataset Overview
The primary table used in this project was:

- names-> containing year, state, name, gender, and births

This dataset enabled longitudinal and regional analysis across multiple decades of U.S. naming history.
