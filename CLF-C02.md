### Cloud Concepts
* Benefits of Cloud Computing
  * Trade fixed expense (hardware and data centres) for variable expense
  * Benefit from massive economies of scale
  * Stop guessing capacity
  * Increase speed and agility 
  * Go global in minutes

* AWS Cloud Adoption Framework (AWS CAF) divides cloud adoption into 6 key areas
  * Business - align cloud adoption with business goals
  * People - manage cultural change and develop skills
  * Governance - establish cloud governance policies
  * Platform - develop and manage cloud infrastructure
  * Security - ensure security in the cloud environment
  * Operations - optimize and manage cloud operations
    
* Shared Responsibilities Model
  * AWS - Security of the cloud (hardware, networking, virtualisation...)
  * Customer - Security in the cloud (data, applications, IAM, OS...)

* AWS Well-Architected Framework
  * Operational Excellence - Focuses on monitoring, automation and continuous improvement to ensure systems run smoothly and effectively
  * Security - Emphasises on protecting data, systems and assets through access controls, data encryption and compliance with security best practices
  * Reliability - Ensures that applications are resilient to failures and able to recover quickly and maintain uptime with fault tolerance and disaster recovery strategies
  * Performance Efficiency - Encourages optimal use of cloud resources including scalability and elasticity
  * Cost optimisation - Optimising resource usage and avoiding unnecessary expenses while scaling efficiently



### Security and Compliance
* Amazon inspector - assess app vulnerabilities and identify deployments that do not meet best practices
* AWS Trusted Advisor - optimise costs, increase performance, improve security and resilience, and operate at scale in cloud
* IAM Access Analyzer - Analyzes IAM policies to identify potential issues and excessive permissions
* IAM credential report - This built-in IAM feature provides detailed information about the rotation history of user passwords and access keys within the account. It shows dates of last password and access key rotation, along with usernames and key IDs
* AWS Artifact - Self-service portal for retrieving AWS compliance and security documentation to assist with audits and regulatory compliance efforts
* AWS Audit Manager - Automates the process of assessing, auditing, and reporting on your AWS environment's compliance with industry standards and regulations, simplifying the preparation for audits
* Amazon Inspector - Discovers workloads, such as Amazon EC2 instances, containers, and Lambda functions, and scans them for software vulnerabilities and unintended network exposure
* AWS Shield - Mainly for DDOS
* AWS WAF - Blocks common web attack patterns
* Network ACLs - Used to control traffic at the network layer
* Security Groups - Operate at the instance level and are stateful firewalls that control inbound and outbound traffic
* AWS Security Token Service - provides temporary, limited-privilege credentials
* IAM Instance Profiles - Used for proving IAM roles to EC2 instances
* Amazon GuardDuty - A threat detection service that continuously monitors for malicious activity and unauthorized behavior in AWS accounts. It generates findings related to security threats
* Amazon Macie - A security service that uses machine learning to automatically discover, classify, and protect sensitive data, such as personally identifiable information (PII), in Amazon S3
* Amazon Detective - A security service that helps users investigate and identify the root cause of potential security issues or suspicious activities.


### Cloud Technology and Services
* AWS snowball edge - portable device to transfer files (transfer data to S3 is free)
* AWS Storage Gateway's File Gateway - hybrid cloud storage service that provides on-premises applications with cloud-backed file storage, enabling seamless access to data stored in Amazon S3
* AWS Fargate - Serverless compute engine for Amazon ECS and Amazon EKS allows users to run containers without managing the underlying infrastructure. Automatically provisions resources
* AWS Lambda - Serverless service for developers to run code without provisioning
* AWS RDS - Fully managed relational database service
* AWS Athena - Interactive query service to analyse data directly in Amazon S3 using standard SQL
* AWS Compute Optimiser - Analyses historical utilisation of EC2 instances and recommends optimal AWS resources for your workload
* AWS SageMaker - Service for building, training and deploying ML models
* Amazon CodeGuru - Automated code reviews and application performance recommendations
* AWS Service Catalog - Centrally manage deployed IT services and govern its Infrastructure As Code templates
* AWS Glue - serverless data integration service that makes it easier to discover, prepare, move, and integrate data from multiple sources for analytics, ML, and application development
* AWS QuickSight - Visualise and analyse data using Business Intelligence to create dashboards
* AWS Professional Services - Global team of experts for hands-on assistance with planning, executing, and optimizing AWS migrations
* AWS Support - Provides technical support plans, but not focused on hands-on migration assistance
* AWS Launch Wizard - Simplifies application deployment
* AWS Managed Services (AMS) - Fully managed service for ongoing operational support, not designed for the initial migration phase
* AWS Elastic Beanstalk - Quickly deploy and manage applications in AWS cloud
* Amazon EC2 - Secure and resizable compute capacity for any workload
* AWS CodeBuild - Build and test code with automatic scaling
* Amazon Personalize - ML service for building personalised recommendation models
* AWS CloudFormation - Manage Infrastructure as code
* AWS CodePipeline - Automates CI/CD
* AWS CodeDeploy - Automate code deployment to various compute services such as Amazon EC2 instances, on-premise servers and AWS Lambda functions
* AWS DirectConnect - Create a dedicated network connection to AWS
* AWS Cloudwatch - Monitoring system that can be used to collect and track metrics, logs and event from AWS resources. It supports setting alarms based on cost metrics
* AWS Knowledge Center - provides answers to FAQ about security
* AWS Chatbot - interactive service that allows you to receive and respond to notification alerts within messaging platforms like slack and amazon chime
* AWS CloudTrail - Records all API calls made in the AWS accounts. It provides detailed history of events
* Amazon EventBridge - An event bus service that enables event-driven architectures
* Amazon Aurora - Fully managed Relational Database with automatic scaling
* Amazon DynamoDB - Fully managed NoSQL database
* Amazon RedShift - Fully managed relational warehouse service
* AWS Transit Gateway - onnects your Amazon Virtual Private Clouds (VPCs) and on-premises networks through a central hub. This connection simplifies your network and puts an end to complex peering relationships.

### Billing and Pricing
* AWS Billing Conductor - create custome pricing and billing for AWS usage
* AWS Cost Explorer - provides cost and usage reports, allowing for analysis of historical costs and usage patterns
* AWS Pricing Calculator - Estimates AWS services based on configurations
* AWS Organisations - Enables you to centrally manage and govern multiple AWS accounts allowing for consolidating billing, organisational unit creation, and applying policies across all accounts
* Amazon EC2 pricing models
  * On-Demand Instances - Pay for compute capacity by the second (with a minimum of 60 seconds) with no long-term commitment, offering flexibility but at a higher cost for short-term or unpredictable workloads
  * Reserved Instances - Pay upfront (or with partial payment) for a one- or three-year term in exchange for a significant discount compared to On-Demand pricing. This is ideal for predictable, steady-state workloads
  * Spot Instances - Bid for unused EC2 capacity at a significantly reduced price, but with the risk of instances being terminated by AWS when capacity is needed elsewhere. Suitable for flexible, fault-tolerant workloads
  * Savings Plans - A flexible pricing model that offers lower rates in exchange for committing to a consistent amount of compute usage over a one- or three-year period, with more flexibility than Reserved Instances
  * Dedicated Hosts - Pay for physical servers dedicated to your use, allowing for licensing portability and compliance with specific licensing requirements, ideal for running legacy workloads or specific regulatory needs
* AWS Budgets - Set budgets based on cost or usage and will alert customers when budget is hit via notifications