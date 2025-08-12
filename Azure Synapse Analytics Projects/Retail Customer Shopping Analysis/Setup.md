## Setup Instructions

### Prerequisites
- Azure subscription
- Azure Synapse Workspace
- Azure Data Lake Storage Gen2
- Power BI Desktop
- Python 3.9+ (optional for local exploration)

### Steps
1. **Create Azure Data Lake Storage Gen2**
   - Create a storage account.
   - Create a container named `customer-data`.

(Azure Synapse Analytics Projects/Retail Customer Shopping Analysis/Images/StorageAccount-Container.png)


2. **Upload Dataset**
   - Download the CSV from Kaggle.
   - Upload to `customer-data/raw/`.
  
Azure Synapse Analytics Projects/Retail Customer Shopping Analysis/Images/FileUpload.png

3. **Set up Azure Synapse Analytics**
   - Create a Synapse workspace.
   - Connect to the Data Lake via linked service.
   - Create a serverless SQL pool.

4. **Export Data into Synapse Analytics**
   - Create db.
   - CREATE EXTERNAL DATA SOURCE shoppinganalysis
   - CREATE EXTERNAL FILE FORMAT delimitedTxtFileFormat
   - CREATE EXTERNAL TABLE ShoppingAnalysis
   - SELECT COUNT(*) FROM ShoppingAnalysis

  [Azure Synapse Analytics Projects/Retail Customer Shopping Analysis/Images/ExportIntoSynapse.png](https://github.com/mittalpk/Data-Engineering-Projects/blob/2e24d612ac0c5fd52f750d75fe400066357fd5f0/Azure%20Synapse%20Analytics%20Projects/Retail%20Customer%20Shopping%20Analysis/Images/ExportIntoSynapse.png)


