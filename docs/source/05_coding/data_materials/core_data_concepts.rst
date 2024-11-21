Core Data Concepts
===================================

1. **Data Warehouse:**

A large, centralized repository of integrated data collected from various sources. It's optimized for query and analysis, supporting business intelligence activities.
A **Data Warehouse** is a centralized repository for **structured data** gathered from various sources within an organization. Built for efficient querying, reporting, and analytics, it supports generating insights and business intelligence.

**Examples**:  

- Amazon Redshift  
- Google BigQuery  
- Snowflake  

2. **Data Mark:**

A subset of a data warehouse, focused on a specific business line or team. It's tailored to meet the specific data needs of that group, improving query performance and relevance.
A **Data Mart** is a smaller, **department-focused version** of a data warehouse. It serves targeted user groups by providing relevant data, reducing complexity, and improving access speed. Commonly used for business areas like sales, finance, or marketing.

**Examples**:  

- Amazon Redshift Spectrum  
- IBM Db2 Data Mart  

3. **Data Lake:**

A vast pool of raw, unstructured data kept in its native format until needed. It offers flexibility and scalability for storing big data, crucial for advanced analytics and machine learning tasks.

4. **Delta Lake**

**Delta Lake** enhances data lakes by adding **ACID transactions, schema enforcement, and performance optimization**. It ensures data accuracy and reliability, making it suitable for analytics and machine learning workloads.

**Examples**:  
- Delta Lake on Apache Spark  

5. **Data Pipeline:**

The series of processes involved in moving data from one system to another, including extracting, transforming, and loading data. It's critical for ensuring data flows smoothly and consistently across an organization.
A **Data Pipeline** consists of processes and tools for **ingesting, transforming, and moving data** between systems. It ensures seamless integration of data from raw sources to analytics platforms.

**Examples**:  
- Apache Airflow  
- AWS Data Pipeline  
- Google Dataflow  

6. **Data Mesh**

**Data Mesh** is a **decentralized approach** to data management where domain teams are responsible for their specific data products. It promotes faster access and ownership, enabling scalability and collaboration in large organizations.

**Examples**:  
- Databricks  
- Starburst  

7. **Data Quality:**

Defined as the degree to which data meets a company's expectations of accuracy, validity, completeness, and consistency. It's essential for maintaining the integrity of analytics and decision-making processes.

8. **Data Mining:**

The process of searching and analyzing large batches of raw data to identify patterns and extract useful information. It's key to uncovering insights that drive business value.

9. **Data Fabric**

A **Data Fabric** is a unified architecture that connects disparate data sources, integration, and management tools into a single layer. It ensures **consistent data governance** and provides seamless access across distributed environments for faster insights.