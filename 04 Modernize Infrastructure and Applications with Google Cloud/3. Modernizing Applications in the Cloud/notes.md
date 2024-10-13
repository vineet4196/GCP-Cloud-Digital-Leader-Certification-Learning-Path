## Introduction

In this section, the focus shifts to **application modernization** following the exploration of IT infrastructure benefits in the cloud. 

An **application** is essentially a software program that assists users in performing various tasks. In today’s digital landscape, applications are ubiquitous, with users expecting intuitive and efficient experiences—from checking emails to tracking fitness via mobile apps.

Historically, applications have been developed on-premises, which often leads to inefficiencies. The on-premises approach can slow down organizations, requiring significant time and specialized IT teams for deployment, and changes can take six months or longer, causing friction within teams.

**Cloud technology** enables businesses to modernize, develop, and manage applications in more agile ways, allowing for quicker responses to user needs. In this section of the course, learners will:

- Compare traditional vs. modern cloud application development methods.
- Explore considerations and tools for **rehosting legacy applications** in the cloud.
- Define **application programming interfaces (APIs)** and their importance.
- Examine the benefits of managing APIs with **Apigee API management**.
- Consider scenarios where a **hybrid or multi-cloud strategy** may be advantageous.

**Main Points:**
- **Application modernization** enhances agility and responsiveness to user needs.
- Traditional on-premises development is often slow and cumbersome.
- Cloud technology allows for faster, more efficient application management.
- Key topics include legacy application rehosting, APIs, Apigee management, and multi-cloud strategies.

## The benefits of the modern cloud and application development

Advancements in **cloud technology** have significantly transformed software application development. Modern cloud development is characterized by flexibility, scalability, and the use of advanced cloud computing technologies.

In contrast to the traditional **monolithic approach**, where applications are developed as a single, tightly coupled unit, modern applications are typically built using **microservices**. These are independently deployable components that can be developed and released quickly, allowing organizations to bring features to market faster.

**Key Benefits of Modern Cloud Application Development:**

1. **Architecture**: Modern applications utilize microservices, enabling faster feature releases without waiting for the entire application to be completed.

2. **Deployment**: Applications are usually deployed in the cloud using **managed** or **partially managed services**. Managed services handle infrastructure management tasks, allowing teams to focus on new development.

3. **Cost**: The **pay-as-you-go** pricing model makes cloud applications cost-effective, as organizations only pay for the resources they utilize.

4. **Development Tools**: Developers can leverage prebuilt **APIs** and tools from cloud providers, accelerating the building and deployment process.

5. **Scalability**: Cloud applications can be easily scaled up or down based on user demand, ensuring high availability and resilience.

6. **Reliability Features**: Built-in capabilities like **load balancing** and **automatic failover** enhance application reliability. Cloud providers also offer robust monitoring tools to quickly identify and address issues.

**Main Points:**
- Modern cloud development emphasizes **microservices** for agility and faster deployment.
- Managed services free up resources for development.
- Cost-effectiveness through a pay-as-you-go model.
- Scalability and reliability are enhanced through built-in features and monitoring tools.

## Rehosting legacy application in the cloud

When businesses decide to modernize by moving operations to the cloud, they often encounter specialized legacy applications that may not be compatible with cloud-native applications. In such cases, a common migration approach is **rehosting** (or "lift and shift"), where applications are moved to the cloud without any modifications.

**Benefits of Rehosting:**
- Access to cloud computing advantages such as **cost savings**, **scalability**, **reliability**, and **security**.

**Potential Drawbacks:**
1. **Complexity**: The migration process can be complicated, requiring careful planning and appropriate resources.
2. **Risk**: Migrating applications introduces inherent risks, necessitating thorough risk assessment and contingency planning.
3. **Vendor Lock-in**: Moving to the cloud may lead to dependence on a specific cloud provider, making future transitions more difficult.

**Solutions Offered by Google Cloud:**
1. **Google Cloud VMware Engine**: This solution allows organizations to migrate existing VMware workloads to the cloud without needing to rearchitect applications, maintaining existing environments while benefiting from Google Cloud's scalability and security. It also provides access to services like BigQuery and Google Kubernetes Engine for further modernization.
   
2. **Bare Metal Solution**: For organizations with Oracle legacy applications, this fully managed infrastructure allows running Oracle workloads on dedicated bare metal servers in the cloud.

**Main Points:**
- **Rehosting** enables cloud benefits but comes with complexity, risk, and potential vendor lock-in.
- Google Cloud provides tailored solutions like VMware Engine and Bare Metal Solution to facilitate the migration of legacy applications while maintaining operational integrity.

## Application Programming Interfaces (APIs)

Implementing software services can be complex, and if each service requires unique coding, it can lead to fragility and errors. A solution to simplify this process is the use of **APIs (Application Programming Interfaces)**. 

**Key Points:**

- **Function of APIs**: APIs enable different software programs to communicate in a standardized and efficient manner. They act as intermediaries, much like a waiter in a restaurant, facilitating requests and responses between programs.

- **Benefits of APIs**:
  - **Efficiency**: Developers can leverage APIs to access functionalities and data from other applications without writing extensive code, saving time and effort.
  - **Google APIs**: Google offers numerous APIs for its products and services, allowing access to features like search, mapping, and translation.

- **Business Opportunities through APIs**:
  - **New Products and Services**: Organizations can create APIs to allow developers to access their data, leading to the development of new offerings.
  - **Revenue Generation**: Charging for API access can create new revenue streams to offset development costs.
  - **Partnerships**: Exposing APIs can foster collaborations with other companies or developers, opening up new business opportunities.

By strategically developing APIs that meet customer and partner needs, organizations can enhance their services and drive growth.

## Apigee API management

Once an organization has implemented APIs, effective maintenance and management are crucial. This can be achieved using **Apigee API management**, Google Cloud's service designed for API operation with enhanced security and automation.

**Key Benefits of Apigee:**

- **Security**: Offers features like authentication, authorization, and data encryption to secure APIs.
- **Analytics**: Provides real-time analytics and historical reporting to track and analyze API usage.
- **Development Tools**: Includes a visual API editor and a test sandbox for easy API development and deployment.
- **API Management Features**: Supports API versioning, documentation, and throttling to control request limits.

**Case Study - AccuWeather**:
AccuWeather successfully shares its weather data through APIs with global partners but aimed to engage individual developers. To do this, they needed a sophisticated API management platform that could:
- Offer different tiers of API products with customized rate limits and pricing.
- Enable quick sign-ups and learning opportunities for developers through a customizable developer portal.

With Apigee, AccuWeather can tailor API consumption to developers' needs while attracting and monitoring traffic effectively through built-in analytics.

## Hybrid and multi-cloud

Organizations can thrive in the cloud, but most enterprise computing still occurs on-premises due to compliance and operational concerns. To modernize IT infrastructure without a full migration, organizations can explore **hybrid** and **multi-cloud** solutions.

**Key Concepts:**

- **Hybrid Cloud**: This combines on-premises or private cloud infrastructure with public cloud services. Many organizations operate in this environment, where some data and applications are in the cloud while others remain on-premises, facilitated by interconnects for interoperability.

- **Multi-Cloud**: Involves using multiple public cloud providers, offering flexibility and secure connectivity between different networks. Organizations may choose this to leverage specific strengths of various cloud providers while keeping parts of their infrastructure on-premises.

**Benefits of Hybrid and Multi-Cloud Solutions**:
- Move specific workloads to the cloud without needing a full-scale migration.
- Enjoy the flexibility, scalability, and cost savings of cloud services for certain tasks.
- Incorporate specialized services like machine learning, data analysis, and IoT.

**Google Cloud's Solution**: 
**GKE Enterprise** is designed for managing Kubernetes applications across hybrid and multi-cloud environments. 

**Key Benefits of GKE Enterprise**:
- **Multi-Cloud and Hybrid Support**: Can run Kubernetes clusters on Google Cloud, AWS, Azure, and more.
- **Centralized Management**: Offers a single console for managing clusters and applications.
- **Security and Compliance**: Includes features to secure clusters and comply with industry regulations.
- **Networking and Load Balancing**: Facilitates efficient networking for applications.
- **Monitoring and Logging**: Provides tools for maintaining application consistency across various environments.