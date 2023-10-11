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
     - Kinesis Data Stream
     - Kinesis Data Firehose
     - Kinesis Data Analytics or Apache Flink
     - Kinesis Video Analytics
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
- Object/File Storage
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
  - **Unknown or Changing Access**
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
    - Stores structured,semi and unstructured data.
  - Backup and restore critical data.
  - Archive data at low cost.

### 1.2 Amazon EFS <a name="aefs"></a>
- Serverless, fully elastic file storage.
- 5 GB of standard storage.
- Scalable, elastic, cloud-native NFS file system.
- Scale on demand to petabytes
- Designed to provide massively parallel shared access to thousands of Amazon EC2 instances
- **Use Cases**
  - Simplify DevOps

### 1.3 Amazon EBS <a name="aebs"></a>
- Easy to use, high performance block storage at any scale
- **Use Cases**
  - Build your SAN in the cloud for I/O intensive applications.
  - Run relational or NoSQL databases.
  - Right-size your big data analytics engines

### 2.2 Amazon Kinesis <a name="akinesis"></a>
Collect, process, and analyze real-time video and data streams.
- **Kinesis Data Stream**
  - Amazon Kinesis Data Streams is a serverless streaming data service that simplifies the capture, processing, and storage of data streams at any scale.
  - Ingest and store data streams from hundreds of thousands of data sources:
    - Log and event data collection
    - IoT device data capture
    - Mobile data collection
    - Gaming data feed
- **Kinesis Data Firehose**
  - Amazon Kinesis Data Firehose is an extract, transform, and load (ETL) service that reliably captures, transforms, and delivers streaming data to data lakes, data stores, and analytics services.
    - Load real-time data
Load streaming data into data lakes, data stores, and analytics tools for:
    - Log and event analytics
    - IoT data analytics
    - Clickstream analytics
Security monitoring

- **Kinesis Vide Stream**
  - With Amazon Kinesis Video Streams, you can more easily and securely stream video from connected devices to AWS for analytics, ML, playback, and other processing.
  
- **Kinesis Data Analytics or Apache Flink**
  - Process and analyze streaming data
  - Get actionable insights from streaming data in real time.
