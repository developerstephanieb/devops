# AWS Certified Cloud Practitioner (CLF-C02): AWS Services and Features 

---

[Analytics](#analytics)   
[Application Integration](#application-integration)   
[Business Applications](#business-applications)   
[Cloud Financial Management](#cloud-financial-management)   
[Compute](#compute)      
[Containers](#containers)   
[Customer Engagement](#customer-engagement)   
[Database](#database)     
[Developer Tools](#developer-tools)   
[End User Computing](#end-user-computing)   
[Frontend Web and Mobile](#frontend-web-and-mobile)   
[Internet of Things (IoT)](#internet-of-things-iot)   
[Machine Learning](#machine-learning)   
[Management and Governance](#management-and-governance)       
[Migration and Transfer](#migration-and-transfer)       
[Networking and Content Delivery](#networking-and-content-delivery)   
[Security, Identity, and Compliance](#security-identity-and-compliance)     
[Serverless](#serverless)   
[Storage](#storage)   

---

## Analytics

**AWS Analytics** services provide the tools necessary to store, process, analyze, and visualize data of any volume, velocity, or variety. These services enable the derivation of actionable insights from raw data.

- **Amazon Athena**: A serverless, interactive query service that makes it easy to analyze data directly in Amazon S3 using standard SQL. There is no infrastructure to manage, and payment is based only on the queries run.
- **AWS Data Exchange**: A service that makes it easy to find, subscribe to, and use third-party data in the cloud. It is used to integrate data from third-party providers (such as Reuters or Foursquare) directly into AWS workloads.
- **Amazon Elastic MapReduce (EMR)**: A cloud big data platform for processing vast amounts of data using open-source tools such as Apache Hadoop, Apache Spark, and Presto. It is used for running large-scale distributed data processing jobs, machine learning applications, and scientific simulations.
- **AWS Glue**: A serverless data integration service that makes it easy to discover, prepare, and combine data for analytics, machine learning, and application development. It is primarily known as an Extract, Transform, and Load (ETL) service.
- **Amazon Kinesis**: A service designed to collect, process, and analyze real-time, streaming data so insights can be gained in seconds or minutes rather than waiting for data collection to finish. It handles streams of data such as website clickstreams, application logs, and IoT telemetry.
- **Amazon Managed Streaming for Apache Kafka (Amazon MSK)**: A fully managed service that makes it easy to build and run applications that use Apache Kafka to process streaming data. It is suitable for organizations already using open-source Kafka that want to reduce operational overhead.
- **Amazon OpenSearch Service**: A managed service that makes it easy to deploy, operate, and scale OpenSearch clusters. It is commonly used for application monitoring, log analytics, and website search.
- **Amazon QuickSight**: A cloud-native, serverless Business Intelligence (BI) service. It allows for the creation and publication of interactive dashboards that include Machine Learning-powered insights. It is accessible from any device and embedded into applications, portals, and websites.
- **Amazon Redshift**: A fully managed, petabyte-scale data warehouse service in the cloud. It uses SQL to analyze structured and semi-structured data across data warehouses, operational databases, and data lakes. It is optimized for online analytical processing (OLAP).

---

## Application Integration

**AWS Application Integration** services enable communication between decoupled components within microservices, distributed systems, and serverless applications. These services allow components to interoperate without being tightly dependent on one another, improving scalability and fault tolerance.

- **Amazon EventBridge**: A serverless event bus service that connects applications using data from various sources. It delivers a stream of real-time data from event sources (such as custom applications, SaaS applications, or AWS services) to targets (such as AWS Lambda functions), enabling the creation of event-driven architectures.
- **Amazon Simple Notification Service (Amazon SNS)**: A fully managed messaging service for both application-to-application (A2A) and application-to-person (A2P) communication. It follows a **publish/subscribe (pub/sub)** model where messages are pushed immediately to subscribers (fan-out), such as email, SMS, or other distributed services.
- **Amazon Simple Queue Service (Amazon SQS)**: A fully managed message queuing service that enables the decoupling and scaling of microservices. It uses a **poll-based** model where messages are stored in a queue until a consumer retrieves, processes, and deletes them. This ensures that no data is lost if the consuming system is temporarily offline or overwhelmed.
- **AWS Step Functions**: A low-code, visual workflow service used to orchestrate AWS services, automate business processes, and build serverless applications. It allows for the coordination of multiple AWS services into serverless workflows (state machines) so complex processes can be managed with error handling and retry logic.

---

## Business Applications

**AWS Business Applications** offer cloud-based software solutions that solve common business challenges, such as communication and customer service, without the need for managing complex infrastructure.

- **Amazon Connect**: A scalable, easy-to-use omnichannel cloud contact center. It enables organizations to set up a customer contact center in minutes that supports both voice and chat. It includes tools for skill-based routing, call recording, and real-time analytics, all paid for on a usage basis (per minute).
- **Amazon Simple Email Service (Amazon SES)**: A cost-effective, flexible, and scalable email service that enables developers to send mail from within any application. It is designed for high-volume email use cases, including transactional emails (e.g., purchase confirmations), marketing emails, and bulk notifications. It also provides features to filter spam and ensure high deliverability rates.

---

## Cloud Financial Management

**AWS Cloud Financial Management** (formerly AWS Cost Management) services provide the tools necessary to organize, report, control, and optimize costs on AWS. These services enable the alignment of cloud spending with business objectives.

- **AWS Billing Conductor**: A service designed to support showback and chargeback workflows by allowing the customization of billing data. It enables the creation of "pro forma" (hypothetical) bills with custom pricing rates (e.g., adding a markup or flat fee) to share with internal teams or customers, separate from the actual standard AWS bill.
- **AWS Budgets**: A tool that enables the setting of custom budgets to track cost and usage. It allows for the configuration of alerts (sent via email or Amazon SNS) that trigger when actual or forecasted spending exceeds defined thresholds, preventing accidental overspending.
- **AWS Cost and Usage Report (CUR)**: The most comprehensive and granular set of cost and usage data available. It delivers detailed line-item billing data (down to the hour or resource level) to an Amazon S3 bucket. This raw data is typically integrated with analytics tools like Amazon Athena or Amazon QuickSight for deep analysis.
- **AWS Cost Explorer**: A tool for visually analyzing historical costs and usage. It provides a dashboard with graphs and charts to help identify trends, pinpoint cost drivers, and forecast future costs for up to 12 months based on historical data.
- **AWS Marketplace**: A curated digital catalog that makes it easy to find, test, buy, and deploy third-party software, data, and services that run on AWS. It simplifies procurement by allowing third-party charges to be consolidated onto the single AWS bill.

---

## Compute

**AWS Compute** services provide the infrastructure required to run applications, ranging from simple virtual private servers to edge computing solutions for ultra-low latency.

- **AWS Batch**: A fully managed service that facilitates the execution of batch computing workloads at any scale. It dynamically provisions the optimal quantity and type of compute resources (e.g., CPU or memory-optimized instances) based on the volume and resource requirements of the submitted jobs, eliminating the need to install and manage batch computing software.
- **Amazon EC2**: A web service that provides secure, resizable compute capacity in the cloud. It offers granular control over virtual servers (instances) and is the foundational service for running custom applications, allowing for the selection of operating systems, processor types, and storage configurations.
- **AWS Elastic Beanstalk**: A Platform as a Service (PaaS) for deploying and scaling web applications and services. Developers simply upload their code, and Elastic Beanstalk automatically handles the deployment, from capacity provisioning and load balancing to auto-scaling and application health monitoring.
- **Amazon Lightsail**: An easy-to-use virtual private server (VPS) service designed for simple workloads, such as WordPress sites or development environments. It offers a simplified console and predictable, monthly pricing that bundles compute, storage, and networking into a single plan.
- **AWS Local Zones**: An infrastructure deployment that places AWS compute, storage, and database services closer to large population and industry centers. This enables the running of latency-sensitive applications (such as real-time gaming or media creation) for end-users in specific geographic locations, while still connecting seamlessly to the parent AWS Region.
- **AWS Outposts**: A fully managed service that extends AWS infrastructure, services, APIs, and tools to virtually any on-premises data center or co-location space. It allows for a consistent hybrid experience, enabling applications to run on-premises for low latency or data residency requirements while being managed just like cloud resources.
- **AWS Wavelength**: An infrastructure offering optimized for mobile edge computing applications. It embeds AWS compute and storage services within 5G networks (at the edge of telecommunications providers), enabling developers to build applications with single-digit millisecond latency for mobile devices and connected vehicles.

---

## Containers

**AWS Container Services** provide the tools to manage, host, and orchestrate containers, which are lightweight, executable packages of software that include everything needed to run an application (code, runtime, system tools, system libraries, and settings).

- **Amazon Elastic Container Registry (Amazon ECR)**: A fully managed container registry that makes it easy to store, manage, share, and deploy container images and artifacts anywhere. It eliminates the need to operate and scale the infrastructure required to power a private container registry. It is integrated with AWS Identity and Access Management (IAM) for resource-level control of each repository.
- **Amazon Elastic Container Service (Amazon ECS)**: A fully managed container orchestration service that helps easily deploy, manage, and scale containerized applications. It is deeply integrated with the rest of the AWS platform and is the preferred choice for developers who want a powerful, simple way to run containers without the complexity of managing a control plane.
- **Amazon Elastic Kubernetes Service (Amazon EKS)**: A managed service that provides the flexibility to start, run, and scale Kubernetes applications in the AWS Cloud or on-premises. It allows for the use of open-source tools and plugins from the Kubernetes community. It is the preferred choice for organizations already using Kubernetes or those desiring compatibility with the open-source ecosystem.

---

## Customer Engagement

**AWS Customer Engagement** services provide the resources, expert guidance, and support mechanisms necessary to help organizations build, migrate, and operate successfully on the AWS Cloud.

- **AWS Activate for Startups**: A program designed to provide startups with the resources they need to get started on AWS. It offers benefits such as AWS credits (to cover bill costs), technical support, and training. It is typically divided into two tiers: **Founders** (for bootstrapped startups) and **Portfolio** (for startups associated with an accelerator or venture capital firm).
- **AWS IQ**: A service that enables customers to find, engage, and pay AWS Certified third-party experts for on-demand project work. It is used to supplement internal teams with external expertise for tasks such as setting up a database, configuring a VPC, or optimizing costs. Work is agreed upon via proposals, and payment is processed directly through the AWS bill.
- **AWS Managed Services (AMS)**: A service that operates AWS infrastructure on behalf of the customer. It provides a "hands-on-keyboard" operational team that manages the day-to-day running of the environment, including monitoring, patch management, security, and backup. It effectively extends an organization's team with AWS operational capabilities.
- **AWS Support**: A tiered subscription service that provides technical assistance and guidance. It is divided into four main plans:
  - **Basic**: Included for all customers. Offers access to customer service, documentation, and the AWS Personal Health Dashboard.
  - **Developer**: Offers business-hours email access to Cloud Support Associates for general guidance.
  - **Business**: Offers 24/7 phone, chat, and email access to Cloud Support Engineers for specific use-case guidance.
  - **Enterprise**: Offers 24/7 access to Senior Cloud Support Engineers and includes a Technical Account Manager (TAM) for consultative architectural guidance and operational reviews.

---

## Database

**AWS Database Services** offer a range of purpose-built engines optimized for specific data models, ensuring that applications can perform efficiently without the operational burden of managing the underlying hardware and software.

- **Amazon Aurora**: A proprietary, fully managed relational database engine compatible with MySQL and PostgreSQL. It is built for the cloud, providing up to five times the throughput of standard MySQL and three times the throughput of standard PostgreSQL. It features a distributed, fault-tolerant, and self-healing storage system that auto-scales up to 128 TiB per database instance.
- **Amazon DynamoDB**: A serverless, fully managed, Key-Value and Document NoSQL database that delivers single-digit millisecond performance at any scale. It handles the heavy lifting of operating and scaling a distributed database, automatically managing data traffic and storage. It includes **Global Tables** to replicate data across multiple AWS Regions for local access and disaster recovery.
- **Amazon MemoryDB for Redis**: A durable, in-memory database service that delivers ultra-fast performance. Unlike Amazon ElastiCache (which is primarily a cache), MemoryDB uses a Multi-AZ transaction log to ensure data durability, making it suitable as a primary database for applications requiring microsecond read and single-digit millisecond write latencies.
- **Amazon Neptune**: A fully managed graph database service built for applications that work with highly connected datasets, such as social networking feeds, recommendation engines, and fraud detection. It supports popular graph query languages like Apache TinkerPop Gremlin and W3C’s SPARQL.
- **Amazon RDS**: A managed service that makes it easy to set up, operate, and scale a relational database in the cloud. It automates time-consuming administration tasks such as hardware provisioning, database setup, patching, and backups. It supports six database engines: Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle Database, and SQL Server.
- **Amazon ElastiCache**: A fully managed in-memory data store, typically used as a cache to improve application performance. By storing frequently accessed data in memory (using Redis or Memcached), it reduces the load on the primary database and decreases latency for end-users.

---

## Developer Tools

**AWS Developer Tools** provide a set of services to build, test, and deploy applications in the cloud. They are designed to help release software faster and more securely using DevOps practices.

- **AWS AppConfig**: A capability of AWS Systems Manager used to create, manage, and deploy application configurations (like feature flags) to valid targets. It allows for the gradual rollout of changes and automatic rollback if errors occur, preventing application outages.
- **AWS CLI**: A unified tool that provides a consistent interface for interacting with all AWS services using commands in a command-line shell (like Bash or PowerShell). It is often used for scripting and automation.
- **AWS Cloud9**: A cloud-based Integrated Development Environment (IDE) that lets you write, run, and debug code with just a browser. It includes a code editor, debugger, and terminal, and comes prepackaged with essential tools for popular programming languages.
- **AWS CloudShell**: A browser-based, pre-authenticated shell that launches directly from the AWS Management Console. It allows for the running of AWS CLI commands and scripts without needing to install or configure tools on a local machine.
- **AWS CodeArtifact**: A fully managed artifact repository service that makes it easy for organizations to securely store, publish, and share software packages (like npm, pip, or Maven packages) used in their development process.
- **AWS CodeBuild**: A fully managed continuous integration service that compiles source code, runs tests, and produces software packages that are ready to deploy. It eliminates the need to provision, manage, and scale build servers.
- **AWS CodeCommit**: A fully managed source control service that hosts secure, private Git repositories. It is used to store code, binaries, and documents, allowing teams to collaborate on code in a secure and highly scalable ecosystem.
- **AWS CodeDeploy**: A fully managed deployment service that automates software deployments to a variety of compute services such as Amazon EC2, AWS Fargate, AWS Lambda, and on-premises servers. It helps avoid downtime during application deployment.
- **AWS CodePipeline**: A fully managed continuous delivery service that automates the release pipelines for fast and reliable application and infrastructure updates. It orchestrates the steps (build, test, deploy) whenever there is a code change.
- **AWS CodeStar**: A service that provides a unified user interface, enabling the management of software development activities in one place. It allows for the quick setting up of an entire continuous delivery toolchain (CodeCommit, CodeBuild, CodePipeline, etc.) using project templates.
- **AWS X-Ray**: A service that helps developers analyze and debug production, distributed applications, such as those built using a microservices architecture. It provides a visual **Service Map** to view the connections between components and identify performance bottlenecks or errors.

---

## End User Computing

**AWS End User Computing (EUC)** services provide secure, remote access to applications and desktops from any device. These services enable the workforce to work from anywhere while keeping data secure within the AWS network rather than on local devices.

- **Amazon AppStream 2.0**: A fully managed application streaming service. It allows users to access desktop applications (such as CAD, 3D design, or legacy Windows apps) through a web browser on any device. It streams the application rather than a full desktop, and the instance is typically non-persistent (data is not saved on the instance itself after the session ends).
- **Amazon WorkSpaces**: A fully managed, secure Desktop-as-a-Service (DaaS) solution. It provides users with a persistent, full cloud desktop (Windows or Linux) that acts just like a physical computer. Users can install applications, save files, and customize the environment, and the state is preserved between sessions.
- **Amazon WorkSpaces Web**: A low-cost, fully managed workspace built specifically to facilitate secure, web-based access to internal websites and Software-as-a-Service (SaaS) applications. It provides a secure browser environment that protects corporate data by isolating the browsing session from the local device and network.

---

## Frontend Web and Mobile

**AWS Frontend Web and Mobile** services provide a set of tools and services that accelerate the development of mobile and web applications, helping developers build secure, scalable apps and deploy them quickly.

- **AWS Amplify**: A set of tools and services that enables mobile and front-end web developers to build secure, scalable full-stack applications, powered by AWS. It consists of a code library, a CLI, and a hosting service. It simplifies the process of configuring backend services (like authentication, storage, and APIs) and connecting them to the frontend application.
- **AWS AppSync**: A serverless GraphQL and Pub/Sub API service that simplifies building modern web and mobile applications. It allows applications to securely access, manipulate, and combine data from one or more data sources (such as DynamoDB, Lambda, or HTTP APIs) via a single endpoint. It also handles real-time data synchronization and offline data capabilities.
- **AWS Device Farm**: A application testing service that lets developers test and interact with Android, iOS, and web applications on many real, physical devices hosted in the AWS Cloud. It allows for the simultaneous execution of tests across hundreds of devices to identify issues before releasing the app to the public.

---

## Internet of Things (IoT)

**AWS Internet of Things (IoT)** services enable the connection of physical devices to the cloud, allowing them to interact with cloud applications and other devices securely.

- **AWS IoT Core**: A managed cloud service that lets connected devices easily and securely interact with cloud applications and other devices. It supports billions of devices and trillions of messages, processing and routing those messages to AWS endpoints securely. It features the Device Shadow, a JSON document that persists the last known state of a device, allowing applications to read or interact with the device even if it is currently offline.
- **AWS IoT Greengrass**: An open-source edge runtime and cloud service for building, deploying, and managing device software. It extends AWS functionality to edge devices, allowing them to act locally on the data they generate while still using the cloud for management, analytics, and durable storage. It enables devices to run AWS Lambda functions, Docker containers, and machine learning models locally, syncing data with the cloud only when connectivity is available.

---

## Machine Learning

**AWS Machine Learning** services are categorized into three layers: the bottom layer for frameworks and infrastructure, the middle layer for machine learning platform services, and the top layer for AI services that provide ready-made intelligence for applications without requiring ML expertise.

- **Amazon Comprehend**: A natural language processing (NLP) service that uses machine learning to find insights and relationships in text. It can identify the language of the text, extract key phrases, places, people, or brands, and understand sentiment (positive, negative, neutral).
- **Amazon Kendra**: An intelligent enterprise search service powered by machine learning. It allows organizations to index and search unstructured data from multiple sources (such as SharePoint, Amazon S3, and Salesforce) using natural language queries, delivering precise answers rather than just a list of links.
- **Amazon Lex**: A service for building conversational interfaces (chatbots) into applications using voice and text. It powers Amazon Alexa and provides the advanced deep learning functionalities of automatic speech recognition (ASR) and natural language understanding (NLU).
- **Amazon Polly**: A service that turns text into lifelike speech. It allows for the creation of applications that talk, enabling you to build speech-enabled products in multiple languages and voices.
- **Amazon Rekognition**: A service that adds image and video analysis to applications. It can identify objects, people, text, scenes, and activities in images and videos, as well as detect inappropriate content.
- **Amazon SageMaker**: A fully managed service used to build, train, and deploy machine learning models. It removes the heavy lifting from each step of the machine learning process, allowing developers to create high-quality models without managing the underlying infrastructure.
- **Amazon Textract**: A service that automatically extracts text, handwriting, and data from scanned documents. It goes beyond simple optical character recognition (OCR) to identify the contents of fields in forms and information stored in tables.
- **Amazon Transcribe**: A service that converts speech into text (Automatic Speech Recognition). It is commonly used to generate captions for videos or to transcribe customer service calls for analysis.
- **Amazon Translate**: A neural machine translation service that delivers fast, high-quality, and affordable language translation. It allows for the localization of content (such as websites and applications) for international users.

---

## Management and Governance

**AWS Management and Governance** services provide the visibility and control needed to maintain a secure, compliant, and operationally efficient cloud environment.

- **AWS Auto Scaling**: A service that monitors applications and automatically adjusts capacity to maintain steady, predictable performance at the lowest possible cost. It enables the configuration of scaling for multiple resources across multiple services (such as Amazon EC2 instances, Amazon ECS tasks, Amazon DynamoDB tables, and Amazon Aurora replicas) in minutes.
- **AWS CloudFormation**: A service that provides a common language for describing and provisioning all the infrastructure resources in a cloud environment. It allows for the modeling of infrastructure using a simple text file (JSON or YAML), enabling the automated and secure deployment of resources (Infrastructure as Code).
- **AWS CloudTrail**: A service that enables governance, compliance, and operational and risk auditing. It records user activity and API usage across AWS services as "events," providing a comprehensive history of actions taken (who did what, where, and when).
- **Amazon CloudWatch**: A monitoring and observability service that provides data and actionable insights to monitor applications, respond to system-wide performance changes, and optimize resource utilization. It collects monitoring and operational data in the form of logs, metrics, and events.
- **AWS Compute Optimizer**: A service that recommends optimal AWS resources for workloads to reduce costs and improve performance. It uses machine learning to analyze historical utilization metrics and offers recommendations for rightsizing instances (e.g., moving from a large instance to a smaller one).
- **AWS Config**: A service that enables the assessment, audit, and evaluation of the configurations of AWS resources. It continuously monitors and records resource configuration changes, allowing for the verification of compliance against internal guidelines (e.g., ensuring all S3 buckets are encrypted).
- **AWS Control Tower**: A service that provides the easiest way to set up and govern a secure, multi-account AWS environment. It automates the creation of a well-architected "landing zone" using best-practice blueprints and enables governance using guardrails.
- **AWS Health Dashboard**: Provides a unified view of the status of AWS services. It consists of the **Service Health Dashboard** (displays the general status of all AWS services to the general public) and the **Personal Health Dashboard** (a personalized view of the performance and availability of the AWS services underlying specific AWS resources).
- **AWS Launch Wizard**: A service that offers a guided way of sizing, configuring, and deploying AWS resources for third-party applications, such as Microsoft SQL Server or SAP, without needing to manually identify and provision individual AWS resources.
- **AWS License Manager**: A service that streamlines the process of managing software licenses (e.g., from Microsoft, SAP, Oracle, and IBM) across AWS and on-premises environments. It helps prevent license violations by tracking usage against the terms of the enterprise agreements.
- **AWS Management Console**: A web-based interface for accessing and managing AWS services. It provides a visual dashboard and is the primary method for manual interaction with the cloud environment.
- **AWS Organizations**: An account management service that enables the consolidation of multiple AWS accounts into an organization that can be centrally managed. It includes capabilities for consolidated billing and the application of policies (Service Control Policies) across groups of accounts.
- **AWS Resource Groups and Tag Editor**: A tool that allows for the management of resources by grouping them based on tags. It enables the creation of custom groups (e.g., "Production-Web-Servers") and the bulk editing of tags across multiple resources.
- **AWS Service Catalog**: A service that allows organizations to create and manage catalogs of IT services that are approved for use on AWS. It ensures that employees can only deploy resources that meet the organization's compliance and security standards.
- **AWS Systems Manager**: A unified interface that allows for the viewing of operational data and the automation of operational tasks across AWS resources. It includes tools for patching, configuring, and managing instances at scale without logging into them.
- **AWS Trusted Advisor**: An online tool that provides real-time guidance to help provision resources following AWS best practices. It inspects the environment and makes recommendations across five categories: Cost Optimization, Performance, Security, Fault Tolerance, and Service Limits.
- **AWS Well-Architected Tool**: A service that helps review the state of workloads and compares them to the latest AWS architectural best practices. It provides a consistent process for measuring architecture using the AWS Well-Architected Framework.

---

## Migration and Transfer

**AWS Migration and Data Transfer** services provide the tools and infrastructure necessary to plan, track, and execute the movement of applications, databases, and data from on-premises environments to the AWS Cloud.

- **AWS Application Discovery Service**: A service that helps enterprise customers plan migration projects by gathering information about their on-premises data centers. It collects configuration and usage data from servers to identify dependencies and map workloads.
- **AWS Application Migration Service**: The primary service for "lift-and-shift" (rehosting) migrations. It automatically converts source servers (physical, virtual, or cloud) to run natively on AWS, minimizing time-intensive, manual processes and reducing downtime.
- **AWS Database Migration Service (AWS DMS)**: A managed service used to migrate databases to AWS quickly and securely. The source database remains fully operational during the migration, minimizing downtime. It supports both **homogeneous** migrations (e.g., Oracle to Oracle) and **heterogeneous** migrations (e.g., Oracle to Amazon Aurora).
- **AWS Migration Hub**: A central location to track the progress of migrations across multiple AWS and partner solutions. It allows for the discovery of existing servers, the planning of migration projects, and the visualization of the status of each application in a single dashboard.
- **AWS Schema Conversion Tool (AWS SCT)**: A desktop application used to facilitate heterogeneous database migrations. It automatically converts the source database schema and a majority of the database code objects (including views, stored procedures, and functions) to a format compatible with the target AWS database.
- **AWS Snow Family**: A collection of physical devices used to migrate data into and out of AWS offline when network bandwidth is insufficient or unavailable.
  - **AWS Snowcone**: The most compact and portable device (approx. 8 TB usable), designed for rugged mobile environments.
  - **AWS Snowball**: A suitcase-sized device available in Storage Optimized (for petabyte-scale data transfer) and Compute Optimized (for running edge computing workloads) versions.
  - **AWS Snowmobile**: An exabyte-scale data transfer service that uses a 45-foot ruggedized shipping container pulled by a semi-truck to move massive amounts of data.
- **AWS Transfer Family**: A fully managed service that simplifies the migration of file transfer workflows to AWS. It provides support for **Secure File Transfer Protocol (SFTP)**, **File Transfer Protocol over SSL (FTPS)**, and **File Transfer Protocol (FTP)** directly into and out of Amazon S3 and Amazon EFS.

---

## Networking and Content Delivery

**AWS Networking and Content Delivery** services provide the underlying infrastructure to link AWS resources to each other and to the internet, as well as the mechanisms to deliver content to end-users with high speed and low latency.

- **Amazon API Gateway**: A fully managed service that makes it easy to create, publish, maintain, monitor, and secure APIs at any scale. It acts as a "front door" for applications to access data, business logic, or functionality from backend services, handling tasks such as traffic management, authorization, and access control.
- **Amazon CloudFront**: A global Content Delivery Network (CDN) service that delivers data, videos, applications, and APIs to viewers globally with low latency and high transfer speeds. It caches content in **Edge Locations** geographically closer to the end-users to reduce the load on the origin server.
- **AWS Direct Connect**: A cloud service solution that establishes a dedicated physical network connection from an on-premises network to AWS. By using a private fiber-optic connection instead of the public internet, it increases bandwidth throughput and provides a more consistent network experience.
- **AWS Global Accelerator**: A networking service that improves the performance of users' traffic by up to 60% using the AWS global network infrastructure. It provides static IP addresses that act as a fixed entry point to an application hosted in one or more AWS Regions, automatically routing traffic to the optimal endpoint.
- **Amazon Route 53**: A highly available and scalable cloud Domain Name System (DNS) web service. It performs three main functions: domain registration, DNS routing (translating www.example.com into IP addresses), and health checking of resources to ensure traffic is only routed to healthy endpoints.
- **Amazon VPC**: A service that enables the provisioning of a logically isolated section of the AWS Cloud where resources can be launched in a virtual network defined by the user. It offers complete control over the virtual networking environment, including selection of IP address ranges, creation of subnets, and configuration of route tables and network gateways.
- **AWS VPN**: A service that establishes secure, encrypted tunnels between a network or device and the AWS Cloud over the public internet.
  - **Site-to-Site VPN**: Connects an entire on-premises network to an Amazon VPC.
  - **Client VPN**: Connects individual users (remote workers) to an Amazon VPC or on-premises resources.

---

## Security, Identity, and Compliance

**AWS Security, Identity, and Compliance** services provide the tools to secure workloads and applications in the cloud, manage identities and access, and maintain compliance with regulatory standards.

- **AWS Artifact**: The central resource for compliance-related information. It provides on-demand access to AWS's security and compliance reports (such as SOC, PCI, and ISO reports) and select online agreements (such as the Business Associate Addendum (BAA) for HIPAA).
- **AWS Audit Manager**: A service that helps continuously audit AWS usage to simplify how risk and compliance are assessed. It automates the collection of evidence to demonstrate compliance with frameworks like GDPR, HIPAA, and PCIDSS.
- **AWS Certificate Manager (ACM)**: A service that handles the complexity of creating, storing, and renewing public and private SSL/TLS certificates. These certificates are used to secure network communications and establish the identity of websites over the internet.
- **AWS CloudHSM**: A cloud-based hardware security module (HSM) that enables the easy generation and use of your own encryption keys on the AWS Cloud. It provides a dedicated hardware device for organizations that require exclusive control over their key management infrastructure to meet strict regulatory compliance.
- **Amazon Cognito**: A service that provides identity management for web and mobile applications. It handles user sign-up, sign-in, and access control, allowing developers to add user authentication to their apps easily. It supports sign-in with social identity providers (like Facebook, Google, and Apple) and enterprise identity providers (via SAML 2.0).
- **Amazon Detective**: A service that simplifies the investigation of potential security issues and suspicious activities. It automatically collects log data from AWS resources and uses machine learning and graph theory to build a linked set of data that helps visualize the root cause of a security finding.
- **AWS Directory Service**: A managed service that enables the use of Microsoft Active Directory (AD) in the AWS Cloud. It allows directory-aware workloads and AWS resources to use managed Active Directory in the cloud or connect to an existing on-premises AD.
- **AWS Firewall Manager**: A security management service that allows for the central configuration and management of firewall rules across all accounts and applications in AWS Organizations. It simplifies the administration of AWS WAF, AWS Shield Advanced, and VPC security groups.
- **Amazon GuardDuty**: A threat detection service that continuously monitors for malicious activity and unauthorized behavior to protect AWS accounts and workloads. It uses machine learning and integrated threat intelligence to detect anomalies, such as cryptocurrency mining or unusual API calls.
- **AWS Identity and Access Management (IAM)**: The central service for controlling access to AWS resources. It enables the creation and management of AWS users and groups, and uses permissions (Policies) to allow or deny their access to specific resources.
- **AWS IAM Identity Center (AWS Single Sign-On)**: The recommended service for managing workforce access to multiple AWS accounts and business applications. It provides a single place to create or connect workforce identities and manage their access across the entire AWS organization.
- **Amazon Inspector**: An automated vulnerability management service that continually scans AWS workloads (such as EC2 instances and container images) for software vulnerabilities and unintended network exposure.
- **AWS Key Management Service (AWS KMS)**: A fully managed service that makes it easy to create and control the cryptographic keys used to encrypt data. It is integrated with most other AWS services to encrypt data stored in those services.
- **Amazon Macie**: A fully managed data security and data privacy service that uses machine learning and pattern matching to discover and protect sensitive data (such as Personally Identifiable Information or PII) stored in Amazon S3.
- **AWS Network Firewall**: A managed firewall service that makes it easy to deploy essential network protections for all Virtual Private Clouds (VPCs). It offers flexible routing and fine-grained packet inspection (Layer 3-7) to filter traffic going in and out of a VPC.
- **AWS Resource Access Manager (AWS RAM)**: A service that enables the sharing of AWS resources (such as subnets, Transit Gateways, or License Manager configurations) with any AWS account or within an AWS Organization. It eliminates the need to create duplicate resources in multiple accounts.
- **AWS Secrets Manager**: A service that helps protect secrets needed to access applications, services, and IT resources. It enables the easy rotation, management, and retrieval of database credentials, API keys, and other secrets throughout their lifecycle.
- **AWS Security Hub**: A cloud security posture management service that performs security best practice checks, aggregates alerts, and enables automated remediation. It collects findings from other AWS security services (like GuardDuty, Inspector, and Macie) into a single dashboard.
- **AWS Shield**: A managed Distributed Denial of Service (DDoS) protection service that safeguards applications running on AWS.
  - **Shield Standard**: Automatically enabled for all AWS customers at no additional cost; protects against common, frequently occurring network and transport layer DDoS attacks.
  - **Shield Advanced**: A paid service that provides higher levels of protection against sophisticated attacks, including near real-time visibility and access to the AWS DDoS Response Team (DRT).
- **AWS WAF (Web Application Firewall)**: A web application firewall that helps protect web applications or APIs against common web exploits and bots that may affect availability, compromise security, or consume excessive resources. It filters traffic based on rules (e.g., block requests from a specific country or containing SQL injection code).

---

## Serverless

**AWS Serverless** services eliminate the need to provision or manage servers. AWS handles the underlying infrastructure management, allowing focus to remain on writing code and building applications.

- **AWS Fargate**: A serverless, event-driven compute service that runs code without provisioning or managing servers. It executes code only when needed and scales automatically. Costs are incurred only for the compute time consumed (measured in milliseconds); there is no charge when the code is not running.
- **AWS Lambda**: A serverless compute engine for containers that works with Amazon ECS and Amazon EKS. It eliminates the need to provision, configure, and scale clusters of virtual machines to run containers. It is designed for workloads that require specific resource controls without the operational overhead of managing the host operating system.

---

## Storage

**AWS Storage** services provide reliable, scalable, and secure options for storing, accessing, and backing up data in the cloud. These services are categorized by the type of storage they provide: Object, Block, or File.

- **AWS Backup**: A centralized, fully managed service that makes it easy to automate data protection across AWS services. It allows for the configuration of backup policies (frequency and retention) and the monitoring of backup activity for services like Amazon EBS, Amazon RDS, Amazon DynamoDB, and Amazon EFS from a single console.
- **Amazon Elastic Block Store (Amazon EBS)**:  A high-performance block storage service designed for use with Amazon EC2. It provides persistent storage volumes that act like physical hard drives attached to virtual servers. It is optimized for transaction-intensive workloads such as databases and enterprise applications.
- **Amazon Elastic File System (Amazon EFS)**: A serverless, fully managed elastic file system that lets you share file data without provisioning or managing storage. It automatically grows and shrinks as files are added or removed. It is designed to be mounted by multiple Linux EC2 instances simultaneously, making it ideal for shared content repositories.
- **AWS Elastic Disaster Recovery**: A service that minimizes downtime and data loss by providing fast, reliable recovery of on-premises and cloud-based applications using affordable storage and minimal compute. It replicates servers to AWS and launches them only when a disaster occurs (Active/Passive strategy).
- **Amazon FSx**: A fully managed service that provides popular commercial file systems. It offers two primary types: **Amazon FSx for Windows File Server** (for applications that need the SMB protocol and Windows compatibility) and **Amazon FSx for Lustre** (for high-performance computing workloads).
- **Amazon S3 (Simple Storage Service)**: An object storage service that offers industry-leading scalability, data availability, security, and performance. It stores data as "objects" within "buckets". It is used for virtually any use case, including data lakes, websites, and mobile applications.
- **Amazon S3 Glacier**: A secure, durable, and extremely low-cost Amazon S3 storage class for data archiving and long-term backup. It is designed for data that is rarely accessed and where retrieval times of minutes to hours are acceptable.
- **AWS Storage Gateway**: A hybrid cloud storage service that connects on-premises applications to AWS cloud storage. It acts as a bridge, allowing on-premises environments to use AWS storage (like S3, EBS, and Glacier) for backup, archiving, and disaster recovery while caching frequently accessed data locally for low latency.
