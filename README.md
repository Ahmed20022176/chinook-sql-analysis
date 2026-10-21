# Chinook SQL Analysis

## Overview
SQL-based analysis of the Chinook database, a fictional digital music store, to answer key business questions about product sales, revenue by region and monthly performance.

## Business questions answered
- Which tracks and genres sell the most?
- Which countries generate the most revenue?
- How does revenue change month by month and year by year?
- Who are the top customers?

## What I did
- Explored the database structure (11 tables, 3,503 tracks, 412 invoices, 2009 to 2013)
- Wrote JOINs across up to 4 tables (InvoiceLine, Track, Album, Artist, Genre)
- Used GROUP BY and aggregate functions to summarize revenue and units sold
- Used CTEs and window functions: `ROW_NUMBER()` to rank the top 3 tracks per genre, and `LAG()` to calculate month-over-month change
- Visualized results with Seaborn and Matplotlib

## Key findings
- **Total revenue:** 2,328.60 across 412 invoices
- **Top market:** USA (523.06), followed by Canada (303.96) and France (195.10)
- **Top genre:** Rock (826.65 revenue, 835 units), well ahead of Latin (382.14) and Metal (261.36)
- **Yearly revenue is stable**, between about 450 and 481, peaking in 2010 (481.45)
- **Top customers:** Helena Holý (Czech Republic, 49.62) and Richard Cunningham (USA, 47.62)
- Best-selling tracks all tie at 2 units, so genre and country are more useful indicators of performance

## SQL concepts used
INNER JOIN | GROUP BY | Aggregate functions | CTEs | Window functions (ROW_NUMBER, LAG) | Date functions (strftime)

## Tools
SQL, SQLite, Python, Pandas, Seaborn, Matplotlib, Google Colab

## Files
- `Chinook_SQL_Analysis.ipynb`: full analysis with queries, results and charts
- `Chinook_Sqlite.sqlite`: the database

## Dataset
Chinook Database (Kaggle)
