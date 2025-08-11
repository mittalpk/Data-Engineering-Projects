# Retail Customer Shopping Analysis – Azure Synapse Analytics

This project analyzes a retail chain's customer shopping data from Istanbul to uncover:
- Top revenue-generating product categories.
- Spending patterns by age and gender.
- Most popular payment methods per location.

The project uses **Azure Synapse Analytics** with **Azure Data Lake Storage Gen2** to store, transform, and query large-scale datasets, and Power BI for visualization.

## Dataset
Source: [Kaggle - Customer Shopping Dataset](https://www.kaggle.com/datasets/mehmettahiraslan/customer-shopping-dataset)

Fields:
- `invoice_no`: Invoice ID
- `date`: Purchase date
- `customer_id`: Unique customer identifier
- `gender`: Male/Female
- `age`: Customer age
- `category`: Product category
- `quantity`: Number of items purchased
- `price`: Price per item
- `payment_method`: Cash/Credit Card/Other
- `shopping_mall`: Location of purchase

## Architecture
1. **Azure Data Lake Storage Gen2** → Stores raw CSV from Kaggle.
2. **Azure Synapse Analytics (Serverless SQL Pool)** → Runs exploratory and transformation queries.
3. **Azure Synapse Pipelines (ETL)** → Cleans and structures the data.
4. **Power BI** → Creates dashboards and visualizations.
