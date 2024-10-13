## Introduction

In the context of the Cloud, "compute" refers to a machine's ability to process information, which includes tasks like storing, retrieving, comparing, and analyzing data. Unlike local servers and storage devices, Cloud computing utilizes a network of remote servers to provide on-demand access to various resources such as applications, storage, and processing power. This approach has gained popularity due to its flexibility, scalability, and cost-effectiveness.

In this course section, you will learn about the benefits of Cloud computing for organizations and explore three key options: **virtual machines, containers, and serverless**.

## The benefits of running compute workloads in the cloud


Organizations should consider running compute workloads in the Cloud for several key benefits:

1. **Total Cost of Ownership (TCO)**: Cloud computing reduces IT costs by eliminating the need for physical infrastructure. Organizations pay only for the resources they use, and long-term commitments can lead to further savings.

2. **Scalability**: Cloud services allow organizations to easily scale resources up or down based on demand, avoiding large upfront investments. This flexibility helps manage sudden spikes or drops in demand efficiently.

3. **Reliability**: Cloud providers ensure high uptime and reliability through multiple data centers and monitoring technologies. This means businesses can trust that their data and applications will be available when needed.

4. **Security**: Cloud providers offer robust security features, including data encryption, identity management, and network security, ensuring data safety and compliance with regulations.

5. **Flexibility**: Organizations can choose and adapt Cloud services as needed, such as easily increasing storage capacity without hassle.

6. **Abstraction**: Cloud providers manage the infrastructure details, allowing organizations to focus on their core business without worrying about hardware or software management.

7. **Faster Time to Market**: Utilizing Cloud services helps organizations deliver products and services more quickly, while also providing access to the latest technologies for innovation.

**Main Points:**
- **TCO**: Reduces IT costs, pay-as-you-go model.
- **Scalability**: Easily adjust resources to meet demand.
- **Reliability**: High uptime and multiple data centers.
- **Security**: Robust features for data safety and compliance.
- **Flexibility**: Adapt services as needed.
- **Abstraction**: Simplifies management of infrastructure.
- **Faster Time to Market**: Accelerates delivery and innovation.

## Virtual Machines

Traditionally, organizations faced technological pressures that tied specific computing hardware to specific applications. **Virtualization technology** has alleviated these pressures by allowing multiple systems, known as **virtual machines (VMs)**, to run on the same hardware. This optimizes resource use, enabling organizations to efficiently run multiple applications on a single server.

**Compute Engine** is Google Cloud's Infrastructure as a Service (IaaS) that allows users to create and run virtual machines on Google’s infrastructure without upfront investments. Users can configure VMs similarly to physical servers, specifying CPU power, memory, storage, and operating systems.

VMs can be created via the **Google Cloud console**, **Google Cloud CLI**, or infrastructure automation tools like **Terraform** and the **Compute Engine API**. Compute Engine charges by the second, with discounts for sustained use and committed use for 1 or 3 years. 

**Preemptible and Spot VMs** offer cost-saving options, potentially reducing costs by up to 90% for workloads that do not require continuous monitoring. However, these VMs can be interrupted by Compute Engine to reclaim capacity, so they are suitable for jobs that can be paused and restarted. Spot VMs have more features and do not have a maximum runtime, but their pricing is currently the same as Preemptible VMs.

Finally, Compute Engine allows users to select machine properties like virtual CPUs, operating systems, and memory through predefined or custom machine types.

**Main Points:**
- **Virtualization**: Allows multiple VMs to run on the same hardware, optimizing resources.
- **Compute Engine**: Google Cloud’s IaaS for creating and running VMs without upfront costs.
- **Billing**: Charged by the second with discounts for sustained and committed use.
- **Cost Savings**: Preemptible and Spot VMs can significantly reduce costs for non-urgent workloads.
- **Configuration**: Users can customize VM properties or use predefined machine types.

## Containers

**Infrastructure as a Service (IaaS)** allows users to share compute resources via virtual machines, enabling developers to deploy their own operating systems and build applications in self-contained environments. 

**Containers** operate on a similar principle by providing isolated environments for running software services, but they are even more efficient. The key difference is that while virtual machines virtualize the entire hardware, containers virtualize only the software layers above the operating system. This leads to faster startup times and significantly lower memory usage.

Each container is packaged with an application and its dependencies, allowing for independent development, testing, and deployment. Containers are particularly suitable for a **microservices architecture**, which consists of smaller services that communicate through APIs or lightweight methods like REST or gRPC.

Containers enable developers to create predictable environments that are isolated from other system resources, allowing for easy updates to specific application parts without affecting the entire system. Their flexibility means containers can run virtually anywhere, simplifying development and deployment processes.

**Main Points:**
- **IaaS**: Enables sharing of compute resources through virtual machines.
- **Containers**: More efficient than VMs; they virtualize software layers, not hardware.
- **Efficiency**: Containers start faster and use less memory.
- **Microservices Architecture**: Supports independent services that communicate via APIs.
- **Ease of Updates**: Containers allow easy changes to specific application parts without system-wide impact.
- **Portability**: Containers can run virtually anywhere, facilitating development and deployment.

## Managing container

**Containers** enhance agility, security, resource optimization, and application management in the cloud. Many organizations use a mix of virtual machines and containers, but as infrastructure becomes more complex, managing numerous containers requires significant oversight.

**Kubernetes**, developed by Google, is an open-source platform designed to manage containerized workloads efficiently. It simplifies orchestrating containers across multiple hosts, scaling them, and deploying updates, thereby improving application reliability and reducing management overhead.

**Google Kubernetes Engine (GKE)** is a managed Kubernetes service that allows users to create customizable clusters of compute engine instances. GKE facilitates quick application deployment and scaling, offering features for monitoring and troubleshooting.

An example is **Ubie**, a Japanese healthcare startup, which reduced infrastructure costs and maintenance by adopting GKE. They utilized GKE Autopilot to manage their cluster infrastructure and benefit from per-pod billing, cutting costs by 20% and eliminating time-consuming maintenance tasks.

Another option for containerized applications on Google Cloud is **Cloud Run**, a fully managed serverless platform that automatically handles infrastructure scaling. It is ideal for stateless applications that need to respond quickly to traffic changes.

**Main Points:**
- **Containers** improve agility, security, and resource management.
- **Kubernetes** helps manage complex containerized workloads efficiently.
- **GKE** allows quick deployment and scaling of applications, reducing operational costs.
- **Ubie's** use of GKE Autopilot resulted in a 20% reduction in infrastructure costs and streamlined maintenance.
- **Cloud Run** is a serverless platform suited for lightweight, stateless applications that require rapid scaling.
- **GKE** is best for complex applications needing control, while **Cloud Run** is ideal for simpler, managed applications.

## Serverless computing

**Serverless computing** modernizes cloud applications by automatically provisioning computing resources as needed, meaning organizations only pay for compute power when actively running queries or applications. Essentially, businesses provide the code for specific functions, while the cloud provider manages the infrastructure.

In serverless computing, **Function as a Service (FaaS)** is a key component where developers write code that responds to specific events, like file uploads or database changes. Google Cloud offers several serverless products, including:

- **Cloud Run:** A managed environment for running containerized applications without infrastructure concerns.
- **Cloud Functions:** A platform for hosting single-purpose functions triggered by events.
- **App Engine:** A service for building and deploying web applications.

**Benefits of serverless computing include:**
- **Reduced operational costs:** The cloud provider manages infrastructure, eliminating the need for significant investment from application owners.
- **Scalability:** Automatic scaling based on demand ensures users only pay for what they use.
- **Faster time to market:** No infrastructure setup allows quicker deployment of applications and features.
- **Reduced development costs:** Developers can focus on application logic without managing infrastructure.
- **Improved resilience:** The cloud provider manages failover and disaster recovery.
- **Pay-per-use pricing model:** Costs are optimized as users only pay for the resources consumed.

An example of a successful application of cloud infrastructure is **Mashme.io**, which provides video collaboration for over 3 million users. Facing challenges like maintaining low latency and minimizing costs, Mashme.io utilized Google Kubernetes Engine (GKE) to leverage Google Cloud's global network. This approach allowed for continuous updates without disrupting user experience, ensuring no downtime for students worldwide.

**Main Points:**
- **Serverless computing** automates resource management, with organizations paying only for active compute use.
- Key services include **Cloud Run**, **Cloud Functions**, and **App Engine**.
- Benefits: reduced costs, scalability, faster deployment, and improved resilience.
- **Mashme.io** exemplifies successful serverless adoption, leveraging GKE for efficient video collaboration with global reach.