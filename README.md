**Description:** To achieve improved data accessibility, enhanced data processing efficiency, and insightful analytics capabilities by establishing a scalable and efficient data pipeline for Just Eat Takeaway delivery dataset, leveraging AWS services.

### 2. **Approach:**
   - **Inception:** Motivated by the need to establish a robust data infrastructure for Just Eat Takeaway to analyze and derive insights from large volumes of data.
   - **AWS Infrastructure Setup:** Set up an AWS environment including EC2 instances for computation, S3 buckets for storage, and IAM roles for security.
   - **ETL Process**: Utilized Mage-ai, an ETL automation tool, in conjunction with EC2 instances, for efficient extraction, transformation, and loading of data. Mage-ai automated the ETL process, ensuring consistency and accuracy in data processing.
   - **Data Ingestion**: Once prepared and transformed, the data was transferred to S3 buckets using Python scripts running on EC2 instances. The Python scripts facilitated the ingestion process, ensuring seamless     transfer of data from the EC2 instances to S3 buckets.
     ![s3storage](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/1ef2b6dc-5b12-4e82-8f6c-cd2dd315deaf)
     
   - **Data Modeling:** Implemented dimensional modeling using Python (pandas library) to design a data warehouse schema optimized for analytics.
     ![Dimensional Modelling](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/92528843-d3b5-4987-a6c4-0c9da508a98f)
     
   - **Data Loading**: After processing, data was loaded into S3 buckets, ensuring easy access and integration for subsequent analysis. The data stored in S3 buckets was made publicly accessible for seamless access by EC2 instances

### 3. **Features and Functionality:**
   - **EC2 Instances:** Leveraged EC2 instances for computational tasks such as data processing, transformation, and loading.
     ![pipeline status in EC2](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/da293885-85c2-417e-a39e-7c79b6064f6a)
     
   - **S3 Storage:** Utilized S3 buckets for scalable and durable storage of raw and processed data, ensuring accessibility and reliability.
   - **Mage-ai ETL Automation:** Employed Mage-ai for automated ETL processes, reducing manual intervention and improving efficiency.
     ![Mage-1](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/518e5f2d-f631-41e6-8863-6e66f6f39fe8)
     ![Mage-2](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/f1b3bbc0-dcd0-44b9-8d0e-c88a7da2d098)
     
   - **Python Scripts:** Leveraged Python scripts to automate data ingestion tasks, facilitating the transfer of data to the AWS ecosystem.
   - **Dimensional Modeling with pandas:** Implemented dimensional modeling techniques using the pandas library to design a star schema for the data warehouse, enabling efficient querying and analysis.

### 4. **Outcomes:**
   - **Improved Data Accessibility:** Established a centralized data repository on AWS S3, enhancing accessibility and collaboration across teams.
   - **Enhanced Data Processing Efficiency:** Leveraged Mage-ai for ETL automation, reducing manual efforts and improving data processing efficiency.
     ![ETL Pipeline](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/951dd1ce-d01c-4001-9af6-5adc401a6533)
     
   - **Insightful Analytics:** Implemented dimensional modeling and analytics on EC2 instances, enabling Just Eat Takeaway to derive actionable insights from large volumes of data.
   - **Scalable Infrastructure:** Built a scalable infrastructure on AWS, ensuring the flexibility to handle increasing data volumes and analytic workloads.

### 5. **Future Plans:**
   - **Advanced Analytics:** Explore advanced analytics techniques such as machine learning and predictive modeling to derive deeper insights from the data.
   - **Real-time Processing:** Implement real-time data processing capabilities to enable immediate insights and decision-making.
   - **Cost Optimization:** Continuously optimize the AWS infrastructure to minimize costs while maximizing performance and scalability.
   - **Collaboration and Integration:** Collaborate with Just Eat Takeaway teams to integrate the data pipeline with existing systems and processes, enabling seamless data-driven decision-making.














































# Overview

Building data pipelines is a crucial component of any data infrastructure as they facilitate the efficient, reliable, and scalable flow of data from source systems to downstream applications. They ensure that data is ingested, processed, transformed, and delivered in a timely manner, enabling organizations to make data-driven decisions, gain valuable insights, and drive business growth. By automating the movement and processing of data, data pipelines reduce manual effort, minimize errors, improve data quality, and enhance overall productivity.

# Functionality

**Data Acquisition:** Download the dataset from Kaggle "Justeat restaurant Data"

**Dimensional Modeling:** The downloaded data is transformed into a star schema using Python

- Identifying facts** (measures of interest) and **dimensions** (descriptive attributes).
- Creating fact and dimension tables with appropriate data types and relationships.
- Cleaning and transforming data to ensure consistency and accuracy.
  


**Storing the model:**

- Saving the data in AWS S3 for easy access for ETL Processing.


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
