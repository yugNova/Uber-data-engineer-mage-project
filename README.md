# Uber Data Analytics | Modern Data Engineering GCP Project 
## Introduction
In this comprehensive project, we leverage Google Cloud Platform to build an advanced ETL pipeline for Uber's data. By integrating cloud storage, mage.ai, and Looker Studio, we transform raw data into valuable insights, driving informed business strategies.

## Architecture
![Project Architecture](architecture.jpg)

## Technology Used
- Programming Language - Python
- Scripting Language - SQL
- Google Cloud Platform
   - BigQuery
   - CLoud Storage
   - Looker Studio
   - Compute Instance
- Mage.AI (Modern Data Pipeline Tool)

** Modern data Pipeline Tool: https://www.mage.ai/

##Dataset Used 
TLC Trip Record data
Yellow and green taxi trip record include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types,  and driver-reported passenger counts.

Here is the dataset - https://github.com/yugNova/Uber-data-engineer-mage-project/blob/main/uber_data.csv 

## Data Model 
![Data Model Image](data_model.jpeg)

## Scripts for Project
- [extract.py](mage-files)
- [load.py](mage-files)
- [transform.py](mage-files)

## Challenge 
1. ### Managing and processing large volumes of data efficiently.
   - Solution - Use Google Cloud Storage to store raw data and BigQuery for processing and analysis. Both are designed to handle large datasets.
  
      - Implement partitioning and clustering in BigQuery to optimize query performance and cost.
    
        
2. ### Ensuring the data is clean, consistent, and free of errors.
   - Solution - Use data validation techniques during the ETL process to check for missing values, duplicates, and inconsistencies.

       -Implement data quality checks in your transformation scripts (transform.py) to handle and correct errors.

3. ### Integrating Mage.AI with Google Cloud services.
   - Solution - Follow Mage.AI’s integration guides and documentation for seamless setup.

       - Use Google Compute Instances to run Mage.AI if needed, ensuring that the environment is properly configured to interact with Google Cloud services.
