# New York Taxi Dataset Analysis using PySpark

This repository contains a Jupyter Notebook demonstrating data processing, cleaning, and analysis of the New York Taxi Dataset using PySpark. The notebook implements a robust and scalable pipeline for handling large datasets, making it ideal for performance benchmarking and gaining actionable insights.

## Features

### Data Loading
- Supports dynamic loading of taxi datasets in multiple sizes:
  - **Small (S)**: Minimal data for quick testing.
  - **Medium (M)**, **Large (L)**, **Extra Large (XL)**, and **XXL**: For progressively larger datasets to evaluate scalability.
- Handles data in Parquet and Delta formats.

### Data Cleaning and Preprocessing
- **Zero-value Removal**: Filters out rows with invalid or zero values for meaningful analysis.
- **Outlier Removal** (optional): Identifies and excludes extreme data points to improve result accuracy.

### Data Enrichment
- Joins trip data with taxi zone names for geographical insights.
- Calculates key metrics like total profit, passenger counts, and trip duration.

### Analytical Insights
- Summarizes trips and profits by taxi zones.
- Identifies the top 10 routes based on:
  1. Number of trips.
  2. Total profit.
  3. Passenger counts.
- Outputs visualizations and metrics for easy interpretation.

## Achievements
1. **Efficient Data Pipeline**: Processes datasets of varying sizes to demonstrate the scalability of PySpark for big data applications.
2. **Insightful Summaries**:
   - Top-performing zones and routes based on profitability and passenger demand.
   - Aggregated trip and zone statistics for further exploration.
3. **Performance Benchmarking**:
   - Allows comparison of processing times across dataset sizes, enabling evaluation of the system's performance and optimization potential.

## How to Use
1. Clone the repository and ensure you have PySpark and necessary dependencies installed.
2. Configure dataset paths and formats as needed in the `init_trips` function.
3. Run the notebook to load, process, and analyze the data.

## Example Output
Below are sample insights derived from the dataset:
- Top 10 routes by trip count and profitability.
- Total trips across different NYC zones.
