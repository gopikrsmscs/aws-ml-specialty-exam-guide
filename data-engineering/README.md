## Data Engineering

Data engineering involves building systems that collect, manage, and convert data into usable information for various purposes.

### Exam Topics

In the AWS exam, you will be tested on the following key topics related to Data Engineering:

1. **Create Data Repositories for Machine Learning**
   - [Amazon S3 (Simple Storage Service)](#as3)
   - [Amazon EFS (Elastic File System)](#aefs)
   - [Amazon EBS (Elastic Block Storage)](#aebs)

2. **Identify and Implement a Data Ingestion Solution**
   - Batch Processing & Stream Processing
   - [Amazon Kinesis](#akinesis)
   - Amazon Kinesis Data Analytics
   - Amazon Kinesis Data Firehose
   - Amazon EMR
   - [AWS Glue](#aglue)
   - AWS DataSync

3. **Identify and Implement a Data Transformation Solution**
   - Transform data in transit
     - [AWS Glue](#aglue)
     - ETL (Extract Transform and Load)
       - Amazon EMR
       - AWS Batch
   - Using Map Reduce
     - Apache Hadoop
     - Apache Spark
     - Apache Hive

### 1.1 AWS S3 <a name="as3"></a>
- Object Storage
- Objects can be up to 5GB in size.
- Objects are stored in buckets.
- Object names must be unique.
- Provides 11 9's of durability.
- S3 Lifecycle management for automatic migration of objects to other S3 Storage Classes.
- **Storage Classes**
  - **General purpose**
    - S3 Standard
      - Low latency and high performance.
      - Designed for 99.99% availability over a given year.
  - **Changing Access**
    - S3 Intelligent-Tiering
      - Data that is accessed less frequently but requires rapid access when needed.
      - No operational overhead, no lifecycle charges, no retrieval charges, and no minimum storage duration.
    - S3 Standard-Infrequent Access
    - S3 One Zone-Infrequent Access
  - **Archive**
    - S3 Glacier Instant Retrieval
      - Rarely accessed and requires retrieval in milliseconds.
    - S3 Glacier Flexible Retrieval (Formerly S3 Glacier)
      - For archive data that is accessed 1—2 times per year and is retrieved asynchronously.
    - S3 Glacier Deep Archive
      - Long-term retention and digital preservation for data that may be accessed once or twice in a year.
- **Use Cases**
  - Build data lakes.
  - Backup and restore critical data.
  - Archive data at low cost.

### 1.2 Amazon EFS <a name="aefs"></a>
(TODO: Add content about Amazon EFS)

### 1.3 Amazon EBS <a name="aebs"></a>
(TODO: Add content about Amazon EBS)
