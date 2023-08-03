## ADF ETL pipeline for a library recommender system

An Azure Data Factory implemention for an ETL pipeline from a library sql server to a Azure Gen2 Datalake organized for a recommender system. This is a cloud implemenatation that serves the same purpose as the following two on premise solutions:

https://github.com/szasadny/Import-Books-And-Keyword-Datasets-Into-MySQL

https://github.com/szasadny/Luigi-ETL-Pipeline

The only difference is that the sink of this solution is an Azure Datalake Storage Account instead of a snowflake SQL schema. The data stored in the sink in the Parquet format for optimized processing.
