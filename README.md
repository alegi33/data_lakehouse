## Date created
10th May 2023

## Project Title
Building an Azure Data Lake for Bike Share Data Analytics

## Description
In this project I implemented Lakehouse architecture on the Azure Databricks platform. I designed a star schema database, imported the raw data into DBFS, and transformed the data into fact and dimension tables according to the star schema. This project was done in Azure Databricks platform using Spark Notebook.

## Objectives
* Design a star schema based on the business outcomes
* Import the data into Azure Databricks using Delta Lake to create a Bronze data store
* Create a gold data store in Delta Lake tables
* Transform the data into the star schema for a Gold data store

## Files used
* raw csv files (https://drive.google.com/drive/folders/1sFpJ2lFZu45PuwirY_8_sQZ04oGoPIbl?usp=share_link)
* date dimension table (https://community.sisense.com/t5/knowledge/date-dimension-file/ta-p/9562)
* datalakehouse_starschema.pdf
* datalakehouse_project_notebook.ipynb

## Dataset
The raw dataset consists of trip, rider, payment and station data in separate csv files. These are the transactional data of a bike sharing platform which needs to be ingested into a database in a star schema model for analytical purposes.

## Data Transformation Approach
1) Raw csv files are uploaded into DBFS file storage system.
2) Using Spark Notebook, the csv files are extracted into the Delta file system and saved as Parquet files.
3) Load the data into tables in Delta storage by creating tables from the Parquet files.
4) Transform the data into star schema model (fact & dimension tables) using PySpark and save them as Delta tables.

## List of Resources
- udacity.com
- community.sisense.com
- dbdiagram.io

## Credits
* [Udacity](udacity.com)
* [community.sisense.com](https://community.sisense.com/t5/knowledge/date-dimension-file/ta-p/9562)
* [dbdiagram.io](https://dbdiagram.io/home)
