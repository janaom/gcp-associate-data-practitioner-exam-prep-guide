# Associate Data Practitioner
(Beta Exam Voucher info)

The Associate Data Practitioner certification validates fundamental skills to secure and manage data on Google Cloud. It bridges the gap between getting started on Google Cloud and the Professional level data certifications.

The beta exam is open to the public with no prerequisites, though 3-6 months of experience managing and using data is recommended. You can review the exam guide [here](https://services.google.com/fh/files/misc/associate_data_practitioner_exam_guide_english.pdf).

First day to sit beta exam: November 6, 2024

Last day to request a voucher: November 22, 2024

Last day to sit beta exam: December 1, 2024

Results expected: December 2024 - January 2025

Only individuals registering with an email associated with a Google Cloud Partner are eligible to receive a voucher. 

Not a Google Cloud Partner? Visit the [Google Cloud Certification site](https://cloud.google.com/learn/certification/data-practitioner)

Please request the exam voucher with a valid partner email domain.

------------

More info about the exam here: https://cloud.google.com/learn/certification/data-practitioner

Associate Data Practitioner Learning Path here: https://www.cloudskillsboost.google/paths/1336

Exam guide here: https://services.google.com/fh/files/misc/associate_data_practitioner_exam_guide_english.pdf

-----------------

❗ **All notes and screenshots are from "Introduction to Data Engineering on Google Cloud" course, here is the [link](https://www.cloudskillsboost.google/paths/1336/course_templates/1157).**

------------------------

# The Role of the Data Engineer

In the most basic sense, a data engineer moves data from data sources to data syncs in four stages: replicate and migrate, ingest, transform, and store.

![image](https://github.com/user-attachments/assets/99b5a102-27e7-40d5-b34b-76191b0a3b47)

# Data sources vs Data sinks

Two examples of Google Cloud products used in the ingest phase are Cloud storage, a data lake holding various types of data sources, and Pub/Sub, an asynchronous messaging system delivering data from external systems.

The transform stage of a data pipeline represents action taken on a data source to adjust, modify, join, or customize a data source so that it matches a specific downstream data or reporting requirement. There are three main transformation patterns: extract and load, extract, load, and transform, and extract, transform, and load.

The store stage of a data pipeline represents the last step when we deposit data in its final form. A data sync is the final stop in the data journey. It's where processed and transformed data is stored for future use, analysis, and decision-making. Two examples of Google Cloud products used in the store phase are BigQuery, a serverless data warehouse, and Bigtable, a highly scalable no SQL database.


# Data formats

Data exists in two primary formats, unstructured and structured. Unstructured data is information stored in a non-tabular form, such as documents, images, and audio files. Unstructured data is usually suited for Cloud Storage, but BigQuery also offers the capability to store unstructured data via object tables. There is also structured data, which represents information stored in tables, rows, and columns.

![image](https://github.com/user-attachments/assets/461f0013-9bae-4606-999a-7252f7dd56af)

# Storage solution options on GCP

![image](https://github.com/user-attachments/assets/92709f9f-776e-4e79-b4e4-807fcc3ad805)

Within Cloud Storage, objects are accessed by using HTTP requests, including ranged GETS to retrieve portions of the data. The only key is the object name. There is object metadata, but the object itself is treated as unstructured bytes. Objects can be up to five terabytes each. Cloud Storage is built for availability, durability, scalability, and consistency. It's an ideal solution for hosting static websites and storing images, videos, objects, and blobs, and any unstructured data.
Cloud Storage has four primary storage classes; standard storage, nearline storage, coldline storage, and archive storage.

You have a full range of cost effective storage services for structured data to choose from when developing with Google Cloud. No one size fits all, and your choice of storage and database solutions will depend on your application and workload. 

![image](https://github.com/user-attachments/assets/c0a3b32c-7986-492e-aa37-993d7ef332cd)

- Cloud SQL is Google Cloud's managed relational database service.
- AlloyDB is a fully managed, high- performance PostgreSQL database service from Google Cloud.
- Spanner is Google Cloud's fully managed relational database service that offers both strong consistency and horizontal scalability.
- Firestore is a fast, fully managed, serverless, NoSQL document database built for automatic scaling, high performance, and ease of application development.
- BigQuery is a fully managed, serverless enterprise data warehouse for analytics.
- Bigtable is a high-performance NoSQL database service. Bigtable is built for fast key-value lookup and supports consistent sub-10 millisecond latency.

![image](https://github.com/user-attachments/assets/418d420b-346b-4bbf-8ccd-731aa389a927)

The two key concepts in data engineering are that of the data lake and the data warehouse. 

- A data lake is a vast repository for storing raw unprocessed data in various formats, including unstructured, semi-structured, and structured. It serves as a centralized storage solution for diverse data types, enabling flexible use cases like data science, applications, and business decision making.

- A data warehouse is a structured repository designed for storing pre-processed and aggregated data from multiple sources. Primarily used for long term business analysis, it enables efficient querying and reporting for informed decision making. Data warehouses often operate as standalone systems, independent of other data storage solutions. 


BigQuery is a fully managed, serverless enterprise data warehouse for analytics. BigQuery has built-in features like machine learning, geospatial analysis, and business intelligence. BigQuery can scan terabytes in seconds and petabytes in minutes. BigQuery is a great solution for online analytical processing, or OLAP, workloads for big data exploration and processing. BigQuery is also well-suited for reporting with business intelligence tools.

BigQuery organizes data tables into units called datasets. When you reference a table from the command line in SQL queries or code, you refer to it by using the construct, project.dataset.table. Access control is through IAM and is at the dataset, table, view, or column level.

# Metadata management options on GCP

Dataplex is a comprehensive data management solution that allows you to centrally discover, manage, monitor, and govern distributed data across your organization. With Dataplex, you can break down data silos, centralize security and governance, while enabling distributed ownership, and easily search and discover data based on business contexts. Dataplex also offers built-in data intelligence, support for open-source tools, and a robust partner ecosystem, helping you to trust your data and accelerate time to insights.

Dataplex lets you standardize and unify metadata, security policies, governance, classification, and data life cycle management across this distributed data.
Another common use case is when your data is accessible only to data engineers, and is later refined and made available to data scientists and analysts.
In this case, you can set up a lake to have the following: A raw zone for the data, which is accessed by data engineers and data scientists.
A curated zone for the data, which is accessed by all users.

# Sharing Datasets using Analytics Hub

You need to consider security and permissions, destination options for data pipelines, data freshness and accuracy, and finally, usage monitoring. Analytics Hub was created to meet these data sharing challenges. Analytics Hub helps organizations unlock the value of data sharing, leading to new insights and business value. With Analytics Hub, you create a rich data ecosystem by publishing and subscribing to analytics-ready datasets. Because data is shared in place, data providers are able to control and monitor how their data is being used.  Analytics Hub provides a self-service way to access valuable and trusted data assets, including data provided by Google. Finally, Analytics Hub provides an opportunity to monetize data assets.

# Quiz

1. **What is the key difference between a data lake and a data warehouse?**
    * Data lakes are used for real-time analytics, while data warehouses are used for long-term storage.
    * Data lakes store only structured data, while data warehouses store unstructured data.
    * + **Data lakes store raw, unprocessed data, while data warehouses store processed and organized data.**
    * Data lakes are managed by data scientists, while data warehouses are managed by data engineers.

2. **What is the purpose of Analytics Hub in Google Cloud?**
    * To automate the process of data cleaning and transformation.
    * + **To enable secure and controlled data sharing within and outside an organization.**
    * To provide a centralized platform for data visualization.
    * To perform complex machine learning tasks on large datasets.

3. **What is the primary function of a data engineer?**
    * Conducting statistical analysis on data.
    * + **Building and maintaining data pipelines.**
    * Designing user interfaces for data visualization.
    * Managing network security for data systems.

4. **Which Google Cloud product is best suited for storing unstructured data like images and videos?**
    * Bigtable
    * Cloud SQL
    * BigQuery
    * + **Cloud Storage**

5. **Which stage in a data pipeline involves modifying and preparing data for specific downstream requirements?**
    * Replicate and migrate
    * Ingest
    * Store
    * + **Transform**


# Replication and migration


Start replicating and migrating data by using tools like the  'gcloud storage' command, Transfer Appliance, Storage Transfer Service,  or Datastream.

Data can originate from on-premises or multi-cloud environments,  including file systems, object stores, HDFS, and relational databases.

Google Cloud provides additional workload migration with options for various database types. Leverage Database Migration Service for seamless transitions from Oracle, MySQL, PostgreSQL, and SQL Server.
For other data formats or complex migrations, use ETL tools like  DataFlow with a wide range of templates that handle NoSQL or  non-relational databases.


With one terabyte of data, a 100 gigabits per second network takes about two minutes to transfer, while the same size on a 100 megabits per second network takes 30 hours.
The 'gcloud storage' command or Storage Transfer Service are suitable for smaller datasets.
For larger datasets, consider Transfer Appliance for faster offline transfer.

You can use the 'gcloud storage' command to transfer small to medium-sized datasets to Cloud Storage. The data can originate from various on-premise sources like file systems, object stores, or HDFS. The 'cp' command, shown in the code snippet, facilitates these ad-hoc transfers directly to Cloud Storage.

To move larger datasets, consider using Storage Transfer Service. Storage Transfer Service efficiently moves large datasets from  on-premises, multicloud file systems, object stores (including Amazon S3  and Azure Blob Storage), and HDFS into Cloud Storage. It boasts high transfer speeds (up to tens of gigabits per second)  and supports scheduled transfers for convenient data migration.

Transfer appliance is Google's solution for moving massive datasets offline. Google provides the hardware, you transfer your data onto it, then ship it back. It is ideal for scenarios with limited bandwidth or very large transfers, and it comes in multiple sizes to suit your needs.

# Datastream

Datastream enables continuous replication of your on-premises or  multi-cloud relational databases such as Oracle, MySQL, PostgresSQ,L or  SQL Server into Google Cloud. Datastream offers change data capture options for historical  backfill or allows you to just propagate new changes with data landing  in Cloud Storage or BigqQuery for analytics. You have flexibility in connectivity options and can selectively replicate data at the schema, table, or column level.

Datastream enables real-time data replication from source systems for various use cases.
It supports direct replication into BigQuery for analytics, allows  custom data processing in Dataflow before loading into BigQuery, and  facilitates event-driven architectures.
Additionally, Datastream can be used with Dataflow templates for  seamless database replication and migration tasks, making it a versatile  tool for integrating data into Google Cloud.

Datastream taps into the source database's write-ahead log (WAL) to capture and process changes for propagation downstream.
Datastream supports reading the logging mechanisms for the  specific source database such as LogMiner for Oracle, binary log for  MySQL, PostgreSQL's logical decoding, and transaction logs from SQL  Server. These change events such as inserts, updates, and deletes are then  processed by Datastream and transformed into structured formats like  Avro or JSON, ready for storage in Google Cloud, typically in BigQuery  tables, enabling near real-time data replication for analytics and other  use cases.

Datastream event messages contain two main sections: generic metadata and payload.
Metadata provides context about the data, like source table, timestamps, and related information.
Payload contains the actual data changes in a key-value format, reflecting column names and their corresponding values.

Datastream event messages also include source-specific metadata in addition to generic metadata and payload.
This metadata provides context about the data's origin within the  source system, including details like the database name, schema, table,  change type (such as INSERT), and other system-specific identifiers.
This additional information helps track data lineage and understand the context of changes replicated from the source database.

![image](https://github.com/user-attachments/assets/586f89aa-838a-46b9-b7a2-b0546815c5fe)


In summary, Google Cloud offers several data migration and replication options.
- The 'gcloud storage' command is suitable for smaller online transfers.
- Storage Transfer Service handles larger online transfers efficiently.
- Transfer Appliance is ideal for massive offline data  migrations, 
- and Datastream provides continuous online replication of  structured data, supporting both batch and streaming velocities.

# Quiz

**Which of the following services efficiently moves large datasets from  on-premises, multicloud file systems, object stores, and HDFS into Cloud  Storage and supports scheduled transfers?**
   * Transfer Appliance           
   * Vertex AI           
   * gcloud storage
   * + **Storage Transfer Service**

**Which of the following tools is best suited for migrating very large datasets offline?**           
   * Datastream
   * gcloud storage command
   * Storage Transfer Service
   * + **Transfer Appliance**

**The ease of migrating data is heavily influenced by which two factors?**
   * Data source and destination platform
   * Data complexity and network latency
   * + **Data size and network bandwidth**
   * Data format and storage type

**In Datastream event messages, which section contains the actual data changes in a key-value format?**           
   * Generic metadata
   * Source-specific metadata
   * Change log
   * + **Payload**

**Which tool or service uses the “cp” command to facilitate  ad-hoc transfers directly to Cloud Storage from various on-premise  sources?**           
   * Datastream
   * Transfer Appliance
   * + **gcloud storage command**
   * Storage Transfer Service

# The Extract and Load Data Pipeline Pattern

![image](https://github.com/user-attachments/assets/1ae189fa-bd06-4d30-b375-814aa0825cf0)

In summary, both external and BigLake tables enable querying data  residing outside of BigQuery, but BigLake offers broader capabilities.
BigLake supports a wide range of data formats and storage  locations, including object stores across multiple cloud providers, and  provides advanced security features like column-level and row-level  security.
External tables are simpler to set up, but lack fine-grained security controls.
BigLake tables offer enhanced performance, security, and  flexibility for querying external data, making them suitable for  enterprise data lake use cases.

# Streaming Data processing options

![image](https://github.com/user-attachments/assets/e6b4d571-849e-48dc-a812-0395adb8f206)

- Dataprep is ideal for data wrangling tasks and offers a serverless option.
- Data Fusion excels at data integration, particularly in hybrid and  multicloud environments, utilizing the open-source CDAP framework.
- Dataproc handles ETL workloads with support for Hadoop, Spark, and  other open source tools, with Serverless Spark as a serverless option.
- Lastly, Dataflow, built on Apache Beam, is recommended for both  batch and streaming ETL workloads, and provides a serverless  architecture.

# Automation Techniques

![image](https://github.com/user-attachments/assets/c81601c6-5e59-4396-81f1-b24957696745)

- Cloud Scheduler and Cloud Composer are suitable for scheduled or  manual triggers, while Cloud Run functions and Eventarc are  event-driven.
- Cloud Scheduler offers low coding effort with YAML, and Cloud Composer requires medium effort with Python.
- Cloud Run functions support multiple languages, while Eventarc is language agnostic.
- As a final note, all options except Cloud Composer are serverless.
