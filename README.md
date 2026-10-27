# Starbucks_Dashboard# 
An interactive Power BI dashboard project exploring Starbucks beverage nutrition and global store distribution. This project combines nutritional data with geographic store information to support data exploration and visual analysis.

## 📌 Project Overview

The project examines two datasets:

- **Starbucks Beverage Nutrition:** Nutritional information for beverages across different categories and preparation types.
- **Starbucks Store Directory:** Information about Starbucks store locations, ownership types, and geographic coordinates worldwide.

The Power BI dashboard presents key nutritional indicators, beverage comparisons, and a map of Starbucks store locations.

## 🎯 Project Objectives

- Analyze nutritional values across Starbucks beverages.
- Compare average calories, sugar, and caffeine.
- Explore beverage categories and preparation types.
- Examine caffeine variations across beverages.
- Visualize Starbucks' geographic store distribution.
- Build an interactive dashboard for easier data exploration.

## 📊 Dashboard Highlights

- **Total Beverages:** Overview of beverage records in the nutrition dataset.
- **Average Calories:** Summary of beverage calorie content.
- **Average Sugar:** Comparison of sugar levels across beverage records.
- **Average Caffeine:** Overview of caffeine content.
- **Beverage Category Analysis:** Explore nutritional patterns across categories.
- **Caffeine Comparison:** Compare average caffeine content by beverage.
- **Global Store Map:** Explore store distribution by country.
- **Interactive Filters:** Filter beverage data using preparation type and protein values.

## 🛠️ Tools & Technologies

- **Power BI Desktop** — Dashboard development and visualization
- **DAX** — Measures and KPI calculations
- **Power Query** — Data preparation and transformation
- **CSV** — Source data format
- **Data Visualization & EDA** — Pattern exploration and comparison

## 📁 Dataset Overview

### 1. Store Directory — `directory.csv`

Contains 25,600 store records and 13 columns covering store identifiers, addresses, country information, ownership type, time zone, and geographic coordinates.

### 2. Beverage Nutrition — `starbucks.csv`

Contains 242 beverage records and 18 columns covering beverage names, categories, preparation types, calories, macronutrients, vitamins, minerals, and caffeine.

## 🔍 Analytical Approach

1. Inspected the source datasets and their column structures.
2. Reviewed data types and missing values.
3. Identified relevant measures for nutritional analysis.
4. Designed KPI cards and comparative charts.
5. Incorporated geographic mapping for store locations.
6. Added filters to support interactive exploration.

## 💡 Key Analytical Questions

- How do calories vary across Starbucks beverage categories?
- What are the average sugar and caffeine levels?
- Which beverages have relatively higher caffeine content?
- How do nutritional characteristics vary across beverage types?
- How are Starbucks stores distributed across countries?
- How can filters help users investigate beverage characteristics?

## ⚠️ Data Considerations

- The store directory and beverage nutrition datasets describe different subjects and do not share an obvious common record-level key.
- The store map and beverage nutrition visuals should therefore be interpreted as separate analytical views unless a valid relationship is established.
- Some store contact details and location fields are missing.
- The caffeine column in the beverage dataset contains a missing value and should be checked before relying on its averages.
- The dataset represents the information provided in the source files, not necessarily Starbucks' current operational footprint or menu.

## 📈 Skills Demonstrated

- Data preparation and quality inspection
- Exploratory data analysis
- DAX measure development
- KPI design
- Interactive report development
- Geographic data visualization
- Analytical storytelling

## 👤 Author

**Srinidhi Bhat**

Aspiring Data Analyst | Power BI | SQL | Python | Data Visualization

This project is part of my ongoing journey to strengthen my analytical skills through practical, project-based learning.

