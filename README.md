# Adventure Works Sales Performance Report (Power BI)

## Overview
A six-page Power BI report for Adventure Works, a fictional bike retailer, built on synthetic data covering January 2023 to September 2026. It answers five questions: are we on target, what drives growth, which products need attention, who are the best customers, and where do online shoppers drop off.

## Data
- Source: a deliberately messy 15-sheet Excel workbook with 134,000+ rows
- 13 types of data-quality issue, including test orders, duplicates, mixed date formats and orphaned customer keys
- After cleaning: 97,661 order lines worth $114.0M, 281 products, 16,628 customers, 10 territories and 4 sales channels

## What I did
- **Power Query:** removed 36 test orders and 225 duplicates, appended four yearly sales sheets, merged and unpivoted tables, fixed locale-specific dates
- **Data model:** star schema with 4 fact and 7 dimension tables, plus a DAX date table
- **DAX:** 60 measures covering time intelligence, ranking, targets and returns, each checked against control totals
- **Report:** 20 visuals across four main pages, a Product Detail drill-through page and a tooltip page
- **Interactivity:** synced slicers, drill-down hierarchies and controlled cross-filtering
- **Accessibility:** colour-blind-safe theme, alt text and tab order
- **Security:** static and dynamic row-level security (USERPRINCIPALNAME), tested with View as

## Key insights
- Growth slowed from 26.9% in 2024 to 9.9% in January–September 2026, with sales at 97.4% of target
- The UK and Canada delivered 76% of 2026 growth
- Electric bikes rose from 6.1% to 41.7% of bike sales since 2023
- The E-Trail 900's return rate reached 7.9% in 2025, four times the bike average
- Customers earning $120,000+ spend 3.7 times as much as others
- Only 16.4% of product-page viewers add to cart

## Tools
Power BI Desktop, Power Query, DAX, Excel

## Files
- `AdventureWorks_Sales.pbix`: the report file
- `AdventureWorks_Sales_Messy_2023-2026.xlsx`: source workbook
- `AdventureWorks_Accessible_Theme.json`: colour theme
- `/screenshots`: one image per report page

## Author
Nand
