# America's cheese divide: Walmart vs Whole Foods

This is a project for [Data Studio](https://journalism.columbia.edu/ms-data-journalism), Spring 2026.

This project analyses how cheese prices differ between Walmart and Whole Foods, and what that price gap reveals about fat content. The price and nutritional data comes from [GroceryDB](https://github.com/Barabasi-Lab/GroceryDB), a research database developed by the Barabasi Lab.

**Project page:** [https://dimuthuattanayake.github.io/cheese-story/](https://dimuthuattanayake.github.io/cheese-story/)

## Methodology

### Data collection and cleaning

* Downloaded the GroceryDB dataset from the [Barabasi Lab GitHub repository](https://github.com/Barabasi-Lab/GroceryDB)
* Filtered the dataset to include only cheese products
* Categorised products into 16 cheese types (Cheddar, Mozzarella, Parmesan, Gouda, etc.) by keyword matching on product names
* Removed uncategorised products and NAs
* Filtered to Walmart and Whole Foods only

### Analysis

* Compared median prices between Walmart and Whole Foods for each cheese type, calculating dollar and percentage gaps
* Calculated the overall median price difference across all cheese types ($2.53)
* For the fat-per-dollar analysis, filtered out outlier fat values (keeping only 0-50g per 100g) to remove data entry errors
* Computed fat-per-dollar ratios (Total Fat / price) for each product, then took the median fat per dollar for each cheese type
* Cross-referenced the price divide with the fat-per-dollar analysis to identify patterns

### Visualisations

* Created a range plot chart showing the price gap between Walmart and Whole Foods for each cheese type in Datawrapper
* Created a bar chart showing median fat per dollar by cheese type in Datawrapper

### Notebooks

| File | Description |
|------|-------------|
| `Cheese_comparison.ipynb` | Filters GroceryDB to cheese, categorises by type, compares median prices between Walmart and Whole Foods, calculates price gaps |
| `cheese_priceV_fat.ipynb` | Calculates fat-per-dollar ratios for each cheese type, filters outliers, computes median fat per dollar |
| `GroceryDB_foods.csv` | Source dataset from GroceryDB |

## New Skills

* Building my first range plot in Datawrapper
* Building a webpage into the portfolio site, then designing it with visualizations

## What more would I like to do?

* use a different methodology for fat per price analysis
* Do the same analysis with a more recent dataset, maybe with Trader Joe's instead of Walmart
* Analyse protein-per-dollar alongside fat-per-dollar to give a fuller nutritional picture
* Investigate whether imported vs loacal labelling explains the price gap within the same cheese type

## Contact

Dimuthu Attanayake, [dca2140@columbia.edu](mailto:dca2140@columbia.edu)
