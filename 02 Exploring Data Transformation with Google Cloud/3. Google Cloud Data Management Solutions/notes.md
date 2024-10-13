## Introduction

### Summary: Data Management in Organizations

**Data is essential** for an organization's operations, making effective storage and management crucial. 

**Google Cloud** offers various data management products and solutions tailored for different business needs.

In this course section, you will learn about:

- **Google Cloud data management options** and their differences.
- **Different storage classes** available with Cloud Storage.
- **How to choose the right storage product** for your organization’s needs.
- **Ways to migrate or modernize** your current database in the cloud. 

These points will help you understand how to effectively manage data in your organization.

## Unstructured data storage

### Summary: Google Cloud Storage Solutions

**Applications need to store data**, such as media or sensor data, and different workloads require different storage solutions. Google Cloud offers several core storage products, including **Cloud Storage**, **Cloud SQL**, **Spanner**, **BigQuery**, **Firestore**, and **Bigtable**.

**Cloud Storage** provides durable and highly available object storage. 

**Key Features of Object Storage:**
- Manages data as **“objects”** rather than files or blocks.
- Each object contains the **data**, relevant **metadata**, and a **globally unique identifier** (URL).
- Commonly used for unstructured data like videos, images, and audio.

**Uses of Cloud Storage:** 
- if data is unstructured use cloud storage
- Serves website content.
- Stores data for archival and disaster recovery.
- Distributes large data objects via direct download.

### **Storage Classes in Cloud Storage:**
1. **Standard Storage**: Best for frequently accessed, “hot” data.
2. **Nearline Storage**: For infrequently accessed data, accessed about once a month (e.g., backups).
3. **Coldline Storage**: For data accessed about once every 90 days.
4. **Archive Storage**: Lowest-cost option for data accessed less than once a year, with higher access costs.

### **Common Characteristics Across Storage Classes:**
- Unlimited storage with no minimum object size.
- Worldwide accessibility and low latency.
- High durability and uniform security features.
- **Geo-redundancy** for disaster protection and performance.

### **Autoclass Feature:**
- Automatically transitions objects to appropriate storage classes based on access patterns.
- Moves less accessed data to colder storage to reduce costs.

This summary captures the essential aspects of Google Cloud's data storage solutions and their management.

## Structured data storage

### Summary: Google Cloud Storage Solutions for Structured Data

In the previous lesson, we learned about **Cloud Storage** for unstructured data. Now, we will focus on Google Cloud storage products suitable for **structured data**.

**Structured Data**:
- Organized in a predefined format that is easily searchable in relational databases.
- Stored in tables, rows, and columns with a clearly defined schema.

### Key Google Cloud Products for Structured Data:

1. **Cloud SQL**:
   - Fully managed relational databases (MySQL, PostgreSQL, SQL Server).
   - Handles routine tasks like updates, backups, and configurations.
   - Benefits include no software installation, managed backups, data encryption, and a network firewall for security.
   - Greater than **99.95% availability**.

2. **Spanner**:
   - Fully managed, mission-critical relational database service.
   - Scales horizontally for high performance and handles spikes in demand.
   - Offers strong global consistency and built-in high availability to reduce downtime.
   - Supports tens of thousands of reads and writes per second.
   - Up to **99.999% availability** with zero downtime for maintenance.

### Choosing Between Cloud SQL and Spanner:
- **Use Spanner** if you need:
  - High transactional consistency and global data.
  - Horizontal scaling for large workloads.
- **Use Cloud SQL** if you want a cost-effective solution without the need for global availability.

3. **BigQuery**:
   - Fully managed data warehouse designed for large datasets (petabytes).
   - Users focus on SQL queries without managing infrastructure.
   - Provides storage and analytics capabilities.
   - Built-in features for machine learning, geospatial analysis, and business intelligence.
   - Data is encrypted at rest by default.
   - Integrates seamlessly with existing business intelligence and data tools.
   - Supports a multicloud strategy, allowing data analysis across multiple cloud providers.
   - Allows machine learning models to be created directly within BigQuery using SQL.

### Conclusion:
These Google Cloud products offer a range of solutions for managing structured data effectively, catering to different organizational needs while enhancing analytics and operational efficiency.


## Semi-Strutred Data storage

### Summary: Google Cloud Storage Solutions for Semi-Structured Data

**Semi-Structured Data**:
- Contains elements of both structured and unstructured data.
- Has some organizational properties (like tags or metadata) but is not as rigid as relational databases.
- Example: An email message, which includes unstructured content and structured elements like sender/recipient details and timestamps.

### Key Google Cloud Products for Semi-Structured Data:

1. **Firestore**:
   - A flexible, horizontally scalable NoSQL cloud database.
   - Designed for real-time data storage and syncing, accessible by mobile and web applications.
   - Data is stored in documents within collections, supporting various data types (nested objects, numbers, strings).
   - **Automatic Scaling**: Adjusts to user demand without losing performance, regardless of database size.
   - **Offline Usage**: Allows uninterrupted access to data even without internet connectivity.

2. **Bigtable**:
   - Google's NoSQL big data database service that powers core Google applications (e.g., Search, Analytics, Maps, Gmail).
   - Designed for handling large workloads with low latency and high throughput.
   - Ideal for operational and analytical applications, such as IoT, user analytics, and financial data analysis.

### Choosing Between Firestore and Bigtable:
- **Use Bigtable** if:
  - You're dealing with over 1 TB of semi-structured or structured data.
  - You require fast responses and high data throughput.
  - Your data is rapidly changing or time-series oriented.
  - You are processing big data for real-time or batch operations, or running machine learning algorithms. 

These Google Cloud products provide effective solutions for managing semi-structured data, catering to various business needs and workloads.

## Choosing the right storage product

### Summary: Choosing the Right Google Cloud Storage Option

When deciding which Google Cloud storage option to use, consider the **data type** and **business needs**.

1. **Unstructured Data**:
   - Use **Cloud Storage**.
   - Select a storage class: Standard, Nearline, Coldline, Archive, or use the **Autoclass** feature for automatic selection.

2. **Structured or Semi-Structured Data**:
   - Determine if workloads are **transactional** or **analytical**:
     - **Transactional Workloads (OLTP)**: Require fast data inserts and updates (e.g., point-of-sale records).
       - If accessed via SQL: Use **Cloud SQL** (best for local to regional scalability) or **Spanner** (best for global scalability).
       - If accessed without SQL: Use **Firestore**, a NoSQL, document-oriented database.
     
     - **Analytical Workloads (OLAP)**: Involve reading entire datasets and complex queries (e.g., analyzing sales trends).
       - If requiring SQL commands: Use **BigQuery**, ideal for analyzing petabyte-scale datasets.
       - If needing a scalable NoSQL solution: Use **Bigtable**, suitable for real-time, high-throughput applications with millisecond latency.

This guidance helps in selecting the most appropriate Google Cloud storage solution based on data requirements and workload types.

## Data migration and modernization

### Summary: Database Modernization and Migration on Google Cloud

Running modern applications on legacy, on-premises databases presents challenges like **latency, throughput, availability,** and **scaling**. **Database modernization** allows organizations to move data from traditional databases to fully managed cloud databases.

#### Migration Methods:
1. **Lift and Shift**:
   - Move databases from on-premises to similar types hosted by a public cloud (e.g., Google Cloud).
   - Benefits: Minimal disruption, cloud management.
   - Drawback: Makes future modernization more complex.

2. **Managed Database Migration**:
   - Migrate to fully managed databases (e.g., from SQL Server, MySQL, PostgreSQL).
   - Requires planning but allows focusing on higher-value work.
   - Tools: Google Cloud’s **Database Migration Service (DMS)** for migration and **Datastream** for data synchronization.

#### Case Study: Wayfair
- **Challenge**: Move from on-premises SQL Server to Google Cloud without disrupting operations for over 3,000 engineers, tens of millions of customers, and 16,000 suppliers.
- **Solution**: 
  - Chose a lift-and-shift strategy using **Cloud SQL** for SQL Server.
  - Google Cloud offered flexibility in choosing engines and products.
  - Post-migration, utilized **Google Kubernetes Engine (GKE)** and **Compute Engine** for services, along with **Pub/Sub** and **Dataflow** for operational data analysis in **BigQuery**.

This approach highlights the benefits of modernizing databases to enhance operational efficiency and scalability.