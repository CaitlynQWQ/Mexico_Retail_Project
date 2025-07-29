# 📍 Understanding the Food Retail Landscape in Mexico City

## 🧭 Project Overview

This project analyzes how the rise of corporate retail businesses is impacting small, traditional food stores in Mexico City, using spatial data from 2010 and 2019. Through rigorous geospatial analysis in **R**, it explores store “births” and “deaths”, spatial clustering patterns, and neighborhood-level concentration changes over time.

The goal: to understand **whether modern food retailers are displacing traditional ones**, and how this reshapes the urban economic geography.

---

## 📊 Data Source

* **DENUE (Directorio Estadístico Nacional de Unidades Económicas)** by INEGI, Mexico
* Two snapshots: **2010** and **2019**, covering food retail businesses in Mexico City.

Key preprocessing challenges:

* Inconsistent street names & mislabeled postal codes
* No unique business IDs across years
* Ambiguous duplicate records and location mismatches

---

## 🛠️ Tools & Packages

* **Data Cleaning**: `dplyr`, `tidyverse`, fuzzy matching
* **Geospatial Analysis**: `sf`, `sp`, `spatstat`, `tmap`
* **Mapping & Visualization**: choropleth maps, clustering plots
* **Statistical Techniques**:

  * Location Quotient (LQ)
  * Spatial Point Pattern Analysis: `G`, `F`, `L`, and `J` functions

---

## 🔍 Key Methods

1. **Data Wrangling**

   * Standardized geolocation and postal codes
   * Matched 2010 and 2019 business records
   * Classified stores into “Traditional” (e.g., *abarrotes*) vs. “Modern” (e.g., supermarkets)

2. **Store Status Detection**

   * Created “birth”, “death”, and “survival” tags for each store based on time slices

3. **Spatial Analysis**

   * Mapped and compared clustering of store types
   * Calculated LQ per municipality and visualized change from 2010 to 2019

---

## 🌎 Key Findings

* Traditional stores became **more spatially clustered** over time.
* Modern stores expanded toward the **northwest and southeast**.
* Several municipalities saw significant **declines in traditional store concentration**.
* Spatial inequality in food retail access may be increasing.

---

## 📁 Repository Structure

| File                                    | Description                                     |
| --------------------------------------- | ----------------------------------------------- |
| `business_birth_and_death_analysis.Rmd` | Identifies store "births" and "deaths"          |
| `correct_postcode_cleanup.Rmd`          | Cleans and harmonizes postal code data          |
| `geospatial_analysis_mexico.Rmd`        | Performs spatial analysis and pattern detection |
| `geospatial_plot_mexico.Rmd`            | Creates mapping visualizations                  |
| `data_cleaning_week4.Rmd`               | Early-stage data cleaning steps                 |
| `poster.pdf`              | Poster summarizing research findings            |

---

## 👩‍💻 About the Author

*Caitlyn Cai* — Data analyst and geospatial enthusiast, passionate about using **R** to uncover urban and economic spatial dynamics.
