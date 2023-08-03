## ADF ETL pipeline for a library recommender system

An Azure Data Factory implemention for a Dataflows ETL pipeline from a library sql server to a Azure Gen2 Datalake organized for a recommender system. This is a cloud implemenatation that serves the same purpose as the following two on premise solutions:

https://github.com/szasadny/Import-Books-And-Keyword-Datasets-Into-MySQL

https://github.com/szasadny/Luigi-ETL-Pipeline

The only difference is that the sink of this solution is an Azure Datalake Storage Account instead of a snowflake SQL schema. The data stored in the sink in the Parquet format for optimized processing.

###  Infrastructure as Code
The adf_publish branch contains the Azure Resource Manager (ARM) template to import this pipeline. The current template assumes a source SQL database of the following format:

![ERD Bibliotheek Database drawio](https://github.com/szasadny/Luigi-ETL-Pipeline/assets/23632768/f3551e9f-262a-4ba8-b281-984de666bd86)
