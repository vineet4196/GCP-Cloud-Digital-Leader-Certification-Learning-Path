## Introduction

Organizations often struggle to make informed business decisions from their collected data due to various blockers that hinder analysis for parts or all of their workforce. However, with Google Cloud, this challenge can be addressed. In the final module of this course, you'll learn about:

- How **Looker** facilitates easy access to necessary data for the workforce.
- The benefits of **streaming analytics** for real-time data utilization.
- Two Google Cloud products, **Pub/Sub** and **Dataflow**, that help modernize data pipelines.

## Business intelligence and insight using looker

Extracting insights from data in a database often requires significant effort and expertise, which can be streamlined using a business intelligence (BI) solution. However, organizations face challenges in finding the right solution. Many options are either too complex for non-technical users or allow limited data analysis, preventing a comprehensive view of the organization’s data.

**Looker**, a Google Cloud BI platform, aims to address these issues by enabling users to analyze, visualize, and share data through interactive dashboards and reports. This empowers teams to explore data independently, ask their own questions, and generate visual insights, fostering a data-driven culture.

Looker integrates with **BigQuery** and over 60 SQL databases, delivering rich, interactive reports without sacrificing performance or security. Its web-based nature facilitates easy integration into existing workflows.

### Example: Diamond Resorts
Diamond Resorts faced challenges with siloed data initiatives, lack of common metrics, and inefficient reporting. By migrating to Looker, they established a unified cloud-based architecture that improved data governance and business agility. They gained real-time insights in under three months, effectively navigating operational changes during COVID-19 and reducing manual reporting time significantly. The transformation allowed them to tackle projects rapidly, showcasing how effective BI solutions can enhance customer service and operational efficiency.

## Streaming analytics

Data traditionally moves in **batches**, meaning large volumes of data are processed at once, often leading to long latency. For instance, payroll and billing systems process data weekly or monthly. While efficient for large datasets, this method doesn’t suit **time-sensitive data**, which can become stale before processing.

**Streaming analytics** addresses this by continuously processing and analyzing data records, allowing real-time insights. This approach is ideal for sources that generate small data sizes continuously, such as equipment sensors, clickstreams, social media feeds, and app activity.

### Key Use Cases for Streaming Analytics:
- **Ecommerce**: Analyze user clickstreams for real-time pricing and inventory management.
- **Financial Services**: Monitor account activity to detect abnormal behaviors and generate security alerts.
- **Investment Services**: Track market changes to adjust customer portfolios based on set constraints.
- **News Media**: Stream user click data to personalize content with demographic information.
- **Utilities**: Monitor power grid throughput to trigger alerts or workflows when thresholds are met.

**Google Cloud** offers two main products for streaming analytics:
1. **Pub/Sub**: Ingests hundreds of millions of events per second.
2. **Dataflow**: Unifies streaming and batch data analysis, creating cohesive data pipelines.

A **data pipeline** involves a series of actions to ingest raw data from various sources and move it to a destination for storage and analysis. 

In the next section, you'll explore these products in more detail.

## Pub/Sub and Dataflow

One of the early stages in a **data pipeline** is **data ingestion**, where large amounts of streaming data are received. This data often streams from multiple sources rather than a single, structured database. For example, **IoT applications** like sensors in taxis send location data every 30 seconds, or temperature sensors in data centers optimize heating and cooling.

**Pub/Sub** is a distributed messaging service that captures messages from various device streams, such as gaming events and IoT devices. The term "Pub/Sub" refers to the publisher/subscriber model where messages are published to subscribers.

Once messages are captured, you need to pipe that data into a **data warehouse** for analysis. This is where **Dataflow** comes in, creating a pipeline to process both streaming and batch data. The term "process" refers to **ETL** (Extract, Transform, Load) steps.

A popular solution for designing these pipelines is **Apache Beam**, an open-source unified programming model for data processing.

### Key Features of Dataflow:
- **Infrastructure Complexity**: Dataflow simplifies infrastructure setup and maintenance, leveraging Google’s infrastructure.
- **Auto Scaling**: Provides reliable auto-scaling to meet pipeline demands.
- **Serverless and Fully Managed**: Developers can build applications without managing back-end infrastructure, as Google Cloud handles tasks like resource provisioning and performance tuning.
- **Automation Tools**: Enables creation of environments that allow for deployment, monitoring, and management without an operations team.

Using a **serverless** and **fully managed** solution like Dataflow allows teams to focus more on analyzing insights from datasets rather than on resource provisioning for successful pipeline execution.