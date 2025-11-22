# AWS Certified Cloud Practitioner Practice Question Set (CLF-C02)

---

## 1. Cloud Concepts

### 1.1 Define the benefits of the AWS Cloud

- **Elastic Load Balancing (ELB)**: Acts as a central entry point, accepting incoming traffic from clients and routing those requests to its registered targets (such as EC2 instances) across one or more Availability Zones. It increases fault tolerance and availability. 

- **Application Load Balancer (ALB)**: Best for HTTP/HTTPS traffic (Layer 7).

- **Network Load Balancer (NLB)**: Best for ultra-high performance TCP/UDP traffic (Layer 4).

- **Gateway Load Balancer (GLB)**: Used to deploy and scale third-party virtual network appliances.

### 1.2 Identify design principles of the AWS Cloud

- **AWS Well-Architected Framework**: A set of guiding principles and best practices used to review and improve a cloud architecture. It is built around five pillars.

- **Operational Excellence Pillar**: The ability to run and monitor systems to deliver business value and to continually improve supporting processes and procedures.

- **Security Pillar**: The ability to protect data, systems, and assets by using cloud technologies to improve your security posture.

- **Reliability Pillar**: The ability of a workload to perform its intended function correctly and consistently and to quickly recover from failure. 

- **Performance Efficiency Pillar**: The ability to use computing resources efficiently to meet system requirements and maintain that efficiency as demand changes.

- **Cost Optimization Pillar**: The ability to run systems to deliver business values at the lowest price point. 

### 1.3 Understand the benefits of and strategies for migration to the AWS Cloud

- **AWS Database Migration Service (AWS DMS)**: Used to migrate databases to or from AWS.

- **AWS Migration Hub**: A service that helps plan and track application migrations.

- **AWS Application Migration Service (AWS MGN)**: An automated lift-and-shift (rehosting) solution for migrations of physical servers or virtual servers that run on them to EC2 instances in AWS.

- **AWS Application Discovery Service**: Collects information about the usage and configuration of on-premises servers to help plan a migration to AWS.

### 1.4 Understand concepts of cloud economics

- **AWS Lambda**: Charges are dependent on the amount of time it takes to run the code and the number of requests for your Lambda functions.

---

## 2. Security and Compliance

### 2.1 Understand the AWS shared responsibility model

- **AWS Shared Responsibility Model**: This is the framework that defines the security and compliance responsibilities between AWS and the customer. In short, AWS is responsible for the security of the cloud, while the customer is responsible for security IN the cloud.

- **AWS's Responsibility (Security OF the Cloud)**: AWS is responsible for protecting the underlying global infrastructure, including the hardware, software, networking, and physical facilities that run AWS services.

- **Customer's Responsibility (Security IN the Cloud)**: The customer is responsible for securing their data and applications. This includes configuring IAM users and policies (e.g., following the principle of least privilege), managing data encryption (e.g., encrypting S3 objects), configuring network security (e.g., Security Groups and NACLs), and determining access permissions for their resources (e.g., deciding if an S3 bucket should be public or private).

### 2.2 Understand AWS Cloud security, governance, and compliance concepts

- **AWS Certificate Manager (ACM)**: A service to create, store, and renew public and private SSL/TLS certificates. These certificates are used to enable encryption in transit (HTTPS) for websites and applications.

- **AWS Resource Access Manager (AWS RAM)**: A service that allows you to securely share your AWS resources (like subnets or Transit Gateways) with other AWS accounts, often within an AWS Organization.

- **AWS Shield**: A service that is used to protect against distributed denial of service (DDoS) attacks. 

- **AWS Security Hub**: A service that is used to centrally view your security posture in AWS.

### 2.3 Identify AWS access management capabilities

- **AWS Management Console Access**: Grants access to the web-based AWS console. It requires a username and password (and optionally MFA) for an IAM user to sign in.

- **Programmatic Access**: Grants access to the AWS API, Command Line Interface (CLI), and SDKs. It requires an Access Key ID and a Secret Access Key for authentication.

### 2.4 Identify components and resources for security

- **AWS Trusted Advisor**: Checks security groups for rules that allow unrestricted access to a resource.

- **AWS Identity and Access Management (IAM)**: Manages permissions that control which AWS resources users can access.

- **Amazon CloudWatch**: Monitoring services used to collect and track metrics for AWS resources.

- **AWS CloudTrail**: Provides an audit record of API calls.

---

## 3. Cloud Technology and Services

### 3.1 Define methods of deploying and operating in the AWS Cloud

- **AWS Site-to-Site VPN**: Creates a secure, encrypted connection (tunnel) between your on-premises network and the AWS Cloud. Unlike Direct Connect, this connection travels over the public internet.

- **AWS Client VPN**: A managed client-based VPN service that allows individual users to securely connect to AWS and on-premises resources from any location. This contrasts with Site-to-Site VPN, which connects an entire network or data center.

- **AWS Direct Connect**: A cloud service that establishes a dedicated network connection from your premises to AWS. It links your internal network to an AWS Direct Connect location, bypassing the public internet to provide more consistent network performance and reduced bandwidth costs.

- **Amazon Connect**: A cloud-based omnichannel contact center service. It enables businesses to set up a customer support center (supporting both voice and chat) quickly and at scale.

### 3.2 Define the AWS global infrastructure

- **Availability Zone (AZ)**: One or more discrete data centers within an AWS Region. Each AZ has independent power, networking, and is isolated from failures in other AZs.

- **Multi-AZ Deployment** (High availability and Resilience): Strategy that involves deploying an application across multiple AZs within the same Region. If one AZ fails, the application continues to run from the other(s), preventing a single point of failure.

- **Cross-Region Deployment** (Low Latency): Strategy used to serve a global audience by placing resources in Regions geographically closer to the end-users.

### 3.4 Identify AWS database services

- **AWS Global Accelerator**: A networking service that improves the availability and performance of applications for global users by providing static IP addresses (a fixed, global entry point) and using the AWS global network to route traffic to the optimal (nearest and healthiest) endpoint.

- **Amazon DynamoDB**: A fully managed serverless NoSQL database service. 

- **Amazon Aurora**: A relational database service that is fully compatible with both MySQL and PostgreSQL.

- **Amazon Elastic Block Store**: A block storage service designed for use with Amazon EC2. It's ideal for transaction-intensive workloads, such as running a database on an EC2 instance.

### 3.5 Identify AWS network services

- **AWS Elastic Beanstalk**: Service used to deploy and scale web applications and services developed with common programming languages on automatically deployed infrastructure with capacity management, load balancing, auto scaling, and monitoring. Facilitates application provisioning and support.

- **Amazon DynamoDB Accelerator (DAX)**: An in-memory cache used to reduce response times from a DynamoDB table from milliseconds to microseconds.

- **Amazon Route 53**: Highly available and scalable DNS web service. The three main functions of Route 53 are registering domain names, routing internet traffic to the resources for the domain, and checking the health of those resources.

- **Amazon CloudFront**: A web service that speeds up the distribution of static and dynamic content, such as .html, .css, .js, and image files, to the users. Content is cached in edge locations. Content that is repeatedly accessed can be served from the edge locations instead of the source S3 bucket.

### 3.6 Identify AWS storage services

- **Amazon S3**: A object storage service. It's designed to store and retrieve any amount of data, such as files, backups, and website assets, from anywhere on the web.

### 3.7 Identify AWS artificial intelligence and machine learning (AI/ML) services and analytics services

- **Amazon Transcribe**: A service that uses machine learning to convert audio data to text.

- **Amazon Polly**: A machine learning service that converts text to speech, including the ability to read text out loud.

- **Amazon Translate**: A machine learning language translation service.

- **Amazon Textract**: A machine learning service that can extract text from scanned documents.

- **Amazon Comprehend**: A natural language processing (NLP) service that uses machine learning to find insights and relationships in text.

### 3.8 Identify services from other in-scope AWS service categories

- **Amazon Inspector**: An automated vulnerability management service that continuously scans your Amazon EC2 instances for software vulnerabilities and unintended network exposure.

- **Amazon Macie**: A data security service that uses machine learning to discover, classify, and protect sensitive data stored in Amazon S3.

- **Amazon GuardDuty**: A threat detection service that continuously monitors your AWS logs (e.g., CloudTrail, VPC Flow Logs, DNS logs) for malicious activity and unauthorized behavior.

- **AWS Secrets Manager**: A service used to manage, retrieve, and rotate secrets (e.g., database credentials and API keys) needed to access your applications, services, and IT resources.

- **Amazon EventBridge**: A serverless event bus that connects applications using events. It ingests events from apps and AWS services and routes them to targets (like Lambda or SQS) to build event-driven architectures.

- **Amazon Simple Queue Service (Amazon SQS)**: A message queuing service used to decouple applications. SQS can host a queue for requests that are sent to applications.

- **Amazon Simple Notification Service (Amazon SNS)**: A publish/subscribe service used to deliver publications (messages) to subscribers. SNS can send notifications, such as mobile text messages, push notifications, or emails, to subscribers of a quality assurance test-failure topic.

---

## 4. Billing, Pricing, and Support

### 4.1 Compare AWS pricing models

- **One-Demand Instances**: The default option with pay-as-you-go pricing. Requires no long-term commitment and are immediately available.

- **Reserved Instances**: Provides a discount in exchange for a 1- or 3-year commitment to use a specific instance type. 

- **Spot Instances**: Uses spare, unused EC2 capacity for a discount.

- **Dedicated Instances**: Run in a VPC on hardware that is physically dedicated to a individual customer. This is often used to meet licensing or compliance constraints. 

### 4.2 Understand resources for billing, budget, and cost management

- **AWS Cloud Map**: Creates and maintains a map of backend services. 

- **AWS Organizations**: Provides centralized governance and billing for an AWS environment, including multiple accounts.

- **AWS Systems Manager OpsCenter**: Provides a central location for IT professionals to view, investigate, and resolve operational work items.

- **AWS Billing and Cost Management Console**: Service used to view, understand, and manage AWS costs and usage.

### 4.3 Identify AWS technical resources and AWS Support options

- **Basic Support Plan**: Free for all AWS accounts. Provides access to customer service for billing and account issues only. It does not include technical support.

- **Developer Support Plan**: The lowest-cost paid plan. Provides email-based technical support during business hours.

- **Business Support Plan**: Provides 24/7 technical support via phone, email, and chat.

- **Enterprise Support Plan**: The highest-level plan, designed for mission-critical workloads. Includes everything in the Business plan plus a dedicated Technical Account Manager (TAM) and a 15-minute response time for critical issues.
