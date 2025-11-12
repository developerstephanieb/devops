# AWS Certified Cloud Practitioner Practice Question Set Study Guide (CLF-C02)

---

##

- **AWS Trusted Advisor**: Checks security groups for rules that allow unrestricted access to a resource.

- **AWS Identity and Access Management (IAM)**: Manages permissions that control which AWS resources users can access.

- **Amazon CloudWatch**: Monitoring services used to collect and track metrics for AWS resources.

- **AWS CloudTrail**: Provides an audit record of API calls.

---

## 

- **AWS Elastic Beanstalk**: Service used to deploy and scale web applications and services developed with common programming languages on automatically deployed infrastructure with capacity management, load balancing, auto scaling, and monitoring. Facilitates application provisioning and support.

- **Amazon DynamoDB Accelerator (DAX)**: An in-memory cache used to reduce response times from a DynamoDB table from milliseconds to microseconds.

- **Amazon Route 53**: Highly available and scalable DNS web service. The three main functions of Route 53 are registering domain names, routing internet traffic to the resources for the domain, and checking the health of those resources.

- **Amazon CloudFront**: A web service that speeds up the distribution of static and dynamic content, such as .html, .css, .js, and image files, to the users. Content is cached in edge locations. Content that is repeatedly accessed can be served from the edge locations instead of the source S3 bucket.

---

##

- **AWS Cloud Map**: Creates and maintains a map of backend services. 

- **AWS Organizations**: Provides centralized governance and billing for an AWS environment, including multiple accounts.

- **AWS Systems Manager OpsCenter**: Provides a central location for IT professionals to view, investigate, and resolve operational work items.

- **AWS Billing and Cost Management Console**: Service used to view, understand, and manage AWS costs and usage.

---

## 

- **Availability Zone (AZ)**: One or more discrete data centers within an AWS Region. Each AZ has independent power, networking, and is isolated from failures in other AZs.

- **Multi-AZ Deployment** (High availability and Resilience): Strategy that involves deploying an application across multiple AZs within the same Region. If one AZ fails, the application continues to run from the other(s), preventing a single point of failure.

- **Cross-Region Deployment** (Low Latency): Strategy used to serve a global audience by placing resources in Regions geographically closer to the end-users.

---

## 

- **AWS Global Accelerator**: A networking service that improves the availability and performance of applications for global users by providing static IP addresses (a fixed, global entry point) and using the AWS global network to route traffic to the optimal (nearest and healthiest) endpoint.

- **Amazon DynamoDB**: A fully managed serverless NoSQL database service. 

- **Amazon Aurora**: A relational database service that is fully compatible with both MySQL and PostgreSQL.

- **Amazon Elastic Block Store**: A block storage service designed for use with Amazon EC2. It's ideal for transaction-intensive workloads, such as running a database on an EC2 instance.

---

##

- **AWS Direct Connect**: A cloud service that establishes a dedicated network connection from your premises to AWS. It links your internal network to an AWS Direct Connect location, bypassing the public internet to provide more consistent network performance and reduced bandwidth costs.

- **AWS Site-to-Site VPN**: Creates a secure, encrypted connection (tunnel) between your on-premises network and the AWS Cloud. Unlike Direct Connect, this connection travels over the public internet.

- **Amazon Connect**: A cloud-based omnichannel contact center service. It enables businesses to set up a customer support center (supporting both voice and chat) quickly and at scale.

---

## 

- **Amazon Transcribe**: A service that uses machine learning to convert audio data to text.

- **Amazon Polly**: A machine learning service that converts text to speech, including the ability to read text out loud.

- **Amazon Translate**: A machine learning language translation service.

- **Amazon Textract**: A machine learning service that can extract text from scanned documents.

- **Amazon Comprehend**: A natural language processing (NLP) service that uses machine learning to find insights and relationships in text.

---

##

- **Amazon EventBridge**: A serverless event bus that connects applications using events. It ingests events from apps and AWS services and routes them to targets (like Lambda or SQS) to build event-driven architectures.

- **Amazon Simple Queue Service (Amazon SQS)**: A message queuing service used to decouple applications. SQS can host a queue for requests that are sent to applications.

- **Amazon Simple Notification Service (Amazon SNS)**: A publish/subscribe service used to deliver publications (messages) to subscribers. SNS can send notifications, such as mobile text messages, push notifications, or emails, to subscribers of a quality assurance test-failure topic.

---

##

- **Basic Support Plan**: Free for all AWS accounts. Provides access to customer service for billing and account issues only. It does not include technical support.

- **Developer Support Plan**: The lowest-cost paid plan. Provides email-based technical support during business hours.

- **Business Support Plan**: Provides 24/7 technical support via phone, email, and chat.

- **Enterprise Support Plan**: The highest-level plan, designed for mission-critical workloads. Includes everything in the Business plan plus a dedicated Technical Account Manager (TAM) and a 15-minute response time for critical issues.

---

##

- **Elastic Load Balancing (ELB)**: Acts as a central entry point, accepting incoming traffic from clients and routing those requests to its registered targets (such as EC2 instances) across one or more Availability Zones. It increases fault tolerance and availability. 

- **Application Load Balancer (ALB)**: Best for HTTP/HTTPS traffic (Layer 7).

- **Network Load Balancer (NLB)**: Best for ultra-high performance TCP/UDP traffic (Layer 4).

- **Gateway Load Balancer (GLB)**: Used to deploy and scale third-party virtual network appliances.

---

##