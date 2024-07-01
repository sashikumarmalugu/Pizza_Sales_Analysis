# Pizza_Sales_Analysis
This project involves ingesting tables from an on-premise SQL Server database to Azure Data Lake using Azure Data Factory. Azure Databricks then transforms the raw data into a clean form. Finally, Microsoft Power BI integrates with Azure Synapse Analytics to build an interactive dashboard.
# Architecture Flow
<img width="678" alt="PizzaSales" src="https://github.com/sashikumarmalugu/Pizza_Sales_Analysis/assets/172464710/87061899-507d-4447-971b-354660710627">

### On-Premise SQL Server:

Represents the source of the data.
Connected to Azure Data Factory (ADF).
### Azure Data Factory (ADF):

Ingests data from the on-premise SQL Server.
Transfers data to Azure Data Lake Storage Gen2.
### Azure Data Lake Storage Gen2:

Stores raw data ingested by ADF.
Connected to Azure Databricks.
### Azure Databricks:

Reads raw data from Azure Data Lake.
Transforms raw data into a clean, processed form.
Stores processed data back in Azure Data Lake or writes directly to Azure Synapse Analytics.
### Azure Synapse Analytics:

Stores the processed data from Azure Databricks.
Provides data to Power BI.
### Microsoft Power BI:

Connects to Azure Synapse Analytics.
Creates interactive dashboards and reports using the processed data.
