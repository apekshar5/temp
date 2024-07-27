```markdown
# Sales Data Analysis

This project aims to perform various analyses and visualizations on sales data provided in JSON format. The main focus is on calculating different sales metrics and visualizing trends and anomalies in the sales data.

## Table of Contents
- [Data Files](#data-files)
- [Usage](#usage)
- [Functions](#functions)
  - [calculate_net_sales](#calculate_net_sales)
  - [calculate_avg_net_sales_price](#calculate_avg_net_sales_price)
  - [calculate_gross_sales](#calculate_gross_sales)
  - [calculate_avg_gross_sales_price](#calculate_avg_gross_sales_price)
  - [calculate_avg_sales_last_5_days](#calculate_avg_sales_last_5_days)
  - [location_with_highest_sales](#location_with_highest_sales)
  - [price_changes](#price_changes)
  - [products_ordered_same_year](#products_ordered_same_year)
  - [visualize_avg_price_per_release_year](#visualize_avg_price_per_release_year)
  - [visualize_distribution_weekly_gross_sales](#visualize_distribution_weekly_gross_sales)
  - [visualize_gross_sales_per_week_with_anomalies](#visualize_gross_sales_per_week_with_anomalies)
  - [visualize_gross_sales_per_week_with_anomalies_2](#visualize_gross_sales_per_week_with_anomalies_2)
- [Main Function](#main-function)

## Data Files

The following JSON files are required for the analysis:
- `products.json`
- `orders.json`
   ```

1. Install the required dependencies:
   ```bash
   pip install pandas matplotlib seaborn scipy
   ```

## Usage

Run the main script to perform all tasks:
```bash
python script.py
```

## Functions

### `calculate_net_sales(orders)`
Calculates the net sales amount by subtracting the total prices of cancelled and returned orders from the total prices of created orders.

### `calculate_avg_net_sales_price(orders)`
Calculates the average net sales price by dividing the net sales amount by the net number of orders (created - cancelled - returned).

### `calculate_gross_sales(orders)`
Calculates the gross sales amount as the total prices of created orders.

### `calculate_avg_gross_sales_price(orders)`
Calculates the average gross sales price by dividing the gross sales amount by the number of created orders.

### `calculate_avg_sales_last_5_days(orders)`
Calculates the average sales amount for the last 5 days from the dataset.

### `location_with_highest_sales(orders)`
Determines the location(s) with the highest sales amount.

### `price_changes(orders)`
Calculates the price changes over time for each product_id, indicating whether the price has risen or fallen.

### `products_ordered_same_year(products, orders)`
Checks if products were ordered in the same year as their release date.

### `visualize_avg_price_per_release_year(products, orders)`
Visualizes the average price per release year for each location.

### `visualize_distribution_weekly_gross_sales(orders)`
Visualizes the distribution of weekly gross sales amount.

### `visualize_gross_sales_per_week_with_anomalies(orders)`
Visualizes the weekly gross sales amount and highlights anomalies using Z-score.

### `visualize_gross_sales_per_week_with_anomalies_2(orders)`
Visualizes the weekly gross sales amount and highlights anomalies using the Interquartile Range (IQR).

## Main Function

The `main()` function orchestrates the execution of all tasks and visualizations. It loads the data, performs calculations, and calls the appropriate visualization functions.

This `README.md` provides a comprehensive overview of the project, including details about the data files, installation steps, usage instructions, and descriptions of the functions. Adjust the GitHub repository link to your actual repository if needed.
