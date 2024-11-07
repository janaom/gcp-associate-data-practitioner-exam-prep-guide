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

All notes and pictures are from "Introduction to Data Engineering on Google Cloud" course, here is the [link](https://www.cloudskillsboost.google/paths/1336/course_templates/1157).

------------------------

# The Role of the Data Engineer

In the most basic sense, a data engineer moves data from data sources to data syncs in four stages: replicate and migrate, ingest, transform, and store.

![image](https://github.com/user-attachments/assets/99b5a102-27e7-40d5-b34b-76191b0a3b47)

# Data sources vs Data sinks

Two examples of Google Cloud products used in the ingest phase are Cloud storage, a data lake holding various types of data sources, and Pub/Sub, an asynchronous messaging system delivering data from external systems.

![image](https://github.com/user-attachments/assets/0d9dd3fc-1ed8-4121-98b8-b1c96a934ddb)

The transform stage of a data pipeline represents action taken on a data source to adjust, modify, join, or customize a data source so that it matches a specific downstream data or reporting requirement. There are three main transformation patterns: extract and load, extract, load, and transform, and extract, transform, and load.

![image](https://github.com/user-attachments/assets/f7da1d75-d8f0-4afe-bad0-78ff984a8f76)

The store stage of a data pipeline represents the last step when we deposit data in its final form. A data sync is the final stop in the data journey. It's where processed and transformed data is stored for future use, analysis, and decision-making. Two examples of Google Cloud products used in the store phase are BigQuery, a serverless data warehouse, and Bigtable, a highly scalable no SQL database.

![image](https://github.com/user-attachments/assets/dd9f9ec0-abaa-430f-8953-5dac647faf05)

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

![image](https://github.com/user-attachments/assets/93c62c10-d952-4ec2-aa1c-bcfb9fa35c54)

BigQuery is a fully managed, serverless enterprise data warehouse for analytics. BigQuery has built-in features like machine learning, geospatial analysis, and business intelligence. BigQuery can scan terabytes in seconds and petabytes in minutes. BigQuery is a great solution for online analytical processing, or OLAP, workloads for big data exploration and processing. BigQuery is also well-suited for reporting with business intelligence tools.

BigQuery organizes data tables into units called datasets. When you reference a table from the command line in SQL queries or code, you refer to it by using the construct, project.dataset.table. Access control is through IAM and is at the dataset, table, view, or column level.

# Metadata management options on GCP

![image](https://github.com/user-attachments/assets/b771561a-a74b-4164-870b-39fe1c48b48d)

Dataplex is a comprehensive data management solution that allows you to centrally discover, manage, monitor, and govern distributed data across your organization. With Dataplex, you can break down data silos, centralize security and governance, while enabling distributed ownership, and easily search and discover data based on business contexts. Dataplex also offers built-in data intelligence, support for open-source tools, and a robust partner ecosystem, helping you to trust your data and accelerate time to insights.

![image](https://github.com/user-attachments/assets/56ee826c-e266-40ff-a4d3-c6500f0ed649)

Dataplex lets you standardize and unify metadata, security policies, governance, classification, and data life cycle management across this distributed data.
Another common use case is when your data is accessible only to data engineers, and is later refined and made available to data scientists and analysts.
In this case, you can set up a lake to have the following: A raw zone for the data, which is accessed by data engineers and data scientists.
A curated zone for the data, which is accessed by all users.

# Sharing Datasets using Analytics Hub

![image](https://github.com/user-attachments/assets/79cc5235-92bd-49e6-955d-a5c7d697e233)

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


