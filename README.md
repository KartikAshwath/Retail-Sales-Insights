# Retail Sales Insights Project

This project processes retail sales data to prepare it for analysis and visualization in tools like Power BI.

## Project Description

The goal of this project is to take raw retail sales data, clean and transform it, and calculate key business metrics. The processed data is then saved to a new file that can be easily imported into business intelligence platforms for further analysis and reporting.

## Data

The project uses the `Retail_Sales_Insights.csv` file, which contains raw retail sales transaction data. The columns in the dataset include:

- **CID**: Customer ID
- **TID**: Transaction ID
- **Gender**: Customer's gender
- **Age Group**: Customer's age group
- **Purchase Date**: Date and time of the purchase
- **...**: Other relevant columns (refer to the original data file for the complete list)
- **Net Amount**: Net amount of the transaction
- **Gross Amount**: Gross amount of the transaction
- **Purchase Method**: Method of purchase
- **Location**: Location of the purchase
- **Discount Name**: Name of the discount applied (if any)
- **Discount Amount (INR)**: Amount of discount in INR

## Notebook Steps

The accompanying Jupyter notebook performs the following steps:

1.  **Data Loading and Preprocessing**:
    - Loads the `Retail_Sales_Insights.csv` file into a pandas DataFrame.
    - Converts the 'Purchase Date' column to a datetime format, handling mixed formats and ensuring day-first interpretation.
    - Fills missing values in the 'Discount Name' column with 'No Discount'.
    - Calculates 'Profit' and 'Profit Margin (%)' based on 'Net Amount' and 'Gross Amount'.

2.  **Key Metrics Summary**:
    - Calculates and prints key summary metrics such as Total Net Revenue, Total Customers, Average Discount Rate, and Average Profit Margin.

3.  **Saving Processed Data**:
    - Saves the processed DataFrame to a new CSV file named `Processed_Retail_Sales_Insights.csv`.

## Visualizations in Power BI

The processed data is well-suited for creating interactive dashboards in business intelligence tools. Here are some suggested visualizations based on the available data:

*   **Track Revenue**: Visualize total revenue over time, by location, or by age group.
*   **Analyze Top Products**: If product information is available (assuming it's in the '...' columns), you can identify and visualize top-selling products.
*   **Sales by Region**: Create maps or bar charts to show sales performance across different locations.
*   **Profitability Analysis**: Visualize profit margin by product category (if available), location, or over time.
*   **Customer Segmentation**: Analyze customer demographics (Gender, Age Group) in relation to purchase behavior.
*   **Discount Performance**: Evaluate the impact of different discounts on sales and profit margins.

You can create interactive dashboards to track these key metrics and gain deeper insights into the retail sales data.

## How to Use

1.  **Data Preparation**: Ensure the `Retail_Sales_Insights.csv` file is in the same directory as the notebook.
2.  **Run the Notebook**: Execute the cells in the notebook sequentially.
3.  **Access Processed Data**: The output file `Processed_Retail_Sales_Insights.csv` will be created in the same directory.
4.  **Analyze in BI Tool**: Import `Processed_Retail_Sales_Insights.csv` into your preferred business intelligence tool (e.g., Power BI) for creating dashboards and reports, utilizing the suggested visualizations above.

## Output File (`Processed_Retail_Sales_Insights.csv`)

This file contains the cleaned and enhanced data from the original dataset, including the newly calculated 'Profit' and 'Profit Margin (%)' columns, ready for immediate use in data analysis and visualization.
