# Advantages of Cloud Computing include:  (IMPORTANT)

- Trade capital for variable expense: Instead of having to invest heavily in data centers and servers before you know how you’re going to use them, you can only pay when you consume computing resources, and only pay for how much you consume. By using AWS, infrastructure costs are converted to a pay-as-you-go model, where customers are charged for the resources that they consume, and those costs are incurred as operating costs instead of as capital expenditures.

- Benefit from massive economies of scale: By using cloud computing, you can achieve a lower variable cost than you can get on your own. Because usage from hundreds of thousands of customers are aggregated in the cloud, providers such as Amazon Web Services can achieve higher economies of scale which translates into lower pay as you go prices.

- Stop guessing capacity: Eliminate guessing on your infrastructure capacity needs. When you make a capacity decision prior to deploying an application, you often either end up sitting on expensive idle resources or dealing with limited capacity. With cloud computing, these problems go away. You can access as much or as little as you need, and scale up and down as required with only a few minutes notice.

- Increase speed and agility: In a cloud computing environment, new IT resources are only ever a click away, which means you reduce the time it takes to make those resources available to your developers from weeks to just minutes. This results in a dramatic increase in agility for the organization, since the cost and time it takes to experiment and develop is significantly lower.

- Stop spending money on running and maintaining data centers: Focus on projects that differentiate your business, not the infrastructure. Cloud computing lets you focus on your own customers, rather than on the heavy lifting of racking, stacking and powering servers.

- Go global in minutes: Easily deploy your application in multiple regions around the world with just a few clicks. This means you can provide a lower latency and better experience for your customers simply and at minimal cost.

## AWS Directory Service 
Is the service that provides single sign-on (SSO) to applications and services on AWS. AWS Directory Service uses secure Windows trusts to enable users to sign in to the AWS Management Console and the AWS Command Line Interface (CLI) using their existing corporate Microsoft Active Directory credentials.

## Amazon Cognito
Allows you to add user sign-up, sign-in, and access control to your web and mobile apps quickly and easily.

## AWS Management Console
The AWS Management Console allows you to access and manage Amazon Web Services through a simple and intuitive web-based user interface. You can only access the AWS management console if you have a valid user name and password.

##  The AWS Command Line Interface (CLI)
Is a unified tool to manage your AWS services. With just one tool to download and configure, you can control multiple AWS services from the command line and automate them through scripts.  

## The AWS Software Development Kit (AWS SDK) 
Can simplify using AWS services in your applications with an API tailored to your programming language or platform. Programming languages supported include Java, .NET, Node.js, PHP, Python, Ruby, Go, and C++.

# General 
- A computer on which AWS runs one or more virtual machines is called a host machine, and each virtual machine is called a guest machine. AWS drives the concept of virtualization by allowing the physical host machine to operate multiple virtual machines as guests (for multiple customers) to help maximize the effective use of computing resources such as memory, network bandwidth and CPU cycles.


- Amazon Web Services (AWS) allows customers to assign metadata to their AWS resources in the form of tags. Each tag is a simple label consisting of a customer-defined key and an optional value that can make it easier to manage, search for, and filter resources. Although there are no inherent types of tags, they enable customers to categorize resources by purpose, owner, environment, or other criteria. An effective tagging strategy will give you improved visibility and monitoring, help you create accurate chargeback/showback models, and get more granular and precise insights into usage and spend by applications and teams.


- Data sovereignty is the concept that information which has been converted and stored in binary digital form is subject to the laws of the country in which it is located. Data sovereignty is a factor you should consider when choosing your AWS region


- AWS Serverless Services include:

**Compute**: AWS Lambda, AWS Fargate

**Messaging**: Amazon SNS, Amazon SQS

**Database**: Amazon DynamoDB, Amazon Aurora Serverless

**Orchestration**: AWS Step Functions

## A pilot light scenario 
Is a disaster recover / business continuity scenario wherein a minimal amount of services are kept running in a failover location to enable the business to meet their Recovery Time Objective (RTO) and Recovery Point Objective (RPO) in the event of a disaster. By nature, a pilot light scenario will take some time to spin up and promote to production (as opposed to an active-active DR scenario) and will therefore not mitigate the per-minute losses that will be experienced by the company in the event of an outage.
Additional information: Recovery time objective (RTO) and recovery point objective (RPO) are two key metrics to consider when developing a disaster recover (DR) plan. RTO represents how many hours it takes customers to return to a working state after a disaster. RPO, which is also expressed in hours, represents how much data customers could lose when a disaster happens. For example, an RPO of 1 hour means that customers could lose up to 1 hour’s worth of data when a disaster occurs.

## Infrastructure as a Service (IaaS)
Contains the basic building blocks for Cloud IT and typically provide access to networking features, computers (virtual or on dedicated hardware), and data storage space. Infrastructure as a Service provides you with the highest level of flexibility and management control over your IT resources and is most similar to existing IT resources that many IT departments and developers are familiar with today.

## Platform as a Service (PaaS)
Removes the need for your organization to manage the underlying infrastructure (usually hardware and operating systems) and allows you to focus on the deployment and management of your applications. This helps you be more efficient as you don’t need to worry about resource procurement, capacity planning, software maintenance, patching, or any of the other undifferentiated heavy lifting involved in running your application. A common example of a PaaS platform is the AWS Elastic Beanstalk service. Developers simply upload their application, and Elastic Beanstalk automatically handles the deployment details of capacity provisioning, load balancing, auto-scaling, and application health monitoring.

##  Software as a Service(SaaS)
provides you with a completed product that is run and managed by the service provider. In most cases, people referring to Software as a Service are referring to end-user applications. With a SaaS offering you do not have to think about how the service is maintained or how the underlying infrastructure is managed; you only need to think about how you will use that particular piece software. A common example of a SaaS application is web-based email where you can send and receive email without having to manage feature additions to the email product or maintaining the servers and operating systems that the email program is running on. 

## AWS Auto Scaling
Is the feature that automates the process of adding/removing server capacity (based on demand). Autoscaling allows you to reduce your costs by automatically turning off resources that aren’t in use. On the other hand, Autoscaling ensures that your application runs effectively by provisioning more server capacity if required.

## Horizontal Scaling
Scaling horizontally takes place through an increase in the number of resources (e.g., adding more hard drives to a storage array or adding more servers to support an application). This is a great way to build Internet-scale applications that leverage the elasticity of cloud computing.

## Vertical Scaling:
Scaling vertically takes place through an increase in the specifications of an individual resource (e.g., upgrading a server with a larger hard drive, adding more memory, or provisioning a faster CPU). On Amazon EC2, this can easily be achieved by stopping an instance and resizing it to an instance type that has more RAM, CPU, I/O,or networking capabilities. This way of scaling can eventually hit a limit and it is not always a cost efficient or highly available approach. However, it is very easy to implement and can be sufficient for many use cases especially as a short term solution.

Vertical-scaling is often limited to the capacity constraints of a single machine, scaling beyond that capacity often involves downtime and comes with an upper limit. With horizontal-scaling it is often easier to scale dynamically by adding more machines in parallel. Hence, in most cases, horizontal-scaling is recommended over vertical-scaling.

## AWS Elastic Load Balancer (ELB) 
Is a service that distributes the incoming application traffic to multiple targets that you define.
- Application Load Balancer (Http and https) More intteligent
- Network Load Balancer(TCP/TLS) More faster
- Classic Load Balancer Not used now.
- Gateway Load Balancer

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
 
##  AWS X-Ray
Is a debugging service that helps developers understand how their application and its underlying services are performing to identify and troubleshoot the root cause of performance issues and errors.
AWS X-Ray helps developers analyze and debug distributed applications in production or under development, such as those built using microservice architecture. With X-Ray, you can understand how your application and its underlying services are performing so you can identify and troubleshoot the root cause of performance issues and errors. X-Ray provides an end-to-end view of requests as they travel through your application, and shows a map of your application’s underlying components. You can use X-Ray to analyze both applications in development and in production, from simple three-tier applications to complex microservices applications consisting of thousands of services. 

## The AWS Well-Architected Framework
The 5 Pillars of the AWS Well-Architected Framework:

- Operational Excellence: The operational excellence pillar includes the ability to run and monitor systems to deliver business value and to continually improve supporting processes and procedures.

- Security: The security pillar includes the ability to protect information, systems, and assets while delivering business value through risk assessments and mitigation strategies.

- Reliability: The reliability pillar includes the ability of a system to recover from infrastructure or service disruptions, dynamically acquire computing resources to meet demand, and mitigate disruptions such as  misconfigurations or transient network issues.

- Performance Efficiency: The performance efficiency pillar includes the ability to use computing resources efficiently to meet system requirements. Key topics include selecting the right resource types and sizes based on workload requirements, monitoring performance, and making informed decisions to maintain efficiency as business needs evolve.

- Cost Optimization: The cost optimization pillar includes the ability to avoid or eliminate unneeded cost or sub-optimal resources.



## AWS Trusted Advisor 
Offers a rich set of best practice checks and recommendations across five categories: cost optimization; security; fault tolerance; performance; and service limits(Service limits, also referred to as Service quotas, are the maximum number of service resources or operations that apply to an AWS account. Understanding your service limits (and how close you are to them) is an important part of managing your AWS deployments – continuous monitoring allows you to request limit increases or shut down resources before the limit is reached. One of the easiest ways to do this is via AWS Trusted Advisor’s Service Limit Dashboard). Like your customized cloud security expert, AWS Trusted Advisor analyzes your AWS environment and provides security recommendations to protect your AWS environment. The service improves the security of your applications by closing gaps, examining permissions, and enabling various AWS security features.
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

## AWS Professional Services organization
Is a global team of experts that helps customers realize their desired business outcomes when using AWS.

## AWS Customer Service
The AWS Customer Service team is at the forefront of this transformational technology assisting a global list of customers that are taking advantage of a growing set of services and features to run their mission-critical applications. The team helps AWS customers understand what Cloud Computing is all about, and whether it can be useful for their business needs.
Can help AWS customers with their billing and account inquiries, and it is included in all AWS support plans (Basic, Developer, Business, and Enterprise). However, due to the fact that AWS Customer Service is not dedicated to specific types of inquiries, it is not as quick or as **efficient as the AWS Support Concierge**.

"AWS Operations Support" is incorrect. AWS Operations Support is an Enterprise support program that provides operations assessments and analysis to identify gaps across the operations lifecycle, as well as recommendations based on best practices.

## Operations Support
Included with the Enterprise support plan, Operations Support provides consultative reviews of your AWS operations and advice for optimization. 

## The AWS Support API 
Provides programmatic access to AWS Support Center features to create, manage, and close support cases, and operationally manage Trusted Advisor check requests and status. AWS Support API is available only for AWS  customers who have a Business or Enterprise support plan.
The service currently provides two different groups of operations:
1- Support Case Management operations to manage the entire life cycle of AWS support cases, from creating a case to resolving it.
2- Trusted Advisor operations to access the checks provided by AWS Trusted Advisor.

## AWS Application Discovery Service
Helps enterprise customers plan migration projects by gathering information about their on-premises data centers.

## AWS Infrastructure Event Management
Is a short-term engagement with AWS Support, included in the Enterprise-level Support product offering, and available for additional purchase for Business-level Support subscribers. AWS Infrastructure Event Management partners with your technical and project resources to gain a deep understanding of your use case and provide architectural and scaling guidance for an event. Common use-case examples for AWS Event Management include advertising launches, new product launches, and infrastructure migrations to AWS.

## AWS Managed Services (AMS) service.
AMS is an AWS service that operates AWS on behalf of enterprise customers and partners. Enterprises want to adopt AWS at scale but often the skills that have served them well in traditional IT do not always translate to success in the cloud. AWS Managed Services (AMS) enables them to migrate to AWS at scale more quickly, reduce their operating costs, improve security and compliance and focus on their differentiating business priorities.

##  APN Consulting Partners 
Are professional services firms that help customers design, architect, build, migrate, and manage their workloads and applications on AWS. Consulting Partners include System Integrators, Strategic Consultancies, Agencies, Managed Service Providers, and Value-Added Resellers. AWS supports the APN Consulting Partners by providing a wide range of resources and training to support their customers.

## APN Technology Partners
Provide software solutions that are either hosted on, or integrated with, the AWS platform. APN Technology Partners include Independent Software Vendors (ISVs), SaaS, PaaS, Developer Tools, Management and Security Vendors.

## A Technical Account Manager (TAM) 
Is your designated technical point of contact who provides advocacy and guidance to help plan and build solutions using best practices and proactively keep your AWS environment operationally healthy. TAM is available only for the Enterprise support plan.

## AWS Server Migration Service (SMS)
Is used to migrate your on-premises workloads to AWS.

## AWS Database Migration Service (DMS)
Helps you migrate databases to AWS easily and securely. The source database remains fully operational during the migration, minimizing downtime to applications that rely on the database. The AWS Database Migration Service can migrate your data to and from most widely used commercial and open-source databases. The service supports homogeneous migrations such as Oracle to Oracle, as well as heterogeneous migrations between different database platforms, such as Oracle to Amazon Aurora or Microsoft SQL Server to MySQL. It also allows you to stream data to Amazon Redshift from any of the supported sources including Amazon Aurora, PostgreSQL, MySQL, MariaDB, Oracle, SAP ASE, and SQL Server, enabling consolidation and easy analysis of data in the petabyte-scale data warehouse. AWS Database Migration Service can also be used for continuous data replication with high availability.   

# Database

## Amazon DynamoDB
Is a NoSQL database service.
DynamoDB is serverless with no servers to provision, patch, or manage and no software to install, maintain, or operate. DynamoDB automatically scales tables up and down to adjust for capacity and maintain performance. Availability and fault tolerance are built in, eliminating the need to architect your applications for these capabilities.
**DAX is a caching feature for use with Amazon DynamoDB**

## Amazon Neptune
Is a graph database service, not a MySQL database service. Amazon Neptune is used to build and run applications that work with highly connected datasets, such as social networking, recommendation engines, and knowledge graphs.

## RDS
use Amazon Elastic Block Store (Amazon EBS) volumes for database and log storage.

## Amazon Aurora
Is a MySQL and PostgreSQL-compatible relational database built for the cloud. Amazon Aurora combines the performance and availability of traditional enterprise databases with the simplicity and cost-effectiveness of open source databases. It delivers up to five times the throughput of standard MySQL and up to three times the throughput of standard PostgreSQL. Amazon Aurora is designed to be compatible with MySQL and with PostgreSQL, so that existing applications and tools can run without requiring modification. It is available through Amazon Relational Database Service (RDS), freeing you from time-consuming administrative tasks such as provisioning, patching, backup, recovery, failure detection, and repair.

## Amazon Redshift 
Is a fully managed data warehouse service that allows you to run complex analytic queries against petabytes of structured data using standard SQL and your existing Business Intelligence (BI) tools.

## Amazon Athena 
Is an interactive query service that is mainly used to analyze data in Amazon S3 using standard SQL.

## Amazon ElastiCache
Is a web service that makes it easy to deploy, operate, and scale an in-memory data store or cache in the cloud. The service improves the performance of web applications by allowing you to retrieve information from fast, managed, in-memory data stores, instead of relying entirely on slower disk-based databases.
The primary purpose of an in-memory data store is to provide ultrafast (submillisecond latency) and inexpensive access to copies of data. Querying a database is always slower and more expensive than locating a copy of that data in a cache. Some database queries are especially expensive to perform. An example is queries that involve joins across multiple tables or queries with intensive calculations. By caching (storing) such query results, you pay the price of the query only once. Then you can quickly retrieve the data multiple times without having to re-execute the query.
ElastiCache supports only two cache engines: **Redis and Memcached**.

## Amazon EMR
Launches clusters in minutes. You don’t need to worry about node provisioning, infrastructure setup, Hadoop configuration, or cluster tuning. Amazon EMR takes care of these tasks so you can focus on analysis.

## AWS Key Management Service (AWS KMS) 
AWS KMS a managed service provides a highly available key storage, management, and auditing solution for you to encrypt data within your own applications and control the encryption of stored data across AWS services. This is multi tenant

## AWS CloudHSM
Is a cloud-based hardware security module (HSM) that enables you to easily generate and use your own encryption keys on the AWS Cloud. This is single tenant KMS.

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

**IAM roles with temporary credentials are useful in the following situations:**

**Applications running on Amazon EC2:** You can use an IAM role to manage temporary credentials for applications running on an EC2 instance and make AWS CLI or AWS API requests. This is more secure than storing access keys within the EC2 instance.

**Federated user access:** Instead of creating an IAM user, you can use existing identities from AWS Directory Service, your enterprise user directory, or a web identity provider. These are known as federated users. AWS assigns a role to a federated user when access is requested through an identity provider.

**AWS service access:** A service role is an IAM role that a service assumes to perform actions on your behalf. An IAM administrator can create, modify, and delete a service role from within IAM.

## IAM policies
Let you allow or deny access to AWS services (such as Amazon S3), individual AWS resources (such as a specific S3 bucket), or individual API actions (such as s3:CreateBucket). An IAM policy can be applied only to IAM users, groups, or roles, and it can never restrict the root identity of the AWS account (The AWS root account).

## If you suspect that your account has been compromised, or if you have received a notification from AWS that the account has been compromised, perform the following tasks: 

- Change your AWS root account password and the passwords of all IAM users. 
- Delete or rotate all root and AWS Identity and Access Management (IAM) access keys.
- Delete any potentially compromised IAM users.
- Delete any resources on your account you didn’t create, such as EC2 instances and AMIs, EBS volumes and snapshots, and IAM users. 
- Respond to any notifications you received from AWS Support through the AWS Support Center. 

## AWS WAF (Web Application Firewall)
Helps protect your web applications from common web exploits that could affect application availability, compromise security, or consume excessive resources. You can use AWS WAF to create custom rules that block common attack patterns, such as SQL injection or cross-site scripting, and rules that are designed for your specific application.

## ![image](https://user-images.githubusercontent.com/43753503/147520243-517a10ac-8a13-4ce9-bc1d-8fbce760963c.png)

## AWS Shield
AWS provides flexible infrastructure and services that help customers implement strong DDoS mitigations and create highly available application architectures that follow AWS Best Practices for DDoS Resiliency. These include services such as Amazon Route 53, Amazon CloudFront, Elastic Load Balancing, and AWS WAF to control and absorb traffic, and deflect unwanted requests. These services integrate with AWS Shield, a managed DDoS protection service that provides always-on detection and automatic inline mitigations to safeguard web applications running on AWS.

## The VPC Flow logs
Feature does not filter traffic. You can use security groups to filter traffic at the instance level and Network ACLs to filter traffic at the subnet level. VPC Flow logs only capture information about the IP traffic going to and from network interfaces in your VPC. This information can help you monitor the traffic that is reaching your instances and diagnose overly restrictive or overly permissive security group and network ACL rules.
AWS customers use VPC Flow logs to troubleshoot connectivity and security issues and make sure that network access rules are working as expected.

## Amazon Inspector
Is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. Amazon Inspector automatically assesses applications for vulnerabilities or deviations from best practices. After performing an assessment, Amazon Inspector produces a detailed list of security findings prioritized by level of severity. These findings can be reviewed directly or as part of a detailed assessment report which is available via the Amazon Inspector console or API. To help get started quickly, Amazon Inspector includes a knowledge base of hundreds of rules mapped to common security best practices and vulnerability definitions. Examples of built-in rules include checking for remote root login being enabled, or vulnerable software versions installed. These rules are regularly updated by AWS security researchers.

## Amazon GuardDuty
Is a threat detection service that continuously monitors for malicious activity and unauthorized behavior to protect your AWS accounts and workloads.
With the cloud, the collection and aggregation of account and network activities is simplified, but it can be time consuming for security teams to continuously analyze event log data for potential threats. GuardDuty analyzes tens of billions of events across multiple AWS data sources, such as AWS CloudTrail, Amazon VPC Flow Logs, and DNS logs. With GuardDuty, you now have an intelligent and cost-effective option for continuous threat detection in the AWS Cloud. The service uses machine learning, anomaly detection, and integrated threat intelligence to identify and prioritize potential threats.

## Amazon Detective 
Is a security service that makes it easy to analyze, investigate, and quickly identify the root cause of potential security issues or suspicious activities.


**How does Amazon Detective differ from Amazon GuardDuty?**

Amazon GuardDuty is helpful in alerting you when something is wrong and pointing out where to go to fix it. But sometimes, there might be a security finding where you need to dig a lot deeper and analyze more information to isolate the root cause and take action.

Amazon Detective simplifies this process by enabling you to easily investigate and quickly get to the root cause of a security finding. Amazon Detective analyzes trillions of events from multiple data sources such as Virtual Private Cloud (VPC) Flow Logs, AWS CloudTrail logs, and automatically creates a unified view of user and resource interactions over time, with all the context and details in one place to help you quickly analyze and get to the root cause of a security finding.

For example, an Amazon GuardDuty finding, like an unusual Console Login API call, can be quickly investigated in Amazon Detective with details about the API call trends over time, and user login attempts on a geolocation map. These details enable you to quickly identify if you think it is legitimate or an indication of a compromised AWS resource.

##  AWS Macie
 A fully managed security service which helps protect your sensitive data in Amazon S3. Amazon Macie uses machine learning to automatically discover, classify, and protect sensitive data in Amazon S3. Amazon Macie recognizes sensitive data such as personally identifiable information (PII) or intellectual property, and provides you with dashboards and alerts that give visibility into how this data is being accessed or moved. The fully managed service continuously monitors data access activity for anomalies, and generates detailed alerts when it detects risk of unauthorized access or inadvertent data leaks. Today, Amazon Macie is available to protect data stored in Amazon S3, with support for additional AWS data stores coming later this year.

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
» EC2 instance pricing varies depending on many variables:

- The buying option (On-demand, Savings Plans, Reserved, Spot, Dedicated)

- Selected instance type

- Selected Region

- Number of instances

- Load balancing

- Allocated Elastic IP Addresses
» With Amazon EC2 on-demand instances, you only pay for the compute capacity you consume, and once you stop using them, there are no additional costs or termination fees.
» With On-Demand instances, you pay for compute capacity by the hour or the second depending on which instances you run. No longer-term commitments or upfront payments are needed.
» With per-second billing, you pay for only what you use. It takes cost of unused minutes and seconds in an hour off of the bill, so you can focus on improving your applications instead of maximizing usage to the hour. Especially, if you manage instances running for irregular periods of time, such as dev/testing, data processing, analytics, batch processing and gaming applications, can benefit.
» Per-second billing is available for instances launched in:
- On-Demand, Reserved and Spot forms
- All regions and Availability Zones
- Amazon Linux, Windows and Ubuntu

#### Dedicated hosts supports the Bring Your Own License (BYOL) model for almost every BYOL scenario

#### Spot instances
Provide a discount (up to 90%) off the On-Demand price. The Spot price is determined by long-term trends in supply and demand for EC2 spare capacity. If the Spot price exceeds the maximum price you specify for a given instance or if capacity is no longer available, your instance will automatically be interrupted.
         Spot Instances are a cost-effective choice if you can be flexible about when your applications run and if you don't mind if your applications get interrupted. For example, Spot Instances are well-suited for data analysis, batch jobs, background processing, and optional tasks. 

####  Dedicated instances
Are used when you need your instances to be physically isolated at the host hardware level from instances that belong to other AWS accounts. Dedicated instances are significantly more expensive than Spot Instances.Dedicated Hosts provide you with EC2 instance capacity on physical servers dedicated to your use. You may need to migrate your applications to a dedicated host to use your eligible software licenses from vendors such as Microsoft and Oracle on Amazon EC2 so that you get the flexibility and cost-effectiveness of using your own licenses, but with the resiliency, simplicity, and elasticity of AWS. Amazon EC2 Dedicated Hosts can also help address corporate compliance requirements because they are dedicated only to a single customer.

####  Reserved instances
Are recommended for Customers that can commit to using EC2 over a 1 or 3-year term to reduce their total computing costs. Even if the project will last for more than a year, the cost-benefit for acquiring Reserved Instances is not as great as the cost-benefit from using Spot Instances. The Spot option provides the largest discount (up to 90%).

- Convertible Reserved Instances
You can exchange one or more Reserved Instances for another Reserved Instance with a different configuration, including instance family, operating system, and tenancy. There are no limits to how many times you perform an exchange, as long as the new Convertible Reserved Instance is of an equal or higher value than the original Convertible Reserved Instances that you are exchanging.

- Standard Reserved Instances
Can't modify them. You can modify attributes such as the Availability Zone, instance size (within the same instance family), and scope of your Reserved Instance (regional or zonal). Standard RIs provide the most significant discount (up to 72% off On-Demand) and are best suited for steady-state usage.
####   Savings Plans
are a flexible pricing model that offers low prices on EC2, Lambda, and Fargate usage, in exchange for a commitment to a consistent amount of usage (measured in $/hour) for a 1 or 3 year term. When you sign up for Savings Plans, you will be charged the discounted Savings Plans price for your usage up to your commitment. For example, if you commit to $10 of compute usage an hour, you will get the Savings Plans prices on that usage up to $10 and any usage beyond the commitment will be charged On Demand rates.

## "Disk disposal" ( Storage Device Decommissioning)
When a storage device has reached the end of its useful life, AWS procedures include a decommissioning process that is designed to prevent customer data from being exposed to unauthorized individuals. All decommissioned magnetic storage devices are degaussed and physically destroyed in accordance with industry-standard practices.

# Storage

## Amazon EC2 Instance Store
Provides temporary block-level storage for your instance. Instance store is ideal for temporary storage of information that changes frequently, such as buffers, caches, scratch data, and other temporary content, or for data that is replicated across a fleet of instances, such as a load-balanced pool of web servers.

## EBS
Amazon EBS is a block level storage that provides storage volumes for use with Amazon EC2 and Amazon RDS. 
Creating snapshots of EBS Volumes can help ensure that you have a backup of your EBS volumes just in case any issues arise.
 EBS Snapshots are incremental backups, which means that only the blocks on the device that have changed after your last snapshot are saved. This minimizes the time required to create the snapshot and saves on storage costs by not duplicating data.
 Amazon EBS encryption offers a straight-forward encryption solution for your EBS resources that doesn't require you to build, maintain, and secure your own key management infrastructure. Encryption operations occur on the servers that host EC2 instances, ensuring the security of both data-at-rest and data-in-transit between an instance and its attached EBS storage.
Amazon EBS volume **data is replicated** across multiple servers within the **same Availability Zone**.

## Amazon EFS 
Amazon Elastic File System (Amazon EFS) provides simple, scalable, elastic file storage for use with AWS Cloud services and on-premises resources. It is easy to use and offers a simple interface that allows you to create and configure file systems quickly and easily. Amazon EFS is built to elastically scale on demand without disrupting applications, growing and shrinking automatically as you add and remove files, so your applications have the storage they need, when they need it. It is designed to provide massively parallel shared access to thousands of Amazon EC2 instances, enabling your applications to achieve high levels of aggregate throughput and IOPS that scale as a file system grows, with consistent low latencies. As a regional service, Amazon EFS is designed for high availability and durability storing data redundantly across multiple Availability Zones.
Data is redundantly stored across multiple Availability Zones providing better durability compared to EBS volumes.

## Amazon S3
Stores any number of objects, but each object does have a size limitation. Individual Amazon S3 objects can range in size from a minimum of 0 bytes to a maximum of 5 terabytes.
- S3 Standard offers high durability, availability, and performance object storage for frequently accessed data.

- Amazon S3 Standard-Infrequent Access (S3 Standard-IA) is for data that is accessed less frequently, but requires rapid access when needed.

- S3 Intelligent-Tiering storage class is designed to optimize costs by automatically moving data to the most cost-effective access tier, without performance impact or operational overhead. It works by storing objects in two access tiers: one tier that is optimized for frequent access and another lower-cost tier that is optimized for infrequent access. For a small monthly monitoring and automation fee per object, Amazon S3 monitors access patterns of the objects in S3 Intelligent-Tiering, and moves the ones that have not been accessed for 30 consecutive days to the infrequent access tier. If an object in the infrequent access tier is accessed, it is automatically moved back to the frequent access tier. There are no retrieval fees when using the S3 Intelligent-Tiering storage class, and no additional tiering fees when objects are moved between access tiers. It is the ideal storage class for long-lived data with access patterns that are unknown or unpredictable.

-  S3 One Zone-Infrequent Access (S3 One Zone-IA) for long-lived, but less frequently accessed data

- Amazon S3 Glacier is a low-cost storage class for data that is rarely accessed; such as archived data.

- Amazon S3 Glacier Deep Archive is an extremely low-cost storage service that provides secure, durable, and flexible storage for long-term data backup and archival. With Amazon S3 Glacier Deep Archive, customers can reliably store their data for as little as $1 per terabyte per month, a significant savings compared to on-premises solutions. Amazon Glacier enables customers to offload the administrative burdens of operating and scaling storage to AWS, so that they don’t have to worry about capacity planning, hardware provisioning, data replication, hardware failure detection and repair, or time-consuming hardware migrations.

Choosing between S3 Glacier and S3 Glacier Deep Archive depends on how quickly you must retrieve your data. With S3 Glacier, you can retrieve your data within a few minutes to several hours (1-5 minutes to 12 hours), whereas with S3 Glacier Deep Archive, the minimum retrieval period is 12 hours.
     
#### Amazon S3 provides a number of security features for the protection of data at rest, which you can use or not depending on your threat profile:

- Permissions: Use bucket-level or object-level permissions alongside IAM policies to protect resources from unauthorized access and to prevent information disclosure, data integrity compromise or deletion.

- Versioning: Amazon S3 supports object versions. Versioning is disabled by default. Enable versioning to store a new version for every modified or deleted object from which you can restore compromised objects if necessary.

- Replication: Although Amazon S3 stores your data across multiple geographically diverse Availability Zones by default, compliance requirements might dictate that you store data at even greater distances. Cross-region replication (CRR) allows you to replicate data between distant AWS Regions to help satisfy these requirements. CRR enables automatic, asynchronous copying of objects across buckets in different AWS Regions.

- Encryption – server side: Amazon S3 supports server-side encryption of user data. Server-side encryption is transparent to the end user. AWS generates a unique encryption key for each object, and then encrypts the object using AES-256.

- Encryption – client side: With client-side encryption you create and manage your own encryption keys. Keys you create are not exported to AWS in clear text. Your applications encrypt data before submitting it to Amazon S3, and decrypt data after receiving it from Amazon S3. Data is stored in an encrypted form, with keys and algorithms only known to you.

##   Amazon S3 Transfer Acceleration
Enables fast, easy, and secure transfers of files over long distances between your client and an S3 bucket. Transfer Acceleration takes advantage of Amazon CloudFront’s globally distributed edge locations. As the data arrives at an edge location, data is routed to Amazon S3 over an optimized network path.

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

## AWS Data Pipeline
Is a web service that helps customers reliably process and move data between different AWS compute and storage services, as well as on-premises data sources.

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

#### AWS Service Control Policies (or AWS Organizations Policies) are a type of organization policy that you can use to manage permissions for all accounts in your organization. SCPs offer central control over the maximum available permissions for all member accounts in your organization. SCPs help you to ensure member accounts stay within your organization's access control guidelines. In SCPs, you can restrict which AWS services, resources, and individual API actions the users and roles in each member account can access. When AWS Organizations blocks access to a service, resource, or API action for a member account, a user or role in that account cannot access it. This block remains in effect even if an administrator of a member account explicitly grants such permissions in an IAM policy.

##  Amazon Cloud Directory
Is a cloud-native, highly scalable, high-performance directory service that provides web-based directories to make it easy for you to organize and manage all your application resources such as users, groups, locations, devices, and policies, and the rich relationships between them.

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

##  Amazon Route 53
Is a global service that provides highly available and scalable Domain Name System (DNS) services, domain name registration, and health-checking web services. It is designed to give developers and businesses an extremely reliable and cost effective way to route end users to Internet applications by translating names like example.com into the numeric IP addresses, such as 192.0.2.1, that computers use to connect to each other.
Route 53 also simplifies the hybrid cloud by providing recursive DNS for your Amazon VPC and on-premises networks over **AWS Direct Connect or AWS VPN**.

## An internet gateway
Is a VPC component that allows communication between your VPC and the internet.

## AWS Outposts
Is an AWS service that delivers the same AWS infrastructure, native AWS services, APIs, and tools to virtually any customer on-premises facility. With AWS Outposts, customers can run AWS services locally on their Outpost, including EC2, EBS, ECS, EKS, and RDS, and also have full access to services available in the Region.
Customers can use AWS Outposts to securely store and process data that needs to remain on-premises or in countries where there is no AWS region. AWS Outposts is ideal for applications that have low latency or local data processing requirements, such as financial services, healthcare, etc.


## AWS Global Accelerator and CloudFront
Are two separate services that use the AWS global network and its edge locations around the world. CloudFront improves performance for both cacheable (e.g., images and videos) and dynamic content (e.g. dynamic site delivery). Global Accelerator is a good fit for specific use cases, such as gaming, IoT or Voice over IP.

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

## AWS Batch
Is a compute service that allows you to run hundreds of thousands of batch computing jobs on AWS. AWS Batch dynamically provisions the optimal quantity and type of compute resources (e.g., CPU or memory optimized instances) based on the volume and specific resource requirements of the batch jobs submitted.

## Aws CodePipeline
Is a fully managed continuous delivery service that helps you automate your release pipelines for fast and reliable application and infrastructure updates.

## AWS CodeCommit
Is a source code control service that hosts secure Git-based repositories. AWS CodeCommit is designed for software developers who need a secure, reliable, and scalable source control system to store and version their code.

## AWS CodeDeploy
Is a deployment service that automates application deployments to Amazon EC2 instances, on-premises instances, serverless Lambda functions, or Amazon ECS services.

## Amazon Lightsail
Amazon Lightsail provides a low-cost Virtual Private Server (VPS) in the cloud.Lightsail plans include everything you need to jumpstart your project – virtual machines, containers, databases, CDN, load balancers, SSD-based storage, DNS management, etc. – for a low, predictable monthly price.

## Amazon Comprehend
is a Natural Language Processing (NLP) service that uses machine learning to find meaning and insights in text. Customers can use Amazon Comprehend to identify the language of the text, extract key phrases, places, people, brands, or events, understand sentiment about products or services, and identify the main topics from a library of documents. The source of this text could be web pages, social media feeds, emails, or articles. Amazon Comprehend is fully managed, so there are no servers to provision, and no machine learning models to build, train, or deploy.

## Amazon QuickSight 
Is a serverless, machine learning-powered business intelligence (BI) service built for the cloud. QuickSight lets you easily create and publish interactive BI dashboards that include Machine Learning-powered insights. QuickSight dashboards can be accessed from any device, and seamlessly embedded into your applications, portals, and websites.
Unlike traditional BI or data discovery solutions, getting started with Amazon QuickSight is simple and fast. When you log in, Amazon QuickSight seamlessly discovers your data sources in AWS services such as Amazon Redshift, Amazon RDS, Amazon Athena, and Amazon Simple Storage Service (Amazon S3). You can connect to any of the data sources discovered by Amazon QuickSight and get insights from this data in minutes. Amazon QuickSight supports rich data discovery and business analytics capabilities to help customers derive valuable insights from their data without worrying about provisioning or managing infrastructure.

## Amazon Personalize
Is a fully managed machine learning service that can be used to deliver highly customized recommendations to customers across industries such as retail, media and entertainment. Amazon Personalize enables developers to build applications with the same machine learning (ML) technology used by Amazon.com for real-time personalized recommendations. Amazon Personalize can be used to personalize the end-user experience over any digital channel. Examples include product recommendations for e-commerce, news articles and content recommendation for publishing, media and social networks, hotel recommendations for travel websites, and credit card recommendations for banks.

## AWS Cloud9 
Is a cloud-based integrated development environment (IDE) that lets you write, run, and debug your code with just a browser. It includes a code editor, debugger, and terminal. Cloud9 comes prepackaged with essential tools for popular programming languages, including JavaScript, Python, PHP, and more, so you don’t need to install files or configure your development machine to start new projects.

## WS Elastic Beanstalk 
Is an application container on top  of Amazon Web Services. Elastic Beanstalk makes it easy for developers to quickly deploy and manage applications in the AWS Cloud. Developers simply upload their application code, and Elastic Beanstalk automatically handles the deployment details of capacity provisioning, load balancing, auto-scaling, and application health monitoring.

## AWS Amplify 
Is used for building secure and scalable web and mobile applications, not deploying applications.

## AWS Glue
Is a fully-managed, Extract, Transform, and Load (ETL) service that automates the time-consuming steps of data preparation for analytics.
Extract, Transform, and Load (ETL) is the process of extracting (collecting) data from various sources (from different databases for example), transform the data depending on business rules/needs (This step helps in preparing the data for analytics and decision making) and load the data into a destination database, often a data warehouse.

##  Amazon Chime
Is a communications service for online meetings.

## Amazon Rekognition 
Is a service that makes it easy to add image analysis to your applications. With Rekognition, you can detect objects, scenes, and faces in images. You can also search and compare faces. The Amazon Rekognition API enables you to quickly add sophisticated deep-learning-based visual search and image classification to your applications.

##  Amazon Polly 
Is a service that turns text into lifelike speech.

## Amazon Kinesis Video Streams
Enables you to securely stream video from connected devices (IoT devices) to AWS for analytics, machine learning (ML), playback, and other processing. Kinesis Video Streams automatically provisions and elastically scales all the infrastructure needed to ingest streaming video data from millions of devices. It durably stores, encrypts, and indexes video data in your streams, and allows you to access your data through easy-to-use APIs.

## Amazon EventBridge (also called Amazon CloudWatch Events)
Amazon EventBridge is a serverless event bus service that  makes it easy for you to build event-driven application architectures. Amazon EventBridge helps you accelerate modernizing and re-orchestrating your architecture with decoupled services and applications. With EventBridge, you can speed up your organization’s development process by allowing teams to iterate on features without explicit dependencies between systems.

## Amazon Simple Notification Service (SNS)
Is a fully managed pub/sub messaging service that enables you to decouple microservices, distributed systems, and serverless applications. Using Amazon SNS topics, your publisher systems can fan out messages to a large number of subscriber endpoints for parallel processing, including AWS Lambda functions, and HTTP/S webhooks. Additionally, SNS can be used to fan out notifications to end users using mobile push, SMS, and email.

## Amazon Simple Queue Service (SQS)
Is a fully managed message queuing service that enables you to send, store, and receive messages between software components at any volume, without losing messages or requiring other services to be available. SQS lets you decouple application components so that they run independently, increasing the overall fault tolerance of the system. Multiple copies of every message are stored redundantly across multiple availability zones so that they are available whenever needed.

## AWS Fargate 
Is a compute engine for Amazon Elastic Container Service (ECS) that allows customers to run containers without having to manage servers or clusters.

##  Amazon SES (Amazon Simple Email Service) 
Is a flexible, affordable, and highly-scalable email messaging platform for businesses and developers.

# Shared Responsibility Model

## Shared Controls
Controls which apply to both the infrastructure layer and customer layers, but in completely separate contexts or perspectives. In a shared control, AWS provides the requirements for the infrastructure and the customer must provide their own control implementation within their use of AWS services.
- Patch Management – AWS is responsible for patching the underlying hosts and fixing flaws within the infrastructure, but customers are responsible for patching their guest OS and applications.

- Configuration Management – AWS maintains the configuration of its infrastructure devices, but a customer is responsible for configuring their own guest operating systems, databases, and applications.

- Awareness & Training - AWS trains AWS employees, but a customer must train their own employees.

