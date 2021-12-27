
## Amazon Cognito
Allows you to add user sign-up, sign-in, and access control to your web and mobile apps quickly and easily.

## AWS Management Console
Is used to access and manage Amazon Web Services through a simple and intuitive web-based user interface. The console itself doesn’t provide any recommendations.

# General 
- A computer on which AWS runs one or more virtual machines is called a host machine, and each virtual machine is called a guest machine. AWS drives the concept of virtualization by allowing the physical host machine to operate multiple virtual machines as guests (for multiple customers) to help maximize the effective use of computing resources such as memory, network bandwidth and CPU cycles.

## AWS Auto Scaling
Is the feature that automates the process of adding/removing server capacity (based on demand). Autoscaling allows you to reduce your costs by automatically turning off resources that aren’t in use. On the other hand, Autoscaling ensures that your application runs effectively by provisioning more server capacity if required.

## Horizontal Scaling
       Scaling horizontally takes place through an increase in the number of resources (e.g., adding more hard drives to a storage array or adding more servers to support an application). This is a great way to build Internet-scale applications that leverage the elasticity of cloud computing.

## Vertical Scaling:
        Scaling vertically takes place through an increase in the specifications of an individual resource (e.g., upgrading a server with a larger hard drive, adding more memory, or provisioning a faster CPU). On Amazon EC2, this can easily be achieved by stopping an instance and resizing it to an instance type that has more RAM, CPU, I/O,or networking capabilities. This way of scaling can eventually hit a limit and it is not always a cost efficient or highly available approach. However, it is very easy to implement and can be sufficient for many use cases especially as a short term solution.

Vertical-scaling is often limited to the capacity constraints of a single machine, scaling beyond that capacity often involves downtime and comes with an upper limit. With horizontal-scaling it is often easier to scale dynamically by adding more machines in parallel. Hence, in most cases, horizontal-scaling is recommended over vertical-scaling.

## AWS Elastic Load Balancer (ELB) 
Is a service that distributes the incoming application traffic to multiple targets that you define.
- Application Load Balancer (Http) More intteligent
- Network Load Balancer(TCP/UDP) More faster
- Classic Load Balancer Not used now.

## The difference between AWS-managed services and customer-managed services:
- For AWS-managed services such as Amazon RDS and Amazon DynamoDB, AWS is responsible for performing all the operations needed to keep the service running.
The AWS-managed services automate time-consuming administration tasks such as hardware provisioning, software setup, patching and backups. The AWS-managed services free customers to focus on their applications so they can give them the fast performance, high availability, security and compatibility they need.
- Examples of AWS-managed services include Amazon RDS, Amazon DynamoDB, Amazon Redshift, Amazon WorkSpaces, Amazon CloudFront, Amazon CloudSearch, and several other services.

- On the other hand, customer-managed services are services that are completely managed by the customer. For example, a service such as Amazon Elastic Compute Cloud (Amazon EC2) is categorized as Infrastructure as a Service (IaaS) and, as such, requires the customer to perform all of the necessary security configuration and management tasks. Customers that deploy an Amazon EC2 instance are responsible for the management of the guest operating system (including updates and security patches), any application software or utilities installed by the customer on the instances, and the configuration of the AWS-provided firewall (called a security group) on each instance.
- Examples of customer-managed services include Amazon Elastic Compute Cloud (Amazon EC2), Amazon Virtual Private Cloud (Amazon VPC), and AWS Identity And Access Management (AWS IAM).


## AWS Personal Health Dashboard
 Provides alerts and remediation guidance when AWS is experiencing events that may impact you. 
 While the Service Health Dashboard displays the general status of AWS services, Personal Health Dashboard gives you a personalized view into
 the performance and availability of the AWS services underlying your AWS resources.

The benefits of the AWS personal health dashboard include:

- A personalized View of Service Health: Personal Health Dashboard gives you a personalized view of the status of the AWS services that power your applications, enabling you to quickly see when AWS is experiencing issues that may impact you. For example, in the event of a lost EBS volume associated with one of your EC2 instances, you would gain quick visibility into the status of the specific service you are using, helping save precious time troubleshooting to determine root cause.

- Proactive Notifications: The dashboard also provides forward looking notifications, and you can set up alerts across multiple channels, including email and mobile notifications, so you receive timely and relevant information to help plan for scheduled changes that may affect you. In the event of AWS hardware maintenance activities that may impact one of your EC2 instances, for example, you would receive an alert with information to help you plan for, and proactively address any issues associated with the upcoming change.

- Detailed Troubleshooting Guidance: When you get an alert, it includes remediation details and specific guidance to enable you to take immediate action to address AWS events impacting your resources. For example, in the event of an AWS hardware failure impacting one of your EBS volumes, your alert would include a list of your affected resources, a recommendation to restore your volume, and links to the steps to help you restore it from a snapshot. This targeted and actionable information reduces the time needed to resolve issues.

## AWS Service Health Dashboard
You can get information about the current status and availability of the general AWS services any time ,is available at this link: https://status.aws.amazon.com/
 
## AWS Budgets
AWS Budgets gives you the ability to set **custom budgets** that alert you when your costs or usage exceed (or are forecasted to exceed) your budgeted amount. The difference between AWS Budgets and Amazon CloudWatch billing alarms is that Amazon CloudWatch billing alarms alert you only when your actual cost exceeds a certain threshold, while AWS Budgets can be configured to alert you when the actual or forecasted cost exceeds a certain threshold.


## AWS Cost Explorer 
Is a free tool that you can use to view your costs and usage. You can view data up to the last 13 months, forecast how much you are likely to spend for the next 12 months, and get recommendations for what Reserved Instances to purchase. You can use AWS Cost Explorer to see patterns in how much you spend on AWS resources over time, identify areas that need further inquiry, and see trends that you can use to understand your costs. You can also specify time ranges for the data, and view time data by day or by month.

## AWS Pricing Calculator
Is a web service that you can use to estimate the cost for your AWS monthly bill based on your expected usage.

## The AWS Cost & Usage Report
Is your one-stop shop for accessing the most detailed information available about your AWS costs and usage.The AWS Cost & Usage Report lists AWS usage for each service category used by an account and its IAM users in hourly or daily line items, as well as any tags that you have activated for cost allocation purposes.

## Amazon CloudWatch
Is used to monitor the utilization of AWS resources and services. You can use CloudWatch to visualize system metrics, take automated actions, troubleshoot performance issues, discover insights to optimize your applications, and ensure they are running smoothly.
In CloudWatch, you can set up a billing alarm that triggers if your costs exceed a threshold that you set. This **CloudWatch alarm** can also be configured to trigger an SNS notification to your email address.

## AWS CloudTrail
Is an AWS service that can be used to monitor all user interactions with the AWS environment.
 AWS CloudTrail is a service that enables governance, compliance, operational auditing, and risk auditing by logging all API calls made within your AWS account. 

## The AWS Well-Architected Framework is based on six pillars:
• Operational Excellence
• Security
• Reliability
• Performance Efficiency
• Cost Optimization
• Sustainability

## AWS Trusted Advisor 
Offers a rich set of best practice checks and recommendations across five categories: cost optimization; security; fault tolerance; performance; and service limits. Like your customized cloud security expert, AWS Trusted Advisor analyzes your AWS environment and provides security recommendations to protect your AWS environment. The service improves the security of your applications by closing gaps, examining permissions, and enabling various AWS security features.
The core security checks include: (Important)

- 1- Security Groups - Specific Ports Unrestricted.

Checks security groups for rules that allow unrestricted access to specific ports. Unrestricted access increases opportunities for malicious activity (hacking, denial-of-service attacks, loss of data).

- 2- Amazon S3 Bucket Permissions.

Checks buckets in Amazon Simple Storage Service (Amazon S3) that have open access permissions. Bucket permissions that grant List access to everyone can result in higher than expected charges if objects in the bucket are listed by unintended users at a high frequency. Bucket permissions that grant Upload/Delete access to everyone create potential security vulnerabilities by allowing anyone to add, modify, or remove items in a bucket. This check examines explicit bucket permissions and associated bucket policies that might override the bucket permissions.

- 3- MFA on Root Account.

Checks the root account and warns if multi-factor authentication (MFA) is not enabled. For increased security, AWS recommends that you protect your account by using MFA, which requires a user to enter a unique authentication code from their MFA hardware or virtual device when interacting with the AWS console and associated websites.

## Amazon Connect 
Cloud-based contact center service that helps businesses to deliver customer service at a low cost.
Available only to customers having an Enterprise Support subscription.

## AWS Knowledge Center 
Is available for everyone free of charge. The AWS Knowledge Center helps answer the questions most frequently asked by AWS customers. The AWS Knowledge Center does not provide guidance on a case-by-case basis.

## AWS Marketplace
Is a curated digital catalog that makes it easy for customers to find, buy, deploy, and manage third-party software and services that customers need to build solutions and run their businesses. AWS Marketplace includes thousands of software listings from popular categories such as security, networking, storage, machine learning, business intelligence, database, and DevOps. AWS Marketplace also simplifies software licensing and procurement with flexible pricing options and multiple deployment methods. Customers can quickly launch pre-configured software with just a few clicks, and choose software solutions in AMI and SaaS formats, as well as other formats. Flexible pricing options include free trial, hourly, monthly, annual, multi-year, and BYOL, and get billed from one source, AWS.

## The AWS Abuse team
Can assist you when AWS resources are being used to engage in the following types of abusive behavior:     

- Spam: You are receiving unwanted emails from an AWS-owned IP address, or AWS resources are being used to spam websites or forums.

- Port scanning: Your logs show that one or more AWS-owned IP addresses are sending packets to multiple ports on your server, and you believe this is an attempt to discover unsecured ports.

- Denial of service attacks (DOS): Your logs show that one or more AWS-owned IP addresses are being used to flood ports on your resources with packets, and you believe this is an attempt to overwhelm or crash your server or software running on your server.    

- Intrusion attempts: Your logs show that one or more AWS-owned IP addresses are being used to attempt to log in to your resources.

- Hosting objectionable or copyrighted content: You have evidence that AWS resources are being used to host or distribute illegal content or distribute copyrighted content without the consent of the copyright holder.

- Distributing malware: You have evidence that AWS resources are being used to distribute software that was knowingly created to compromise or cause harm to computers or machines on which it is installed.
Note: Anyone can report abuse of AWS resources, not just AWS customers.

## AWS Support Concierge Service
 AWS Support Concierge is available only for AWS Enterprise support subscribers and is dedicated only to help AWS customers with their billing and account inquiries.

## AWS Customer Service
The AWS Customer Service team is at the forefront of this transformational technology assisting a global list of customers that are taking advantage of a growing set of services and features to run their mission-critical applications. The team helps AWS customers understand what Cloud Computing is all about, and whether it can be useful for their business needs.
Can help AWS customers with their billing and account inquiries, and it is included in all AWS support plans (Basic, Developer, Business, and Enterprise). However, due to the fact that AWS Customer Service is not dedicated to specific types of inquiries, it is not as quick or as **efficient as the AWS Support Concierge**.

"AWS Operations Support" is incorrect. AWS Operations Support is an Enterprise support program that provides operations assessments and analysis to identify gaps across the operations lifecycle, as well as recommendations based on best practices.
## AWS Application Discovery Service
Helps enterprise customers plan migration projects by gathering information about their on-premises data centers.

## AWS Infrastructure Event Management
Is a short-term engagement with AWS Support, included in the Enterprise-level Support product offering, and available for additional purchase for Business-level Support subscribers. AWS Infrastructure Event Management partners with your technical and project resources to gain a deep understanding of your use case and provide architectural and scaling guidance for an event. Common use-case examples for AWS Event Management include advertising launches, new product launches, and infrastructure migrations to AWS.

## AWS Managed Services (AMS) service.
AMS is an AWS service that operates AWS on behalf of enterprise customers and partners. Enterprises want to adopt AWS at scale but often the skills that have served them well in traditional IT do not always translate to success in the cloud. AWS Managed Services (AMS) enables them to migrate to AWS at scale more quickly, reduce their operating costs, improve security and compliance and focus on their differentiating business priorities.

## AWS Server Migration Service (SMS)
Is used to migrate your on-premises workloads to AWS.

## AWS Database Migration Service (DMS)
Helps you migrate databases to AWS easily and securely. The source database remains fully operational during the migration, minimizing downtime to applications that rely on the database. The AWS Database Migration Service can migrate your data to and from most widely used commercial and open-source databases. The service supports homogeneous migrations such as Oracle to Oracle, as well as heterogeneous migrations between different database platforms, such as Oracle to Amazon Aurora or Microsoft SQL Server to MySQL. It also allows you to stream data to Amazon Redshift from any of the supported sources including Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle, SAP ASE, and SQL Server, enabling consolidation and easy analysis of data in the petabyte-scale data warehouse. AWS Database Migration Service can also be used for continuous data replication with high availability.   

# Database

## Amazon DynamoDB
Is a NoSQL database service.
DynamoDB is serverless with no servers to provision, patch, or manage and no software to install, maintain, or operate. DynamoDB automatically scales tables up and down to adjust for capacity and maintain performance. Availability and fault tolerance are built in, eliminating the need to architect your applications for these capabilities.

## Amazon Neptune
Is a graph database service, not a MySQL database service. Amazon Neptune is used to build and run applications that work with highly connected datasets, such as social networking, recommendation engines, and knowledge graphs.

## Amazon Aurora
Is a MySQL and PostgreSQL-compatible relational database built for the cloud. Amazon Aurora combines the performance and availability of traditional enterprise databases with the simplicity and cost-effectiveness of open source databases. It delivers up to five times the throughput of standard MySQL and up to three times the throughput of standard PostgreSQL. Amazon Aurora is designed to be compatible with MySQL and with PostgreSQL, so that existing applications and tools can run without requiring modification. It is available through Amazon Relational Database Service (RDS), freeing you from time-consuming administrative tasks such as provisioning, patching, backup, recovery, failure detection, and repair.

## Amazon Redshift 
Is a fully managed data warehouse service that allows you to run complex analytic queries against petabytes of structured data using standard SQL and your existing Business Intelligence (BI) tools.

## Amazon Athena 
Is an interactive query service that is mainly used to analyze data in Amazon S3 using standard SQL.

## Amazon ElastiCache
Is a web service that makes it easy to deploy, operate, and scale an in-memory data store or cache in the cloud. The service improves the performance of web applications by allowing you to retrieve information from fast, managed, in-memory data stores, instead of relying entirely on slower disk-based databases.
        The primary purpose of an in-memory data store is to provide ultrafast (submillisecond latency) and inexpensive access to copies of data. Querying a database is always slower and more expensive than locating a copy of that data in a cache. Some database queries are especially expensive to perform. An example is queries that involve joins across multiple tables or queries with intensive calculations. By caching (storing) such query results, you pay the price of the query only once. Then you can quickly retrieve the data multiple times without having to re-execute the query.

## Amazon EMR
Launches clusters in minutes. You don’t need to worry about node provisioning, infrastructure setup, Hadoop configuration, or cluster tuning. Amazon EMR takes care of these tasks so you can focus on analysis.

## AWS Key Management Service (AWS KMS) 
AWS KMS a managed service provides a highly available key storage, management, and auditing solution for you to encrypt data within your own applications and control the encryption of stored data across AWS services.

# Security

## IAM user
Is an entity that you create in AWS to represent the person or application that uses it to directly interact with AWS. A primary use for IAM users is to give people the ability to sign in to the AWS Management Console for interactive tasks and to make programmatic requests to AWS services using the API or CLI. A user in AWS consists of a name, a password to sign into the AWS Management Console, and up to two access keys that can be used with the API or CLI. When you create an IAM user, you grant it permissions by making it a member of a group that has appropriate permission policies attached (recommended), or by directly attaching policies to the user.

## IAM group 
Is a collection of IAM users that are managed as a unit. Groups let you specify permissions for multiple users, which can make it easier to manage the permissions for those users. For example, you could have a group called Admins and give that group the types of permissions that administrators typically need. Any user in that group automatically has the permissions that are assigned to the group. If a new user joins your organization and needs administrator privileges, you can assign the appropriate permissions by adding the user to that group. Similarly, if a person changes jobs in your organization, instead of editing that user's permissions, you can remove him or her from the old groups and add him or her to the appropriate new groups.

## IAM role
Is an IAM identity that you can create in your account that has specific permissions. IAM roles allow you to delegate access (for a limited time) to users or services that normally don't have access to your organization's AWS resources. IAM users or AWS services can assume a role to obtain temporary security credentials that can be used to interact with specific AWS resources. 

             You can use roles to delegate access to users, applications, or services that don't normally have access to your AWS resources. For example, you might want to grant users in your AWS account access to resources they don't usually have, or grant users in one AWS account access to resources in another account. Or you might want to allow a mobile app to use AWS resources, but not want to embed AWS keys within the app. Sometimes you want to give AWS access to users who already have identities defined outside of AWS, such as in your corporate directory. Or, you might want to grant access to your account to third parties so that they can perform an audit on your resources. For these scenarios, you can delegate access to AWS resources using an IAM role.
Additional information:

An IAM role is similar to an IAM user, in that it is an AWS identity with permission policies that determine what the identity can and cannot do in AWS. However, instead of being uniquely associated with one person, a role is intended to be assumable by anyone (or any service, application, ...etc) who needs it. Also, a role does not have standard long-term credentials such as a password or access keys associated with it. Instead, when you assume a role, it provides you with temporary security credentials for your role session. IAM roles are meant to be assumed by authorized entities, such as IAM users, applications, or an AWS service such as Amazon EC2.


## AWS Shield
AWS provides flexible infrastructure and services that help customers implement strong DDoS mitigations and create highly available application architectures that follow AWS Best Practices for DDoS Resiliency. These include services such as Amazon Route 53, Amazon CloudFront, Elastic Load Balancing, and AWS WAF to control and absorb traffic, and deflect unwanted requests. These services integrate with AWS Shield, a managed DDoS protection service that provides always-on detection and automatic inline mitigations to safeguard web applications running on AWS.

## Amazon Inspector
Is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. Amazon Inspector automatically assesses applications for vulnerabilities or deviations from best practices. After performing an assessment, Amazon Inspector produces a detailed list of security findings prioritized by level of severity. These findings can be reviewed directly or as part of a detailed assessment report which is available via the Amazon Inspector console or API. To help get started quickly, Amazon Inspector includes a knowledge base of hundreds of rules mapped to common security best practices and vulnerability definitions. Examples of built-in rules include checking for remote root login being enabled, or vulnerable software versions installed. These rules are regularly updated by AWS security researchers.

## Penetration testing
Is the practice of testing a network or web application to find security vulnerabilities that an attacker could exploit. Penetration testing is much more related to security, not fault tolerance. 
AWS customers are welcome to carry out security assessments and penetration tests against their AWS infrastructure without prior approval for 8 services:

1- Amazon EC2 instances, NAT Gateways, and Elastic Load Balancers.

2- Amazon RDS.

3- Amazon CloudFront.

4- Amazon Aurora.

5- Amazon API Gateways.

6- AWS Lambda and Lambda Edge functions.

7- Amazon Lightsail resources.

8- Amazon Elastic Beanstalk environments.



## Amazon Elastic Compute Cloud (Amazon EC2)
Is a service that gives you complete control over your compute resources. Apart from patching the underlying host - which is the responsibility of AWS - you are responsible for managing almost everything in your server instances when using Amazon EC2.
» There are no startup or termination fees associated with Amazon EC2.
» With Amazon EC2 on-demand instances, you only pay for the compute capacity you consume, and once you stop using them, there are no additional costs or termination fees.
» With On-Demand instances, you pay for compute capacity by the hour or the second depending on which instances you run. No longer-term commitments or upfront payments are needed.
» With per-second billing, you pay for only what you use. It takes cost of unused minutes and seconds in an hour off of the bill, so you can focus on improving your applications instead of maximizing usage to the hour. Especially, if you manage instances running for irregular periods of time, such as dev/testing, data processing, analytics, batch processing and gaming applications, can benefit.
» Per-second billing is available for instances launched in:
- On-Demand, Reserved and Spot forms
- All regions and Availability Zones
- Amazon Linux, Windows and Ubuntu

#### Spot instances
Provide a discount (up to 90%) off the On-Demand price. The Spot price is determined by long-term trends in supply and demand for EC2 spare capacity. If the Spot price exceeds the maximum price you specify for a given instance or if capacity is no longer available, your instance will automatically be interrupted.
         Spot Instances are a cost-effective choice if you can be flexible about when your applications run and if you don't mind if your applications get interrupted. For example, Spot Instances are well-suited for data analysis, batch jobs, background processing, and optional tasks. 

####  Dedicated instances
Are used when you need your instances to be physically isolated at the host hardware level from instances that belong to other AWS accounts. Dedicated instances are significantly more expensive than Spot Instances

####  Reserved instances
Are recommended for Customers that can commit to using EC2 over a 1 or 3-year term to reduce their total computing costs. Even if the project will last for more than a year, the cost-benefit for acquiring Reserved Instances is not as great as the cost-benefit from using Spot Instances. The Spot option provides the largest discount (up to 90%).

- Convertible Reserved Instances
You can exchange one or more Reserved Instances for another Reserved Instance with a different configuration, including instance family, operating system, and tenancy. There are no limits to how many times you perform an exchange, as long as the new Convertible Reserved Instance is of an equal or higher value than the original Convertible Reserved Instances that you are exchanging.

- Standard Reserved Instances
Can't modify them. You can modify attributes such as the Availability Zone, instance size (within the same instance family), and scope of your Reserved Instance (regional or zonal). Standard RIs provide the most significant discount (up to 72% off On-Demand) and are best suited for steady-state usage.

## "Disk disposal" ( Storage Device Decommissioning)
When a storage device has reached the end of its useful life, AWS procedures include a decommissioning process that is designed to prevent customer data from being exposed to unauthorized individuals. All decommissioned magnetic storage devices are degaussed and physically destroyed in accordance with industry-standard practices.

# Storage
## EBS
Amazon EBS is a block level storage that provides storage volumes for use with Amazon EC2 and Amazon RDS. 
Creating snapshots of EBS Volumes can help ensure that you have a backup of your EBS volumes just in case any issues arise.
 EBS Snapshots are incremental backups, which means that only the blocks on the device that have changed after your last snapshot are saved. This minimizes the time required to create the snapshot and saves on storage costs by not duplicating data.
 Amazon EBS encryption offers a straight-forward encryption solution for your EBS resources that doesn't require you to build, maintain, and secure your own key management infrastructure. Encryption operations occur on the servers that host EC2 instances, ensuring the security of both data-at-rest and data-in-transit between an instance and its attached EBS storage.

## Amazon S3
Stores any number of objects, but each object does have a size limitation. Individual Amazon S3 objects can range in size from a minimum of 0 bytes to a maximum of 5 terabytes.
- S3 Standard offers high durability, availability, and performance object storage for frequently accessed data.

- Amazon S3 Standard-Infrequent Access (S3 Standard-IA) is for data that is accessed less frequently, but requires rapid access when needed.

- S3 Intelligent-Tiering storage class is designed to optimize costs by automatically moving data to the most cost-effective access tier, without performance impact or operational overhead. It works by storing objects in two access tiers: one tier that is optimized for frequent access and another lower-cost tier that is optimized for infrequent access. For a small monthly monitoring and automation fee per object, Amazon S3 monitors access patterns of the objects in S3 Intelligent-Tiering, and moves the ones that have not been accessed for 30 consecutive days to the infrequent access tier. If an object in the infrequent access tier is accessed, it is automatically moved back to the frequent access tier. There are no retrieval fees when using the S3 Intelligent-Tiering storage class, and no additional tiering fees when objects are moved between access tiers. It is the ideal storage class for long-lived data with access patterns that are unknown or unpredictable.

- Amazon S3 Glacier is a low-cost storage class for data that is rarely accessed; such as archived data.

- Amazon S3 Glacier Deep Archive is an extremely low-cost storage service that provides secure, durable, and flexible storage for long-term data backup and archival. With Amazon S3 Glacier Deep Archive, customers can reliably store their data for as little as $1 per terabyte per month, a significant savings compared to on-premises solutions. Amazon Glacier enables customers to offload the administrative burdens of operating and scaling storage to AWS, so that they don’t have to worry about capacity planning, hardware provisioning, data replication, hardware failure detection and repair, or time-consuming hardware migrations.


## AWS Snowball
Is a petabyte-scale data transport solution that uses secure appliances to transfer large amounts of data into and out of the AWS cloud. Using Snowball addresses common challenges with large-scale data transfers, including high network costs, long transfer times, and security concerns. AWS Customers use Snowball to migrate analytics data, genomics data, video libraries, image repositories, and backups. Transferring data with Snowball is simple, fast, secure, and can cost as little as one-fifth the cost of using high-speed internet.
Additionally, With AWS Snowball, you can access the compute power of the AWS Cloud locally and cost-effectively in places where connecting to the internet might not be an option. AWS Snowball is a perfect choice if you need to run computing in rugged, austere, mobile, or disconnected (or intermittently connected) environments.
With AWS Snowball, you have the choice of two devices, Snowball Edge Compute Optimized with more computing capabilities, suited for higher performance workloads, or Snowball Edge Storage Optimized with more storage, which is suited for large-scale data migrations and capacity-oriented workloads.
#### Snowball Edge Storage Optimized
Is the optimal choice if you need to securely and quickly transfer dozens of terabytes to petabytes of data to AWS. It is also a good fit for running general purpose analysis such as IoT data aggregation and transformation.

#### Snowball Edge Compute Optimized
Is the optimal choice if you need powerful compute and high-speed storage for data processing. Examples include high-resolution video processing, advanced IoT data analytics, and real-time optimization of machine learning models.

## AWS Snowmobile
Is the exabyte-scale data migration service that allows you to move very large datasets from on-premises to AWS.

## AWS Storage Gateway
A hybrid cloud storage between on-premises environments and the AWS Cloud . It is the service that enables your on-premises applications to seamlessly use AWS cloud storage.

# Configuration Management

## AWS CloudFormation
Allows you to use programming languages or a simple text file to model and provision, in an automated and secure manner, all the resources needed for your applications across all regions and accounts. Enables AWS architects to **manage infrastructure as code**

## AWS Config 
Is a fully managed service that provides you with an AWS resource inventory, configuration history, and configuration change notifications to enable security and governance. With AWS Config you can discover existing AWS resources, export a complete inventory of your AWS resources with all configuration details, and determine how a resource was configured at any point in time. These capabilities enable compliance auditing, security analysis, and resource change tracking.

## AWS OpsWorks
Is a configuration management service that provides managed instances of Chef and Puppet.Chef and Puppet are automation platforms that allow you to use code to automate the configurations of your servers.

## AWS Organizations
Provides central governance and management across multiple AWS accounts and has five main benefits:

1) Centrally manage access polices across multiple AWS accounts.

2) Automate AWS account creation and management.

3) Control access to AWS services.

4) Consolidate billing across multiple AWS accounts.

5) Configure AWS services across multiple accounts.
## AWS Systems Manager
Gives you visibility and control of your infrastructure on AWS. Systems Manager provides a unified user interface so you can view operational data from multiple AWS services and allows you to automate operational tasks across your AWS resources.

## AWS Quick Start Reference Deployments 
Outline the architectures for popular enterprise solutions on AWS and provide AWS CloudFormation templates to automate their deployment. Each Quick Start launches, configures, and runs the AWS compute, network, storage, and other services required to deploy a specific workload on AWS, using AWS best practices for security and availability.
         Quick Starts are built by AWS solutions architects and partners to help you deploy popular technologies on AWS, based on AWS best practices. These accelerators reduce hundreds of manual installation and configuration procedures into just a few steps, so you can build your production environment quickly and start using it immediately.
Used to deploy popular technologies - such as **IBM MQ** - on AWS with the least amount of effort and time

## AWS Artifact
Is a self-service audit artifact retrieval portal tat provides customers with on-demand access to AWS’ compliance documentation and AWS agreements. You can use AWS Artifact Agreements to review, accept, and track the status of AWS agreements such as the Business Associate Addendum (BAA).
You can also use AWS Artifact Reports to download AWS security and compliance documents, such as AWS ISO certifications, Payment Card Industry (PCI), and System and Organization Control (SOC) reports.

## AWS Certificate Manager
Is a service that lets you easily provision, manage, and deploy public and private Secure Sockets Layer/Transport Layer Security (SSL/TLS) certificates for use with AWS services and your internal connected resources

## AWS Secrets Manager
Is a secrets management service that enables you to store, retrieve, rotate, audit, and monitor secrets centrally. AWS Secrets Manager allows you to manage secrets such as database credentials, on-premises resource credentials, SaaS application credentials, third-party API keys, and Secure Shell (SSH) keys.

## AWS Global Accelerator and CloudFront
Are two separate services that use the AWS global network and its edge locations around the world. CloudFront improves performance for both cacheable (e.g., images and videos) and dynamic content (e.g. dynamic site delivery). Global Accelerator is a good fit for specific use cases, such as gaming, IoT or Voice over IP.

##  Amazon Route 53
Is a global service that provides highly available and scalable Domain Name System (DNS) services, domain name registration, and health-checking web services. It is designed to give developers and businesses an extremely reliable and cost effective way to route end users to Internet applications by translating names like example.com into the numeric IP addresses, such as 192.0.2.1, that computers use to connect to each other.

                Route 53 also simplifies the hybrid cloud by providing recursive DNS for your Amazon VPC and on-premises networks over AWS Direct Connect or AWS VPN.
## Amazon CloudFront
Is a fast content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to customers globally with low latency, high transfer speeds, all within a developer-friendly environment.

The use cases of Amazon CloudFront include:

- #### Accelerate static website content delivery.

CloudFront can speed up the delivery of your static content (for example, images, style sheets, JavaScript, and so on) to viewers across the globe. By using CloudFront, you can take advantage of the AWS backbone network and CloudFront edge servers to give your viewers a fast, safe, and reliable experience when they visit your website.

- #### Live & on-demand video streaming.
The Amazon CloudFront CDN offers multiple options for streaming your media – both pre-recorded files and live events – at sustained, high throughput required for 4K delivery to global viewers.

- #### Security.

CloudFront integrates seamlessly with AWS Shield for Layer 3/4 DDoS mitigation and AWS WAF for Layer 7 protection.

- #### Customizable content delivery with Lambda@Edge.

Lambda@Edge is a feature of Amazon CloudFront that lets you run code closer to users of your application, which improves performance and reduces latency.

## Amazon Kinesis Video Streams
Enables you to securely stream video from connected devices (IoT devices) to AWS for analytics, machine learning (ML), playback, and other processing. Kinesis Video Streams automatically provisions and elastically scales all the infrastructure needed to ingest streaming video data from millions of devices. It durably stores, encrypts, and indexes video data in your streams, and allows you to access your data through easy-to-use APIs.

## Amazon Simple Notification Service (SNS)
Is a fully managed pub/sub messaging service that enables you to decouple microservices, distributed systems, and serverless applications. Using Amazon SNS topics, your publisher systems can fan out messages to a large number of subscriber endpoints for parallel processing, including AWS Lambda functions, and HTTP/S webhooks. Additionally, SNS can be used to fan out notifications to end users using mobile push, SMS, and email.

## Amazon Simple Queue Service (SQS)
Is a fully managed message queuing service that enables you to send, store, and receive messages between software components at any volume, without losing messages or requiring other services to be available. SQS lets you decouple application components so that they run independently, increasing the overall fault tolerance of the system. Multiple copies of every message are stored redundantly across multiple availability zones so that they are available whenever needed.

##  Amazon SES (Amazon Simple Email Service) 
Is a flexible, affordable, and highly-scalable email messaging platform for businesses and developers.

# Shared Responsibility Model

## Shared Controls
Controls which apply to both the infrastructure layer and customer layers, but in completely separate contexts or perspectives. In a shared control, AWS provides the requirements for the infrastructure and the customer must provide their own control implementation within their use of AWS services.
- Patch Management – AWS is responsible for patching the underlying hosts and fixing flaws within the infrastructure, but customers are responsible for patching their guest OS and applications.

- Configuration Management – AWS maintains the configuration of its infrastructure devices, but a customer is responsible for configuring their own guest operating systems, databases, and applications.

- Awareness & Training - AWS trains AWS employees, but a customer must train their own employees.

