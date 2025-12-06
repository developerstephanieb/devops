# AWS Certified Cloud Practitioner (CLF-C02): Technologies and Concepts

---
 
[Application Programming Interfaces (API)](#application-programming-interfaces-api)   
[Benefits of Migrating to the AWS Cloud](#benefits-of-migrating-to-the-aws-cloud)  
[AWS Cloud Adoption Framework (AWS CAF)](#aws-cloud-adoption-framework-aws-caf)  
[AWS Compliance](#aws-compliance)   
[Compute](#compute)   !!!   
[Cost Management](#cost-management)   
[Databases](#databases)   !!!   
[Amazon EC2 Instance Types](#amazon-ec2-instance-types)    
[AWS Global Infrastructure](#aws-global-infrastructure)   
[Infrastructure as Code (IaC)](#infrastructure-as-code-iac)    
[AWS Knowledge Center](#aws-knowledge-center)   
[Machine Learning](#machine-learning)    !!!   
[Management and Governance](#management-and-governance)   !!!   
[Migration and data transfer](#migration-and-data-transfer)   !!!   
[Network services](#network-services)   !!!   
[AWS Partner Network](#aws-partner-network)   
[AWS Prescriptive Guidance](#aws-prescriptive-guidance)   
[AWS Pricing Calculator](#aws-pricing-calculator)   
[AWS Professional Services](#aws-professional-services)   
[AWS re:Post](#aws-repost)   
[AWS SDKs](#aws-sdks)   
[Security](#security)   !!!   
[AWS Security Blog](#aws-security-blog)   
[AWS Security Center](#aws-security-center)   
[AWS shared responsibility model](#aws-shared-responsibility-model)   
[AWS Solutions Architects](#aws-solutions-architects)   
[Storage](#storage)    !!!      
[AWS Support Center](#aws-support-center)   
[AWS Support plans](#aws-support-plans)   
[AWS Well-Architected Framework](#aws-well-architected-framework)   

---

## Application Programming Interfaces (API)

**Application Programming Interfaces (API)** serve as the primary mechanism through which users and applications interact with the AWS platform. Every action performed on AWS, whether clicking a button in a web browser or running a script, results in an API call to an AWS service endpoint. 

- **Three Methods of Access**: AWS APIs can be accessed via three primary interfaces:
  - **AWS Management Console**: A browser-based Graphical User Interface (GUI) suitable for manual resource provisioning, monitoring, and visual management.
  - **AWS Command Line Interface (CLI)**: A unified tool that enables control of AWS services from a command line shell, allowing for the automation of repetitive tasks through scripts.
  - **AWS Software Development Kits (SDKs)**: Libraries that allow interaction with AWS services directly from application code (e.g., Python, Java, Node.js), handling details like connection management and authentication.
- **Statelessness**: AWS APIs are generally stateless, meaning each request must contain all the necessary information (authentication credentials, action, parameters) to be processed, without relying on previous requests.
- **Public vs Private Connectivity**: APIs can be public (accessible over the internet) or private (only accessible within the Virtual Private Cloud).

---

## Benefits of Migrating to the AWS Cloud

The **Six Advantages of Cloud Computing** describe the fundamental shifts in economic and operational models when moving from on-premises infrastructure to the cloud.

- **Trade capital expense for variable expense**: Organizations can avoid heavy upfront investment in physical data centers (CapEx) in favor of paying only for computing resources consumed (OpEx).
- **Benefit from massive economies of scale**: Due to the aggregate usage from hundreds of thousands of customers, AWS achieves lower variable costs than an individual organization could achieve alone. These savings are passed on to the customer in the form of lower pay-as-you-go prices.
- **Stop guessing capacity**: Cloud computing eliminates the need to predict infrastructure requirements in advance. Resources scale up or down automatically to match demand, preventing expensive idle resources or capacity shortages.
- **Increase speed and agility**: IT resources can be launched in minutes rather than weeks. This drastically reduces the time and cost required to experiment and develop new applications.
- **Stop spending money running and maintaining data centers**: Focus shifts to developing applications and differentiating business value rather than the heavy lifting of racking, stacking, and powering servers.
- **Go global in minutes**: Applications can be deployed in multiple AWS Regions around the world with just a few clicks, providing lower latency and a better experience for customers regardless of their location.

---

## AWS Cloud Adoption Framework (AWS CAF)

The **AWS Cloud Adoption Framework (AWS CAF)** provides a comprehensive set of guidelines to help organizations structure and execute their digital transformation strategies. It organizes guidance into six areas of focus, known as **Perspectives**, which are separated into Business Capabilities and Technical Capabilities.

- **Business Perspective**: Focuses on ensuring that cloud adoption aligns with business goals and measurable outcomes. It addresses strategy, product management, and business insights.
- **People Perspective**: Focuses on organizational change management, culture, and training. It addresses workforce transformation and preparing teams for cloud operations.
- **Governance Perspective**: Focuses on orchestrating cloud initiatives to maximize organizational benefits while minimizing risks. It addresses portfolio management and program management.
- **Platform Perspective**: Focuses on the architectural design and modernization of infrastructure and applications. It addresses the delivery of scalable and resilient cloud solutions.
- **Security Perspective**: Focuses on achieving confidentiality, integrity, and availability of data and workloads. It addresses compliance, risk management, and identity management.
- **Operations Perspective**: Focuses on the health, availability, and performance of IT services. It addresses the monitoring, management, and automation of cloud environments.

---

### AWS Compliance 

**AWS Compliance** refers to the set of controls, tools, and certifications that enable organizations to adhere to legal, regulatory, and industry standards while running workloads on AWS.

- **AWS Artifact**: The central, self-service portal for on-demand access to AWS compliance reports and agreements. It is the primary resource for retrieving audit artifacts to demonstrate AWS security controls to auditors or regulators.
- **Artifact Reports vs. Agreements**: AWS Artifact is divided into two sections: **Reports** (access to third-party audit reports like SOC, PCI DSS, and ISO certifications) and **Agreements** (review and sign legal documents such as the Business Associate Addendum (BAA) for HIPAA).
- **Shared Responsibility for Compliance**: Compliance is a shared responsibility. AWS ensures the compliance of the underlying infrastructure (e.g., physical security of data centers), while the customer is responsible for the compliance of the data and applications they place on that infrastructure.
- **Inheritance of Controls**: Customers inherit the compliance controls maintained by AWS. For example, a customer automatically inherits AWS’s physical security controls but must still configure their own access controls and encryption to meet their specific regulatory requirements.
- **Key Compliance Programs**: AWS maintains compliance with numerous global standards. Common examples referenced include **SOC** (System and Organization Controls) for financial reporting and security, **PCI DSS** (Payment Card Industry Data Security Standard) for handling credit card data, **HIPAA** (Health Insurance Portability and Accountability Act) for healthcare data, and **FedRAMP** for US government data.

---

### Compute

**Compute** in the cloud refers to the on-demand delivery of IT resources (primarily Central Processing Unit or CPU power and memory) over the internet with pay-as-you-go pricing. It replaces the need to purchase, house, and maintain physical servers.

- **Compute Capacity**: The amount of computational power required to run an application. In the cloud, this capacity is elastic, meaning it can be scaled up or down instantly to match the workload demand.
- **Virtualization**: The fundamental technology powering cloud compute. It allows a single physical server to be partitioned into multiple virtual machines (VMs), each acting as an independent server with its own operating system (OS) and resources.
- **Three Primary Compute Models**:
  - **Virtual Machines (Infrastructure as a Service - IaaS)**: Provides the highest level of flexibility and control. The user manages the guest operating system and the software stack (e.g., Amazon EC2).
  - **Container Services**: A method of operating system virtualization that allows for running applications in isolated processes called containers. Containers package code and its dependencies together, ensuring consistency across different environments (e.g., Amazon ECS, Amazon EKS).
  - **Serverless Computing (Function as a Service - FaaS)**: Removes the operational overhead of managing servers entirely. The cloud provider automatically provisions and scales the infrastructure required to run the code. Users pay only for the compute time consumed (e.g., AWS Lambda).
- **Scalability**: The ability to increase or decrease compute resources. **Vertical Scaling** (scaling up) involves increasing the power of a single instance (e.g., adding more RAM), while **Horizontal Scaling** (scaling out) involves adding more instances to a system to handle increased load.

---

### Cost Management

**Cost Management** encompasses the tools and strategies used to budget, forecast, and optimize spending on AWS. It requires shifting from a fixed-expense mindset (Data Centers) to a variable-expense mindset (Cloud).

- **Fundamentals of AWS Pricing**: While pricing models vary by service, there are three fundamental drivers of cost on AWS:
  - **Compute**: Charged per hour or per second (e.g., EC2 instances, Lambda execution time).
  - **Storage**: Charged by the amount of data stored (e.g., GBs in S3 or EBS).
  - **Data Transfer**: Generally, Data In is free, while Data Out (transferring data out of AWS to the internet) is charged.
- **Total Cost of Ownership (TCO)**: A financial estimate intended to help determine the direct and indirect costs of a product or system. In the context of AWS, it helps compare the cost of running an entire infrastructure environment on-premises (including power, cooling, real estate, and IT labor) versus running it in the AWS Cloud.
- **Consolidated Billing**: A feature of AWS Organizations that enables the combination of bills from multiple AWS accounts into a single payment method. This provides a unified view of costs and facilitates volume discounts by aggregating usage across all accounts.
- **Cost Allocation Tags**: Metadata (key-value pairs) assigned to AWS resources to categorize and track costs. Tagging resources allows for the filtering and reporting of costs specifically for distinct projects, departments, or cost centers.
- **Savings Plans vs. Reserved Instances**: Two major discount models used to manage costs. 
  - **Reserved Instances (RIs)**: Offer significant discounts for committing to a specific instance configuration for 1 or 3 years. 
  - **Savings Plans**: Offer similar discounts but are more flexible, requiring only a commitment to a specific amount of spend regardless of the instance type or region used.

---

### Databases

**Databases** in the cloud provide organized storage for data, allowing for efficient retrieval, management, and updates. AWS offers a broad range of database options, categorized primarily by their data model and management level.

- **Managed vs. Unmanaged**:
  - **Unmanaged (Self-Managed)**: Involves provisioning an EC2 instance and installing a database engine (like MySQL or Oracle) manually. This provides full control over the configuration but requires the user to handle all patching, backups, and scaling.
  - **Managed Services**: Services like Amazon RDS or Amazon DynamoDB where AWS handles the "heavy lifting" of database administration, including hardware provisioning, setup, patching, and backups. This allows focus to remain on application development.
- **Relational Databases (SQL)**: These databases store data in a structured format using rows and tables with a fixed schema. They rely on Structured Query Language (SQL) and are ideal for complex transaction processing (e.g., ERP systems, financial records). They typically scale vertically (adding more power to a single instance).
- **Non-Relational Databases (NoSQL)**: These databases use flexible schemas (such as key-value pairs, documents, or graphs) rather than rigid tables. They are optimized for high-performance, massive scale, and rapid iteration. They typically scale horizontally (adding more servers to the cluster).
- **High Availability (Multi-AZ)**: A deployment configuration (common in Amazon RDS) where a primary database instance is automatically replicated to a standby instance in a different Availability Zone. If the primary fails, AWS automatically fails over to the standby, minimizing downtime.
- **Read Scalability (Read Replicas)**: A feature that allows for the creation of read-only copies of a database. Applications can route read traffic to these replicas to reduce the load on the primary database, thereby improving overall performance for read-heavy workloads.
- **In-Memory Databases**: specialized databases (like Amazon ElastiCache) that store data in primary memory (RAM) rather than on disk. This results in microsecond latency, making them ideal for caching frequently accessed data to speed up applications.

---

### Amazon EC2 Instance Types

**Amazon EC2 Instance Types** determine the hardware configuration of the host computer used for the instance. Each type offers different compute, memory, and storage capabilities, which are grouped into families (such as **General Purpose**, **Compute Optimized**, and **Memory Optimized**) to fit different use cases. **EC2 Purchasing Options** (also known as Pricing Models) allow for the optimization of costs based on the consistency and flexibility of the workload.

- **On-Demand Instances**: The default pay-as-you-go model. Payment is made for compute capacity by the second or hour with no long-term commitment or upfront payments. This is ideal for short-term, irregular workloads or applications being developed and tested for the first time.
- **Savings Plans**: A flexible pricing model that offers low prices (up to 72% savings) in exchange for a commitment to a consistent amount of usage (measured in $/hour) for a 1 or 3-year term. This model applies to usage across Amazon EC2, AWS Lambda, and AWS Fargate.
- **Reserved Instances (RI)**: Provides a significant discount (up to 72%) compared to On-Demand pricing in exchange for a 1 or 3-year term commitment. 
  - **Standard RIs** offer the highest discount but are less flexible; the instance type and operating system are fixed. 
  - **Convertible RIs** offer a lower discount than Standard RIs but allow the exchange of the instance for another with different attributes (e.g., different instance family) during the term.
- **Spot Instances**: Allow the use of spare Amazon EC2 computing capacity for up to 90% off the On-Demand price. However, AWS can reclaim the instance with only a 2-minute warning if the capacity is needed elsewhere. This is suitable for fault-tolerant, stateless workloads like batch processing or data analysis.
- **Dedicated Hosts**: A physical server fully dedicated to a single customer's use. This option is typically required to meet strict regulatory compliance or to use existing server-bound software licenses (BYOL - Bring Your Own License) that are billed per socket or per core.
- **Dedicated Instances**: Instances that run in a Virtual Private Cloud (VPC) on hardware that's dedicated to a single customer. Unlike Dedicated Hosts, these do not offer visibility into the underlying sockets or physical cores of the host hardware.

---

### AWS Global Infrastructure

**AWS Global Infrastructure** refers to the physical hardware and network arrangement that spans the globe. It is designed and built to deliver a flexible, reliable, scalable, and secure cloud computing environment with high quality global network performance.

- **Regions**: A Region is a physical location in the world where AWS clusters data centers. Each Region is entirely independent and isolated from other Regions to ensure fault tolerance and stability.

- **Availability Zones (AZs)**: Each Region consists of three or more Availability Zones. An AZ is a discrete location within a Region that is engineered to be isolated from failures in other AZs. They provide inexpensive, low-latency network connectivity to other AZs in the same Region.

- **Data Centers**: The fundamental building block of the infrastructure. A single Availability Zone consists of one or more discrete data centers, each with redundant power, networking, and connectivity, housed in separate facilities.

- **Edge Locations**: Specialized data centers used by **Amazon CloudFront** (CDN) to cache content closer to end-users. These locations are more numerous than Regions and help reduce latency by delivering content from the location geographically nearest to the user.

- **Regional Data Sovereignty**: A critical concept for compliance. Data stored in a specific Region never leaves that Region unless explicitly moved or replicated. This ensures organizations can meet local data residency laws and regulations.

- **Factors for Selecting a Region**: When deploying resources, the choice of Region is determined by four main factors:

  1. **Data Governance**: Adherence to local laws regarding where data must reside.

  2. **Proximity**: Reducing latency by choosing a Region close to the target user base.

  3. **Cost**: Pricing for AWS services varies by Region based on local operational costs (e.g., electricity, taxes).

  4. **Service Availability**: Not all AWS services are available in every Region immediately upon launch.

---

### Infrastructure as Code (IaC)

**Infrastructure as Code (IaC)** is the practice of provisioning and managing IT infrastructure using configuration files and code rather than through manual configuration in the AWS Management Console. This approach treats infrastructure with the same rigor as application code.

- **AWS CloudFormation**: The primary AWS service for Infrastructure as Code. It allows for the modeling of an entire infrastructure in a text file. CloudFormation reads the file and automatically provisions and configures the resources described within it.

- **Templates**: The "blueprint" files used by CloudFormation, written in either JSON or YAML format. These templates describe the desired resources (e.g., an EC2 instance, an S3 bucket) and their dependencies.

- **Stacks**: When CloudFormation executes a template, it creates a **Stack**. A Stack is a collection of AWS resources that are managed as a single unit. If a stack is deleted, all resources defined within that stack are automatically deleted, ensuring clean removal of infrastructure.

- **Repeatability and Consistency**: IaC eliminates the manual errors and inconsistencies associated with human configuration. The same template can be used to deploy identical environments (e.g., Development, Staging, Production) in multiple Regions with guaranteed consistency.

- **Version Control**: Because infrastructure is defined as code, templates can be stored in version control systems (like Git). This allows for tracking changes over time, peer reviews of infrastructure changes, and the ability to roll back to previous versions if issues arise.

- **AWS Cloud Development Kit (AWS CDK)**: An open-source software development framework that allows for the definition of cloud application resources using familiar programming languages (such as Python, Java, or TypeScript) instead of JSON or YAML. The CDK compiles this code into CloudFormation templates.

---

### AWS Knowledge Center

**The AWS Knowledge Center** is a searchable database of support articles and videos covering the most frequent questions and requests received by AWS Support.

- **Authoritative Source**: Content is created and updated by the same AWS Support engineers and architects who handle customer cases daily, ensuring the solutions are practical, technically accurate, and up-to-date.

- **Problem Solving**: It serves as a primary resource for troubleshooting without needing to contact support. It contains specific solutions to common technical issues, detailed explanations of error messages, and "how-to" guides for configuring services.

- **Public Accessibility**: The Knowledge Center is publicly available on the internet. Access does not require an AWS account or a paid support plan.

- **Integration with Case Creation**: When a user attempts to create a support case within the AWS Management Console, the system automatically suggests relevant Knowledge Center articles based on the service and issue selected. This often allows for issue resolution before a case is formally submitted.

---

### Machine Learning

### Management and Governance

### Migration and data transfer

- AWS DataSync: An online data transfer service that automates moving data between on-premises storage and AWS storage services (like S3 or EFS). It uses a proprietary protocol to transfer data up to 10 times faster than open-source tools.

### Network services
### AWS Partner Network
### AWS Prescriptive Guidance
### AWS Pricing Calculator
### AWS Professional Services
### AWS re:Post
### AWS SDKs
### Security
### AWS Security Blog
### AWS Security Center
### AWS shared responsibility model
### AWS Solutions Architects
### Storage
### AWS Support Center
### AWS Support plans
### AWS Well-Architected Framework

---

