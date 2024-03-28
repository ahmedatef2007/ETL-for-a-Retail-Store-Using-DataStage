
# Data Modeling and Analysis for a Retail Store Using DataStage

## Project Overview:

This project implements a star-schema data warehousing flow using IBM InfoSphere DataStage. It involves joining sequential text files to create a data mart and performing analysis to gain insights into a fictional retail store's operations.

The objective is to efficiently extract, transform, and load (ETL) data from sequential text files, create a star-schema-based data mart, and derive meaningful analysis from it.

## Problem Statement:

A fictitious national department store aims to build a star-schema-based sales analysis data warehouse using sequential text files as the data source. Changes in dimension attributes are expected over time, requiring preservation of versions within the data warehouse.

The challenge is to accurately preserve changes in the star-schema data warehouse and enable queries related to prior versions of dimension attributes.

## Data Source:

Sequential text files serve as the data source for populating the star schema and creating the data mart.
![image](https://github.com/ahmedatef2007/Retail-Store-Data-Modeling-and-Analysis-using-IBM-DataStage/assets/60139719/5791e119-6dbb-464f-8467-45c550bad4bd)


## Project Steps:

The primary tool employed to address the problem is IBM InfoSphere DataStage, serving as an ETL tool. The steps involved are as follows:

**1- Building the Physical Data Model:** Construction of a star schema comprising three dimensions: `product`, `retail`, and `customer`, along with a fact table named `transactions`.

![image](https://github.com/ahmedatef2007/Retail-Store-Data-Modeling-and-Analysis-using-IBM-DataStage/assets/60139719/c1c725a1-ee30-4a13-9048-0583663d5a95)



**2- Extraction:** Extraction of data from the data warehouse, ensuring the inclusion of pertinent customer, store, and product information.

**3- Transformation:** Application of transformations to align extracted data with business requirements. This includes converting customer name columns to uppercase.

**4- Data Mart Creation:** Development of a data mart , containing transactional data for each customer categorized by customer type ("citizen" or "foreign"), product information, and purchased stock.

**5- Loading:** Loading of transformed data into a data mart .

**6- Data Mart Analysis:** Utilization of the data mart to fulfill various business needs, such as:

- Displaying the count of transactions for each employee in every store.
- Identifying the customer type ("citizen" or "foreign") generating the highest profit.
- Awarding bonuses to customers contributing the most to profit.

## Project Files:

- DataStage Dsx File : Contains the files for the DataStage jobs and the Meta Data for the files used.
- Dataset: Holds the data after being modeled in a star schema data warehouse format.
- MetaData: Stores the metadata of tables utilized in the DataStage jobs.
- Output_Data: Provides samples of analyzed data.

## DataStage Jobs:

![image](https://github.com/ahmedatef2007/Retail-Store-Data-Modeling-and-Analysis-using-IBM-DataStage/assets/60139719/782b6801-a3c3-4e5b-bae1-c5f7053c7b78)

![image](https://github.com/ahmedatef2007/Retail-Store-Data-Modeling-and-Analysis-using-IBM-DataStage/assets/60139719/8de30892-5b0e-41f1-bf13-ff58b347d8bd)

![image](https://github.com/ahmedatef2007/Retail-Store-Data-Modeling-and-Analysis-using-IBM-DataStage/assets/60139719/928e623d-2bed-40d7-a298-ffce36f3eee0)

![image](https://github.com/ahmedatef2007/Retail-Store-Data-Modeling-and-Analysis-using-IBM-DataStage/assets/60139719/c2926563-a848-419a-a784-091260d809be)


