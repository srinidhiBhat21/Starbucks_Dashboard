# ☕ Starbucks Analytics Dashboard — Power BI

## 📌 Overview

The Starbucks Analytics Dashboard is an interactive Power BI report designed to explore beverage nutrition and global store distribution.

The dashboard combines KPI cards, comparative charts, interactive filters, and geographic mapping to make the supplied Starbucks datasets easier to explore.

**Tool:** Microsoft Power BI Desktop

## 🎯 Dashboard Objectives

- Summarize important beverage nutrition metrics.
- Compare nutritional characteristics across beverage categories.
- Explore average caffeine levels across beverages.
- Enable filtering by beverage preparation and protein values.
- Visualize the geographic distribution of Starbucks stores.

## 📊 Key Performance Indicators

### 1. Total Beverages

Displays the total number of beverage records represented by the dashboard's underlying measure.

This KPI provides a high-level overview of the beverage dataset.

### 2. Average Calories

Summarizes the average calorie content of beverage records.

This metric supports comparisons between beverage categories and helps identify differences in energy content.

### 3. Average Sugar

Displays average sugar content across the relevant beverage records.

This KPI helps users explore sugar variation across beverage types and preparation options.

### 4. Average Caffeine

Summarizes caffeine content across the available beverage records.

This measure supports the identification of beverage categories and products with comparatively high caffeine levels.

*The exact results depend on the DAX measure definitions, active filters, and handling of missing values.*

## 📈 Visualizations

### Beverage Category Analysis

An area chart compares average calories across beverage categories.

**Purpose:**
- Explore variation in average calories between categories.
- Identify categories with comparatively higher or lower average calorie content.
- Support nutritional comparisons.

### Beverage Category Distribution

A doughnut chart represents the distribution of beverage records across categories using the total beverage measure.

**Purpose:**
- Understand the composition of the beverage dataset.
- Compare the relative contribution of beverage categories.
- Identify categories with more or fewer records.

### Average Caffeine by Category

A clustered bar chart compares average caffeine content across beverage categories.

**Purpose:**
- Compare caffeine levels across categories.
- Identify categories with relatively high average caffeine.
- Support beverage-level exploration.

### Global Starbucks Store Map

A geographic map uses the store directory's country and coordinate information.

**Purpose:**
- Explore the international distribution of Starbucks locations.
- View the geographic spread of the store directory.
- Investigate store coverage across different countries.

The number of visible map locations depends on the geographic fields, data quality, and map aggregation settings.

### Beverage-Level Caffeine Comparison

A column chart compares average caffeine values across individual beverages.

**Purpose:**
- Examine differences in caffeine content between beverages.
- Identify relatively high-caffeine options.
- Explore variation between beverage records.

## 🎛️ Interactive Filters

### Beverage Preparation

The preparation filter enables users to select beverage preparation variants and investigate how the selected records affect dashboard metrics and charts.

### Protein Range

The protein filter enables users to restrict the beverage records to a selected protein range.

These filters help users explore the data from different perspectives rather than relying solely on overall averages.

## 🧮 Measures and Calculations

The report includes measures for total beverages, average calories, average sugar, and average caffeine.

Illustrative DAX formulas for these metrics are shown below. Confirm that your actual measure names and data types match before replacing existing measures.

```dax
Total Beverages =
COUNTROWS(starbucks)
```

```dax
Avg Cals =
AVERAGE(starbucks[Calories])
```

```dax
Avg Sugar =
AVERAGE(starbucks[ Sugars (g)])
```

```dax
Avg Caff =
AVERAGE(starbucks[Caffeine (mg)])
```

**Important:** The source file contains leading or trailing spaces in some column names, and the caffeine column may be stored as text. Adjust the column references and convert data types in Power Query as necessary. These examples are not a verification of the exact formulas already implemented in the PBIX file.

## 🗺️ Data Sources

### Beverage Nutrition

**File:** `starbucks.csv`

Contains beverage names, categories, preparation types, calories, macronutrients, vitamins, minerals, and caffeine content.

### Store Directory

**File:** `directory.csv`

Contains store identifiers, names, addresses, ownership classifications, countries, time zones, and geographic coordinates.

The two datasets support separate analyses. Do not assume that beverage records can be directly joined to individual stores.

## 🚀 How to Open the Dashboard

1. Download or clone the project repository.
2. Install Microsoft Power BI Desktop if it is not already installed.
3. Open `Starbucks_Dashboard.pbix`.
4. If prompted, update the data source paths to the locations of `starbucks.csv` and `directory.csv`.
5. Refresh the data if required.
6. Use the filters to explore beverage nutrition and compare the displayed metrics.
7. Interact with the charts and map to investigate the available data.

## 🔍 Suggested Business Questions

- Which beverage categories have higher average calorie content?
- How does average sugar content vary across beverage records?
- Which beverages have relatively high caffeine content?
- How does beverage preparation affect nutritional comparisons?
- What does the store map reveal about Starbucks' geographic reach?
- How do interactive filters change the metrics and chart comparisons?

## 📚 Skills Demonstrated

- Power BI dashboard development
- DAX measures and KPI creation
- Data modeling and Power Query
- Exploratory data analysis
- Comparative data visualization
- Geographic mapping
- Interactive report design
- Analytical communication

## 👤 Author

**Srinidhi Bhat**

Aspiring Data Analyst | Power BI | SQL | Python | Data Analytics


