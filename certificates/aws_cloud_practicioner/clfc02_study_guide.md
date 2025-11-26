# AWS Certified Cloud Practitioner Study Guide (CLF-C02)

---

## 1. Technologies and Concepts

### Application Programming Interfaces (API)

**Application Programming Interfaces (API)** serve as the primary mechanism through which users and applications interact with the AWS platform. Every action performed on AWS, whether clicking a button in a web browser or running a script, ultimately results in an API call to the respective AWS service. AWS APIs can be accessed via the AWS Management Console (GUI), the AWS Command Line Interface (CLI), and AWS Software Development Kits (SDKs).

- **AWS Management Console**: A web-based interface that provides a visual dashboard for managing AWS resources. It is suitable for manual resource provisioning and monitoring but is less efficient for automation.

- **AWS Command Line Interface (CLI)**: A unified tool that enables the control of AWS services from a command line shell. This method is often used for automating repetitive tasks and managing resources through scripts.

- **AWS Software Development Kits (SDKs)**: These libraries allow developers to interact with AWS services directly from application code (e.g., Python, Java, Node.js). SDKs handle low-level details such as authentication, retries, and connection management.

- **Public vs Private**: APIs can be public (accessible over the internet) or private (only accessible within the Virtual Private Cloud).

### Benefits of migrating to the AWS Cloud

The **Six Advantages of Cloud Computing** describe the fundamental shifts in economic and operational models when moving from on-premises infrastructure to the cloud.

- **Trade capital expense for variable expense**: Organizations can avoid heavy upfront investment in physical data centers (CapEx) in favor of paying only for computing resources consumed (OpEx).

- **Benefit from massive economies of scale**: Due to the aggregate usage from hundreds of thousands of customers, AWS achieves lower variable costs than an individual organization could achieve alone. These savings are passed on to the customer in the form of lower pay-as-you-go prices.

- **Stop guessing capacity**: Cloud computing eliminates the need to predict infrastructure requirements in advance. Resources scale up or down automatically to match demand, preventing expensive idle resources or capacity shortages.

- **Increase speed and agility**: IT resources can be launched in minutes rather than weeks. This drastically reduces the time and cost required to experiment and develop new applications.

- **Stop spending money running and maintaining data centers**: Focus shifts to developing applications and differentiating business value rather than the heavy lifting of racking, stacking, and powering servers.

- **Go global in minutes**: Applications can be deployed in multiple AWS Regions around the world with just a few clicks, providing lower latency and a better experience for customers regardless of their location.

### AWS Cloud Adoption Framework (AWS CAF)

The **AWS Cloud Adoption Framework (AWS CAF)** provides a comprehensive set of guidelines to help organizations structure and execute their digital transformation strategies. It organizes guidance into six areas of focus, known as **Perspectives**, which are separated into Business Capabilities and Technical Capabilities.

- **Business Perspective**: Focuses on ensuring that cloud adoption aligns with business goals and measurable outcomes. It addresses strategy, product management, and business insights.

- **People Perspective**: Focuses on organizational change management, culture, and training. It addresses workforce transformation and preparing teams for cloud operations.

- **Governance Perspective**: Focuses on orchestrating cloud initiatives to maximize organizational benefits while minimizing risks. It addresses portfolio management and program management.

- **Platform Perspective**: Focuses on the architectural design and modernization of infrastructure and applications. It addresses the delivery of scalable and resilient cloud solutions.

- **Security Perspective**: Focuses on achieving confidentiality, integrity, and availability of data and workloads. It addresses compliance, risk management, and identity management.

- **Operations Perspective**: Focuses on the health, availability, and performance of IT services. It addresses the monitoring, management, and automation of cloud environments.

### AWS Compliance 
### Compute
### Cost management
### Databases
### Amazon EC2 instance types (for example, Reserved, On-Demand, Spot)
### AWS global infrastructure (for example, AWS Regions, Availability Zones)
### Infrastructure as code (IaC)
### AWS Knowledge Center
### Machine learning
### Management and governance
### Migration and data transfer
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

## 2. AWS Services and Features

### Analytics
- Amazon Athena:
- AWS Data Exchange:
- Amazon EMR:
- AWS Glue:
- Amazon Kinesis:
- Amazon Managed Streaming for Apache Kafka (Amazon MSK):
- Amazon OpenSearch Service:
- Amazon QuickSight:
- Amazon Redshift:

### Application Integration
- Amazon EventBridge:
- Amazon Simple Notification Service (Amazon SNS):
- Amazon Simple Queue Service (Amazon SQS):
- AWS Step Functions:

### Business Applications
- Amazon Connect:
- Amazon Simple Email Service (Amazon SES):

### Cloud Financial Management
- AWS Billing Conductor:
- AWS Budgets:
- AWS Cost and Usage Report:
- AWS Cost Explorer:
- AWS Marketplace:

### Compute
- AWS Batch:
- Amazon EC2:
- AWS Elastic Beanstalk:
- Amazon Lightsail:
- AWS Local Zones:
- AWS Outposts:
- AWS Wavelength:

### Containers
- Amazon Elastic Container Registry (Amazon ECR):
- Amazon Elastic Container Service (Amazon ECS):
- Amazon Elastic Kubernetes Service (Amazon EKS):

### Customer Engagement
- AWS Activate for Startups:
- AWS IQ:
- AWS Managed Services (AMS):
- AWS Support:

### Database
- Amazon Aurora:
- Amazon DynamoDB:
- Amazon MemoryDB for Redis:
- Amazon Neptune:
- Amazon RDS:

### Developer Tools
- AWS AppConfig:
- AWS CLI:
- AWS Cloud9:
- AWS CloudShell:
- AWS CodeArtifact:
- AWS CodeBuild:
- AWS CodeCommit:
- AWS CodeDeploy:
- AWS CodePipeline:
- AWS CodeStar:
- AWS X-Ray:

### End User Computing
- Amazon AppStream 2.0:
- Amazon WorkSpaces:
- Amazon WorkSpaces Web:

### Frontend Web and Mobile
- AWS Amplify:
- AWS AppSync:
- AWS Device Farm:

### Internet of Things (IoT)
- AWS IoT Core:
- AWS IoT Greengrass:

### Machine Learning
- Amazon Comprehend:
- Amazon Kendra:
- Amazon Lex:
- Amazon Polly:
- Amazon Rekognition:
- Amazon SageMaker:
- Amazon Textract:
- Amazon Transcribe:
- Amazon Translate:

### Management and Governance
- AWS Auto Scaling:
- AWS CloudFormation:
- AWS CloudTrail:
- Amazon CloudWatch:
- AWS Compute Optimizer:
- AWS Config:
- AWS Control Tower:
- AWS Health Dashboard:
- AWS Launch Wizard:
- AWS License Manager:
- AWS Management Console:
- AWS Organizations:
- AWS Resource Groups and Tag Editor:
- AWS Service Catalog:
- AWS Systems Manager:
- AWS Trusted Advisor:
- AWS Well-Architected Tool:

### Migration and Transfer
- AWS Application Discovery Service:
- AWS Application Migration Service:
- AWS Database Migration Service (AWS DMS):
- AWS Migration Hub:
- AWS Schema Conversion Tool (AWS SCT):
- AWS Snow Family:
- AWS Transfer Family:

### Networking and Content Delivery
- Amazon API Gateway:
- Amazon CloudFront:
- AWS Direct Connect:
- AWS Global Accelerator:
- Amazon Route 53:
- Amazon VPC:
- AWS VPN:

### Security, Identity, and Compliance
- AWS Artifact:
- AWS Audit Manager:
- AWS Certificate Manager (ACM):
- AWS CloudHSM:
- Amazon Cognito:
- Amazon Detective:
- AWS Directory Service:
- AWS Firewall Manager:
- Amazon GuardDuty:
- AWS Identity and Access Management (IAM):
- AWS IAM Identity Center (AWS Single Sign-On):
- Amazon Inspector:
- AWS Key Management Service (AWS KMS):
- Amazon Macie:
- AWS Network Firewall:
- AWS Resource Access Manager (AWS RAM):
- AWS Secrets Manager:
- AWS Security Hub:
- AWS Shield:
- AWS WAF:

### Serverless
- AWS Fargate:
- AWS Lambda:

### Storage
- AWS Backup:
- Amazon Elastic Block Store (Amazon EBS):
- Amazon Elastic File System (Amazon EFS):
- AWS Elastic Disaster Recovery:
- Amazon FSx:
- Amazon S3:
- Amazon S3 Glacier:
- AWS Storage Gateway:
