### **Description:** 
To achieve improved data accessibility, enhanced data processing efficiency, and insightful analytics capabilities by establishing a scalable and efficient data pipeline for Just Eat Takeaway delivery dataset, leveraging AWS services.

### **Approach:**
   - **Inception:** Motivated by the need to establish a robust data infrastructure for Just Eat Takeaway to analyze and derive insights from large volumes of data.
   - **AWS Infrastructure Setup:** Set up an AWS environment including EC2 instances for computation, S3 buckets for storage, and IAM roles for security.
   - **ETL Process**: Utilized Mage-ai, an ETL automation tool, in conjunction with EC2 instances, for efficient extraction, transformation, and loading of data. Mage-ai automated the ETL process, ensuring consistency and accuracy in data processing.
   - **Data Ingestion**: Once prepared and transformed, the data was transferred to S3 buckets using Python scripts running on EC2 instances. The Python scripts facilitated the ingestion process, ensuring seamless     transfer of data from the EC2 instances to S3 buckets.
     ![s3storage](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/1ef2b6dc-5b12-4e82-8f6c-cd2dd315deaf)
     
   - **Data Modeling:** Implemented dimensional modeling using Python (pandas library) to design a data warehouse schema optimized for analytics.
     ![Dimensional Modelling](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/92528843-d3b5-4987-a6c4-0c9da508a98f)
     
   - **Data Loading**: After processing, data was loaded into S3 buckets, ensuring easy access and integration for subsequent analysis. The data stored in S3 buckets was made publicly accessible for seamless access by EC2 instances

### **Features and Functionality:**
   - **EC2 Instances:** Leveraged EC2 instances for computational tasks such as data processing, transformation, and loading.
     ![pipeline status in EC2](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/da293885-85c2-417e-a39e-7c79b6064f6a)
     
   - **S3 Storage:** Utilized S3 buckets for scalable and durable storage of raw and processed data, ensuring accessibility and reliability.
   - **Mage-ai ETL Automation:** Employed Mage-ai for automated ETL processes, reducing manual intervention and improving efficiency.
     ![Mage-1](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/518e5f2d-f631-41e6-8863-6e66f6f39fe8)
     ![Mage-2](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/f1b3bbc0-dcd0-44b9-8d0e-c88a7da2d098)
     
   - **Python Scripts:** Leveraged Python scripts to automate data ingestion tasks, facilitating the transfer of data to the AWS ecosystem.
   - **Dimensional Modeling with pandas:** Implemented dimensional modeling techniques using the pandas library to design a star schema for the data warehouse, enabling efficient querying and analysis.

### **Outcomes:**
   - **Improved Data Accessibility:** Established a centralized data repository on AWS S3, enhancing accessibility and collaboration across teams.
   - **Enhanced Data Processing Efficiency:** Leveraged Mage-ai for ETL automation, reducing manual efforts and improving data processing efficiency.
     ![ETL Pipeline](https://github.com/Ashvakg/Justeats_DataEngineering/assets/83398283/951dd1ce-d01c-4001-9af6-5adc401a6533)
     
   - **Insightful Analytics:** Implemented dimensional modeling and analytics on EC2 instances, enabling Just Eat Takeaway to derive actionable insights from large volumes of data.
   - **Scalable Infrastructure:** Built a scalable infrastructure on AWS, ensuring the flexibility to handle increasing data volumes and analytic workloads.

### **Future Plans:**
   - **Advanced Analytics:** Explore advanced analytics techniques such as machine learning and predictive modeling to derive deeper insights from the data.
   - **Real-time Processing:** Implement real-time data processing capabilities to enable immediate insights and decision-making.
   - **Cost Optimization:** Continuously optimize the AWS infrastructure to minimize costs while maximizing performance and scalability.
   - **Collaboration and Integration:** Collaborate with Just Eat Takeaway teams to integrate the data pipeline with existing systems and processes, enabling seamless data-driven decision-making.
