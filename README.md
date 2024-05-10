---------------------------------------------
**Repository summary**

1.  **Intro** 🧳



2.  **Tech Stack** 🤖


3.  **Features** 🤳🏽


4.  **Process** 👣


5.  **Learning** 💡



6.  **Improvement** 🔩



7.  **Running the Project** ⚙️


8.  **More** 🙌🏽



---------------------------------------------

# 🖥️ Data Terms ☁️

 Everything about Data manipulatons terms

# Data Storage

## Spreadsheet

A spreadsheet is a digital document that organizes data into rows and columns, forming cells where data can be stored and manipulated. It is primarily used in contexts where data needs to be structured visually for better analysis, manipulation, and reporting. Spreadsheets are versatile and can handle a variety of information types, including numerical data, text, and formulas. They are commonly used for financial calculations, data analysis, record keeping, and resource planning.

The most widely used spreadsheet software includes Microsoft Excel, Google Sheets, and Apple Numbers. These tools offer functionalities like formula-based calculations, pivot tables, graphing tools, and macros for automating repetitive tasks.

Despite their versatility, spreadsheets have several limitations:

**Scalability**:  They can become slow and cumbersome as the volume of data grows, making them unsuitable for handling very large datasets or real-time data processing.

**Error-Prone**:  Manual data entry and formula setup can lead to errors that are hard to trace and correct.

**Collaboration Issues**: While modern cloud-based solutions like Google Sheets allow for better collaboration, traditional spreadsheets can be difficult to manage and synchronize across multiple users.

**Security**: Basic spreadsheets provide limited security options for sensitive data, lacking advanced access controls and audit trails.

**Data Integrity**: Without strict controls, data in spreadsheets can be easily altered, leading to issues with data consistency and reliability.

## DataFrame

A DataFrame is a two-dimensional, size-mutable, potentially heterogeneous tabular data structure with labeled axes (rows and columns). It is widely used in data manipulation, data analysis, and data cleaning processes, particularly in the context of programming and data science environments.

DataFrames are used to store and manipulate structured data, where each column can have a type, such as integer, float, or string. They are ideal for handling complex operations involving large datasets, such as grouping data, merging multiple data sources, and pivot operations, which are cumbersome in traditional spreadsheets.

The most commonly used DataFrame implementations are found in:

**Pandas (Python)**: Offers extensive capabilities for data manipulation and analysis.

**Apache Spark DataFrame (Scala, Python, Java)**: Designed for big data processing and analysis on distributed systems.

**R DataFrame (R)**: Utilized primarily within the statistical computing community.

**DataFrames.jl (Julia)**: Provides high-performance data manipulation capabilities.


Despite their power and flexibility, DataFrames have several limitations:

**Memory Usage**: In single-machine implementations like Pandas, a DataFrame can consume substantial memory, which can limit its ability to handle very large datasets efficiently.

**Complexity**: The functionality of DataFrames can be complex to understand and use effectively, particularly in terms of their methods and the best practices for optimizing performance.

**Mutable State**: DataFrames are mutable, meaning that they can be changed after creation. This can lead to unintended side effects if not carefully managed.

**Performance Issues**: While highly optimized, operations on large DataFrames can still be slow, especially if not properly vectorized or if operating over a network in distributed systems like Spark.

**Type Safety**: Some DataFrame implementations, particularly in dynamically typed languages, might suffer from type safety issues, leading to runtime errors that are difficult to debug.

## Database

A database is an organized collection of structured information or data, typically stored electronically in a computer system. It is used across various contexts such as business operations, online applications, data analytics, and anywhere that requires storage, retrieval, management, and manipulation of data.

Databases are designed to handle various types of information, ranging from simple data like names and addresses to more complex data like transaction processing systems or interactive websites.

There are several types of databases, including:

**Relational databases (RDBMS)**: Store data in tables and rows, with structured query language (SQL) used for managing and querying data. Examples include MySQL, PostgreSQL, and Oracle.

**NoSQL databases**: Designed for specific data models and have flexible schemas for building modern applications. NoSQL types include key-value, document, columnar, and graph databases. Examples include MongoDB, Cassandra, and Neo4j.

**In-memory databases**: Store data in a computer’s main memory instead of on disk, which allows for faster data retrieval. Examples include Redis and SAP HANA.

**Distributed databases**: Spread data across multiple physical locations, either within the same physical system or spread across networks. Examples include Cassandra and Amazon DynamoDB.

**Object-oriented databases**: Store data in the form of objects, as used in object-oriented programming. Examples include db4o and Objectivity.

Despite the versatility and power of databases, they come with several limitations:

**Complexity**: Setting up and maintaining a database can be complex, requiring specialized knowledge, particularly for tuning performance and ensuring security.

**Cost**: Depending on the type of database and scale of deployment, costs can be high for both hardware and software maintenance.

**Scalability**: While many modern databases are built to scale out, traditional databases can be difficult to scale horizontally and might require significant resources to manage large volumes of data effectively.

**Data Integrity**: Maintaining data integrity, especially in distributed databases, can be challenging due to issues like data replication, concurrent data access, and eventual consistency.

**Security Vulnerabilities**: Databases are a prime target for cyber attacks, requiring robust security measures to prevent unauthorized access and data breaches.

## Data Wharehouse


A data warehouse is a centralized repository that stores integrated data from multiple sources. It is specifically structured for query and analysis, providing support for decision making, reporting, and business intelligence. Data warehouses are typically used in enterprise scenarios where organizations need to analyze large volumes of data from various business processes and departments for better strategic insights.

Data warehouses are designed to handle diverse types of information, including sales data, financial data, customer data, and beyond, making them ideal for historical data analysis and generating business insights.

There are several types of data warehouse architectures:

**Single-Tier Architecture**: Designed to minimize the amount of data stored by removing data redundancy. However, it is rarely used due to its limitations in handling complex queries and analytics directly on the operational systems.

**Two-Tier Architecture**: Separates physically available data from the user's view, enhancing performance and allowing users to access data without impacting the operational systems.

**Three-Tier Architecture**: The most common type, which includes the bottom tier (database server), the middle tier (analytics engine), and the top tier (client front-end tools). This structure supports data cleaning, integration, and transformations (ETL), making it robust for handling complex queries.

Despite their advantages, data warehouses have several limitations:

**Complexity**: The design, implementation, and maintenance of a data warehouse can be complex and time-consuming.

**Cost**: Significant initial and ongoing costs for setup, maintenance, and scaling, including hardware and software investments.

**Inflexibility**: Traditional data warehouses can be rigid in terms of schema design, which can make adapting to changes in business requirements challenging.

**Latency**: Due to the ETL process, there can be a delay between data collection and availability for analysis.

**Scalability**: Scaling a data warehouse to handle increased loads involves considerable complexity and expense, particularly with physical server constraints.

## Data Mart

A datamart is a specialized subset of a data warehouse that focuses on a specific business line or department, such as sales, finance, or marketing. It provides a smaller, more targeted view of an organization’s data for specific analytics or reporting purposes. Datamarts are typically used in contexts where businesses require rapid access to specific types of data that are segmented from the larger datasets stored in a data warehouse.

Datamarts are designed to facilitate access to commonly needed data sets, streamlining the process of data retrieval and analysis for specific business functions or user groups. They are suitable for specialized information needs that don't require the breadth of data typically found in a full data warehouse.

There are several types of datamarts based on their method of sourcing data:

**Independent Datamarts**: These are created without a central data warehouse and are developed by extracting data directly from internal or external data sources. They are quick to implement but can create data consistency issues.

**Dependent Datamarts**: These are sourced from an existing data warehouse. This ensures consistency across the organization but requires a significant upfront investment in a data warehouse infrastructure.

**Hybrid Datamarts**: Combine data from existing data warehouses and additional external sources. This type offers flexibility but can be complex to manage due to varying data origins.

Despite their benefits, datamarts have several limitations:

**Data Silos**: Since datamarts often focus on specific departments, they can lead to data silos where integrated analysis across the organization is challenging.

**Maintenance Overhead**: Managing multiple datamarts can become complex and costly, especially when they are independent and need to be synchronized.

**Scalability**: Similar to data warehouses, scaling datamarts to accommodate growing data needs can be difficult and expensive.

**Data Consistency**: In the case of independent datamarts, maintaining data consistency and avoiding redundancy across multiple datamarts can be challenging.

**Limited Scope**: While the focused nature of datamarts is beneficial for departmental use, it can be a limitation when broader insights across the enterprise are needed.

## Data Lake

A data lake is a large-scale storage repository and processing engine that holds a vast amount of raw data in its native format until it is needed. Unlike a traditional data warehouse, which stores data in a structured format, data lakes are designed to store unstructured, semi-structured, and structured data. This flexibility allows data lakes to support a wide variety of analytics including machine learning, real-time analytics, and big data processing.

Data lakes are typically used in contexts where organizations need to capture and store large volumes of diverse data from multiple sources without initially knowing how they will use that data. They are suitable for industries like marketing, social media, healthcare, and financial services, where data can be collected in various forms and later analyzed for different purposes.

There are several approaches or architectures for implementing a data lake:

**Storage-Based Data Lake**: Often built on platforms like Amazon S3, Microsoft Azure Data Lake Storage, or Google Cloud Storage. This type emphasizes the scalability and durability of cloud storage to manage large volumes of diverse data.

**Hadoop-Based Data Lake**: Utilizes the Hadoop ecosystem for storing and processing data. It typically involves HDFS for storage, MapReduce for processing, and other Hadoop components like Hive and Pig.

**Proprietary Software Data Lake**: Solutions provided by vendors that integrate storage, processing, and management into a single platform, such as IBM, Oracle, and SAP.

Despite the benefits, data lakes also have several limitations:

**Complexity**: Managing and deriving value from a data lake can be complex due to the variety of data formats and the need for advanced data processing techniques.

**Data Quality and Governance**: Without proper governance, data lakes can become data swamps. Poor quality data or unmanaged data can lead to unreliable analytics results.

**Security**: Ensuring data security in a data lake is challenging due to the sheer volume of data and its diverse nature.

**Skill Requirements**: Utilizing data lakes effectively requires a high level of expertise in data engineering and data science, making it resource-intensive.

**Integration**: Integrating data from various sources into a data lake in a usable form can be challenging and time-consuming.

## Delta Lake

Delta Lake is an open-source storage layer that brings reliability to data lakes. Delta Lake provides ACID (Atomicity, Consistency, Isolation, Durability) transaction properties to big data workloads, enhancing the capabilities of a data lake to support robust data handling and analytics. It is built on top of existing data lake technologies and is fully compatible with Apache Spark.

Delta Lake is typically used in contexts where data quality, reliability, and strong governance are required but still need the scalability and cost-effectiveness of a data lake. It is ideal for scenarios involving big data processing, streaming data analytics, machine learning, and real-time data ingestion.

The primary type of Delta Lake is implemented as a storage layer that sits above a traditional data lake, utilizing Parquet files as its base storage format. It manages metadata for each dataset in a transaction log that records details about every change made to the data.

While Delta Lake offers several significant advantages, it also has some limitations:

**Performance Overhead**: The transaction log mechanism can introduce some performance overhead, especially in scenarios with high-frequency updates or access patterns that are not well-optimized.

**Complexity in Setup and Management**: Setting up and managing a Delta Lake architecture, especially at scale, requires a good understanding of both the underlying data lake technology and the Delta Lake layer.

**Dependency on Apache Spark**: While Delta Lake is highly optimized for use with Apache Spark, this can be a limitation for organizations that do not use Spark as part of their data architecture.

**Limited to Certain Ecosystems**: Since Delta Lake is primarily designed to enhance data lakes that use Parquet files, its use is somewhat restricted to environments that are compatible with this format and with Spark.

**Data Consistency**: While it enhances data consistency compared to basic data lakes, the eventual consistency model in highly distributed environments can still pose challenges for some real-time applications.

## Data Mesh



# Data Proces

## Data Ingestion

## ETL

## ELT

## Reverse ETL

## Staging area

## Data Migration



##  Load

## Data pipeline

## Data Wrangling

## Data Testing Frameworks

# Data Engineering Terms

## Data Modeling

## Schema 

## Big Data

## Data Architecture

## Data Governance

## Data Automation

## Data Orchestration

## Data Quality

## Data Model Deployment

## Schema Evolution

## Data Versioning


## Data Partitioning

## Change Data Capture

## Data Serialization

## Batch Processing

## Data Streaming

## Resource Managment

# Data Era

##

##

##



