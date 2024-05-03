# Just_Eat_Takeaway-end-to-end_Pipeline_building

This project focuses on Dimensional Modeling, building ETL Pipeline in Mage.ai using EC2 Instance from AWS services, storing the data model in S3 and loading the data into S3 bucket using PutObject into S3. Future scope of this project to be querying using Athena and leverage AWS Quicksight/Power BI for insights.

# Overview

Building data pipelines is a crucial component of any data infrastructure as they facilitate the efficient, reliable, and scalable flow of data from source systems to downstream applications. They ensure that data is ingested, processed, transformed, and delivered in a timely manner, enabling organizations to make data-driven decisions, gain valuable insights, and drive business growth. By automating the movement and processing of data, data pipelines reduce manual effort, minimize errors, improve data quality, and enhance overall productivity.

# Functionality

**Data Acquisition:** Download the dataset from Kaggle "Justeat restaurant Data"

**Dimensional Modeling:** The downloaded data is transformed into a star schema using Python

- Identifying facts** (measures of interest) and **dimensions** (descriptive attributes).
- Creating fact and dimension tables with appropriate data types and relationships.
- Cleaning and transforming data to ensure consistency and accuracy.
  
  ![Dimensional Modelling](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/92528843-d3b5-4987-a6c4-0c9da508a98f)

**Storing the model:**

- Saving the data in AWS S3 for easy access for ETL Processing.
![s3storage](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/1ef2b6dc-5b12-4e82-8f6c-cd2dd315deaf)

**ETL Processing:**

- Created an EC2 instance in AWS to run Mage-ai which will perfrom the ETL Task.
![pipeline status in EC2](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/da293885-85c2-417e-a39e-7c79b6064f6a)

    
**Extraction:**: Data is extracted from S3 bucket into Mage-ai

![Mage-1](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/518e5f2d-f631-41e6-8863-6e66f6f39fe8)

![Mage-2](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/f1b3bbc0-dcd0-44b9-8d0e-c88a7da2d098)

**Transformation** logic is done here, converting the flat file into fact and dimension.

Any further processing or aggregation can be performed 

**Data Loading:** The final processed data is loaded into another AWS service for further analysis (e.g., Amazon Redshift, Athena, Kinesis).

**ETL Pipeline in Mage-ai**
![ETL Pipeline](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/951dd1ce-d01c-4001-9af6-5adc401a6533)


**Benefits:**

- Automated and Efficient: The script automates data acquisition, dimensional modeling, and ETL, improving efficiency and reducing manual effort.
- Scalable: The pipeline can be easily scaled to handle larger datasets and increased processing needs.
- Improved Data Analysis: Dimensional modeling organizes data for efficient analysis and querying.
- Flexibility: Mage.ai allows for complex transformations and advanced workflows within the ETL process.
  
**Prerequisites**

- An AWS account with S3 bucket access and an EC2 instance.
- Mage.ai installed on the EC2 Instance. (See https://github.com/mage-ai/mage-ai for installation instructions)
- Kaggle Account to download the dataset.
