## Introduction

Using **cloud technology** for business improvements or large-scale transformations can be challenging. A common issue many organizations face, regardless of their cloud provider, is **managing cloud costs**.

For large organizations, shifting from predictable **capital expenditures** (like building and maintaining IT infrastructure) to **agile operating expenditures** using cloud resources requires significant changes in processes and organization. 

**Managing cloud costs** requires constant vigilance and **real-time monitoring**. Since almost anyone can access cloud resources on demand, managing IT infrastructure costs now involves more people across various teams, not just the finance team. You might even find yourself responsible for **IT budgeting**.

Understanding how cloud technology impacts costs will help you maximize the value your organization gets from the cloud. 

In this first section of the course, you'll learn about:
- The **fundamentals of cloud cost management**
- **Cloud financial governance best practices**
- How to control access using the **resource hierarchy**
- Methods to control **cloud consumption** 

These concepts are key to effectively managing cloud costs in your organization!

## Fundamentals of cloud and financial governance

Easy access to **cloud resources** creates a need for precise, **real-time control** over consumption. Having **cloud financial governance**, which includes processes and controls for managing cloud spending, can be crucial to avoid budget overruns and maintain peace of mind.

As organizations evolve, a core team from technology, finance, and business functions must collaborate to keep cloud costs in check and make timely decisions. The variable nature of cloud costs affects **people, processes, and technology**.

### People
In smaller organizations, one person may handle multiple roles related to cloud infrastructure and finance, including budgeting and tracking optimization. In larger organizations, the **finance team** typically focuses on financial planning and may struggle to monitor daily or monthly cloud spending. Team members from technology and business lines can provide insights on cloud resource usage but often don’t consider costs in their decisions. Therefore, effective cloud cost management requires a partnership across finance, technology, and business functions, possibly through a **cloud center of excellence**. This centralized team ensures best practices are followed and can make real-time decisions when spending exceeds plans.

### Process
Organizations should regularly monitor and analyze their cloud usage and costs. The finance team should review these results weekly or monthly, charge costs back to the appropriate teams, and decide on any necessary changes to optimize spending. Cultivating a culture of **accountability** helps identify waste quickly and maximizes cloud investment, encouraging collaboration across teams to align spending with business objectives.

### Technology
Google Cloud offers built-in tools to help organizations monitor and manage costs effectively. These tools provide visibility, promote accountability for cloud spending, control costs to mitigate overspending risks, and offer intelligent recommendations for optimizing usage. You’ll learn more about these tools later in this section.

## Cloud financial governance best practices

**cloud financial governance best practices** that organizations can adopt to improve predictability and control over their cloud resources:

### 1. Identify Who Manages Cloud Costs
- Establish a **mixed team** of IT managers and financial controllers.
- Create a **culture of accountability** for costs by defining clear ownership for projects and sharing cost views with all relevant departments. This encourages responsible spending and ensures that teams are accountable for their expenses.
- Use **Google Cloud financial governance policies** to control spending and visibility across the organization.

### 2. Understand Invoices vs. Cost Management Tools
- An **invoice** is a request for payment from the cloud provider, while **cost management tools** help track, analyze, and optimize cloud spending.
- Organizations need to know **not just how much they spent, but why**. Cost management tools, like those in the Google Cloud console, provide insights into spending patterns and can uncover trends.

### 3. Use Google Cloud’s Cost Management Tools
- Google Cloud offers strong financial governance tools to align strategic priorities with cloud usage.
- Start by **capturing** details about cloud resource usage, who is using them, and the associated costs.
- Assign responsibilities for monitoring this information and establish a communication plan with stakeholders to ensure that cost management is prioritized.

### Monitoring and Reporting
- Regularly **review cost reports**, ideally on a weekly basis, to monitor trends and identify potential waste.
- Utilize tools like the **Google Cloud Pricing Calculator** to estimate how changes in usage will affect costs. 

### Implementation
- After learning these best practices, it’s essential to **implement** them. If these practices are outside your responsibility, ensure that the relevant stakeholders are informed.

By following these steps, organizations can effectively manage and optimize their cloud spending.

## Using the resource hierarchy to control access

Controlling access to cloud resources is crucial in cloud computing. Unlike on-premises infrastructure, where physical access controls were sufficient, managing access in the cloud requires a different approach. 

### Google Cloud Resource Hierarchy
- **Structure**: Google Cloud organizes resources into a **tree-like structure** known as the resource hierarchy, which consists of four levels:
  1. **Resources**: These include virtual machines, Cloud Storage buckets, etc.
  2. **Projects**: Collections of resources.
  3. **Folders**: Organize projects and other folders.
  4. **Organization Node**: The top-level node that encompasses all projects, folders, and resources in an organization.

### Policies and Access Control
- **Policies**: Define who can access resources and what actions they can perform. These can be set at the project, folder, or organization levels.
- **Granular Control**: Assign roles and permissions at various levels for more precise access management.

### Benefits of Resource Hierarchy
1. **Granular Access Control**: Roles can be assigned at different levels, allowing tailored permissions.
2. **Inheritance of Permissions**: Permissions set at higher levels are automatically inherited by lower levels, simplifying management.
3. **Enhanced Security**: By applying the principle of least privilege, access is limited to only what is necessary, reducing the risk of unauthorized access.
4. **Visibility and Auditing**: Track permissions and changes across levels for better accountability and security monitoring.

Understanding and utilizing the Google Cloud resource hierarchy is essential for effective access management and security compliance.

## Controlling cloud consumption

Organizations aim to control cloud consumption for various reasons, including:

- **Cost Savings**: Preventing overspending on unnecessary resources.
- **Increased Visibility**: Understanding resource usage to identify cost reduction areas.
- **Improved Compliance**: Ensuring the cloud environment meets industry regulations.

### Google Cloud Tools for Controlling Consumption
1. **Resource Quota Policies**: 
   - Set limits on resource usage for projects or users.
   - Help prevent overspending and keep usage within budget.

2. **Budget Threshold Rules**: 
   - Allow you to set alerts when cloud costs exceed a certain amount.
   - Serve as early warnings for potential cost overruns, enabling corrective actions.

3. **Cloud Billing Reports**: 
   - Offer a reactive approach to track and understand past spending on Google Cloud resources.
   - Enable detailed cost analysis by exporting billing data to BigQuery and visualizing it with tools like Looker Studio.

### Cost Optimization
- After analyzing cloud spending, organizations can optimize costs through **Committed Use Discounts (CUDs)**. If resource needs are predictable, purchasing a commitment can yield discounted prices in exchange for a minimum resource usage commitment over a specified term.