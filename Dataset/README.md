# 📁 Starbucks Analytics — Dataset Documentation

## Overview

This project uses two CSV datasets to explore Starbucks beverage nutrition and global store locations.

The datasets support two distinct analytical perspectives:

1. Nutritional analysis of Starbucks beverages.
2. Geographic analysis of Starbucks store distribution.

## 1. `starbucks.csv` — Beverage Nutrition Dataset

### Dataset Summary

| Property | Details |
|---|---|
| Records | 242 |
| Columns | 18 |
| File format | CSV |
| Primary focus | Beverage nutrition |
| Analytical use | Nutritional comparisons and beverage analysis |

### Column Description

| Column | Description |
|---|---|
| `Beverage_category` | Category of the beverage |
| `Beverage` | Name of the beverage |
| `Beverage_prep` | Beverage preparation or serving variant |
| `Calories` | Calories per listed beverage serving |
| `Total Fat (g)` | Total fat in grams |
| `Trans Fat (g)` | Trans fat in grams |
| `Saturated Fat (g)` | Saturated fat in grams |
| `Sodium (mg)` | Sodium in milligrams |
| `Total Carbohydrates (g)` | Total carbohydrates in grams |
| `Cholesterol (mg)` | Cholesterol in milligrams |
| `Dietary Fibre (g)` | Dietary fibre in grams |
| `Sugars (g)` | Sugar content in grams |
| `Protein (g)` | Protein content in grams |
| `Vitamin A (% DV)` | Percentage of daily value for vitamin A |
| `Vitamin C (% DV)` | Percentage of daily value for vitamin C |
| `Calcium (% DV)` | Percentage of daily value for calcium |
| `Iron (% DV)` | Percentage of daily value for iron |
| `Caffeine (mg)` | Caffeine content in milligrams |

### Analytical Applications

- Compare calories across beverage categories.
- Examine sugar and protein content.
- Identify beverages with relatively high caffeine content.
- Compare nutritional values across preparation types.
- Explore relationships between beverage categories and nutritional characteristics.

### Data Quality Considerations

- The `Caffeine (mg)` column contains one missing value.
- Some numerical columns may require data type conversion because they are stored as text.
- Nutritional percentages include `%` symbols and may require cleaning before numerical analysis.
- Column names contain inconsistent leading or trailing spaces.
- Verify serving-size consistency when comparing beverage records.

## 2. `directory.csv` — Starbucks Store Directory

### Dataset Summary

| Property | Details |
|---|---|
| Records | 25,600 |
| Columns | 13 |
| File format | CSV |
| Primary focus | Store locations |
| Analytical use | Geographic and ownership analysis |

### Column Description

| Column | Description |
|---|---|
| `Brand` | Store brand |
| `Store Number` | Store identifier |
| `Store Name` | Name of the store |
| `Ownership Type` | Ownership classification, such as licensed |
| `Street Address` | Street-level address |
| `City` | City where the store is located |
| `State/Province` | State or province |
| `Country` | Country code |
| `Postcode` | Postal or ZIP code |
| `Phone Number` | Store contact number |
| `Timezone` | Store's time zone |
| `Longitude` | Geographic longitude |
| `Latitude` | Geographic latitude |

### Analytical Applications

- Visualize store locations on a geographic map.
- Examine store distribution by country and region.
- Compare store ownership classifications.
- Explore the geographic spread of the Starbucks network.
- Investigate missing location and contact information.

### Data Quality Considerations

The supplied dataset contains missing values in several fields:

| Column | Missing records |
|---|---:|
| `Street Address` | 2 |
| `City` | 15 |
| `Postcode` | 1,522 |
| `Phone Number` | 6,861 |
| `Longitude` | 1 |
| `Latitude` | 1 |

These values should be handled appropriately for the intended analysis. In particular, records without valid geographic coordinates may not display correctly on a map.

## 🔗 Relationship Between the Datasets

The beverage nutrition dataset describes products, while the store directory describes physical locations.

There is no obvious shared record-level key between these datasets. They should be treated as separate analytical subjects unless a valid business relationship is identified.

## 🧹 Recommended Data Preparation

1. Inspect column names and data types.
2. Remove unnecessary leading and trailing spaces from column names.
3. Convert numeric text fields into appropriate numeric data types.
4. Handle missing caffeine values before calculating averages.
5. Standardize percentage-based nutritional columns where numerical analysis is required.
6. Validate latitude and longitude values before geographic mapping.
7. Retain store identifiers as text to preserve their original format.

## 🛠️ Tools

- Power BI Desktop
- Power Query
- DAX
- CSV datasets

## 📌 Disclaimer

This documentation describes the supplied files. It does not establish that the data represents Starbucks' current menu or store network. Nutritional values should be interpreted according to the serving and preparation information provided in the source dataset.

