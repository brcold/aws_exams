

Q1. A company needs to transfer data between an Amazon S3 bucket and an on-premises application, Who is responsible for the security of this data, according to the AWS shared responsibility model? 

- [x] A. The company
- B. AWS
- C. Firewall vendor
- D. AWS Marketplace partner 

> According to the AWS shared responsibility model, both the company and AWS have responsibilities for the security of data being transferred between an Amazon S3 bucket and an on-premises application. The shared responsibility model states that AWS is responsible for the security of the cloud infrastructure, such as the physical security of the data centers and the underlying services they provide.

> On the other hand, the company is responsible for the security of their data and applications, including configuring secure access controls, implementing encryption, and ensuring the secure transfer of data.

---

Q2. Which abilities are benefits of the AWS Cloud? (Select TWO.)

- A. Trade variable expenses for capital expenses
- [x] B. Deploy globally in minutes
- C. Plan capacity in advance of deployments
- [x] D.Take advantage of economies of scale
- E. Reduce dependencies on network connectivity


> B. Deploy globally in minutes: AWS provides a global infrastructure that allows you to deploy your applications and services in multiple regions around the world quickly. This enables you to reach a global audience and reduce latency by having your resources closer to your users.

> D. Take advantage of economies of scale: AWS operates at a massive scale, which allows them to achieve cost efficiencies that are passed on to customers. By using AWS, you can benefit from their economies of scale and access cost-effective resources and services.

---


Q3. Which AWS service or feature provides log information of the inbound and outbound traffic on network interfaces in a VPC?

- A. Amazon CloudWatch Logs
- B. AWS CloudTrail
- [x] C. VPC Flow Logs
- D. AWS Identity and Access Management (IAM)


> VPC flow logs are available at three levels: VPC, subnet, network interface

> VPC Flow Logs is a feature that enables you to capture information about the IP traffic going to and from network interfaces within a VPC. It provides visibility into the network traffic within your VPC, including details such as source and destination IP addresses, ports, protocols, and the number of packets and bytes transferred, as well as information about the traffic flow (e.g., whether the traffic was accepted or rejected). This can be useful for monitoring, troubleshooting, and security analysis purposes.
 
Amazon CloudWatch Logs is a monitoring and observability service that enables you to collect and track metrics, collect and monitor log files, and set alarms. While it can be used in conjunction with VPC Flow Logs to store and analyze the log data, it does not provide the VPC traffic log information itself. AWS CloudTrail is a service that records AWS account activity and API usage. It is primarily used for auditing, security monitoring, and operational troubleshooting. 

CloudTrail captures information about the API calls made on your account, but it does not provide detailed network traffic logs. AWS Identity and Access Management (IAM) is a service that enables you to securely control access to AWS resources. It is used for managing user identities, authentication, and access permissions. IAM does not provide VPC traffic log information.
Therefore, VPC Flow Logs is the correct answer for providing log information of the inbound and outbound traffic on network interfaces in a VPC.


---

Q4. Which AWS service enables users to check for vulnerabilities on Amazon EC2 instances by using predefined assessment templates?

- A. AWS WAF
- B. AWS Trusted Advisor
- [x] C. Amazon Inspector
- D. AWS Shield


> Amazon Inspector is a vulnerability management service that continually scans AWS workloads for software vulnerabilities and unintended network exposure. With a few actions in the AWS Management Console, you can use Amazon Inspector across all accounts in your organization. Once started, it automatically discovers running EC2 instances, container images residing in Amazon ECR, and Lambda functions at scale, then immediately starts assessing them for known vulnerabilities.

> Amazon Inspector is an automated security assessment service that helps you identify security vulnerabilities and deviations from best practices in your EC2 instances and applications. It provides predefined assessment templates based on industry standards and best practices, such as the Center for Internet Security (CIS) benchmarks.

> Amazon Inspector performs security assessments by analyzing the configuration of your EC2 instances, including the operating system, network configuration, and installed software.

---

Q5. A company wants to provide managed Windows virtual desktops and applications to its remote employees over secure network connections. Which AWS services can the company use to meet these requirements? (Select TWO.)

- A. Amazon Connect
- [x] B. Amazon AppStream 2.0
- [x] C. Amazon WorkSpaces
- D. AWS Site-to-Site VPN
- E. Amazon Elastic Container Service (Amazon ECS)

 

> B. Amazon AppStream 2.0: Amazon AppStream 2.0 is a fully managed application streaming service that allows you to stream desktop applications securely to users on various devices. It supports Windows applications, including desktop applications, and provides a consistent and responsive user experience.

> C. Amazon WorkSpaces: Amazon WorkSpaces is a managed desktop-as-a-service (DaaS) offering that allows you to provision Windows virtual desktops for remote users. It provides a range of hardware and software configurations, allowing you to customize the desktop experience for your employees. WorkSpaces can be accessed securely over the internet from various devices.


 
> B. Amazon AppStream 2.0: Amazon AppStream 2.0 is a fully managed application streaming service that allows users to stream desktop applications securely to any device, including Windows-based applications. With AppStream 2.0, the company can deliver Windows virtual desktops and applications to remote employees over secure network connections. It provides a scalable and secure solution for application delivery without the need to manage underlying infrastructure.

> C. Amazon WorkSpaces: Amazon WorkSpaces is a fully managed Desktop-as-a-Service (DaaS) solution that provides Windows-based virtual desktops to users. It allows remote employees to access their personalized desktop environments from any supported device with an internet connection. WorkSpaces provides a secure and managed environment for running Windows desktop applications, and it supports features such as multi-factor authentication and encryption to ensure data security.

Let's briefly review the other options:

A. Amazon Connect: Amazon Connect is a cloud-based contact center service that enables companies to set up and manage a customer contact center. While it provides capabilities for customer interactions and support, it does not specifically address the requirement of providing managed Windows virtual desktops and applications to remote employees.

D. AWS Site-to-Site VPN: AWS Site-to-Site VPN allows you to establish secure network connections between your on-premises network and your Virtual Private Cloud (VPC) in AWS. While it provides secure network connectivity, it does not directly provide the capability to deliver managed Windows virtual desktops and applications.

E. Amazon Elastic Container Service (Amazon ECS): Amazon ECS is a container orchestration service that allows you to run applications in Docker containers. However, it is not specifically designed for delivering managed Windows virtual desktops and applications.

---


Q6. A company is migrating its applications from on-premises to the AWS Cloud. The company wants to ensure that the applications are assigned only the minimum permissions that are needed to perform all operations. Which AWS service will meet these requirements?

- [x] A. AWS Identity and Access Management (IAM)
- B. Amazon CloudWatch
- C. Amazon Macie
- D. Amazon GuardDuty
 

> AWS Identity and Access Management (IAM) is a service that enables you to manage access to AWS resources securely.

> With IAM, you can define fine-grained permissions and policies to control access to various AWS services and resources. By using IAM, you can create and manage IAM roles, users, and groups, and assign them specific permissions based on the principle of least privilege. This ensures that applications have only the necessary permissions to perform their required operations.
 

---

Q7.A company is planning to migrate its application to the AWS Cloud. Which AWS tool or set of resources should the company use to analyze and assess its readiness for migration?

- [x] A. AWS Cloud Adoption Framework (AWS CAF)
- B. AWS Pricing Calculator
- C. AWS Well-Architected Framework
- D. AWS Budgets

---

Q8. Which actions are best practices for an AWS account root user? (Select TWO.)

- A. Share root user credentials with team members
- B. Create multiple root users for the account, separated by environment.
- [x] C. Enable multi-factor authentication (MFA) on the root user
- [x] D. Create an IAM user with administrator privileges for daily administrative tasks, instead of using the root user
- E. Use programmatic access instead of the root user and password



> C. Enable multi-factor authentication (MFA) on the root user: Enabling MFA adds an extra layer of security to the root user account by requiring an additional authentication factor, such as a code from a mobile app or a hardware token, along with the password.

> D. Create an IAM user with administrator privileges for daily administrative tasks, instead of using the root user: It is recommended to create a separate IAM user with administrative privileges for regular administrative tasks. This helps improve security by reducing the need to use the root user credentials, which should be reserved for exceptional cases.
 
---

Q9. Which capabilities are in the platform perspective of the AWS Cloud Adoption Framework (AWS CAF)? (Select TWO.)

- A. Performance and capacity management  (operations)
- [x] B. Data engineering (platform)
- [x] C. Continuous integration and continuous delivery (CI/CD) (platform)
- D. Infrastructure protection (security)
- E. Change and release management (operations) 


---

> [!IMPORTANT]
> Q10. A company wants to design a centralized storage system to manage the configuration data and passwords for its critical business applications. Which AWS service or capability will meet these requirements MOST cost-effectively?

- [x] A. AWS Systems Manager Parameter Store
- B. AWS Secrets Manager
- C. AWS Config
- D. Amazon S3


> AWS Systems Manager Parameter Store is a service that provides secure storage for configuration data such as passwords, database strings, API keys, and other configuration details. It allows you to store and retrieve configuration parameters across different AWS services and applications.

> Parameter Store provides encryption at rest and in transit, access management through IAM policies, and integration with other AWS services like AWS Lambda and AWS CloudFormation.

> Compared to other options, AWS Systems Manager Parameter Store is a cost-effective solution for managing configuration data and passwords as it provides the necessary security and integration capabilities at a lower cost compared to specialized services like AWS Secrets Manager.

---

Q11. A company wants to migrate unstructured data to AWS. The data needs to be securely moved with inflight encryption and end-to-end data validation. Which AWS service will meet these requirements?

- A. AWS Application Migration Service
- B. Amazon Elastic File System (Amazon EFS)
- [x] C. AWS DataSync
- D. AWS Migration Hub

 
> AWS DataSync is a service designed for fast and secure data transfer between on-premises storage systems and AWS storage services. It supports the migration of large volumes of data, including unstructured data, while ensuring data integrity and security.

> AWS DataSync supports in-flight encryption by using SSL/TLS protocols during data transfer, ensuring that the data is encrypted while in transit. This helps protect the data from unauthorized access or interception during the migration process.

> Additionally, AWS DataSync provides end-to-end data validation to ensure data integrity. It uses checksums to compare the source and destination data to verify that the transferred data is accurate and intact. This helps guarantee that the data transferred to AWS is unaltered and complete.


---

> [!IMPORTANT]
> Q12. A company wants to assess its operational readiness. It also wants to identify and mitigate any operational risks ahead of a new product launch. Which AWS Support plan offers guidance and support for this kind of event at no additional charge?

- A. AWS Business Support
- B. AWS Basic Support
- C. AWS Developer Support
- [x] D. AWS Enterprise Support

 

https://aws.amazon.com/premiumsupport/plans/
> AWS Countdown, formerly known as AWS Infrastructure Event Management (IEM), helps you throughout the project lifecycle to assess cloud operational readiness, identify and mitigate risks, and plan capacity, using proven playbooks developed by AWS experts.
> AWS Countdown is a service designed for a broad range of cloud use cases, including cloud migration services, cloud modernization, product launches, and go-live events.
https://aws.amazon.com/premiumsupport/aws-countdown/
> AWS Countdown has replaced AWS IEM and is included with Enterprise Support. Enterprise On-Ramp customers receive one (1) Countdown engagement each year at no cost. AWS Countdown Premium is available for Business Support, Enterprise On-Ramp, and Enterprise Support customers as a monthly subscription for an additional fee.
> belong to launch support
https://us-east-1.console.aws.amazon.com/support/plans/home?region=us-east-1#/


> AWS Enterprise Support provides a comprehensive level of support for businesses at scale. It includes features such as 24/7 access to AWS Support engineers, guidance for architectural best practices, and support for operational events like new product launches. AWS Enterprise Support offers proactive guidance and support to help customers assess their operational readiness and address any operational risks they may encounter.
> 
---


> [!IMPORTANT]
> Q13. A user wants to securely automate the management and rotation of credentials that are shared between applications, while spending the least amount of time on managing tasks. Which AWS service or feature can be used to accomplish this?

- A. AWS CloudHSM
- B. AWS Key Management Service (AWS KMS)
- [x] C. AWS Secrets Manager
- D. Server-side encryption


> AWS Secrets Manager is a fully managed service that helps you protect secrets, such as database credentials, API keys, and other sensitive information that applications need to access. It provides a central repository for storing and managing secrets securely.

> With AWS Secrets Manager, you can automate the rotation of secrets, which includes automatically generating new credentials and updating the applications that use them. This helps ensure that the credentials are regularly changed, reducing the risk of unauthorized access.

> AWS Secrets Manager also integrates with AWS services and other applications, making it easier to retrieve and manage secrets programmatically. It offers a simple API and SDKs for interacting with secrets, enabling secure access to credentials from within applications.

> By utilizing AWS Secrets Manager, you can automate the management and rotation of shared credentials while minimizing the time spent on manual tasks.
 

---


Q14. A network engineer needs to build a hybrid cloud architecture connecting on-premises networks to the AWS Cloud using AWS Direct Connect. The company has a few VPCs in a single AWS Region and expects to increase the number of VPCs to hundreds over time. Which AWS service or feature should the engineer use to simplify and scale this connectivity as the VPCs increase in number?

- A. VPC endpoints
- [x] B. AWS Transit Gateway
- C. Amazon Route 53
- D. AWS Secrets Manager

>  AWS Transit Gateway is a service that simplifies network connectivity and routing for multiple VPCs and on-premises networks. It acts as a hub that allows you to connect your VPCs and on-premises networks using a single gateway. With AWS Transit Gateway, you can scale your connectivity as the number of VPCs increases without the need for complex and manual network configurations.

> By using AWS Transit Gateway, the network engineer can centrally manage and scale connectivity between on-premises networks and hundreds of VPCs, simplifying the overall hybrid cloud architecture.


---


> [!IMPORTANT]
> Q15. A company needs to engage third-party consultants to help maintain and support its AWS environment and the company's business needs. Which AWS service or resource will meet these requirements?

- A. AWS Support
- B. AWS Organizations
- C. AWS Service Catalog
- [x] D. AWS Partner Network (APN)

 
> The AWS Partner Network (APN) is a global community of partners who offer a wide range of consulting and professional services to help customers design, architect, build, migrate, and manage their applications and workloads on AWS. APN partners are certified and experienced in various AWS services and solutions, making them suitable for providing the required expertise and support.
> By engaging with APN partners, the company can access a pool of qualified consultants who can assist with maintaining and supporting the AWS environment, ensuring that the company's business needs are met effectively.
 

---


Q16. Which AWS service provides command line access to AWS tools and resources directly from a web browser?

- A. AWS CloudHSM
- [x] B. AWS CloudShell
- C. Amazon WorkSpaces
- D. AWS Cloud Map


>  AWS CloudShell is a browser-based, pre-authenticated shell environment that provides you with a command-line interface (CLI) for managing and interacting with your AWS resources. 
 
> AWS CloudShell is a browser-based shell environment that provides a command line interface (CLI) pre-authenticated with AWS credentials. It allows users to run AWS CLI commands and access AWS tools and SDKs without the need for local installation or configuration.

> With AWS CloudShell, users can execute commands, write scripts, and interact with AWS services through the command line interface. It comes pre-configured with commonly used AWS CLI tools and provides persistent storage for storing scripts and files.

> AWS CloudHSM (option A) is a service that provides hardware security modules (HSMs) to help protect sensitive data and cryptographic keys in the AWS Cloud.  

> Amazon WorkSpaces (option C) is a fully managed desktop-as-a-service (DaaS) solution that allows users to access virtual desktops in the cloud. While it provides a desktop environment, it does not specifically provide command line access to AWS tools and resources from a web browser.

> AWS Cloud Map (option D) is a service that allows users to discover and manage cloud resources dynamically. It is primarily used for service discovery within distributed systems and does not provide command line access to AWS tools and resources from a web browser.
 

---


> [!IMPORTANT]
> Q17. A company needs to centrally configure and manage Amazon VPC security groups across multiple AWS accounts within an organization in AWS Organizations. Which AWS service should the company use to meet these requirements?

- [x] A. AWS Firewall Manager
- B. Amazon GuardDuty
- C. Amazon Detective
- D. AWS Web Application Firewall (WAF)


> AWS Firewall Manager is a security management service that allows organizations to centrally configure and manage firewall rules and security group policies across multiple AWS accounts. It provides a single place to define and enforce security policies consistently across the organization.

> With AWS Firewall Manager, the company can create security group policies and apply them to multiple VPCs and accounts within the organization. It simplifies the management and enforcement of security group rules, ensuring that consistent security configurations are maintained.

> Amazon GuardDuty (option B) is a threat detection service that monitors AWS accounts for malicious activity and unauthorized behavior. It focuses on threat detection rather than centrally managing security groups.

> Amazon Detective (option C) is a service that helps analyze, investigate, and visualize security data to identify potential security issues. It does not specifically address the central configuration and management of security groups.

> AWS WAF (option D) is a web application firewall service that helps protect web applications from common web exploits. While it provides security for web applications, it does not offer centralized management of security groups across multiple accounts.
 


---


Q18. A library wants to automate the classification of electronic books based on the contents of the books. Which AWS service should the library use to meet this requirement?

- A. Amazon Redshift
- B. Amazon CloudSearch
- [x] C. Amazon Comprehend
- D. Amazon Aurora


> Amazon Comprehend is a natural language processing (NLP) service provided by AWS. It uses machine learning algorithms to analyze text and extract insights such as sentiment analysis, entity recognition, key phrase extraction, and language detection. In the case of the library, it can utilize Amazon Comprehend to automatically analyze the contents of electronic books. By leveraging the NLP capabilities of Amazon Comprehend, the service can classify the books based on their content, extract relevant information, and provide valuable insights about the books' topics, themes, or categories.

> Amazon Redshift (option A) is a fully managed data warehousing service designed for analyzing large datasets.  
> Amazon CloudSearch (option B) is a fully managed search service that provides full-text search capabilities for applications. 
 
---

> [!IMPORTANT]
> Q19. Which tool should a developer use to integrate AWS service features directly into an application?

- [x] A. AWS Software Development Kit
- B. AWS CodeDeploy
- C. AWS Lambda
- D. AWS Batch
 

> The AWS SDK provides a set of libraries, APIs, and tools that enable developers to interact with and utilize AWS services within their applications. The SDKs are available for various programming languages and provide a convenient way to access and integrate AWS services programmatically.

> By using the AWS SDK, developers can leverage the functionality and features of AWS services directly within their applications. They can make API calls, manage resources, and interact with AWS services such as Amazon S3, Amazon EC2, AWS Lambda, and many others.

> AWS CodeDeploy (option B) is a service that automates the deployment of applications to Amazon EC2 instances or on-premises instances. It focuses on deploying applications rather than integrating AWS service features directly into an application.

> AWS Lambda (option C) is a serverless compute service that allows developers to run their code without provisioning or managing servers. While Lambda can be used to build applications and workflows, it is not specifically designed for integrating AWS service features into an application.


> AWS Batch (option D) is a service for running batch computing workloads in the AWS Cloud. It is used to manage and schedule batch jobs, but it does not focus on integrating AWS service features into an application.
 


---

> [!IMPORTANT]
> Q20. A company wants to define a central data protection policy that works across AWS services for compute, storage, and database resources. Which AWS service will meet this requirement?

- A. AWS Batch
- B. AWS Elastic Disaster Recovery
- [x] C. AWS Backup
- D. Amazon FSx


> AWS Backup is a fully managed backup service that centralizes and automates the backup of data across AWS services. It provides a unified interface and workflow to manage backups for various AWS resources, including compute instances, storage volumes, databases, and file systems.

> With AWS Backup, the company can define backup policies and schedules that apply to different AWS services. It allows for consistent and centralized management of backups, making it easier to enforce data protection policies across the organization.

>AWS Batch (option A) is a service for running batch computing workloads in the AWS Cloud. It is not specifically designed for data protection policies.

 
> Amazon FSx (option D) is a fully managed file storage service. While it provides data protection mechanisms, it is focused on file storage rather than defining central data protection policies across various AWS services.

---

Q21. A company plans to migrate its application to AWS and run the application on Amazon EC2 instances. The application will have Continuous usage for 1 year. Which EC2 instance purchasing option will meet these requirements MOST cost-effectively?

- [x] A. Reserved Instances
- B. Spot Instances
- C. On-Demand Instances
- D. Dedicated Hosts


---


Q22. Which options are AWS Cloud Adoption Framework (AWS CAF) security perspective capabilities? (Select TWO.)

- A. Observability  (operations)
- B. Incident and problem management (operations)
- [x] C. Incident response (security)
- [x] D. Infrastructure protection (security)
- E. Availability and continuity  (operations) 
 
---

> [!IMPORTANT]
> Q23. Which AWS feature provides a no-cost platform for AWS users to join community groups, ask questions, find answers, and read community-generated articles about best practices?

- A. AWS Knowledge Center
- [x] B. AWS re:Post
- C. AWS IQ
- D. AWS Enterprise Support
 

> AWS re:Post is a feature that provides a no-cost platform for AWS users to join community groups, ask questions, find answers, and read community-generated articles about best practices. It is an online community forum where users can engage with other AWS users, share knowledge, and seek assistance from peers.

> The AWS Knowledge Center (option A) is a resource hub that provides official documentation, whitepapers, FAQs, and articles, but it is not specifically designed as a platform for community engagement.

> AWS IQ (option C) is a platform that connects AWS customers with AWS-certified experts for paid project-based work and is not a no-cost platform for community engagement.

> AWS Enterprise Support (option D) is a paid support plan offered by AWS for enterprise customers and does not provide a free platform for community engagement.

---

Q24. Which option is an environment that consists of one or more data centers?

- A. Amazon CloudFront
- [x] B. Availability Zone
- C. VPC
- D. AWS Outposts
 

> An Availability Zone (AZ) is a distinct location within an AWS Region that contains one or more data centers. Each AZ is designed to be isolated from failures in other AZs and provides redundant power, networking, and cooling. By distributing resources across multiple AZs within a Region, AWS aims to achieve high availability and fault tolerance.

> A. Amazon CloudFront is a content delivery network (CDN) service that caches and delivers content from edge locations worldwide. It does not represent an environment consisting of data centers.
> B. Availability Zone (AZ) is the correct option. It represents a distinct location within an AWS Region that comprises one or more data centers.

> C. VPC (Virtual Private Cloud) is a virtual network environment within AWS that allows users to launch AWS resources in a logically isolated section of the AWS cloud. It does not directly represent an environment consisting of data centers.

>D. AWS Outposts is a service that allows customers to deploy AWS infrastructure, including compute and storage, within their own on-premises data centers. While it involves deploying infrastructure, it is not an environment that consists of multiple data centers, as it is typically deployed in a single location.
 

---

Q25. A company has a fleet of cargo ships. The cargo ships have sensors that collect data at sea, where there is intermittent or no internet connectivity. The company needs to collect, format, and process the data at sea and move the data to AWS later. Which AWS service should the company use to meet these requirements?

- A. AWS IoT Core
- B. Amazon Lightsail
- C. AWS Storage Gateway
- [x] D. AWS Snowball Edge
 

AWS Snowball Edge is a data transfer device that is designed to handle large-scale data migration and edge computing scenarios. It is equipped with onboard storage and compute capabilities, making it suitable for use in remote or disconnected environments.

With AWS Snowball Edge, the company can collect and store the data from the cargo ship's sensors locally on the device. It provides data transfer options such as Snowball client software or Snowball Edge Compute Optimized instances to format and process the data onboard the device itself.

Once the cargo ship returns to an area with internet connectivity, the company can then physically ship the Snowball Edge device back to AWS, where the data can be securely transferred to Amazon S3 or other AWS services for further processing and analysis.

Let's review the other options:

A. AWS IoT Core is a service that enables the connection, management, and ingestion of data from IoT devices. While it can handle IoT data, it requires internet connectivity, which may not be available at sea.

B. Amazon Lightsail is a simplified virtual private server (VPS) service. It is not specifically designed for data collection, processing, or offline scenarios.

C. AWS Storage Gateway is a hybrid cloud storage service that enables on-premises applications to seamlessly use AWS cloud storage. It is not specifically designed for data collection and processing in disconnected environments.
 

---

> [!IMPORTANT]
> Q26. Which top-level key performance indicator (KPI) is available in AWS rightsizing recommendations of Cost Optimization?

- A. Container modernization opportunities
- [x] B. Estimated monthly savings
- C. Reserved instances savings
- D. Compute savings recommendations



To filter your rightsizing recommendations: Open the Billing and Cost Management console at https://console.aws.amazon.com/costmanagement/.

In the navigation pane, under Legacy pages, choose Rightsizing.
https://us-east-1.console.aws.amazon.com/costmanagement/home?region=us-east-1#/rightsizing
You can see the following top-level key performance indicators (KPIs) in your rightsizing recommendations:

- Optimization opportunities – The number of recommendations available based on your resources and usage
- Estimated monthly savings – The sum of the projected monthly savings associated with each of the recommendations provided
- Estimated savings (%) – The available savings relative to the direct instance costs (On-Demand) associated with the instances in the recommendation list




> In AWS rightsizing recommendations, the Estimated monthly savings KPI provides an estimate of the potential cost savings that can be achieved by right-sizing instances or modifying instance types. It helps users identify opportunities to optimize their infrastructure and reduce costs.

> A. Container modernization opportunities: This option is not directly related to rightsizing recommendations or cost optimization. It refers to opportunities for modernizing applications by adopting containerization technologies.

> C. Reserved instances savings: Reserved instances savings are not specifically a top-level KPI in rightsizing recommendations. Reserved instances are a purchasing option that can provide cost savings, but they are not directly related to rightsizing recommendations.

> D. Compute savings recommendations: While compute savings recommendations are part of rightsizing, they are not the top-level KPI mentioned in the question. Compute savings recommendations provide insights and recommendations to optimize compute resources, but the Estimated monthly savings KPI encompasses a broader view of potential cost savings.
 

---

Q27. A company is deploying a machine learning (ML) research project that will require a lot of compute power over several months. The ML processing jobs do not need to run at specific times. Which Amazon EC2 instance purchasing option will meet these requirements at the lowest cost?

- A. On-Demand Instances
- [x] B. Spot Instances
- C. Reserved Instances
- D. Dedicated Instances

 > not on-demand

Spot Instances allow users to bid on unused EC2 instances, enabling them to access spare capacity at a significantly reduced cost compared to On-Demand Instances. The pricing for Spot Instances is determined by supply and demand, and the bids that users place. If the Spot price exceeds the bid price, the instance is terminated.

Since the ML processing jobs do not have specific time constraints and can be run when spare capacity is available, Spot Instances can be a cost-effective option. However, it's important to note that Spot Instances can be interrupted if the Spot price rises above the bid price or if the capacity is needed by On-Demand or Reserved Instances.

Let's review the other options:

A. On-Demand Instances provide instances with no upfront costs or long-term commitments but are billed at the full On-Demand price. They are suitable for workloads that require flexibility and do not have predictable usage patterns. However, for long-term, high compute workloads, Spot Instances are generally more cost-effective.

C. Reserved Instances offer a significant discount compared to On-Demand Instances but require upfront payment or a commitment for a specified term (1 or 3 years). Reserved Instances are more suitable for workloads with consistent usage patterns over an extended period. They may not be the most cost-effective option for a research project that doesn't require specific timing.

D. Dedicated Instances provide physical servers dedicated to a single customer and offer additional isolation and compliance options. However, they do not typically provide cost savings compared to On-Demand Instances and are not the best option for cost optimization.
 

---

Q28. Which of the following is a recommended design principle for AWS Cloud architecture?

- A. Design tightly coupled components
- B. Build a single application component that can handle all the application functionality.
- C. Make large changes on fewer iterations to reduce chances of failure.
- [x] D. Avoid monolithic architecture by segmenting workloads
 

Monolithic architecture refers to an approach where an application is built as a single, large, and tightly-coupled unit. In contrast, the recommended practice in AWS Cloud architecture is to segment workloads into smaller, loosely-coupled components. This approach promotes scalability, flexibility, and fault isolation.

By segmenting workloads, you can design and deploy individual components independently, allowing for easier management, scalability, and fault tolerance. This approach aligns with the principles of microservices architecture and promotes modularity, decoupling, and efficient resource utilization.

Let's review the other options:

A. Designing tightly coupled components is not recommended in AWS Cloud architecture. Tightly coupling components can lead to challenges in scaling, maintenance, and flexibility.

B. Building a single application component that handles all functionality goes against the idea of breaking down workloads into smaller, scalable components. It can lead to challenges in deployment, maintenance, and the ability to scale individual functions independently.

C. Making large changes on fewer iterations to reduce chances of failure is not a recommended design principle. Instead, a more agile approach that promotes smaller, incremental changes and frequent iterations is generally advised for improved agility, testing, and faster time to market.

 
---


Q29. A company wants to run its workloads in the AWS Cloud effectively, reduce management overhead, and improve processes. Which AWS Well-Architected Framework pillar represents these requirements?

- A. Reliability
- [x] B. Operational excellence
- C. Performance efficiency
- D. Cost optimization

 > keywords: improve processes 
 

---


Q30. Which of the following is a managed AWS service that is used specifically for extract, transform, and load (ETL) data?

- A. Amazon Athena
- [x] B. AWS Glue
- C. Amazon S3
- D. AWS Snowball Edge

 

> AWS Glue is a fully managed extract, transform, and load (ETL) service that makes it easy to prepare and load data for analytics. It provides capabilities for discovering, cataloging, transforming, and moving data between various data stores.

> With AWS Glue, users can create and manage data transformation workflows, define and schedule ETL jobs, and automatically generate ETL code for data transformations. It supports a visual interface for building ETL workflows and provides integration with other AWS services such as Amazon S3, Amazon RDS, Amazon Redshift, and more.



> A. Amazon Athena is a query service that allows users to analyze data stored in Amazon S3 using standard SQL. While it can be used to query and analyze data, it is not specifically designed for ETL processes.

> C. Amazon S3 (Simple Storage Service) is an object storage service that provides industry-leading scalability, durability, and security. While it is commonly used for storing data, it does not provide specific ETL capabilities.

> D. AWS Snowball Edge is a data transfer and edge computing device. While it can be used for data transfer and offline processing, it is not a managed service specifically designed for ETL operations.
 


---
Q31. Which AWS service or feature is a browser-based, pre-authenticated service that can be launched directly from the AWS Management Console?

- A. AWS API
- B. AWS Lightsail
- C. AWS Cloud9
- [x] D. AWS CloudShell


 
AWS CloudShell is a browser-based, pre-authenticated shell environment that provides you with access to a command-line interface (CLI) for managing and interacting with your AWS resources. It can be launched directly from the AWS Management Console, eliminating the need to install and configure the CLI on your local machine.

With AWS CloudShell, you can run AWS CLI commands, AWS SDKs, and other tools to manage your AWS resources. It comes pre-configured with common tools and programming languages, making it easy to access and use from the browser.

The other options are not the correct answers for this scenario:

A. AWS API is not a recognized AWS service or feature.

B. AWS Lightsail: AWS Lightsail is a simplified virtual private server (VPS) service that provides pre-configured instances for running applications. It is not a browser-based, pre-authenticated service launched directly from the AWS Management Console.
 
C. AWS Cloud9: AWS Cloud9 is an integrated development environment (IDE) in the cloud that allows you to write, run, and debug code. While it is browser-based and can be launched from the AWS Management Console, it does not have pre-authentication and requires you to authenticate within the Cloud9 environment.


 

---

Q32. A company wants to provide access to Windows file shares in AWS from its on-premises workloads. The company does not want to provision any additional infrastructure or applications in its data center. Which AWS service will meet these requirements?

- [x] A. Amazon FSx File Gateway
- B. AWS DataSync
- C. Amazon S3
- D. AWS Snow Family

 
> Amazon FSx File Gateway provides a fully managed file storage gateway for hybrid cloud environments. It allows you to securely access Amazon FSx for Windows File Server file shares over the Internet from your on-premises environment without the need for additional infrastructure or applications in your data center.

By deploying an Amazon FSx File Gateway in your on-premises environment, you can establish a secure connection to your Amazon FSx for Windows File Server file shares hosted in AWS. This enables your on-premises workloads to access the file shares as if they were local, providing seamless integration between your on-premises and AWS environments.

The other options are not the correct answers for this scenario:

B. AWS DataSync: AWS DataSync is a service for migrating and transferring data between on-premises storage systems and AWS. While it can be used to transfer data to and from AWS, it does not provide direct access to Windows file shares in AWS.

C. Amazon S3: Amazon S3 is an object storage service that allows you to store and retrieve large amounts of unstructured data. While it can be used for file storage, it does not provide native support for Windows file shares or the ability to access file shares from on-premises workloads without additional infrastructure.

D. AWS Snow Family: The AWS Snow Family consists of physical devices (Snowcone, Snowball, and Snowmobile) designed to securely and efficiently transfer large amounts of data into and out of AWS. While they can be used for data migration, they do not provide direct access to Windows file shares in AWS.

Therefore, the correct answer is A. Amazon FSx File Gateway as the AWS service that will meet the requirements of providing access to Windows file shares in AWS from on-premises workloads without provisioning additional infrastructure or applications in the data center.

---

Q33. Which AWS service provides highly durable object storage?

- [x] A. Amazon S3
- B. Amazon Elastic File System (Amazon EFS)
- C. Amazon Elastic Block Store (Amazon EBS)
- D. Amazon FSx

 
---

Q34. A company has an uninterruptible application that runs on Amazon EC2 instances. The application constantly processes a backlog of files in an Amazon Simple Queue Service (Amazon SQS) queue. This usage is expected to continue to grow for years. What is the MOST cost-effective EC2 instance purchasing model to meet these requirements?

- A. Spot Instances
- B. On-Demand Instances
- [x] C. Savings Plans
- D. Dedicated Hosts

> Savings Plans are the most cost-effective EC2 instance purchasing model for long-term usage scenarios. Savings Plans provide flexible pricing options with significant cost savings compared to On-Demand Instances.

By purchasing Savings Plans, you commit to a specific amount of compute usage (measured in dollars per hour) over a term of one or three years. This commitment allows you to benefit from discounted rates on your EC2 usage, including both On-Demand Instances and Reserved Instances.

In the given scenario, where the application is expected to continue processing files for years, Savings Plans offer the advantage of long-term cost optimization. With the commitment to a specific amount of compute usage, the company can benefit from significant cost savings over the extended duration of the application.

The other options are not the most cost-effective for this scenario:

A. Spot Instances: Spot Instances are suitable for applications with flexible start and end times or those that can handle interruptions. While Spot Instances offer the potential for significant cost savings, they are not the best choice for an uninterruptible application that requires constant processing.

B. On-Demand Instances: On-Demand Instances are the default pricing model for EC2 and offer no upfront commitments or long-term contracts. While they provide flexibility, they do not offer the same level of cost savings as other purchasing options like Savings Plans.

D. Dedicated Hosts: Dedicated Hosts provide physical servers dedicated to your use, which can be beneficial for compliance, licensing, or hardware-bound workloads. However, they are not specifically designed for cost optimization and are typically more expensive than other EC2 instance purchasing options.
 

---


Q35. Which design principles support the reliability pillar of the AWS Well-Architected Framework? (Select TWO)

- A. Perform operations as code (operational excellence)
- B. Enable traceability (security)
- [x] C. Automatically scale to meet demand (relibility)
- D. Deploy resources globally to improve response time (performance efficiency)
- [x] E. Automatically recover from failure (relibility)
 

---

Q36. A company needs to provision, manage, and deploy public and private SSL/TLS certificates for use with AWS services. Which AWS service will meet these requirements?

- A. AWS Key Management Service (AWS KMS)
- [x] B. AWS Certificate Manager (ACM)
- C. AWS Security Hub
- D. Amazon Inspector

> secure sockets layer/ transport layer security

> AWS Certificate Manager (ACM) is a service that simplifies the process of provisioning, managing, and deploying SSL/TLS certificates for use with AWS services. ACM provides both public and private SSL/TLS certificates that can be used to secure websites, applications, and other resources running on AWS.

With ACM, you can request and manage SSL/TLS certificates for use with AWS services such as Amazon CloudFront, Elastic Load Balancing, Amazon API Gateway, and Amazon Elastic Beanstalk. ACM takes care of the complexity of certificate renewal, deployment, and integration with these services, making it easier to manage SSL/TLS certificates at scale.

The other options are not the correct answers for this scenario:

A. AWS Key Management Service (AWS KMS): AWS KMS is a service that helps you create and control the encryption keys used to encrypt your data. While it can be used to manage keys for SSL/TLS certificates, it does not directly provide the capability to provision, manage, and deploy SSL/TLS certificates like ACM.

C. AWS Security Hub: AWS Security Hub is a service that provides a comprehensive view of your security posture across multiple AWS accounts. While it can help with security monitoring and compliance, it does not provide the specific functionality required to provision, manage, and deploy SSL/TLS certificates.

D. Amazon Inspector: Amazon Inspector is a security assessment service that helps you identify security vulnerabilities and deviations from best practices in your applications and infrastructure. While it can help with security assessments, it does not provide the functionality to provision, manage, and deploy SSL/TLS certificates.
 

---

> [!IMPORTANT]
> Q37. Which AWS service or feature improves network performance by sending traffic through the AWS worldwide network infrastructure?

- A. Route table
- B. AWS Transit Gateway
- [x] C. AWS Global Accelerator
- D. Amazon VPC


AWS Global Accelerator is a service that improves the performance and availability of your applications by directing traffic through the AWS global network infrastructure. It uses the AWS global network backbone to optimize the path between your users and your applications, reducing latency and increasing throughput.

With AWS Global Accelerator, you can create accelerators that act as entry points to your applications running in one or more AWS Regions. When clients send traffic to the accelerator, it intelligently routes the traffic to the nearest AWS edge location, reducing the distance and improving the network performance. It also automatically routes traffic to healthy endpoints in your application, even if they are distributed across multiple AWS Regions.

The other options are not the correct answers for this scenario:

A. Route table: A route table is a component of Amazon VPC that controls the traffic between subnets. While it is an important networking component, it does not directly improve network performance by leveraging the AWS worldwide network infrastructure like AWS Global Accelerator.

B. AWS Transit Gateway: AWS Transit Gateway is a service that simplifies connectivity between Amazon VPCs and on-premises networks. While it provides a scalable and centralized hub for network traffic, it does not specifically improve network performance by leveraging the AWS worldwide network infrastructure.

D. Amazon VPC: Amazon VPC (Virtual Private Cloud) is a service that enables you to launch AWS resources in a virtual network. While it provides networking capabilities and isolation for your resources, it does not have a specific feature to improve network performance by leveraging the AWS worldwide network infrastructure.


---


Q38. Which AWS security service protects applications from distributed denial of service attacks with always-on detection and automatic inline mitigations?

- A. Amazon Inspector
- B. AWS Web Application Firewall (AWS WAF)
- C. Elastic Load Balancing (ELB)
- [x] D. AWS Shield



AWS Shield is a managed Distributed Denial of Service (DDoS) protection service that safeguards applications running on AWS. AWS Shield provides always-on detection and automatic inline mitigations that minimize application downtime and latency, so there is no need to engage AWS Support to benefit from DDoS protection. There are two tiers of AWS Shield - Standard and Advanced.


---

Q39. Which AWS tool gives users the ability to plan their service usage, service costs, and instance reservations, and also allows them to set custom alerts when their costs or usage exceed established thresholds?

- A. Cost Explorer
- [x] B. AWS Budgets
- C. AWS Cost and Usage report
- D. Reserved Instance reporting


AWS Budgets is an AWS tool that allows users to plan their service usage, service costs, and instance reservations. It provides users with the ability to set custom alerts when their costs or usage exceed established thresholds. With AWS Budgets, users can monitor their AWS spend closely and take proactive actions to optimize their costs and usage.


---
Q40. Which AWS service helps users audit API activity across their AWS account?

- [x] A. AWS CloudTrail
- B. Amazon Inspector
- C. AWS WAF
- D. AWS Config


AWS CloudTrail is the AWS service that helps users audit API activity across their AWS account. It provides a comprehensive history of API calls made within an AWS account, including details such as the identity of the caller, the time of the call, the source IP address, the request parameters, and the response elements returned by the AWS service. This information can be used for security analysis, resource change tracking, compliance auditing, and troubleshooting purposes.


---

Q41. A company needs to use third-party software for its workload on AWS. Which AWS service or feature can the company use to purchase the software?

- A. AWS Resource Access Manager
- B. AWS Managed Services
- C. AWS License Manager
- [x] D. AWS Marketplace

AWS Marketplace is the AWS service or feature that enables companies to purchase and deploy third-party software directly from the AWS platform. It offers a wide selection of software solutions, including both free and paid options, across various categories such as security, networking, databases, analytics, and more. Users can browse through different software listings, compare pricing and features, and easily deploy the chosen software onto their AWS infrastructure. AWS Marketplace provides a convenient and trusted platform for companies to discover, procure, and manage third-party software solutions for their workload on AWS.

---

> [!IMPORTANT]
> Q42. What are the benefits of consolidated billing for AWS Cloud services? (Select TWO.)

- [x] A. Volume discounts
- B. A minimal additional fee for use
- [x] C. One bill for multiple accounts
- D. Installment payment options
- E. Custom cost and usage budget creation


You can use the consolidated billing feature in AWS Organizations to consolidate billing and payment for multiple AWS accounts. 
Every organization in AWS Organizations has a management account that pays the charges of all the member accounts. For more information about organizations, see the AWS Organizations User Guide.

Consolidated billing has the following benefits:

- One bill – You get one bill for multiple accounts in the same SOR (Seller of Record: the legal AWS entity (such as Amazon Web Services, Inc., or a local AWS subsidiary in your country) that is responsible for selling AWS services to you and issuing your invoices). If an organization has accounts from multiple SORs, you receive one bill per SOR.
- Easy tracking – You can track the charges across multiple accounts and download the combined cost and usage data.
- Combined usage – You can combine the usage across all accounts in the organization to share the volume pricing discounts, Reserved Instance discounts, and Savings Plans. This can result in a lower charge for your project, department, or company than with individual standalone accounts. For more information, see Volume discounts.
- No extra fee – Consolidated billing is offered at no additional cost.

 

---

Q43. Which AWS service or feature can be used to create a private connection between an on-premises workload and an AWS Cloud workload?

- A. Amazon Route 53
- B. Amazon Macie
- [x] C. AWS Direct Connect
- D. AWS PrivateLink


PrivateLink provides direct secure connections from VPCs to other AWS services. It's similar to the AWS Direct Connect service in that it establishes private connections to the AWS cloud, except Direct Connect links users' on-premises environments to AWS. PrivateLink, on the other hand, secures traffic from users' VPC environments, which are already in AWS.

---

> [!IMPORTANT]
> Q44. Which AWS service can be used to retrieve compliance reports on demand?

- A. AWS Secrets Manager
- [x] B. AWS Artifact
- C. AWS Security Hub
- D. AWS Certificate Manager


AWS Artifact is the AWS service that can be used to retrieve compliance reports on demand. It provides access to various compliance and security documents, including 
- industry-specific certifications,
- attestations of compliance,
- third-party audit reports, and more.

These reports can be downloaded directly from AWS Artifact, allowing users to easily access the necessary documentation to meet their compliance requirements.


---

Q45. Which of the following is an AWS value proposition that describes a user's ability to scale infrastructure based on demand?

- A. Speed of innovation
- [x] B. Resource elasticity
- C. Decoupled architecture
- D. Global deployment


---

Q46. Which AWS service enables companies to deploy an application close to end users?

- [x] A. Amazon CloudFront
- B. AWS Auto Scaling
- C. AWS AppSync
- D. Amazon Route 53

Amazon CloudFront is the AWS service that enables companies to deploy an application close to end users. It is a content delivery network (CDN) service that helps deliver static, dynamic, and streaming content to end users with low latency and high data transfer speeds. By caching content at edge locations around the world, CloudFront brings the application closer to end users, reducing latency and improving the overall performance of the application. This allows companies to provide a faster and more responsive user experience to their customers.
 

---

Q47. Which pillar of the AWS Well-Architected Framework refers to the ability of a system to recover from infrastructure or service disruptions and dynamically acquire computing resources to meet demand?

- A. Security
- [x] B. Reliability
- C. Performance efficiency
- D. Cost optimization

 

---

Q48. Which security service automatically recognizes and classifies sensitive data or intellectual property on AWS?

- A. Amazon GuardDuty
- [x] B. Amazon Macie
- C. Amazon Inspector
- D. AWS Shield
 


---

Q49. Which task is a customer's responsibility, according to the AWS shared responsibility model?

- [x] A. Management of the guest operating systems
- B. Maintenance of the configuration of infrastructure devices
- C. Management of the host operating systems and virtualization
- D. Maintenance of the software that powers Availability Zones

 

---

Q50. Which AWS benefit is demonstrated by on-demand technology services that enable companies to replace upfront fixed expenses with variable expenses?

- A. High availability
- B. Economies of scale
- [x] C. Pay-as-you-go pricing
- D. Global reach
 

---


Q51. Which AWS service can run a managed PostgreSQL database that provides online transaction processing (OLTP)?

- A. Amazon DynamoDB
- B. Amazon Athena
- [x] C. Amazon RDS
- D. Amazon EMR
 

---


> [!IMPORTANT]
> Q52. A user wants to allow applications running on an Amazon EC2 instance to make calls to other AWS services. The access granted must be secure. Which AWS service or feature should be used?

- A. Security groups
- B. AWS Firewall Manager
- [x] C. IAM roles
- D. IAM user SSH keys


IAM (Identity and Access Management) roles provide temporary security credentials that can be attached to an EC2 instance. These roles define the permissions and access policies for the instance. By assigning an IAM role to an EC2 instance, applications running on that instance can securely access other AWS services without the need for storing long-term access keys or credentials on the instance itself.
Security groups (option A) are used to control inbound and outbound traffic at the instance level, but they do not grant secure access to AWS services.
AWS Firewall Manager (option B) is a service used to manage firewall rules across multiple accounts and resources, but it does not grant access to AWS services.
IAM user SSH keys (option D) are used for authenticating and accessing EC2 instances via Secure Shell (SSH), but they do not grant access to AWS services.


---

Q53. A developer needs to maintain a development environment infrastructure and a production environment infrastructure in a repeatable fashion. Which AWS service should the developer use to meet these requirements?

- A. AWS Ground Station
- B. AWS Shield
- C. AWS IoT Device Defender
- [x] D. AWS CloudFormation

> AWS CloudFormation is the AWS service that should be used to maintain development and production environment infrastructures in a repeatable fashion. CloudFormation allows developers to define their infrastructure as code using templates. These templates describe the desired resources and configurations in a declarative manner. By using CloudFormation, developers can easily create, manage, and update their infrastructure stacks, ensuring consistency and repeatability across different environments.
AWS Ground Station (option A) is a service for satellite communications.
AWS Shield (option B) is a managed Distributed Denial of Service (DDoS) protection service.
AWS IoT Device Defender (option C) is a security service for IoT devices. Therefore, none of these options are suitable for maintaining development and production infrastructure in a repeatable fashion.

 
---

Q54. Which of the following are advantages of the AWS Cloud? (Select TWO.)

- A. Trade variable expenses for capital expenses
- [x] B. High economies of scale
- [x] C. Launch globally in minutes
- D. Focus on managing hardware infrastructure
- E. Overprovision to ensure capacity

 

---

Q55. Which actions are the responsibility of AWS, according to the AWS shared responsibility model? (Select TWO)

- [x] A. Securing the virtualization layer
- B. Patching the operating system on Amazon EC2 instances
- C. Enforcing a strict password policy for IAM users
- [x] D. Patching the operating system on Amazon RDS instances
- E. Configuring security groups and network ACLS

 

---

Q56. A company needs a central user portal so that users can log in to third-party business applications that support Security Assertion Markup Language (SAML). Which AWS service will meet this requirement?

- A. AWS Identity and Access Management (IAM)
- B. Amazon Cognito
- [x] C. AWS Single Sign-On
- D. AWS CLI


---



Q57. What is the customer ALWAYS responsible for managing, according to the AWS shared responsibility model?

- A. Software licenses
- B. Networking
- [x] C. Customer data
- D. Encryption keys




While AWS manages and maintains the underlying infrastructure and services, customers are ultimately responsible for the management and protection of their own data stored on AWS. This includes tasks such as data classification, encryption, access control, backups, and compliance with applicable regulations and data protection laws.
Options A, B, and D may be managed by either AWS or the customer depending on the specific service or feature being used:
A. Software licenses: The responsibility for managing software licenses can vary depending on the specific software being used. Some AWS services include the necessary licenses, while for others, customers may need to provide their own licenses.
B. Networking: AWS provides a range of networking capabilities, including virtual private clouds (VPCs), subnets, routing, and security groups. While AWS manages the underlying network infrastructure, customers are responsible for configuring and managing their own networking within the AWS environment.
D. Encryption keys: AWS offers various encryption options, including managed encryption services. Customers are responsible for managing their own encryption keys, including the creation, rotation, and storage of these keys when using AWS encryption services.


---


Q58. A company needs to perform data processing once a week that typically takes about 5 hours to complete. Which AWS service should the company use for this workload?

- A. AWS Lambda
- [x] B. Amazon EC2
- C. AWS CodeDeploy
- D. AWS Wavelength

A. AWS Lambda:
Maximum execution time is 15 minutes ❌. Unsuitable for 5-hour jobs.

C. AWS CodeDeploy: A deployment service for applications (e.g., EC2, Lambda), not a compute service ❌.

D. AWS Wavelength: Designed for ultra-low-latency edge computing (e.g., 5G applications), not batch processing ❌

AWS Wavelength: Run applications using AWS Infrastructure and services in AWS telco (telecommunications company) partners' data centers to meet your low latency, data residency, and resiliency needs. https://aws.amazon.com/wavelength/

---


> [!IMPORTANT]
> Q59. A company that uses AWS needs to transfer 2 TB of data. Which type of transfer of that data would result in no cost for the company?

- [x] A. Inbound data transfer from the internet
- B. Outbound data transfer to the internet
- C. Data transfer between AWS Regions
- D. Data transfer between Availability Zones

Inbound data transfer from the internet to AWS services does not incur any additional charges. AWS does not charge for data transferred into their services from the internet. Therefore, if a company needs to transfer 2 TB of data into their AWS environment from the internet, there would be no cost associated with this transfer.
Options B, C, and D all involve data transfer within the AWS network and may incur costs based on the specific region, service, and amount of data transferred.
B. Outbound data transfer to the internet: Data transferred from AWS services to the internet is subject to outbound data transfer costs.
C. Data transfer between AWS Regions: Data transferred between different AWS regions will incur data transfer costs.
D. Data transfer between Availability Zones: Data transferred between Availability Zones within the same region may also incur data transfer costs.
Therefore, the only option that would result in no cost for the company is A, inbound data transfer from the internet.


---

> [!IMPORTANT]
> Q60. Which AWS services or features provide disaster recovery solutions for Amazon EC2 instances? (Select TWO.)

- A. EC2 Reserved Instances
- [x] B. EC2 Amazon Machine Images (AMIs)
- [x] C. Amazon Elastic Block Store (Amazon EBS) snapshots
- D. AWS Shield
- E. Amazon GuardDuty

 
EC2 Amazon Machine Images (AMIs) (option B) can be used for disaster recovery solutions for Amazon EC2 instances. AMIs are essentially a template that contains the root file system and configuration settings of an EC2 instance. By creating regular backups or snapshots of your EC2 instances as AMIs, you can quickly launch new instances from these images in the event of a failure or disaster.

Amazon Elastic Block Store (Amazon EBS) snapshots (option C) can also be used for disaster recovery solutions for EC2 instances. EBS snapshots capture incremental changes to your EBS volumes, allowing you to create backups of your data and configurations. These snapshots can be used to restore EBS volumes or create new volumes in the event of a failure or disaster.

Options A, D, and E are not directly related to disaster recovery solutions for EC2 instances:
A. EC2 Reserved Instances: Reserved Instances are a pricing option for EC2 instances and do not provide specific disaster recovery functionality.
D. AWS Shield: AWS Shield is a managed Distributed Denial of Service (DDoS) protection service and is focused on protecting your applications from DDoS attacks rather than providing disaster recovery solutions.
E. Amazon GuardDuty: Amazon GuardDuty is a threat detection service that helps identify potential security threats and unauthorized activities in your AWS environment. While it contributes to overall security, it is not specifically designed for disaster recovery purposes.

You can back up Amazon EC2 instances used by your workload as Amazon Machine Images (AMIs). The AMI is created from snapshots of your instance's root volume and any other EBS volumes attached to your instance. You can use this AMI to launch a restored version of the EC2 instance. The AWS services or features that provide disaster recovery solutions for Amazon EC2 instances are:
C. Amazon Elastic Block Store (Amazon EBS) snapshots: Amazon EBS is a block storage service for use with Amazon EC2 instances. EBS snapshots are point-in-time copies of an EBS volume that can be used to create a new volume or restore an existing volume. EBS snapshots can be used to recover data in the event of an instance failure, or to create a new instance in a different region or Availability Zone.
B. Amazon Machine Images (AMIs): An AMI is a pre-configured virtual machine image that contains the operating system, application software, and any other required components needed to launch an instance. AMIs can be used to create new instances in the same or a different region, which can be useful for disaster recovery purposes.



---

Q61. A company has a set of ecommerce applications. The applications need to be able to send messages to each other. Which AWS service meets this requirement?

- A. AWS Auto Scaling
- B. Elastic Load Balancing
- [x] C. Amazon Simple Queue Service (Amazon SQS)
- D. Amazon Kinesis Data Streams



Amazon Simple Queue Service (Amazon SQS)  is a fully managed message queuing service that enables reliable and scalable communication between distributed software components and microservices. Applications can send messages to an SQS queue, and other applications can retrieve and process those messages asynchronously.

Options A and B, AWS Auto Scaling and Elastic Load Balancing, are services focused on scaling and load balancing infrastructure resources and do not provide direct messaging capabilities between applications.

Option D, Amazon Kinesis Data Streams, is a service for real-time streaming data processing, which is suitable for scenarios where large amounts of data need to be processed in real-time rather than facilitating direct messaging between applications.


---


> [!IMPORTANT]
> Q62. Which action will help increase security in the AWS Cloud?

- A. Enable programmatic access for all IAM users.
- B. Use IAM users instead of IAM roles to delegate permissions
- [x] C. Rotate access keys on a reoccurring basis
- D. Use inline policies instead of customer managed policies



Using IAM roles instead of IAM users (B) is generally considered a best practice for delegating permissions, as roles provide temporary credentials that can be assumed by trusted entities and automatically rotated by AWS. 

Using inline policies (D) instead of customer managed policies can also be more error-prone and difficult to manage at scale, as they are attached directly to individual users or groups rather than separated into reusable policies.


---

Q63. Which AWS service is a key-value database that provides sub-millisecond latency on a large scale?

- [x] A. Amazon DynamoDB
- B. Amazon Aurora
- C. Amazon DocumentDB (with MongoDB compatibility)
- D. Amazon Neptune



Option B, Amazon Aurora, is a relational database service provided by AWS. While Aurora provides high performance and scalability, it is not specifically a key-value database.
Option C, Amazon DocumentDB (with MongoDB compatibility), is a document database service provided by AWS that is compatible with MongoDB's API and supports querying and indexing JSON-like documents. It is not a key-value database.

Note: MongoDB is a source-available, cross-platform, document-oriented database program. Classified as a NoSQL database product, MongoDB uses JSON-like documents with optional schemas. 

Option D, Amazon Neptune, is a graph database service provided by AWS that is optimized for storing and querying highly connected data such as relationships and networks. It is not a key-value database either.

---

> [!IMPORTANT]
> Q64. A company is planning to move data backups to the AWS Cloud. The company needs to replace on-premises storage with storage that is cloud-based but locally cached. Which AWS service meets these requirements?

- [x] A. AWS Storage Gateway
- B. AWS Snowcone
- C. AWS Backup
- D. Amazon Elastic File System (Amazon EFS)

> locally cached

AWS Storage Gateway is the AWS service that meets the requirements of replacing on-premises storage with cloud-based storage that can be locally cached. It is a hybrid cloud storage service that enables seamless integration between on-premises applications and AWS storage infrastructure. One of its features is the ability to provide a local cache for frequently accessed data, allowing applications to access data quickly while still storing the primary data in the cloud.
Option B, AWS Snowcone, is a portable and rugged storage device designed for edge computing and offline data transfer scenarios. While it can be used for data backups, it does not provide the capability of locally caching data for ongoing access.
Option C, AWS Backup, is a fully managed backup service provided by AWS. It supports backing up various AWS services and on-premises resources to the cloud, but it does not provide local caching of data.
Option D, Amazon Elastic File System (Amazon EFS), is a scalable and fully managed file storage service provided by AWS. While it offers cloud-based storage, it does not provide a local cache for data.

---

> [!IMPORTANT]
> Q65. Which actions are examples of a company's effort to rightsize its AWS resources to control cloud costs? (Select TWO.)

- A. Switch from Amazon RDS to Amazon DynamoDB to accommodate NoSQL datasets.
- [x] B. Base the selection of Amazon EC2 instance types on past utilization patterns
- [x] C. Use Amazon S3 Lifecycle policies to move objects that users access infrequently to lower-cost storage tiers
- D. Use Multi-AZ deployments for Amazon RDS
- E. Replace existing Amazon EC2 instances with AWS Elastic Beanstalk


Basing the selection of Amazon EC2 instance types on past utilization patterns (option B) allows a company to rightsize its resources by choosing instances that align with their actual workload requirements. This helps avoid overprovisioning and reduces unnecessary costs.
Using Amazon S3 Lifecycle policies to move objects that users access infrequently to lower-cost storage tiers (option C) is another way to control costs. By automatically transitioning less frequently accessed objects to lower-cost storage classes, such as Amazon S3 Glacier or Amazon S3 Deep Archive, companies can optimize storage costs without sacrificing accessibility to the data.
Option A, switching from Amazon RDS to Amazon DynamoDB to accommodate NoSQL datasets, may or may not be a cost-saving measure, depending on the specific use case and workload requirements. It is primarily a consideration for database technology selection rather than rightsizing AWS resources for cost control.
Option D, using Multi-AZ deployments for Amazon RDS, is a high availability and fault-tolerant configuration option but does not directly relate to rightsizing resources for cost control.
Option E, replacing existing Amazon EC2 instances with AWS Elastic Beanstalk, is a deployment platform and management service and does not specifically address rightsizing AWS resources for cost control.

---

Q66. A company needs to organize its resources and track AWS costs on a detailed level. The company needs to categorize costs by business department, environment, and application. Which solution will meet these requirements?

- A. Access the AWS Cost Management console to organize resources, set an AWS budget, and receive notifications of unintentional usage
- [x] B. Use tags to organize the resources. Activate cost allocation tags to track AWS costs on a detailed level
- C. Create Amazon CloudWatch dashboards to visually organize and track costs individually.
- D. Access the AWS Billing and Cost Management dashboard to organize and track resource consumption on a detailed level
 
  
 
AWS provides cost allocation tags that can be applied to resources such as Amazon EC2 instances, Amazon S3 buckets, and others for tracking and managing costs. By using tags, the company can easily categorize costs according to business department, environment, or application.
Option A is incorrect because while it allows you to set a budget and receive notifications of unintentional usage, it does not directly address the requirement to categorize costs by business department, environment, and application. Option C, creating Amazon CloudWatch dashboards, is useful for monitoring but does not directly address the requirement to categorize costs in detail. Option D, accessing the AWS Billing and Cost Management dashboard, provides visibility into resource consumption but may not provide granular enough views to categorize costs by department, environment, or application.

 
B. Use tags to organize the resources. Activate cost allocation tags to track AWS costs on a detailed level.
Tags are key-value pairs that can be assigned to AWS resources to help categorize and organize them. Cost allocation tags, specifically, are used to categorize costs across multiple AWS services and can be applied to EC2 instances, S3 buckets, RDS databases, and other resources. By using cost allocation tags, the company can track AWS costs on a detailed level, categorized by business department, environment, and application.
Let's break down the other options:
A. Access the AWS Cost Management console to organize resources, set an AWS budget, and receive notifications of unintentional usage. While the Cost Management console is useful for setting budgets and receiving notifications, it doesn't directly address the requirement of organizing resources and tracking costs by department, environment, and application unless tags are used in conjunction. C. Create Amazon CloudWatch dashboards to visually organize and track costs individually. CloudWatch dashboards are used for monitoring metrics and creating visualizations, but they are not designed for tracking costs.
D. Access the AWS Billing and Cost Management dashboard to organize and track resource consumption on a detailed level. The Billing and Cost Management dashboard provides an overview of costs and resource usage, but without cost allocation tags, it won't allow the company to categorize costs by department, environment, and application.
Therefore, the correct answer is B. Use tags to organize the resources and activate cost allocation tags to track AWS costs on a detailed level.



---

Q67. A company wants to grant users in one AWS account access to resources in another AWS account. The users do not currently have permission to access the Resources. Which AWS service will meet this requirement?

- A. IAM group
- [x] B. IAM role
- C. IAM tag
- D. IAM Access Analyzer

To grant users in one AWS account access to resources in another AWS account, you can use IAM roles. IAM roles are a secure way to delegate access to resources within and across AWS accounts. By creating a role in the target AWS account and defining the desired permissions, you can then grant users from the source AWS account temporary access to assume that role and access the resources.
IAM groups (A) are used to organize IAM users and apply common permissions to multiple users at once within the same AWS account. They do not provide cross-account access.
IAM tags (C) are key-value pairs that can be attached to IAM entities (users, groups, roles) for easier management and policy-based permissions. While they can help with organization and tagging of resources, they do not directly provide cross-account access.
IAM Access Analyzer (D) is a service that helps identify unintended access and resource sharing within your AWS environment by analyzing resource policies. It does not provide the ability to grant cross-account access.

---

Q68 is the same as Q53

---

> [!IMPORTANT]
> Q69. A company wants a time-series database service that makes it easier to store and analyze trillions of events each day. Which AWS service will meet this requirement?

- A. Amazon Neptune
- [x] B. Amazon Timestream
- C. Amazon Forecast
- D. Amazon DocumentDB (with MongoDB compatibility)

> Keywords: time-series database 

Amazon Timestream is the AWS service that is designed specifically for storing and analyzing trillions of time-series events per day. It provides a purpose-built, serverless database that can handle high-volume and high-velocity data streams. With Timestream, you can easily ingest, store, and query time-series data for various use cases such as IoT applications, log analytics, and monitoring.

Amazon Neptune (A) is a fully managed graph database service that is optimized for storing and querying highly connected data. 

Amazon Forecast (C) is a service that uses machine learning to generate accurate forecasts for time-series data. While it is useful for forecasting future trends, it is not intended for storing and analyzing large volumes of time-series events.

Amazon DocumentDB (with MongoDB compatibility) (D) is a fully managed, MongoDB-compatible document database service.  

---

Q70. A company wants to modernize and convert a monolithic application into microservices. The company wants to move the application to AWS. Which migration strategy should the company use?

- A. Rehost
- B. Replatform
- C. Repurchase
- [x] D. Refactor



> The company should use the migration strategy of refactoring to modernize and convert a monolithic application into microservices when moving it to AWS. Refactoring involves restructuring the application's architecture and codebase to break it down into smaller, loosely coupled, and independently deployable microservices. This approach allows for improved scalability, agility, and maintainability of the application.
> Rehost (A), also known as lift-and-shift, involves migrating the application to AWS without making any significant changes to its architecture or code. It may provide minimal benefits in terms of scalability and cost optimization but does not achieve the full potential of a microservices architecture.
> Replatform (B) involves making some modifications to the application's architecture or infrastructure components while preserving most of its existing functionality. While this can offer some improvements, it may not fully leverage the advantages of microservices.
> Repurchase (C) refers to replacing the existing application with a different off-the-shelf software solution. This strategy is not applicable for converting a monolithic application into microservices on AWS.

---



Q71. A company needs to run a pre-installed third-party firewall on an Amazon EC2 Instance. Which AWS service or feature can provide this solution?

- A. Network ACLs
- B. Security groups
- [x] C. AWS Marketplace
- D. AWS Trusted Advisor


---


Q72. A company wants to migrate its on-premises relational databases to the AWS Cloud. The company wants to use infrastructure as close to its current geographical location as possible. Which AWS service or resource should the company use to select its Amazon RDS deployment area?

- A. Amazon Connect
- B. AWS Wavelength
- [x] C. AWS Regions
- D. AWS Direct Connect


---

> [!IMPORTANT]
> Q73. Which AWS service provides a single location to track the progress of application migrations?

- A. AWS Application Discovery Service
- B. AWS Application Migration Service
- C. AWS Service Catalog
- [x] D. AWS Migration Hub



AWS Migration Hub provides a single location to track the progress of application migrations. It allows you to monitor and track the migration of your applications across multiple AWS services, such as AWS Server Migration Service, AWS Database Migration Service, and others. With Migration Hub, you can view the status of each migration task, track resource utilization, and access detailed migration reports.
AWS Application Discovery Service (A) is a separate AWS service that helps you discover and understand your existing on-premises applications and their dependencies. While it can provide insights for planning migrations, it does not track the progress of application migrations.
AWS Application Migration Service (B) is a service designed specifically for migrating applications to AWS. However, it does not provide a single location to track the progress of application migrations.
AWS Service Catalog (C) is a service that allows organizations to create and manage catalogs of IT services that can be provisioned by end-users. It does not specifically track application migration progress.

--- 

Q74 is the same as Q30

---


Q75 is the same as Q31

---

Q76. Which AWS service or tool gives users the ability to connect with AWS and deploy resources programmatically?

- A. Amazon QuickSight
- B. AWS PrivateLink
- C. AWS Direct Connect
- [x] D. AWS SDKs

AWS SDKs (Software Development Kits) give users the ability to connect with AWS and deploy resources programmatically. The AWS SDKs are sets of libraries and tools that provide APIs (Application Programming Interfaces) for various programming languages, allowing developers to interact with AWS services directly from their code. By using the AWS SDKs, developers can automate the creation, management, and configuration of AWS resources.

Amazon QuickSight (A) is a business intelligence and data visualization service. While it allows users to connect to and analyze data in AWS, it does not provide the ability to deploy resources programmatically.

AWS PrivateLink (B) is a networking feature that enables private connectivity between VPCs (Virtual Private Clouds), AWS services, and on-premises applications over the AWS network without exposing traffic to the public internet. It is not specifically designed for connecting with AWS and deploying resources programmatically.

AWS Direct Connect (C) is a network service that provides dedicated private network connections between on-premises environments and AWS. While it enables reliable and secure connectivity to AWS, it does not offer direct programmable access to AWS services.
 

---

Q77. A company plans to use an Amazon Snowball Edge device to transfer files to the AWS Cloud. Which activities related to a Snowball Edge device are available to the company at no cost?

- A. Use of the Snowball Edge appliance for a 10-day period
- B. The transfer of data out of Amazon S3 and to the Snowball Edge appliance
- [x] C. The transfer of data from the Snowball Edge appliance into Amazon S3
- D. Daily use of the Snowball Edge appliance after 10 days

---

Q78. A company has deployed applications on Amazon EC2 instances. The company needs to assess application vulnerabilities and must identify infrastructure deployments that do not meet best practices. Which AWS service can the company use to meet these requirements?

- A. AWS Trusted Advisor
- [x] B. Amazon Inspector
- C. AWS Config
- D. Amazon GuardDuty
 

> A. AWS Trusted Advisor: Provides recommendations for cost optimization, performance, security, fault tolerance, and service limits. However, it focuses on account-level best practices and does not perform deep application vulnerability scanning.

> B. Amazon Inspector: An automated vulnerability management service that scans applications on EC2 instances for software vulnerabilities and deviations from security best practices. It assesses application vulnerabilities (e.g., CVEs) and checks infrastructure against AWS security best practices, making it suitable for both requirements.

> C. AWS Config: Tracks resource configurations and compliance over time. It helps identify infrastructure deviations from desired configurations but does not assess application-level vulnerabilities.

> D. Amazon GuardDuty: A threat detection service that monitors for malicious activity using machine learning and threat intelligence. It focuses on security threats, not vulnerability assessments or best practice checks for infrastructure deployments.

  
---

Q79. A company has a centralized group of users with large file storage requirements that have exceeded the space available on premises. The company wants to extend its file storage capabilities for this group while retaining the performance benefit of sharing content locally. What is the MOST operationally efficient AWS solution for this scenario?

- A. Create an Amazon S3 bucket for each user. Mount each bucket by using an S3 file system mounting utility.
- [x] B. Configure and deploy an AWS Storage Gateway file gateway. Connect each user's workstation to the file gateway.
- C. Move each user's working environment to Amazon WorkSpaces. Set up an Amazon WorkDocs account for each user.
- D. Deploy an Amazon EC2 instance and attach an Amazon Elastic Block Store (Amazon EBS) Provisioned IOPS volume. Share the EBS volume directly with the users.

---

Q80. According to security best practices, how should an Amazon EC2 instance be given access to an Amazon S3 bucket?

- A. Hard code an IAM user's secret key and access key directly in the application, and upload the file.
- B. Store the IAM user's secret key and access key in a text file on the EC2 instance, read the keys, then upload the file.
- [x] C. Have the EC2 instance assume a role to obtain the privileges to upload the file.
- D. Modify the S3 bucket policy so that any service can upload to it at any time.


---
> [!IMPORTANT]
> Q81. Which option is a customer responsibility when using Amazon DynamoDB under the AWS Shared Responsibility Model?

- A. Physical security of DynamoDB
- B. Patching of DynamoDB
- [x] C. Access to DynamoDB tables
- D. Encryption of data at rest in DynamoDB

<img width="905" alt="image" src="https://github.com/user-attachments/assets/c04c09c8-3999-4028-bc47-b8f106f600c3" />

encryption is enforced. cannout be opted out

Encryption at rest: All user data stored in Amazon DynamoDB is fully encrypted at rest. By default, Amazon DynamoDB manages the encryption key, and you are not charged any fee for using it.

Encryption key management
- Owned by Amazon DynamoDB (used by multiple accounts https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#aws-owned-cmk): The AWS KMS key is owned and managed by DynamoDB. You are not charged an additional fee for using this key.
- AWS managed key Learn: Key alias: aws/dynamodb. The key is stored in your account and is managed by AWS Key Management Service (AWS KMS). AWS KMS charges apply.
- Stored in your account, and owned and managed by you: The key is stored in your account and is owned and managed by you. AWS KMS charges apply.

So, while customers can choose KMS keys (customer-managed keys), enabling/configuring encryption is done via DynamoDB settings. The act of encrypting/decrypting data is handled by AWS .

 

Data in transit: All your data in DynamoDB is encrypted in transit. By default, communications to and from DynamoDB use the HTTPS protocol, which protects network traffic by using Secure Sockets Layer (SSL)/Transport Layer Security (TLS) encryption.

Data in use: Protect your data before sending it to DynamoDB using client-side encryption.
https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/encryption.usagenotes.html


---


Q82. Which option is a perspective that includes foundational capabilities of the AWS Cloud Adoption Framework (AWS CAF)?

- A. Sustainability
- B. Performance efficiency
- [x] C. Governance
- D. Reliability

---


Q83. A company is running and managing its own Docker environment on Amazon EC2 instances. The company wants an alternative to help manage cluster size, scheduling, and environment maintenance. Which AWS service meets these requirements?

- A. AWS Lambda
- B. Amazon RDS
- [x] C. AWS Fargate
- D. Amazon Athena

---


Q84. A company wants to run a NoSQL database on Amazon EC2 instances. Which task is the responsibility of AWS in this scenario?

- A. Update the guest operating system of the EC2 instances.
- B. Maintain high availability at the database layer.
- [x] C. Patch the physical infrastructure that hosts the EC2 instances.
- D. Configure the security group firewall.


---

Q85. Which AWS services or tools can identify rightsizing opportunities for Amazon EC2 instances? (Choose two.)

- [x] A. AWS Cost Explorer
- B. AWS Billing Conductor
- C. Amazon CodeGuru
- D. Amazon SageMaker
- [x] E. AWS Compute Optimizer


AWS Cost Explorer: 
- Provides rightsizing recommendations by analyzing EC2 resource utilization (CPU, memory, network, disk I/O) over the past 14 days to identify underutilized or idle instances;
- Generates actionable insights (e.g., downsizing instance types or terminating idle instances) with estimated savings in the AWS Billing Console;
- Supports filtering by tags to attribute costs to departments or projects, aligning with financial accountability.

AWS Compute Optimizer:

- Uses machine learning to analyze EC2 utilization metrics (vCPU, memory, network) and recommends optimal instance types based on workload patterns;
- Offers customizable preferences (e.g., CPU headroom, 32-day lookback period) to tailor recommendations for performance or cost savings;
- Extends recommendations to EC2 Auto Scaling Groups, ensuring scaling policies align with cost efficiency 28.

Why Not the Others?
B. AWS Billing Conductor: A billing customization tool for consolidating invoices and applying pricing rules—not designed for resource optimization.

C. Amazon CodeGuru: Focuses on code quality review (performance issues, security flaws) via ML—unrelated to infrastructure rightsizing.

D. Amazon SageMaker: A managed service for machine learning workflows—does not provide infrastructure optimization insights


---

> [!IMPORTANT]
> Q86. Which of the following are benefits of using AWS Trusted Advisor? (Choose two.)

- A. Providing high-performance container orchestration
- B. Creating and rotating encryption keys
- [x] C. Detecting underutilized resources to save costs
- [x] D. Improving security by proactively monitoring the AWS environment
- E. Implementing enforced tagging across AWS resources

---

Q87. Which of the following is an advantage that users experience when they move on-premises workloads to the AWS Cloud?

- [x] A. Elimination of expenses for running and maintaining data centers
- B. Price discounts that are identical to discounts from hardware providers
- C. Distribution of all operational controls to AWS
- D. Elimination of operational expenses

---

> [!IMPORTANT]
> Q88. A company wants to manage deployed IT services and govern its infrastructure as code (IaC) templates. Which AWS service will meet this requirement?

- A. AWS Resource Explorer
- [x] B. AWS Service Catalog
- C. AWS Organizations
- D. AWS Systems Manager


---

Q89. Which AWS service or tool helps users visualize, understand, and manage spending and usage over time?

- A. AWS Organizations
- B. AWS Pricing Calculator
- [x] C. AWS Cost Explorer
- D. AWS Service Catalog

---

Q90. A company is using a central data platform to manage multiple types of data for its customers. The company wants to use AWS services to discover, transform, and visualize the data. Which combination of AWS services should the company use to meet these requirements? (Choose two.)

- [x] A. AWS Glue
- B. Amazon Elastic File System (Amazon EFS)
- C. Amazon Redshift
- [x] D. Amazon QuickSight
- E. Amazon Quantum Ledger Database (Amazon QLDB)

---

> [!IMPORTANT]
> Q91. A global company wants to migrate its third-party applications to the AWS Cloud. The company wants help from a global team of experts to complete the migration faster and more reliably in accordance with AWS internal best practices. Which AWS service or resource will meet these requirements?

- A. AWS Support
- [x] B. AWS Professional Services
- C. AWS Launch Wizard
- D. AWS Managed Services (AMS)


---

Q92. An e-learning platform needs to run an application for 2 months each year. The application will be deployed on Amazon EC2 instances. Any application downtime during those 2 months must be avoided. Which EC2 purchasing option will meet these requirements MOST cost-effectively?

- A. Reserved Instances
- B. Dedicated Hosts
- C. Spot Instances
- [x] D. On-Demand Instances


---

Q93. A developer wants to deploy an application quickly on AWS without manually creating the required resources. Which AWS service will meet these requirements?

- A. Amazon EC2
- [x] B. AWS Elastic Beanstalk
- C. AWS CodeBuild
- D. Amazon Personalize

---

> [!IMPORTANT]
> Q94. A company is storing sensitive customer data in an Amazon S3 bucket. The company wants to protect the data from accidental deletion or overwriting. Which S3 feature should the company use to meet these requirements?

- A. S3 Lifecycle rules
- [x] B. S3 Versioning
- C. S3 bucket policies
- D. S3 server-side encryption

---

Q95. Which AWS service provides the ability to manage infrastructure as code?

- A. AWS CodePipeline
- B. AWS CodeDeploy
- C. AWS Direct Connect
- [x] D. AWS CloudFormation

---

Q97. Which AWS service or feature allows a user to establish a dedicated network connection between a company's on-premises data center and the AWS Cloud?

- [x] A. AWS Direct Connect
- B. VPC peering
- C. AWS VPN
- D. Amazon Route 53

---
Q98. Which option is a physical location of the AWS global infrastructure?

- A. AWS DataSync
- [x] B. AWS Region
- C. Amazon Connect
- D. AWS Organizations

---

Q99. A company wants to protect its AWS Cloud information, systems, and assets while performing risk assessment and mitigation tasks. Which pillar of the AWS Well-Architected Framework is supported by these goals?

- A. Reliability
- [x] B. Security
- C. Operational excellence
- D. Performance efficiency

---

Q100. What is the purpose of having an internet gateway within a VPC?

- A. To create a VPN connection to the VPC
- [x] B. To allow communication between the VPC and the internet
- C. To impose bandwidth constraints on internet traffic
- D. To load balance traffic from the internet across Amazon EC2 instances


---

Q101. A company is running a monolithic on-premises application that does not scale and is difficult to maintain. The company has a plan to migrate the application to AWS and divide the application into microservices. Which best practice of the AWS Well-Architected Framework is the company following with this plan?

- A. Integrate functional testing as part of AWS deployment.
- B. Use automation to deploy changes.
- C. Deploy the application to multiple locations.
- [x] D. Implement loosely coupled dependencies.


The best practice of implementing loosely coupled dependencies aligns with the company's plan to migrate the monolithic on-premises application to AWS and divide it into microservices.

In a monolithic application, components are tightly coupled, meaning a change in one component can have a cascading effect on other components. This makes the application difficult to scale, maintain, and update. By dividing the application into microservices, the company aims to create smaller, independent services that are loosely coupled, allowing them to be developed, deployed, and scaled independently.

Here's how implementing loosely coupled dependencies relates to the company's plan:

Microservices architecture: Dividing the monolithic application into microservices involves breaking down the application into smaller, self-contained services that have well-defined boundaries. Each microservice can have its own codebase, data store, and communication mechanism. This architectural approach promotes loose coupling between the services, as they interact through well-defined APIs or messaging systems.

Scalability and maintenance: By implementing loosely coupled dependencies, the company can scale and maintain individual microservices independently. This allows them to scale specific services based on demand, update individual services without impacting others, and isolate failures to specific services rather than affecting the entire application.

Flexibility and agility: Loosely coupled dependencies enable faster development and deployment cycles. Teams can work independently on different microservices, allowing for parallel development and faster time-to-market. Changes or updates to one microservice can be deployed without affecting others, reducing the risk of unintended consequences.

By following the best practice of implementing loosely coupled dependencies, the company can achieve the benefits of a microservices architecture, including scalability, maintainability, flexibility, and agility.

---

Q102. A company has an AWS account. The company wants to audit its password and access key rotation details for compliance purposes. Which AWS service or tool will meet this requirement?

- A. IAM Access Analyzer
- B. AWS Artifact
- [x] C. IAM credential report
- D. AWS Audit Manager



> The IAM credential report is a built-in feature of AWS Identity and Access Management (IAM) that provides detailed information about the IAM users and their respective access keys, passwords, and other security-related information. The credential report can be generated on demand or scheduled to be generated periodically, such as daily, weekly, or monthly. Here's how the IAM credential report meets the requirement:
- Password information: The IAM credential report includes details about IAM users' password status, including when passwords were last used, when they were last rotated, and whether they are set to expire. This information helps in auditing password rotation practices and ensuring compliance with security policies.
- Access key information: The report also contains information about IAM users' access keys, including their creation date, last usage date, and rotation status. It provides insights into access key rotation practices, which is crucial for maintaining the security of AWS resources.

> By analyzing the IAM credential report, the company can identify users who have not rotated their passwords or access keys according to the desired policy, enabling them to take appropriate actions to ensure compliance and enhance security.

 

> A. IAM Access Analyzer: IAM Access Analyzer is a service that helps identify unintended access to resources by analyzing resource policies. While it can be useful for identifying potential security issues, it does not specifically provide password and access key rotation details for compliance purposes.

> B. AWS Artifact: AWS Artifact is a service that provides access to AWS compliance reports and other compliance-related documents. While it offers a range of compliance-related information, it does not specifically provide password and access key rotation details.

> D. AWS Audit Manager: AWS Audit Manager is a service that helps automate and simplify the process of auditing AWS resources for compliance with industry standards and regulations. While it can assist in compliance auditing, it does not specifically focus on password and access key rotation details.

---
> [!IMPORTANT]
> Q103. (Multiple choice) A company wants to receive a notification when a specific AWS cost threshold is reached. Which AWS services or tools can the company use to meet this requirement? (Choose two.)

- A. Amazon Simple Queue Service (Amazon SQS)
- [x] B. AWS Budgets
- C. Cost Explorer
- [x] D. Amazon CloudWatch
- E. AWS Cost and Usage Report


> AWS Budgets allows you to set custom cost or usage thresholds for your AWS account.
> Amazon CloudWatch: allow  setting up alarms based on predefined or custom metrics

B. AWS Budgets: AWS Budgets allows you to set custom cost or usage thresholds for your AWS account. You can create a budget and specify the desired threshold amount. When the actual costs reach or exceed the threshold, AWS Budgets can send notifications via email or Amazon Simple Notification Service (SNS) to alert you of the threshold breach.

D. Amazon CloudWatch: Amazon CloudWatch is a monitoring service that can be used to track and collect metrics, logs, and events from various AWS resources. It provides the capability to set up alarms based on predefined or custom metrics. You can create a CloudWatch alarm that triggers when the cost metric exceeds the specified threshold. The alarm can then send a notification via SNS, email, or other supported channels.

Let's briefly review the other options:

A. Amazon Simple Queue Service (Amazon SQS): Amazon SQS is a fully managed message queuing service. While it can be used for decoupling and distributing workloads, it is not directly applicable to receiving cost threshold notifications.

C. Cost Explorer: Cost Explorer is a tool within the AWS Management Console that provides visualization and analysis of your AWS costs and usage. While it can help you analyze historical costs and usage patterns, it does not provide real-time notifications for cost threshold breaches.

E. AWS Cost and Usage Report: AWS Cost and Usage Report provides a detailed, comprehensive report of your AWS costs and usage. However, it is not a real-time monitoring or notification tool.

---

Q104. Which AWS service or resource provides answers to the most frequently asked security-related questions that AWS receives from its users?

- A. AWS Artifact
- B. Amazon Connect
- C. AWS Chatbot
- [x] D. AWS Knowledge Center

---

> [!IMPORTANT]
> Q105. (Multiple choice) Which tasks are customer responsibilities, according to the AWS shared responsibility model? (Choose two.)

- [x] A. Configure the AWS provided security group firewall.
- [x] B. Classify company assets in the AWS Cloud.
- C. Determine which Availability Zones to use for Amazon S3 buckets.
- D. Patch or upgrade Amazon DynamoDB.
- E. Select Amazon EC2 instances to run AWS Lambda on.


According to the AWS shared responsibility model, customers are responsible for security and management of the content, applications, and access to their AWS resources, while AWS is responsible for the security of the cloud infrastructure that runs those services. Based on this model, the customer responsibilities for the given tasks are:
A. Configure the AWS provided security group firewall. - This is a customer responsibility. Customers need to configure security groups to control inbound and outbound traffic to their EC2 instances and other resources.
B. Classify company assets in the AWS Cloud. - This is also a customer responsibility. Customers are responsible for classifying their data and assets in the cloud to ensure compliance with relevant regulations and internal policies.
C. Determine which Availability Zones to use for Amazon S3 buckets. - Availability Zones (AZs) are managed by AWS. Amazon S3 abstracts AZ selection from customers, automatically replicating data across AZs

D. Patch or upgrade Amazon DynamoDB. - This is not a customer responsibility. AWS is responsible for patching and upgrading the underlying infrastructure and software of its managed services like DynamoDB.
E. Select Amazon EC2 instances to run AWS Lambda on. -  AWS Lambda is a serverless compute service that runs code without provisioning or managing servers. It does not run on EC2 instances directly in the traditional sense. Customers configure Lambda functions and AWS handles the underlying compute resources, including scaling, patching, and upgrades.
 

---

Q106. (Multiple choice) Which of the following are pillars of the AWS Well-Architected Framework? (Choose two.)

- A. Availability
- [x] B. Reliability
- C. Scalability
- D. Responsive design
- [x] E. Operational excellence

---

> [!IMPORTANT]
> Q107. Which AWS service or feature is used to send both text and email messages from distributed applications?

- [x] A. Amazon Simple Notification Service (Amazon SNS)
- B. Amazon Simple Email Service (Amazon SES)
- C. Amazon CloudWatch alerts
- D. Amazon Simple Queue Service (Amazon SQS)


---


Q108. A user needs programmatic access to AWS resources through the AWS CLI or the AWS API. Which option will provide the user with the appropriate access?

- A. Amazon Inspector
- [x] B. Access keys
- C. SSH public keys
- D. AWS Key Management Service (AWS KMS) keys

> Access keys (comprising an Access Key ID and Secret Access Key) are explicitly designed for programmatic access to AWS services via the AWS CLI, SDKs, or API.
 

---


Q109. A company runs thousands of simultaneous simulations using AWS Batch. Each simulation is stateless, is fault tolerant, and runs for up to 3 hours. Which pricing model enables the company to optimize costs and meet these requirements?

- A. Reserved Instances
- [x] B. Spot Instances
- C. On-Demand Instances
- D. Dedicated Instances

> keyword: stateless; fault tolerance
---

Q110. (Multiple choice) What does the concept of agility mean in AWS Cloud computing? (Choose two.)

- [x]  A. The speed at which AWS resources are implemented
- B. The speed at which AWS creates new AWS Regions
- [x] C. The ability to experiment quickly
- D. The elimination of wasted capacity
- E. The low cost of entry into cloud computing


---

Q111. A company needs to block SQL injection attacks. Which AWS service or feature can meet this requirement?

- [x] A. AWS WAF
- B. AWS Shield
- C. Network ACLs
- D. Security groups

---

> [!IMPORTANT]
> Q112. Which AWS service or feature identifies whether an Amazon S3 bucket or an IAM role has been shared with an external entity?

- A. AWS Service Catalog
- B. AWS Systems Manager
- [x] C. AWS IAM Access Analyzer
- D. AWS Organizations

https://github.com/justinjiajia/certifications/tree/main/aws/service_img_demo/iam/iam_access_analyser

---

Q113. A cloud practitioner needs to obtain AWS compliance reports before migrating an environment to the AWS Cloud. How can these reports be generated?

- A. Contact the AWS Compliance team.
- [x] B. Download the reports from AWS Artifact.
- C. Open a case with AWS Support.
- D. Generate the reports with Amazon Macie.

---

Q114. An ecommerce company has migrated its IT infrastructure from an on-premises data center to the AWS Cloud. Which cost is the company's direct responsibility?

- [x] A. Cost of application software licenses
- B. Cost of the hardware infrastructure on AWS
- C. Cost of power for the AWS servers
- D. Cost of physical security for the AWS data center


---

Q115. A company is setting up AWS Identity and Access Management (IAM) on an AWS account. Which recommendation complies with IAM security best practices?

- A. Use the account root user access keys for administrative tasks.
- B. Grant broad permissions so that all company employees can access the resources they need.
- [x] C. Turn on multi-factor authentication (MFA) for added security during the login process.
- D. Avoid rotating credentials to prevent issues in production applications.

---

Q116. Elasticity in the AWS Cloud refers to which of the following? (Choose two.)

- A. How quickly an Amazon EC2 instance can be restarted
- [x] B. The ability to rightsize resources as demand shifts
- C. The maximum amount of RAM an Amazon EC2 instance can use
- D. The pay-as-you-go billing model
- [x] E. How easily resources can be procured when they are needed


---

Q117. Which service enables customers to audit API calls in their AWS accounts?

- [x] A. AWS CloudTrail
- B. AWS Trusted Advisor
- C. Amazon Inspector
- D. AWS X-Ray

---

Q118. What is a customer responsibility when using AWS Lambda according to the AWS shared responsibility model?

- [x] A. Managing the code within the Lambda function
- B. Confirming that the hardware is working in the data center
- C. Patching the operating system
- D. Shutting down Lambda functions when they are no longer in use

---

Q119. A company has 5 TB of data stored in Amazon S3. The company plans to occasionally run queries on the data for analysis. Which AWS service should the company use to run these queries in the MOST cost-effective manner?

- A. Amazon Redshift
- [x] B. Amazon Athena
- C. Amazon Kinesis
- D. Amazon RDS

---

> [!IMPORTANT]
> Q120. Which AWS service can be used at no additional cost?

- A. Amazon SageMaker
- B. AWS Config
- [x] C. AWS Organizations
- D. Amazon CloudWatch


AWS Organizations: always free, with no usage-based charges. It enables centralized management of multiple AWS accounts (e.g., consolidated billing, policy enforcement, organizational units) without any fees.
 
A. Amazon SageMaker	Offers limited free tiers (e.g., 4,000 free API requests, 20 MB metadata storage), but compute/storage usage incurs charges beyond free limits.

B. AWS Config	Charges for configuration items ($0.003–$0.012/item), rule evaluations ($0.001–$0.0005/evaluation), and conformance packs. Free tier only covers first 7,500 config items.


D. Amazon CloudWatch:	Free tier includes 5 GB log storage, 10 custom metrics, and 3 dashboards. Exceeding these limits triggers charges (e.g., $0.50/GB for logs, $0.30/metric)

---

Q121. Which AWS Cloud Adoption Framework (AWS CAF) capability belongs to the people perspective?

- A. Data architecture (platform)
- B. Event management (operations)
- [x] C. Cloud fluency (people)
- D. Strategic partnership (business)


---

Q122. A company wants to make an upfront commitment for continued use of its production Amazon EC2 instances in exchange for a reduced overall cost. Which pricing options meet these requirements with the LOWEST cost? (Choose two.)

- A. Spot Instances
- B. On-Demand Instances
- [x] C. Reserved Instances
- [x] D. Savings Plans
- E. Dedicated Hosts


---

Q123. A company is exploring the use of the AWS Cloud, and needs to create a cost estimate for a project before the infrastructure is provisioned. Which AWS service or feature can be used to estimate costs before deployment?

- A. AWS Free Tier
- [x] B. AWS Pricing Calculator
- C. AWS Billing and Cost Management
- D. AWS Cost and Usage Report

---

> [!IMPORTANT]
> Q124. A company is building an application that needs to deliver images and videos globally with minimal latency. Which approach can the company use to accomplish this in a cost effective manner?

- [x] A. Deliver the content through Amazon CloudFront.
- B. Store the content on Amazon S3 and enable S3 cross-region replication.
- C. Implement a VPN across multiple AWS Regions.
- D. Deliver the content through AWS PrivateLink.


Low Latency: Uses 230+ global edge locations to cache and serve content closer to users, reducing latency by 30–50% compared to single-region solutions.

Cost Efficiency: Reduces origin load: Caches content at edges, lowering S3 data transfer/request costs.

Volume discounts: Bandwidth pricing drops significantly with usage (e.g., 10+ TB/month = $0.02–$0.04/GB).

Free tier: Includes 1 TB of data transfer and 10 million HTTP/HTTPS requests monthly.

Optimized Media Delivery: Supports video/image compression, adaptive bitrate streaming (HLS/DASH), and DDoS protection.

Why Not the Others?
Option	Key Flaws
B. S3 Cross-Region Replication (CRR)	Duplicates storage costs across regions ($0.023/GB/month per copy) and does not reduce latency (users still access content from S3 buckets in fixed regions, not edges).
C. VPN Across Regions	High latency (traffic routes through VPN gateways), complex/expensive setup ($0.05–$0.12/hour per VPN + data transfer fees). Not designed for content delivery.
D. AWS PrivateLink	Enables private VPC connectivity ($0.01/hour per endpoint + $0.01/GB data). Unusable for public content delivery and adds no latency benefits.


---
Q125. Which option is a benefit of the economies of scale based on the advantages of cloud computing?

- A. The ability to trade variable expense for fixed expense
- B. Increased speed and agility
- [x] C. Lower variable costs over fixed costs
- D. Increased operational costs across data centers


---

Q126. Which of the following is a software development framework that a company can use to define cloud resources as code and provision the resources through AWS CloudFormation?

- A. AWS CLI
- B. AWS Developer Center
- [x] C. AWS Cloud Development Kit (AWS CDK)
- D. AWS CodeStar

>AWS CodeStar Connections is a new feature that allows services like AWS CodePipeline to access third-party code source provider. For example, you can now seamlessly connect your Atlassian Bitbucket Cloud source repository to AWS CodePipeline. This allows you to automate  the build, test, and deploy phases of your release process each time a code change occurs.

>AWS renamed AWS CodeStar Connections to AWS CodeConnections. 

The AWS CDK is an open-source software development framework that enables developers to define cloud infrastructure using familiar programming languages (e.g., TypeScript, Python, Java, C#/.NET, Go) and provisions these resources through AWS CloudFormation136. Key features include:

Infrastructure as Code (IaC): 

Define AWS resources (e.g., EC2 instances, S3 buckets, Lambda functions) using high-level code constructs, reducing boilerplate and complexity. Behind the scenes, CDK synthesizes code into AWS CloudFormation templates for deployment.

Developer-Centric Workflow:

Leverage programming features like loops, conditionals, and object-oriented design to create reusable, modular components called constructs.

Integrates with IDEs for syntax highlighting, auto-completion, and testing.

Multi-Cloud and Hybrid Support:

Extend beyond AWS to manage resources in other clouds (e.g., Azure, GCP) via CloudFormation custom resources, enabling unified multicloud IaC.

Why Not the Others?
Option	Reason for Exclusion
A. AWS CLI	A command-line tool for interacting with AWS services—not a development framework for defining IaC.
B. AWS Developer Center: A resource hub for documentation and guides 
D. AWS CodeStar	A project management service for CI/CD pipelines—does not define or provision infrastructure


---

Q127. A company is developing an application that uses multiple AWS services. The application needs to use temporary, limited-privilege credentials for authentication with other AWS APIs. Which AWS service or feature should the company use to meet these authentication requirements?

- A. Amazon API Gateway
- B. IAM users
- [x] C. AWS Security Token Service (AWS STS)
- D. IAM instance profiles

> keywords: temporary; limited-privilege

Why AWS STS?
Temporary Credentials Generation:
AWS STS generates short-lived credentials (access key ID, secret access key, and session token) valid for minutes to hours, ensuring credentials automatically expire and cannot be reused. This minimizes security risks compared to long-term credentials.

Least-Privilege Enforcement:

Credentials inherit permissions from IAM roles or are restricted via session policies, ensuring applications only access necessary resources.

Example: An app assuming a role with S3 read-only access cannot modify or delete objects.

Dynamic Credential Delivery:

Integrates with AWS compute services (e.g., EC2, Lambda) to automatically deliver credentials via instance metadata or environment variables, eliminating manual key management.

For non-AWS workloads (e.g., on-premises), use IAM Roles Anywhere or federation APIs (AssumeRoleWithWebIdentity).

Use Cases:

Cross-account access: Assume roles in other AWS accounts.

Federated access: Authenticate via external identity providers (e.g., Google, Active Directory) using AssumeRoleWithSAML or AssumeRoleWithWebIdentity.

MFA-protected access: Generate credentials requiring multi-factor authentication via GetSessionToken.

❌ Why Not the Others?
Option	Reason for Exclusion
A. Amazon API Gateway	Manages API endpoints but does not issue credentials. Used for routing HTTP requests, not authentication.
B. IAM Users	Provides long-term access keys (never expire unless rotated manually), violating the "temporary" requirement and increasing security risks.
D. IAM Instance Profiles	Delivers temporary credentials only to EC2 instances via attached roles. Not usable for serverless (e.g., Lambda) or hybrid workloads


---


Q128. Which AWS service is a cloud security posture management (CSPM) service that aggregates alerts from various AWS services and partner products in a standardized format?

- [x] A. AWS Security Hub
- B. AWS Trusted Advisor
- C. Amazon EventBridge
- D. Amazon GuardDuty

standardized format: AWS Security Findings Format (ASFF).

B. AWS Trusted Advisor:	Provides cost/performance/security recommendations but cannot aggregate external alerts or normalize findings.
C. Amazon EventBridge:	An event bus for routing messages (e.g., S3 uploads) but lacks security-specific aggregation or CSPM capabilities.
D. Amazon GuardDuty:	A threat detection service for malicious activity but does not aggregate multi-source alerts or manage security posture.

---


Q129. Which AWS service is always provided at no charge?

- A. Amazon S3
- [x] B. AWS Identity and Access Management (IAM)
- C. Elastic Load Balancers
- D. AWS WAF


Why IAM Is Always Free:
No Usage Fees: IAM enables identity and access management (e.g., creating users, roles, policies) without any costs. It is categorized under "Always Free" in the AWS Free Tier, available indefinitely to both new and existing customers.

Core Security Service: Manages permissions for AWS resources (e.g., S3 buckets, EC2 instances) and integrates with all AWS services at zero cost.

Why Other Services Are Not Free:
 
A. Amazon S3: 5 GB storage free for 12 months only (Standard Storage tier). Charges apply for storage, requests, and data transfer beyond free limits.

C. Elastic Load Balancers: 750 hours free for 12 months (Application/Classic Load Balancer). Post-free tier: $0.025/hour + data transfer fees.

D. AWS WAF: No free tier; charges for web ACLs ($5/month) and rules ($1/rule/month) + request fees ($0.60/million) 


---


Q130. To reduce costs, a company is planning to migrate a NoSQL database to AWS. Which AWS service is fully managed and can automatically scale throughput capacity to meet database workload demands?

- A. Amazon Redshift
- B. Amazon Aurora
- [x] C. Amazon DynamoDB
- D. Amazon RDS

 
---


Q131. A company is using Amazon DynamoDB. Which task is the company's responsibility, according to the AWS shared responsibility model?

- A. Patch the operating system.
- B. Provision hosts.
- [x] C. Manage database access permissions.
- D. Secure the operating system.


---

Q132. A company has a test AWS environment. A company is planning on testing an application within AWS. The application testing can be interrupted and does not need to run continuously. Which Amazon EC2 purchasing option will meet these requirements MOST cost-effectively?

- A. On-Demand Instances
- B. Dedicated Instances
- [x] C. Spot Instances
- D. Reserved Instances

---

Q133. Which AWS service gives users the ability to discover and protect sensitive data that is stored in Amazon S3 buckets?

- [x] A. Amazon Macie
- B. Amazon Detective
- C. Amazon GuardDuty
- D. AWS IAM Access Analyzer

---


Q134. Which of the following services can be used to block network traffic to an instance? (Choose two.)

- [x] A. Security groups
- B. Amazon Virtual Private Cloud (Amazon VPC) flow logs
- [x] C. Network ACLs
- D. Amazon CloudWatch
- E. AWS CloudTrail

---

Q135. Which AWS service can identify when an Amazon EC2 instance was terminated?

- A. AWS Identity and Access Management (IAM)
- [x] B. AWS CloudTrail
- C. AWS Compute Optimizer
- D. Amazon EventBridge

 


C. AWS Compute Optimizer: AWS Compute Optimizer is a service that provides recommendations for optimizing EC2 instance performance and cost. While it can provide insights into instance utilization and sizing, it does not focus on identifying instance termination events.

D. Amazon EventBridge: Amazon EventBridge is an event-driven service that allows you to build event-driven architectures within AWS. While it can be used to react to various events and trigger actions, it does not provide specific functionality to identify instance termination events.

---


Q136. Which of the following is a fully managed MySQL-compatible database?

- A. Amazon S3
- B. Amazon DynamoDB
- C. Amazon Redshift
- [x] D. Amazon Aurora  

> MySQL and PostgreSQL
---


Q137. Which AWS service supports a hybrid architecture that gives users the ability to extend AWS infrastructure, AWS services, APIs, and tools to data centers, co-location environments, or on-premises facilities?

- A. AWS Snowmobile
- B. AWS Local Zones
- [x] C. AWS Outposts 
- D. AWS Fargate



AWS Outposts is a fully managed service that extends AWS infrastructure, services, APIs, and tools to customer premises. It enables a hybrid architecture by bringing native AWS services, such as Amazon EC2, Amazon EBS, and Amazon S3, to on-premises environments. With AWS Outposts, customers can run applications and workloads locally, while seamlessly connecting to other AWS services in the cloud.

Key features and benefits of AWS Outposts include:

- Native AWS services: AWS Outposts provides access to a subset of AWS services and features that are available in the AWS cloud. This allows customers to use familiar AWS services and tools while running them on-premises.
- Fully managed service: AWS manages the installation, configuration, and maintenance of the Outposts infrastructure, ensuring a consistent experience with the AWS cloud environment.
- Hybrid capabilities: AWS Outposts enables hybrid architectures by providing seamless integration with other AWS services in the cloud. Customers can use Outposts to address data residency requirements, reduce data transfer costs, and meet low-latency application requirements.
- Local data processing: With AWS Outposts, customers can process and store sensitive data locally, allowing them to meet compliance and regulatory requirements that may necessitate data locality.

Let's briefly review the other options:

A. AWS Snowmobile: AWS Snowmobile is a data transfer service that helps customers move large amounts of data into and out of AWS. It is a physical data transfer solution in the form of a secure shipping container, designed for massive data migration projects. While Snowmobile facilitates data transfer, it does not support a hybrid architecture.

B. AWS Local Zones: AWS Local Zones are an extension of AWS regions and provide low-latency access to AWS services in select geographic locations. Local Zones are designed to support specific workloads that require very low latency to end-users. While they provide local access to AWS services, they do not specifically support extending AWS infrastructure to on-premises environments.

D. AWS Fargate: AWS Fargate is a serverless compute engine for containers that allows users to run containers without managing the underlying infrastructure. It is a fully managed service for container orchestration but does not provide specific capabilities for extending AWS infrastructure to on-premises facilities.


---

Q138. Which AWS service can run a managed PostgreSQL database that provides online transaction processing (OLTP)?

- A. Amazon DynamoDB
- B. Amazon Athena
- [x] C. Amazon RDS  
- D. Amazon EMR

---


Q139 is the same as Q5. 


---

> [!IMPORTANT]
> Q140. A company wants to monitor for misconfigured security groups that are allowing unrestricted access to specific ports. Which AWS service will meet this requirement?

- [x] A. AWS Trusted Advisor  
- B. Amazon CloudWatch
- C. Amazon GuardDuty
- D. AWS Health Dashboard

---

Q141 is the same as Q63. 

---

Q142. A company wants to establish a schedule for rotating database user credentials. Which AWS service will support this requirement with the LEAST amount of operational overhead?

- A. AWS Systems Manager
- [x] B. AWS Secrets Manager
- C. AWS License Manager
- D. AWS Managed Services

---

Q143. Which AWS service is used to provide encryption for Amazon EBS?

- A. AWS Certificate Manager
- B. AWS Systems Manager
- [x] C. AWS KMS
- D. AWS Config

---

Q144. A company wants to manage its AWS Cloud resources through a web interface. Which AWS service will meet this requirement?

- [x] A. AWS Management Console
- B. AWS CLI
- C. AWS SDK
- D. AWS Cloud9

---

Q145. Which AWS Cloud benefit is shown by an architecture's ability to withstand failures with minimal downtime?

- A. Agility
- B. Elasticity
- C. Scalability
- [x] D. High availability

--- 

Q146 is the same as Q53

---

Q147. Which task is the customer's responsibility, according to the AWS shared responsibility model?

- A. Maintain the security of the AWS Cloud.
- [x] B. Configure firewalls and networks.
- C. Patch the operating system of Amazon RDS instances.
- D. Implement physical and environmental controls.

--- 

> [!IMPORTANT]
> Q148. Which AWS service helps deliver highly available applications with fast failover for multi-Region and Multi-AZ architectures?

- A. AWS WAF
- [x] B. AWS Global Accelerator
- C. AWS Shield
- D. AWS Direct Connect 


---
> [!IMPORTANT]
> Q149. A user wants to review all Amazon S3 buckets with ACLs and S3 bucket policies in the S3 console. Which AWS service or resource will meet this requirement?

- A. S3 Multi-Region Access Points
- B. S3 Storage Lens
- C. AWS IAM Identity Center (AWS Single Sign-On)
- [x] D. Access Analyzer for S3

<img width="800" alt="image" src="https://github.com/user-attachments/assets/af078fa8-e2fd-4ff1-910b-b3e6e6e1c7ad" />


Access Analyzer for S3 is a feature within the AWS Identity and Access Management (IAM) service that helps you identify and review the access permissions for your S3 buckets. It allows you to analyze the policies and access control lists (ACLs) associated with your S3 buckets to ensure that they are configured correctly and do not grant unintended access.

By using Access Analyzer for S3, you can access a centralized view of all your S3 buckets' permissions and quickly identify any potential security risks or misconfigurations. It provides detailed findings that highlight any overly permissive access settings, including both bucket policies and ACLs.

You can access Access Analyzer for S3 directly from the S3 console, where you'll be able to review the access findings for each bucket and take appropriate actions to remediate any identified issues. This helps you ensure that your S3 buckets have the desired access controls in place and helps improve the security posture of your S3 resources.

 
Let's briefly review the other options:

A. S3 Multi-Region Access Points: S3 Multi-Region Access Points is a feature that simplifies access management for S3 buckets across multiple AWS Regions. While it enhances access management, it is not specifically designed for reviewing ACLs and bucket policies.

B. S3 Storage Lens: S3 Storage Lens is a feature that provides insights and analytics on your S3 storage usage and activity. While it provides valuable information about your buckets, it does not specifically focus on reviewing ACLs and bucket policies.

C. AWS IAM Identity Center (AWS Single Sign-On): AWS Single Sign-On (SSO) is a service that simplifies access management for multiple AWS accounts and applications. It is not directly related to reviewing ACLs and bucket policies for S3 buckets.

 
---

Q150. What is the best resource for a user to find compliance-related information and reports about AWS?

- [x] A. AWS Artifact
- B. AWS Marketplace
- C. Amazon Inspector
- D. AWS Support

---


Q151. Which responsibility belongs to AWS when a company hosts its databases on Amazon EC2 instances?
- A. Database backups
- B. Database software patches
- C. Operating system patches
- [x] D. Operating system installations

---

Q152. Which of the following are advantages of moving to the AWS Cloud? (Choose two.)

- A. The ability to turn over the responsibility for all security to AWS.
- [x] B. The ability to use the pay-as-you-go model.  
- C. The ability to have full control over the physical infrastructure.
- [x] D. No longer having to guess what capacity will be required.  
- E. No longer worrying about users access controls.

---


Q153. Which AWS service is a hybrid cloud storage service that provides on-premises users access to virtually unlimited cloud storage?
- A. AWS DataSync
- B. Amazon S3 Glacier
- [x] C. AWS Storage Gateway 
- D. Amazon Elastic Block Store (Amazon EBS)


---


Q154. A company plans to migrate to AWS and wants to create cost estimates for its AWS use cases. Which AWS service or tool can the company use to meet these requirements?
- [x] A. AWS Pricing Calculator  
- B. Amazon CloudWatch
- C. AWS Cost Explorer
- D. AWS Budgets

---

Q155. Which of the following is a recommended design principle of the AWS Well-Architected Framework?
- A. Reduce downtime by making infrastructure changes infrequently and in large increments.
- B. Invest the time to configure infrastructure manually.
- [x] C. Learn to improve from operational failures. (operational excellence pillar)
- D. Use monolithic application design for centralization.


---

Q156. Using AWS Identity and Access Management (IAM) to grant access only to the resources needed to perform a task is a concept known as:
- A. restricted access.
- B. as-needed access.
- [x] C. least privilege access. 
- D. token access.

---

Q157. Which AWS service or tool can be used to set up a firewall to control traffic going into and coming out of an Amazon VPC subnet?
- A. Security group
- B. AWS WAF
- C. AWS Firewall Manager
- [x] D. Network ACL  


---
> [!IMPORTANT]
> Q158. A company wants to operate a data warehouse to analyze data without managing the data warehouse infrastructure. Which AWS service will meet this requirement?

- A. Amazon Aurora
- [x] B. Amazon Redshift Serverless  
- C. AWS Lambda
- D. Amazon RDS

> Amazon Redshift is a fully managed data warehousing service provided by AWS. However, the traditional Amazon Redshift service requires you to provision and manage the infrastructure, including cluster sizing, scaling, and maintenance.
> Amazon Redshift Serverless, on the other hand, is a recent addition to the Amazon Redshift family. It is a serverless variant that eliminates the need for infrastructure management. With Amazon Redshift Serverless, you can focus solely on analyzing your data without worrying about managing the underlying infrastructure.
> Amazon Redshift Serverless automatically scales compute and memory resources based on the workload demand. When queries are executed, the service automatically provisions the necessary resources to process the workload efficiently, and scales down when the workload decreases. This autoscaling capability allows you to optimize costs and performance based on your data analysis needs.
> By using Amazon Redshift Serverless, you can offload the responsibility of infrastructure management to AWS, allowing you to focus on analyzing your data and extracting insights from it.

> Let's briefly review the other options:
> A. Amazon Aurora: Amazon Aurora is a relational database service provided by AWS. While it is suitable for storing and analyzing data, it is not specifically designed as a data warehousing service.
> C. AWS Lambda: AWS Lambda is a serverless compute service that allows you to run code without provisioning or managing servers. While AWS Lambda can be used for data processing and analytics, it is not specifically designed as a data warehousing service.
> D. Amazon RDS: Amazon RDS (Relational Database Service) is a managed database service provided by AWS. It supports various database engines, including Amazon Aurora, MySQL, PostgreSQL, and others. While it can be used for data storage and analysis, it is not specifically designed as a data warehousing service.


---

Q159. How does AWS Cloud computing help businesses reduce costs? (Choose two.)

- A. AWS charges the same prices for services in every AWS Region.
- [x] B. AWS enables capacity to be adjusted on demand.
- C. AWS offers discounts for Amazon EC2 instances that remain idle for more than 1 week.
- D. AWS does not charge for data sent from the AWS Cloud to the internet.
- [x] E. AWS eliminates many of the costs of building and maintaining on-premises data centers.


---

Q160. Which task is the responsibility of AWS when using AWS services?

- A. Management of IAM user permissions
- B. Creation of security group rules for outbound access
- [x] C. Maintenance of physical and environmental controls
- D. Application of Amazon EC2 operating system patches

---


Q161. A company wants to automate infrastructure deployment by using infrastructure as code (IaC). The company wants to scale production stacks so the stacks can be deployed in multiple AWS Regions. Which AWS service will meet these requirements?

- A. Amazon CloudWatch
- B. AWS Config
- C. AWS Trusted Advisor
- [x] D. AWS CloudFormation

---

Q162. Which option is an AWS Cloud Adoption Framework (AWS CAF) platform perspective capability?

- [x] A. Data architecture (platform)
- B. Data protection (security)
- C. Data governance (governance)
- D. Data science (business)
 
---


Q163. A company is running a workload in the AWS Cloud. Which AWS best practice ensures the MOST cost-effective architecture for the workload?

- A. Loose coupling
- [x] B. Rightsizing
- C. Caching
- D. Redundancy

---

Q164. A company is using a third-party service to back up 10 TB of data to a tape library. The on-premises backup server is running out of space. The company wants to use AWS services for the backups without changing its existing backup workflows. Which AWS service should the company use to meet these requirements?

- A. Amazon Elastic Block Store (Amazon EBS)
- [x] B. AWS Storage Gateway
- C. Amazon Elastic Container Service (Amazon ECS)
- D. AWS Lambda

---

Q165. Which tasks are the customer's responsibility, according to the AWS shared responsibility model? (Choose two.)

- A. Establish the global infrastructure.
- [x] B. Perform client-side data encryption.
- [x] C. Configure IAM credentials.
- D. Secure edge locations.
- E. Patch Amazon RDS DB instances.

---
> [!IMPORTANT]
> Q166. A developer has been hired by a large company and needs AWS credentials. Which are security best practices that should be followed? (Choose two.)

- [x] A. Grant the developer access to only the AWS resources needed to perform the job.
- B. Share the AWS account root user credentials with the developer.
- C. Add the developer to the administrator's group in AWS IAM.
- D. Configure a password policy that ensures the developer's password cannot be changed.
- [x] E. Ensure the account password policy requires a minimum length.

---
Q167. A company has multiple AWS accounts that include compute workloads that cannot be interrupted. The company wants to obtain billing discounts that are based on the company's use of AWS services. Which AWS feature or purchasing option will meet these requirements?

- A. Resource tagging
- [x] B. Consolidated billing
- C. Pay-as-you-go pricing
- D. Spot Instances

Consolidated billing is an AWS feature that allows organizations to consolidate the billing and payment for multiple AWS accounts. By consolidating the billing, the company can benefit from volume discounts and pricing tiers based on their overall AWS usage across all accounts.

With consolidated billing, the company can aggregate usage across their accounts, which can help them reach higher usage tiers and qualify for volume discounts. This is particularly beneficial when the company has multiple accounts with compute workloads that cannot be interrupted, as they can benefit from cost savings based on their overall usage.

Resource tagging (option A) is a feature that allows organizations to assign metadata tags to AWS resources for organizational and cost allocation purposes. While tags can help with tracking and cost allocation, they do not directly provide billing discounts.

Pay-as-you-go pricing (option C) is the default pricing model for AWS services, where customers pay for the resources and services they consume on an hourly or usage basis. While pay-as-you-go pricing offers flexibility, it does not provide specific billing discounts based on usage.

Spot Instances (option D) are spare compute instances that are offered at significantly reduced prices compared to On-Demand instances. Spot Instances can help reduce costs but they are not directly related to obtaining billing discounts based on overall AWS usage.

---


Q168. A user wants to allow applications running on an Amazon EC2 instance to make calls to other AWS services. The access granted must be secure. Which AWS service or feature should be used?

- A. Security groups
- B. AWS Firewall Manager
- [x] C. IAM roles
- D. IAM user SSH keys

---

Q169. A company wants a fully managed Windows file server for its Windows-based applications. Which AWS service will meet this requirement?

- [x] A. Amazon FSx
- B. Amazon Elastic Kubernetes Service (Amazon EKS)
- C. Amazon Elastic Container Service (Amazon ECS)
- D. Amazon EMR

Amazon FSx is a fully managed file storage service provided by AWS. It offers file systems that are compatible with Windows applications, providing a native Windows file server experience. Amazon FSx for Windows File Server is specifically designed to provide file storage for Windows-based workloads.

With Amazon FSx for Windows File Server, you can easily create and manage file systems that can be accessed by multiple EC2 instances. It supports the SMB (Server Message Block) protocol, allowing seamless integration with Windows applications and workloads.

On the other hand, options B, C, and D are not specifically designed for Windows file server requirements:

B. Amazon Elastic Kubernetes Service (Amazon EKS) is a managed Kubernetes service that is primarily used for containerized applications and orchestration. It is not designed specifically for fully managed Windows file server capabilities.

C. Amazon Elastic Container Service (Amazon ECS) is a container orchestration service similar to Amazon EKS. It is also not specifically designed to provide a fully managed Windows file server.

D. Amazon EMR (Elastic MapReduce) is a managed big data processing service that runs on Apache Hadoop. It is not designed to provide a file server for Windows-based applications.

---

Q170. A company wants to migrate its NFS on-premises workload to AWS. Which AWS Storage Gateway type should the company use to meet this requirement?

- A. Tape Gateway
- B. Volume Gateway
- C. Amazon FSx File Gateway
- [x] D. Amazon S3 File Gateway

> With Amazon S3 File Gateway, Cloud storage is made accessible to database and application servers as locally mountable file shares, using industry-standard file protocols:
> Linux clients: NFS (versions 3 and 4.1)
> Windows clients: SMB (versions 2 and 3)

---
Q171. A company needs to track the activity in its AWS accounts, and needs to know when an API call is made against its AWS resources. Which AWS tool or service can be used to meet these requirements?

- A. Amazon CloudWatch
- B. Amazon Inspector
- [x] C. AWS CloudTrail
- D. AWS IAM

---

Q172. A company has an uninterruptible application that runs on Amazon EC2 instances. The application constantly processes a backlog of files in an Amazon Simple Queue Service (Amazon SQS) queue. This usage is expected to continue to grow for years. What is the MOST cost-effective EC2 instance purchasing model to meet these requirements?

- A. Spot Instances
- B. On-Demand Instances
- [x] C. Savings Plans
- D. Dedicated Hosts


Savings Plans offer significant cost savings for long-term usage of EC2 instances. With Savings Plans, you commit to a consistent amount of compute usage (measured in dollars per hour) over a 1- or 3-year term. In return, you receive a discounted rate on your EC2 usage, which can result in substantial cost savings compared to On-Demand Instances.

Since the company's application is expected to continue growing for years, committing to a 1- or 3-year term with Savings Plans allows them to lock in discounted rates for their EC2 instances over the long term. This ensures cost predictability and maximizes cost savings as the application’s usage scales.

Spot Instances (option A) can offer even greater cost savings compared to On-Demand Instances, but they come with the risk of potential interruptions. As the company’s application is described as uninterruptible, Spot Instances may not be suitable unless the application can handle interruptions and is designed for fault tolerance.

On-Demand Instances (option B) offer flexibility and are billed per hour of usage with no upfront commitment. However, they are generally more expensive compared to other purchasing options like Savings Plans for long-term, consistent usage.

Dedicated Hosts (option D) provide physical EC2 servers dedicated exclusively to the company's account. While they offer additional control and compliance benefits, they are generally more expensive and not specifically tailored for cost-effective instances.

---


Q173. A company wants an AWS service to provide product recommendations based on its customer data. Which AWS service will meet this requirement?

- A. Amazon Polly
- [x] B. Amazon Personalize
- C. Amazon Comprehend
- D. Amazon Rekognition
 


---
> [!IMPORTANT]
> Q174. A company is planning its migration to the AWS Cloud. The company is identifying its capability gaps by using the AWS Cloud Adoption Framework (AWS CAF) perspectives. Which phase of the cloud transformation journey includes these identification activities?

- A. Envision
- [x] B. Align
- C. Scale
- D. Launch

---

Q175. A social media company wants to protect its web application from common web exploits such as SQL injections and cross-site scripting.
Which AWS service will meet these requirements?

- A. Amazon Inspector
- [x] B. AWS WAF
- C. Amazon GuardDuty
- D. Amazon CloudWatch

> SQL injections and cross-site scripting
---

> [!IMPORTANT]
> Q176. Which fully managed AWS service assists with the creation, testing, and management of custom Amazon EC2 images?

- [x] A. EC2 Image Builder
- B. Amazon Machine Image (AMI)
- C. AWS Launch Wizard
- D. AWS Elastic Beanstalk

EC2 Image Builder is a service that helps automate the creation, testing, and deployment of custom Amazon Machine Images (AMIs) for EC2 instances. It provides a graphical interface and a set of pre-configured templates to simplify the process of building and maintaining custom images.

With EC2 Image Builder, you can define a pipeline that includes a series of build steps, such as installing software packages, configuring settings, and running tests. These steps can be combined and automated to create fully customized and validated AMIs.

The service integrates with AWS Identity and Access Management (IAM), AWS Systems Manager, and other AWS services to provide a secure and efficient image building process. It also supports versioning and lifecycle management of AMIs, allowing you to easily update and manage your custom images over time.

Amazon Machine Image (AMI) (option B) is a virtual machine image used to launch EC2 instances. While AMIs are closely related to custom images, AMIs themselves are not a fully managed service for creating and managing custom images.
 

---

Q177. A company wants an automated process to continuously scan its Amazon EC2 instances for software vulnerabilities. Which AWS service will meet these requirements?

- A. Amazon GuardDuty
- [x] B. Amazon Inspector
- C. Amazon Detective
- D. Amazon Cognito

Amazon Inspector is a security assessment service that helps identify vulnerabilities and compliance issues in applications deployed on Amazon EC2 instances. It provides automated security assessments by analyzing the network configuration, operating system, and installed software packages on EC2 instances.

With Amazon Inspector, you can define assessment targets and specify rules packages to scan for common vulnerabilities and exposures (CVEs), security best practices, and compliance standards. It performs automated security checks and generates detailed findings and recommendations to help you understand and address potential vulnerabilities.

By configuring Amazon Inspector to run continuously or on a scheduled basis, you can achieve ongoing and automated vulnerability scanning for your EC2 instances. This allows you to identify and mitigate vulnerabilities in a proactive and timely manner.

Amazon GuardDuty (option A) is a threat detection service that uses machine learning and anomaly detection to identify suspicious or malicious activity in your AWS environment. While it can help detect certain types of threats, it is not specifically designed for software vulnerability scanning.

Amazon Detective (option C) is a service that helps analyze, investigate, and visualize security data. It focuses on providing insights into security incidents and threat patterns, rather than conducting vulnerability scans.

Amazon Cognito (option D) is an identity management service that provides user authentication and authorization for applications. While it is important for managing user access, it is not designed for vulnerability scanning of EC2 instances.

---

Q178. A company plans to deploy containers on AWS. The company wants full control of the compute resources that host the containers. Which AWS service will meet these requirements?

- A. Amazon Elastic Kubernetes Service (Amazon EKS)
- B. AWS Fargate
- [x] C. Amazon EC2
- D. Amazon Elastic Container Service (Amazon ECS)



Why Amazon EC2?

- Full Compute Control: Directly manage EC2 instances (OS, storage, networking, scaling, security patches). Choose instance types (e.g., GPU-optimized for AI), configure kernel parameters, and install custom software.

- Container Flexibility: Deploy containers via Docker or orchestrate with Kubernetes (kops/kubeadm), Amazon ECS (ECS on EC2 mode), or Amazon EKS (self-managed node groups).

A. Amazon EKS	Managed control plane, but worker nodes run on EC2/Fargate. With EC2 nodes, you control the instances but not the Kubernetes control plane (managed by AWS).
B. AWS Fargate	Serverless—AWS manages all underlying infrastructure. No EC2 access or host-level control.
D. Amazon ECS	In "Fargate launch type," no EC2 control. In "EC2 launch type," you manage EC2 instances but rely on ECS for orchestration (partial control trade-off).

For absolute control over compute resources, Amazon EC2 (Option C) is the only solution. Pair with open-source tools (e.g., Kubernetes) for orchestration without sacrificing infrastructure control.

Amazon EC2 provides virtual servers in the cloud, allowing you to have full control over the compute resources, including the underlying infrastructure, for hosting containers. With EC2, you can provision and manage virtual machines known as instances, and then deploy containers onto these instances using container orchestration tools like Docker or Kubernetes.

By using Amazon EC2, you have complete control over the configuration, scaling, and management of the EC2 instances hosting your containers. You can choose the instance types, storage options, networking settings, and other parameters to meet your specific requirements. This level of control allows you to optimize the performance, security, and cost-efficiency of your containerized applications.

On the other hand, the other options are not focused on providing full control of the compute resources hosting containers:
 

A. Amazon Elastic Kubernetes Service (Amazon EKS) is a managed Kubernetes service that simplifies the deployment and management of containerized applications using Kubernetes. While it provides a higher level of abstraction and automation, it does not offer the same level of control over the underlying compute resources as Amazon EC2.

B. AWS Fargate is a serverless compute engine for containers that allows you to run containers without managing the underlying infrastructure. While it provides ease of use and abstracts away the compute resources, it does not provide the same level of control over the underlying compute resources as Amazon EC2.

D. Amazon Elastic Container Service (Amazon ECS) is a container orchestration service that simplifies the deployment and management of containers. While it offers some configuration options, it does not provide the same level of control over the compute resources as Amazon EC2.


---
> [!IMPORTANT]
> Q179. Which AWS service or feature allows users to create new AWS accounts, group multiple accounts to organize workflows, and apply policies to groups of accounts?

- A. AWS Identity and Access Management (IAM)
- B. AWS Trusted Advisor
- C. AWS CloudFormation
- [x] D. AWS Organizations  


> AWS Organizations SCPs: Use an AWS Organizations service control policy (SCP) to define the maximum permissions for IAM users and IAM roles within accounts in your organization or organizational unit (OU). SCPs limit permissions that identity-based policies or resource-based policies grant to IAM users or IAM roles within the account. SCPs do not grant permissions.

> AWS Organizations RCPs: Use an AWS Organizations resource control policy (RCP) to define the maximum permissions for resources within accounts in your organization or organizational unit (OU). RCPs limit permissions that identity-based and resource-based policies can grant to resources in accounts within your organization. RCPs do not grant permissions.

---

Q180. A company wants to store and retrieve files in Amazon S3 for its existing on-premises applications by using industry-standard file system protocols. Which AWS service will meet these requirements?

- A. AWS DataSync
- B. AWS Snowball Edge
- [x] C. Amazon S3 File Gateway  
- D. AWS Transfer Family


--- 

Q181. A company wants to block SQL injection attacks. Which AWS service or feature should the company use to meet this requirement?

- [x] A. AWS WAF
- B. Network ACLs
- C. Security groups
- D. AWS Certificate Manager (ACM)

 
---

Q182. A company wants a unified tool to provide a consistent method to interact with AWS services. Which AWS service or tool will meet this requirement?

- [x] A. AWS CLI  
- B. Amazon Elastic Container Service (Amazon ECS)
- C. AWS Cloud9
- D. AWS Virtual Private Network (AWS VPN)


> B. Amazon ECS	A container orchestration service—only manages Docker containers, not a general-purpose AWS interaction tool.
> C. AWS Cloud9	A cloud-based IDE for coding—not designed for broad AWS service management.
> D. AWS VPN	A networking service for secure connectivity—does not interact with AWS services.


---

Q183. A company needs to evaluate its AWS environment and provide best practice recommendations in five categories: cost, performance, service limits, fault tolerance and security. Which AWS service can the company use to meet these requirements?

- A. AWS Shield
- B. AWS WAF
- [x] C. AWS Trusted Advisor 
- D. AWS Service Catalog

---

Q184. Which perspective in the AWS Cloud Adoption Framework (AWS CAF) includes capabilities for configuration management and patch management?

- A. Platform
- [x] B. Operations  
- C. Security
- D. Governance

---


Q185. A company has a compute workload that is steady, predictable, and uninterruptible. Which Amazon EC2 instance purchasing options meet these requirements MOST cost-effectively? (Choose two.)

- A. On-Demand Instances
- [x] B. Reserved Instances
- C. Spot Instances
- [x] D. Saving Plans  
- E. Dedicated Hosts


---


Q186. Which Amazon EC2 pricing model is the MOST cost efficient for an uninterruptible workload that runs once a year for 24 hours?

- [x] A. On-Demand Instances
- B. Reserved Instances
- C. Spot Instances
- D. Dedicated Instances

---

Q187. Which option is a shared responsibility between AWS and its customers under the AWS shared responsibility model?

- A. Configuration of Amazon EC2 instance operating systems
- B. Application file system server-side encryption
- [x] C. Patch management
- D. Security of the physical infrastructure

---

> [!IMPORTANT]
> Q188. A company wants to migrate its on-premises workloads to the AWS Cloud. The company wants to separate workloads for chargeback to different departments. Which AWS services or features will meet these requirements? (Choose two.)

- A. Placement groups
- [x] B. Consolidated billing
- C. Edge locations
- D. AWS Config
- [x] E. Multiple AWS accounts


B. Consolidated billing: Consolidated billing is a feature provided by AWS that allows organizations to consolidate usage and billing information across multiple AWS accounts. With consolidated billing, the company can create a single payment method for all accounts and receive a single, comprehensive bill. This enables the company to separate workloads for chargeback to different departments while maintaining centralized billing and management.

E. Multiple AWS accounts: AWS allows organizations to create and manage multiple AWS accounts within their overall AWS organization. Each account can be used to isolate workloads and resources for different departments or business units. By using multiple AWS accounts, the company can have separate environments, resources, and billing for each department, allowing for clear separation and chargeback.

The other options are not directly related to separating workloads for chargeback:

A. Placement groups: Placement groups are used to influence the placement of EC2 instances within the AWS infrastructure to meet specific requirements such as low-latency networking or high-performance computing. They do not provide the capability to separate workloads for chargeback purposes.

C. Edge locations: Edge locations refer to the global network of AWS edge locations that are part of Amazon CloudFront, the content delivery network service. Edge locations are used to cache and deliver content to end users with low latency. They are not relevant to separating workloads for chargeback.

D. AWS Config: AWS Config is a service that provides a detailed inventory of AWS resources and tracks changes to these resources over time. It helps with compliance, security, and resource management but does not directly address the requirement of separating workloads for chargeback.

---

Q189. Which task is a responsibility of AWS, according to the AWS shared responsibility model?

- A. Enable client-side encryption for objects that are stored in Amazon S3.
- B. Configure IAM security policies to comply with the principle of least privilege.
- C. Patch the guest operating system on an Amazon EC2 instance.
- [x] D. Apply updates to the Nitro Hypervisor.

---

Q190. Which option is a benefit of using AWS for cloud computing?

- A. Trade variable expense for fixed expense
- [x] B. Pay-as-you-go pricing
- C. Decreased speed and agility
- D. Spending money running and maintaining data centers

---

Q191. Which option is an AWS Cloud Adoption Framework (AWS CAF) business perspective capability?

- A. Culture evolution (people)
- B. Event management  (operations)
- [x] C. Data monetization (business)
- D. Platform architecture (platform)

---

> [!IMPORTANT]
> Q192. A company is assessing its AWS Business Support plan to determine if the plan still meets the company's needs. The company is considering switching to AWS Enterprise Support. Which additional benefit will the company receive with AWS Enterprise Support?

- A. A full set of AWS Trusted Advisor checks
- B. Phone, email, and chat access to cloud support engineers 24 hours a day, 7 days a week
- [x] C. A designated technical account manager (TAM) to assist in monitoring and optimization
- D. A consultative review and architecture guidance for the company's applications



> A. Full Trusted Advisor checks:	Already included in Business Support (and higher tiers).

> B. 24/7 support access	Available in Business Support (and higher tiers).

> D. Consultative architecture guidance:	Offered in Enterprise On-Ramp (lower tier) and Enterprise Support


---


Q193. Which pricing model will interrupt a running Amazon EC2 instance if capacity becomes temporarily unavailable?
- A. On-Demand Instances
- B. Standard Reserved Instances
- [x] C. Spot Instances
- D. Convertible Reserved Instances


---

Q194. Which AWS service or component allows inbound traffic from the internet to access a VPC?

- [x] A. Internet gateway
- B. NAT gateway
- C. AWS WAF
- D. VPC peering
 
> An internet gateway is a horizontally scalable, redundant, and highly available AWS-managed component that allows communication between instances within a VPC and the internet. It serves as a gateway for internet-bound traffic to and from a VPC. It enables inbound and outbound communication between instances in the VPC and the internet.
> By attaching an internet gateway to a VPC, instances within the VPC can have public IP addresses and can be accessed from the internet. This allows inbound traffic from the internet to reach the instances within the VPC.

> The other options mentioned are not the correct choices for enabling inbound internet access to a VPC:

> B. NAT gateway: A NAT (Network Address Translation) gateway is used for instances within a private subnet to access the internet. It allows outbound traffic from the instances to the internet but does not enable inbound traffic from the internet to reach the instances.

> C. AWS WAF: AWS WAF (Web Application Firewall) is a service used to protect web applications from common web exploits and attacks. While it can filter and control inbound traffic to web applications, it does not provide direct inbound access to a VPC.

> D. VPC peering: VPC peering allows direct communication between two VPCs using private IP addresses. It enables instances in separate VPCs to communicate with each other, but it does not provide direct inbound access from the internet.

---

Q195. What does the Amazon S3 Intelligent-Tiering storage class offer?

- A. Payment flexibility by reserving storage capacity
- B. Long-term retention of data by copying the data to an encrypted Amazon Elastic Block Store (Amazon EBS) volume
- [x] C. Automatic cost savings by moving objects between tiers based on access pattern changes
- D. Secure, durable, and lowest cost storage for data archival
 
> The Amazon S3 Intelligent-Tiering storage class offers automatic cost savings by moving objects between tiers based on access pattern changes.
With Intelligent-Tiering, Amazon S3 automatically analyzes the access patterns of objects and moves them between access tiers.

https://github.com/justinjiajia/certifications/blob/main/aws/cloud_practitioner/concepts.md#s3-intelligent-tiering

> This storage class is designed to optimize costs by automatically transitioning objects between storage tiers based on their access patterns. It eliminates the need for manual management and tiering decisions, allowing users to benefit from cost savings without sacrificing performance or availability.
 
> A. Payment flexibility by reserving storage capacity: This feature is not specific to the Intelligent-Tiering storage class. Payment flexibility by reserving storage capacity is related to options like Amazon S3 Standard, S3 Standard-IA (Infrequent Access), and S3 One Zone-IA storage classes.
> B. Long-term retention of data by copying the data to an encrypted Amazon Elastic Block Store (Amazon EBS) volume: The Intelligent-Tiering storage class does not involve copying data to an Amazon EBS volume. It is focused on optimizing storage costs based on access patterns.
> D. Secure, durable, and lowest cost storage for data archival: While Amazon S3 offers secure, durable, and low-cost storage, the Intelligent-Tiering storage class specifically focuses on cost optimization by automatically moving objects between tiers based on access patterns, rather than being explicitly designed for data archival.

---


Q196. What is a benefit of using AWS serverless computing?
- A. Application deployment and management are not required
- B. Application security will be fully managed by AWS.
- C. Monitoring and logging are not needed.
- [x] D. Management of infrastructure is offloaded to AWS.

 
A benefit of using AWS serverless computing is that the management of infrastructure is offloaded to AWS.
With serverless computing, such as AWS Lambda, developers can focus on writing and deploying code without the need to manage underlying infrastructure. AWS handles the provisioning and scaling of the infrastructure resources required to run the serverless applications. This includes managing servers, operating systems, patching, and capacity planning. Developers can simply upload their code and let AWS handle the rest.
This offloading of infrastructure management allows developers to focus on writing application logic and delivering business value rather than getting bogged down with infrastructure-related tasks. It provides scalability, elasticity, and automatic resource allocation, allowing applications to scale seamlessly without the need for manual intervention.

The other options mentioned are not accurate benefits of using AWS serverless computing:
A. Application deployment and management are not required: Application deployment and management are still required when using serverless computing, but the management of infrastructure is handled by AWS. Developers are responsible for deploying and managing their application code. B. Application security will be fully managed by AWS: While AWS provides security capabilities and services, it is the responsibility of the developer to implement proper security measures for their serverless applications. AWS provides a secure infrastructure, but application-level security and access control are still the responsibility of the developer.
C. Monitoring and logging are not needed: Monitoring and logging are essential for understanding the behavior and performance of serverless applications. While AWS provides monitoring and logging services like Amazon CloudWatch, developers still need to configure and utilize these services to gain insights into their applications. 

---

> [!IMPORTANT]
> Q197. A company launched an Amazon EC2 instance with the latest Amazon Linux 2 Amazon Machine Image (AMI). Which actions can a system administrator take to connect to the EC2 instance? (Select TWO.)

- [x] A. Use Amazon EC2 Instance Connect
- B. Use a Remote Desktop Protocol (RDP) connection
- C. Use AWS Batch
- [x] D. Use AWS Systems Manager Session Manager
- E. Use Amazon Connect

 <img width="1275" alt="image" src="https://github.com/user-attachments/assets/a82e5268-48c7-49fc-bfb4-6d3535909c35" />

A. Use Amazon EC2 Instance Connect: Amazon EC2 Instance Connect provides a simple and secure way to connect to your EC2 instances using Secure Shell (SSH). It eliminates the need to manage SSH keys manually and allows you to connect to your instances using the EC2 console, AWS CLI, or AWS SDKs. This option is commonly used for Linux-based instances, including the Amazon Linux 2 AMI.
D. Use AWS Systems Manager Session Manager: AWS Systems Manager Session Manager provides a secure and auditable way to manage and access your EC2 instances without the need for SSH or RDP connections. It allows you to open interactive shell sessions to your instances directly from the AWS Management Console, AWS CLI, or AWS SDKs. This option is suitable for both Linux-based and Windows-based instances, including instances running the Amazon Linux 2 AMI.
The other options mentioned are not valid for connecting to an EC2 instance with the latest Amazon Linux 2 AMI:
B. Use a Remote Desktop Protocol (RDP) connection: RDP is used for connecting to Windows-based instances, while the Amazon Linux 2 AMI is a Linux-based AMI. RDP is not applicable in this case.
C. Use AWS Batch: AWS Batch is a service for running batch computing workloads across managed compute environments. It is not a method for connecting to EC2 instances.
E. Use Amazon Connect: Amazon Connect is a cloud-based contact center service for customer interactions. It is not used for connecting to EC2 instances.
 


<img width="1275" alt="image" src="https://github.com/user-attachments/assets/6211d5a7-8771-49ef-baa8-0dc5bc26b473" />


---


Q198. What does Amazon CloudFront provide?

- A. Automatic scaling for all resources to power an application from a single unified interface
- [x] B. Secure delivery of data, videos, applications, and APIs to users globally with low latency
- C. Ability to directly manage traffic globally through a variety of routing types, including latency-based routing, geo DNS geoproximity, and weighted round robin
- D. Automatic distribution of incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, IP addresses, and AWS Lambda functions


Amazon CloudFront is a content delivery network (CDN) provided by AWS. It offers secure and efficient global delivery of data, videos, applications, and APIs to users with low latency.
CloudFront caches and replicates content across a network of edge locations strategically located around the world. When users request content, CloudFront serves the data from the nearest edge location, reducing latency and improving the overall performance of content delivery. It helps ensure that content is delivered quickly to users regardless of their geographical location.
CloudFront also provides security features such as DDoS mitigation, SSL/TLS encryption, and access control mechanisms. It helps protect content from unauthorized access and ensures secure delivery.
The other options mentioned are not accurate descriptions of what Amazon CloudFront provides:
A. Automatic scaling for all resources to power an application from a single unified interface: Automatic scaling and resource management are not the primary functions of CloudFront. While CloudFront can handle high traffic loads and scale to accommodate demand, it is specifically designed for content delivery rather than managing all application resources.
C. Ability to directly manage traffic globally through a variety of routing types, including latency-based routing, geo DNS geoproximity, and weighted round-robin: This description aligns more with Amazon Route 53, which is AWS's scalable domain name system (DNS) web service, rather than CloudFront. Route 53 provides DNS routing capabilities, while CloudFront focuses on content delivery.
D. Automatic distribution of incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, IP addresses, and AWS Lambda functions: This description aligns more with Elastic Load Balancing (ELB) services, such as Application Load Balancer (ALB) or Network Load Balancer (NLB), which distribute incoming traffic across multiple targets. CloudFront primarily focuses on content delivery rather than load balancing application traffic.

---

Q199. Which AWS service can companies use to create infrastructure from code?
- A. Amazon Elastic Kubernetes Service (Amazon EKS)
- B. AWS Outposts
- C. AWS CodePipeline
- [x] D. AWS CloudFormation

AWS CloudFormation is the AWS service that allows companies to create infrastructure from code. It is an infrastructure as code (IaC) service that enables users to define and provision AWS resources in a declarative manner. With CloudFormation, you can create templates written in JSON or YAML that describe the desired state of your infrastructure. These templates can include various AWS resources such as EC2 instances, S3 buckets, databases, networking components, and more.
By using CloudFormation, companies can automate the provisioning and management of their AWS infrastructure. The templates can be version-controlled, shared, and reused, providing consistency and reproducibility across environments. CloudFormation takes care of provisioning and configuring the specified resources, ensuring that the infrastructure is created accurately and according to the defined template.
The other options mentioned are not specifically used for creating infrastructure from code:
A. Amazon Elastic Kubernetes Service (Amazon EKS): Amazon EKS is a managed Kubernetes service that simplifies the deployment, management, and scaling of containerized applications using Kubernetes. While it enables companies to manage containerized applications, it is not focused on creating infrastructure from code.
B. AWS Outposts: AWS Outposts is a service that extends AWS infrastructure and services to on- premises or co-location environments. It allows companies to run AWS services on their own hardware. While it provides an on-premises extension of AWS, it is not specifically used for creating infrastructure from code.
C. AWS CodePipeline: AWS CodePipeline is a fully managed continuous delivery service that helps automate the build, test, and deployment of applications. While it provides a workflow for managing application delivery, it is not primarily focused on creating infrastructure from code.

---

Q200. Which AWS service is a relational database compatible with MySQL and PostgreSQL?
- A. Amazon Redshift
- B. Amazon DynamoDB
- [x] C. Amazon Aurora
- D. Amazon Neptune


Amazon Aurora is the AWS service that is compatible with MySQL and PostgreSQL. It is a fully managed relational database engine that provides high performance, scalability, and durability. Amazon Aurora is designed to be compatible with MySQL and PostgreSQL, which means that applications and tools that work with MySQL or PostgreSQL can be used with Aurora with little to no modification.
Amazon Aurora offers several enhancements over traditional MySQL and PostgreSQL databases, including increased performance and scalability. It utilizes a distributed storage system and replicates data across multiple availability zones for high availability and durability. Aurora also provides automatic backups, automated software patching, and seamless scaling capabilities.
The other options mentioned are not relational databases compatible with MySQL and PostgreSQL:
A. Amazon Redshift: Amazon Redshift is a fully managed data warehousing service that is optimized for online analytical processing (OLAP) workloads. It is not compatible with MySQL or PostgreSQL but uses its own variant of PostgreSQL.
B. Amazon DynamoDB: Amazon DynamoDB is a fully managed NoSQL database service. It is not a relational database and is not compatible with MySQL or PostgreSQL.
D. Amazon Neptune: Amazon Neptune is a fully managed graph database service. It is designed for highly connected data and is not a relational database compatible with MySQL or PostgreSQL.

---

Q201 is the same as Q92. 

---

> [!IMPORTANT]
> Q202. A company wants to deploy some of its resources in the AWS Cloud. To meet regulatory requirements, the data must remain local and on premises. There must be low latency between AWS and the company resources. Which AWS service or feature can be used to meet these requirements?

- A. AWS Local Zones
- B. Availability Zones
- [x] C. AWS Outposts
- D. AWS Wavelength Zones

 
> AWS Outposts is a fully managed service that extends AWS infrastructure, services, APIs, and tools to customer premises or colocation environments. With AWS Outposts, you can deploy AWS services and run applications on hardware infrastructure that is located on premises or within the colocation facility. This allows you to keep sensitive data on premises while still leveraging the benefits of AWS services and low- latency connectivity.
> AWS Outposts provides the same native AWS services, APIs, and tools that are available in the public AWS regions. You can use services such as Amazon EC2, Amazon EBS, Amazon S3, and more on your Outposts deployment. This allows you to develop, test, and run applications using familiar AWS tools and services while keeping the data local and meeting regulatory requirements.


> A. AWS Local Zones: AWS Local Zones are an extension of AWS infrastructure that places compute, storage, database, and other select services closer to large population centers. They are designed to reduce latency for specific workloads but do not provide the capability to keep data local and on premises.

>B. Availability Zones: Availability Zones are isolated data center locations within an AWS Region. They provide redundancy and fault tolerance within a region but do not meet the requirement of keeping data local and on premises.
> D. AWS Wavelength Zones: AWS Wavelength Zones are designed for applications that require ultra-low latency connectivity to mobile devices. They are optimized for mobile edge computing but do not provide the capability to keep data local and on premises.
 

---


Q203. A team of researchers is going to collect data at remote locations around the world. Many locations do not have internet connectivity. The team needs to capture the data in the field, and transfer it to the AWS Cloud later. Which AWS service will support these requirements?

- A) AWS Outposts
- B) AWS Transfer Family
- [x] C) AWS Snow Family
- D) AWS Migration Hub


The AWS Snow Family consists of physical devices designed to securely and efficiently transfer large amounts of data to and from the AWS Cloud in situations where internet connectivity is limited, unreliable, or not available.
The Snow Family devices include AWS Snowcone, AWS Snowball, and AWS Snowmobile. These devices provide ruggedized, portable storage options that can be shipped to the remote locations where data is being collected. The team can capture the data in the field using various methods (e.g., sensors, cameras, devices), and then store the data on the Snow Family devices.
Once the data is stored on the Snow Family devices, they can be securely shipped back to an AWS region with internet connectivity. AWS handles the data transfer process and ensures the security and integrity of the data during transit.
Upon arrival at the AWS region, the data stored on the Snow Family devices can be ingested into the AWS Cloud using Snowball or Snowmobile data transfer services. These services provide fast and secure data transfer and integration with AWS storage services such as Amazon S3 or Amazon Glacier.
The other options mentioned are not suitable for meeting the specified requirements:
A. AWS Outposts: AWS Outposts extends AWS infrastructure, services, and tools to customer premises or colocation environments. It does not directly support capturing data in remote locations without internet connectivity.
B. AWS Transfer Family: The AWS Transfer Family is a managed service that enables the creation of fully managed file transfer servers for transferring files over protocols such as FTP, FTPS, SFTP, and Amazon S3. It requires internet connectivity and is not designed for offline data capture in remote locations.
D. AWS Migration Hub: AWS Migration Hub is a service that provides a single location to track the progress of application migrations to the AWS Cloud. It does not support offline data capture and transfer from remote locations.

---

Q204. A solutions architect needs to maintain a fleet of Amazon EC2 instances so that any impaired instances are replaced with new ones. Which AWS service should the solutions architect use?

- A) Amazon Elastic Container Service (Amazon ECS)
- B) Amazon GuardDuty
- C) AWS Shield
- [x] D) AWS Auto Scaling

> AWS Auto Scaling is a service that automatically adjusts the number of EC2 instances in a fleet based on predefined scaling policies. It helps ensure that the desired number of instances are available to handle the application workload and automatically replaces impaired instances to maintain the desired capacity.
By using AWS Auto Scaling, you can define scaling policies that specify how the fleet should scale based on metrics such as CPU utilization, network traffic, or custom application metrics. When an instance becomes impaired or fails, AWS Auto Scaling can automatically terminate the impaired instance and launch a new one to maintain the desired fleet capacity and availability.

> AWS Auto Scaling provides a flexible and automated way to manage and maintain the fleet of EC2 instances. It helps optimize resource utilization and ensures that the application workload is handled efficiently, even in the event of instance failures or impairments.

> The other options mentioned are not specifically designed for maintaining a fleet of EC2 instances and replacing impaired instances:
> A. Amazon Elastic Container Service (Amazon ECS): Amazon ECS is a container orchestration service for running Docker containers. While it allows you to manage and scale containerized applications, it is not focused on maintaining EC2 instances or replacing impaired instances.
> B. Amazon GuardDuty: Amazon GuardDuty is a threat detection service that continuously monitors for malicious activity and unauthorized behavior in your AWS accounts and workloads. It is not designed for maintaining and replacing EC2 instances.
> C. AWS Shield: AWS Shield is a managed Distributed Denial of Service (DDoS) protection service. It helps protect applications against DDoS attacks but does not specifically address maintaining and replacing EC2 instances.

---

> [!IMPORTANT]
> Q205. Which AWS service will help a company plan a migration to AWS by collecting the configuration, usage, and behavior data of on-premises data centers?

- A) AWS Resource Groups
- [x] B) AWS Application Discovery Service
- C) AWS Service Catalog
- D) AWS Systems Manager


AWS Application Discovery Service is a service that helps enterprises plan their migration to AWS by discovering and collecting information about their on-premises applications and infrastructure. It collects data about the configuration, dependencies, usage, and performance of on-premises systems, providing insights that can aid in the planning and execution of a migration to AWS.
With AWS Application Discovery Service, companies can gain visibility into their existing infrastructure, including servers, network devices, and software applications. It automatically discovers and collects information using lightweight agents installed on the servers or by utilizing data from existing inventory tools.
The collected data can be used to understand the interdependencies between various components, estimate the resources needed in AWS, identify potential migration challenges, and generate a migration plan. The data collected by AWS Application Discovery Service can be exported to AWS Migration Hub for centralized visibility and management of the migration process.
The other options mentioned are not specifically designed for collecting data to plan a migration:
A. AWS Resource Groups: AWS Resource Groups is a service that allows users to create and manage collections of AWS resources based on tags, resource types, or other criteria. It is not directly focused on collecting data for migration planning purposes.
C. AWS Service Catalog: AWS Service Catalog is a service that enables organizations to create and manage catalogs of IT services that can be provisioned by users within their organization. While it helps with service management, it is not designed for collecting data for migration planning.
D. AWS Systems Manager: AWS Systems Manager is a management service that helps manage EC2 instances and on-premises systems at scale. While it provides capabilities for configuration management and automation, it does not specifically collect data for migration planning.

---

Q206. Which of the following AWS services are serverless? (Select TWO.)

- A) AWS Outposts
- B) Amazon EC2
- C) Amazon Elastic Kubernetes Service (Amazon EKS)
- [x] D) AWS Fargate
- [x] E) AWS Lambda

Serverless computing is a cloud computing model where the cloud provider takes care of the underlying infrastructure and server management, allowing developers to focus on writing and deploying code without worrying about server provisioning, scaling, and maintenance.
Among the options provided, the following AWS services are serverless:
D. AWS Fargate: AWS Fargate is a serverless compute engine for containers. It allows you to run containers without managing the underlying infrastructure. With Fargate, you can focus on defining and running your containerized applications without the need to provision or manage EC2 instances explicitly.
E. AWS Lambda: AWS Lambda is a serverless computing service that lets you run your code without provisioning or managing servers. You can simply upload your code to Lambda, and it automatically handles the scaling, capacity provisioning, and availability of your applications. Lambda functions are triggered by various events and can be used for a wide range of use cases, such as data processing, real- time file processing, API backends, and more.
The other options mentioned are not serverless:
A. AWS Outposts: AWS Outposts is a service that extends AWS infrastructure, services, APIs, and tools to customer premises or colocation environments. It brings AWS services to the customer's data center, providing a consistent hybrid cloud experience. However, it does not fall under the serverless computing model.
B. Amazon EC2: Amazon EC2 (Elastic Compute Cloud) is a web service that provides resizable compute capacity in the cloud. It gives you full control over virtual servers, also known as instances, and requires you to provision, manage, and scale the instances yourself. It is not serverless as it involves server management.
C. Amazon Elastic Kubernetes Service (Amazon EKS): Amazon EKS is a managed Kubernetes service that simplifies the deployment, management, and scaling of containerized applications using Kubernetes. While it abstracts the management of the Kubernetes control plane, it still requires you to provision and manage the underlying EC2 instances or Fargate profiles where the Kubernetes worker nodes run. Hence, it is not serverless.


---

Q207. Which of the following is an AWS Well-Architected Framework design principle for operational excellence in the AWS Cloud?

- A) Go global in minutes. (performance efficiency)
- [x] B) Make frequent, small, reversible changes. (operational excellence)
- C) Implement a strong foundation of identity and access management. (security)
- D) Stop spending money on hardware infrastructure for data center operations. (cost optimization)

---

Q209. Which of the following are pillars of the AWS Well-Architected Framework? (Select TWO.)

- A) High availability
- [x] B) Performance efficiency
- [x] C) Cost optimization
- D) Going global in minutes
- E) Continuous development

---

Q210. Which cloud computing advantage is a company applying when it uses AWS Regions to increase application availability to users in different countries?

- A) Pay-as-you-go pricing
- B) Capacity forecasting
- C) Economies of scale
- [x] D) Global reach


---
> [!IMPORTANT]
> Q211. Which AWS services can a company use to achieve a loosely coupled architecture? (Select TWO.)

- A) Amazon WorkSpaces
- [x] B) Amazon Simple Queue Service (Amazon SQS)
- C) Amazon Connect
- D) AWS Trusted Advisor
- [x] E) AWS Step Functions

Amazon SQS enables decoupling between the components of an application by allowing them to communicate asynchronously, without requiring direct integration or dependency between them. This helps to ensure that each component can work independently and at its own pace.

AWS Step Functions is another service that allows developers to build applications using workflows, which can be used to decompose complex processes into smaller, more manageable tasks. By doing this, it becomes easier to manage and modify the individual components of a system, thereby promoting loose coupling.

---


Q212. A company wants to integrate natural language processing (NLP) into business intelligence (BI) dashboards. The company wants to ask questions and receive answers with relevant visualizations. Which AWS service or tool will meet these requirements?

- A) Amazon Macie
- B) Amazon Rekognition
- [x] C) Amazon QuickSight
- D) Amazon Lex


Amazon QuickSight is a fully managed business intelligence service provided by AWS. It allows users to create interactive dashboards, perform ad-hoc analysis, and generate insights from various data sources. QuickSight supports natural language queries, which means users can ask questions in plain language and receive relevant visualizations as answers.
With QuickSight's NLP capabilities, users can use conversational language to query data, such as asking for sales trends, comparing performance between regions, or filtering data based on specific criteria. QuickSight's machine learning algorithms and intelligent auto-narratives help generate relevant visualizations and insights based on the queries.



A. Amazon Macie: Amazon Macie is a security service that focuses on data discovery and classification. It helps identify and protect sensitive data, such as personally identifiable information (PII), but it does not provide the capabilities for integrating NLP into BI dashboards.
 

---

Q213. A company wants to migrate its applications to the AWS Cloud. The company plans to identify and prioritize any business transformation opportunities and evaluate its AWS Cloud readiness. Which AWS service or tool should the company use to meet these requirements?

- [x] A) AWS Cloud Adoption Framework (AWS CAF)
- B) AWS Managed Services (AMS)
- C) AWS Well-Architected Framework
- D) AWS Migration Hub

---


Q214. Which AWS service or resource provides single-tenant physical servers in the AWS Cloud?

- A) Amazon Elastic Container Service (Amazon ECS)
- B) Amazon Elastic Kubernetes Service (Amazon EKS)
- [x] C) Amazon EC2 Dedicated Host
- D) Amazon EC2 Spot Instances




Amazon EC2 Dedicated Host is the AWS service that provides single-tenant physical servers in the AWS Cloud. With Amazon EC2 Dedicated Hosts, you have full control over the underlying physical server and can use it to run instances of your choice, including instances from Amazon EC2, Amazon RDS, and Amazon Elastic Cache.
Dedicated Hosts are ideal for workloads that have specific licensing requirements, need to meet regulatory and compliance requirements, or require complete control over the underlying infrastructure. By using Dedicated Hosts, you can ensure that your instances are isolated and dedicated to your organization, providing consistent performance and security.
The other options mentioned are not correct:
A. Amazon Elastic Container Service (Amazon ECS): Amazon ECS is a fully managed container orchestration service that allows you to run and manage containers on a cluster of EC2 instances or AWS Fargate. It does not provide single-tenant physical servers.
B. Amazon Elastic Kubernetes Service (Amazon EKS): Amazon EKS is a managed Kubernetes service that allows you to run Kubernetes clusters in the AWS Cloud. It also does not provide single-tenant physical servers.
D. Amazon EC2 Spot Instances: Amazon EC2 Spot Instances allow you to bid on spare EC2 compute capacity and run instances at a significantly lower cost. However, Spot Instances do not guarantee single- tenant physical servers as they are part of the shared pool of EC2 resources.


---
> [!IMPORTANT]
> Q215. Which of the following are benefits that a company receives when it moves an on-premises production workload to AWS? (Select TWO.)

- A) AWS trains the company's staff on the use of all the AWS services
- B) AWS manages all security in the cloud
- C) AWS offers free support from technical account managers (TAMs)
- [x] D) AWS offers high availability
- [x] E) AWS provides economies of scale


awareness and training is a shared responsibility
AWS manages all security of the cloud

---

Q216. A company needs to connect its on-premises data center to the AWS Cloud. The company needs a dedicated, low-latency connection with consistent network performance. Which AWS service will meet these requirements?

- A) AWS Global Accelerator
- B) Amazon CloudFront
- [x] C) AWS Direct Connect
- D) AWS Managed VPN


AWS Direct Connect enables customers to establish a private and dedicated network connection between their on-premises infrastructure and AWS. This connection bypasses the public internet, providing a more reliable and consistent network performance compared to internet-based connections.
With AWS Direct Connect, customers can choose from various connection options, including dedicated connections and hosted connections. These connections can be provisioned with specific bandwidth requirements to meet the company's needs for low-latency and consistent network performance.
On the other hand, the other options mentioned are not suitable for the given requirements:
A. AWS Global Accelerator: AWS Global Accelerator is a service that improves the availability and performance of applications by using the AWS global network infrastructure. While it can optimize global network routing, it does not provide a dedicated, low-latency connection between an on-premises data center and the AWS Cloud.
B. Amazon CloudFront: Amazon CloudFront is a content delivery network (CDN) service that accelerates the delivery of content to end users. It is primarily used for caching and distributing static and dynamic content. While it can improve content delivery performance, it does not provide a dedicated, low-latency connection between an on-premises data center and the AWS Cloud.
D. AWS Managed VPN: AWS Managed VPN allows customers to establish a secure and encrypted connection between their on-premises network and the AWS Cloud using VPN tunnels. While it provides secure connectivity, it relies on the public internet and may not offer the same level of low-latency and consistent network performance as AWS Direct Connect.


---


Q217. Which AWS service provides the ability to host a NoSQL database in the AWS Cloud?

- A) Amazon Aurora
- [x] B) Amazon DynamoDB
- C) Amazon RDS
- D) Amazon Redshift



Amazon DynamoDB is the AWS service that provides the ability to host a NoSQL database in the AWS Cloud.
DynamoDB is a fully managed NoSQL database service that offers fast and predictable performance with seamless scalability. It is designed to handle large-scale applications and can automatically scale up or down based on the workload demands.
With DynamoDB, you can store and retrieve any amount of data while maintaining low latency and high throughput. It offers features such as automatic data replication across multiple Availability Zones for high availability and durability.
 
Amazon Redshift (option D) is a fully managed data warehousing service designed for online analytical processing (OLAP) rather than hosting NoSQL databases.


---

> [!IMPORTANT]
> Q218. A company wants to receive alerts to monitor its overall operating costs for its AWS public cloud infrastructure. Which AWS offering will meet these requirements?

- A) Amazon EventBridge
- B) Compute Savings Plans
- [x] C) AWS Budgets
- D) Migration Evaluator


> AWS Budgets is a service that allows you to set custom cost and usage budgets for your AWS resources and services. It provides you with visibility and control over your AWS costs by sending alerts when your actual or forecasted costs exceed the thresholds you define.
With AWS Budgets, you can set up budget thresholds based on various criteria such as total costs, specific service costs, usage, or custom filters. When the actual costs breach the defined thresholds, AWS Budgets can send notifications via email or Amazon Simple Notification Service (SNS) to alert you about the cost overruns.
> By utilizing AWS Budgets, companies can proactively monitor their costs, set spending limits, and take necessary actions to optimize their AWS infrastructure and manage their overall operating costs effectively.
> The other options mentioned are not suitable for the given requirements:
> A. Amazon EventBridge: Amazon EventBridge is a serverless event bus service that enables you to route events between AWS services, SaaS applications, and your own applications. While it can be used for event-driven architecture, it is not specifically focused on monitoring operating costs.
> B. Compute Savings Plans: Compute Savings Plans are a pricing model offered by AWS to reduce costs for EC2 compute usage. While they can help optimize costs for compute resources, they do not provide alerts or monitoring for overall operating costs across the entire AWS infrastructure.
> D. Migration Evaluator: Migration Evaluator is a tool provided by AWS to analyze on-premises workloads and estimate the costs and benefits of migrating them to AWS. It is not designed for ongoing monitoring of operating costs in the AWS cloud.


---

Q219. A company wants to run its workload on Amazon EC2 instances for more than 1 year. This workload will run continuously. Which option offers a discounted hourly rate compared to the hourly rate of On-Demand Instances?

- A) AWS Graviton processor
- B) Dedicated Hosts
- [x] C) EC2 Instance Savings Plans
- D) Amazon EC2 Auto Scaling instances


EC2 Instance Savings Plans offer a discounted hourly rate compared to On-Demand Instances for long- term usage of Amazon EC2 instances.
EC2 Instance Savings Plans are a pricing model that provides significant savings for customers who commit to using EC2 instances for a term of 1 or 3 years. With Instance Savings Plans, customers receive a discounted rate on the hourly cost of EC2 instances in exchange for their commitment to a consistent usage over the term.
By purchasing an EC2 Instance Savings Plan, companies can significantly reduce their EC2 costs for long- running workloads. The discount applies to the hourly rate of the EC2 instances, providing cost savings compared to the On-Demand pricing.
The other options mentioned are not directly related to discounted hourly rates compared to On-Demand Instances:
A. AWS Graviton processor: AWS Graviton processors are ARM-based processors that power certain EC2 instance types. While they can offer cost savings due to their efficiency, they do not provide a discounted hourly rate compared to On-Demand Instances.
B. Dedicated Hosts: Dedicated Hosts are physical servers dedicated to a specific customer's use. They provide control and visibility over the underlying host hardware but do not offer a discounted hourly rate compared to On-Demand Instances.
D. Amazon EC2 Auto Scaling instances: Amazon EC2 Auto Scaling allows for dynamic scaling of EC2 instances based on demand. While it can help optimize costs by automatically adjusting the number of instances, it does not provide a discounted hourly rate compared to On-Demand Instances.

---

> [!IMPORTANT]
> Q220. A company wants to use machine learning capabilities to analyze log data from its Amazon EC2 instances and efficiently conduct security investigations. Which AWS service will meet these requirements?

- A) Amazon Inspector
- B) Amazon QuickSight
- [x] C) Amazon Detective
- D) Amazon GuardDuty


Amazon Detective is the AWS service that will meet the requirements of using machine learning capabilities to analyze log data from Amazon EC2 instances and efficiently conduct security investigations.
Amazon Detective is a security service that helps you analyze, investigate, and quickly identify the root cause of potential security issues or suspicious activities in your AWS environment. It leverages machine learning, statistical analysis, and graph theory to analyze data from various sources, including VPC Flow Logs and AWS CloudTrail logs.
With Amazon Detective, you can gain insights into the security posture of your EC2 instances by automatically aggregating and analyzing log data. It generates visualizations and creates interactive graphs to provide a comprehensive view of your AWS resources, network traffic, and user behavior. This helps security teams efficiently conduct investigations and identify any potential security threats or anomalies.
The other options mentioned are not directly related to analyzing log data for security investigations:
A. Amazon Inspector: Amazon Inspector is an automated security assessment service that helps you identify security vulnerabilities and compliance violations in your EC2 instances and applications. While it offers security assessment capabilities, it does not specifically focus on log analysis or security investigations.
B. Amazon QuickSight: Amazon QuickSight is a business intelligence service that enables you to create interactive dashboards and perform data analysis. While it can help visualize data, it is not designed for log analysis or security investigations.
D. Amazon GuardDuty: Amazon GuardDuty is a threat detection service that continuously monitors your AWS environment for potential security threats and suspicious activities. While it offers threat detection capabilities, it is not specifically focused on log analysis or conducting security investigations.

---

Q221. Which AWS service uses a combination of publishers and subscribers?

- A) AWS Lambda
- [x] B) Amazon Simple Notification Service (Amazon SNS)
- C) Amazon CloudWatch
- D) AWS CloudFormation


Amazon Simple Notification Service (Amazon SNS) is the AWS service that uses a combination of publishers and subscribers.
Amazon SNS is a fully managed messaging service that enables you to publish messages from various sources (publishers) and deliver them to multiple subscribers or endpoints. It follows the publish-subscribe messaging pattern, where publishers send messages to topics, and subscribers receive the messages from those topics.
Publishers in Amazon SNS can be various AWS services, applications, or systems that generate messages or events. Subscribers can be other AWS services, endpoints such as email addresses or mobile devices, or even HTTP/HTTPS endpoints.
When a publisher sends a message to a topic in Amazon SNS, the service delivers the message to all the subscribers that have subscribed to that topic. Subscribers can receive the messages through various protocols such as email, SMS, mobile push notifications, or by invoking HTTP/HTTPS endpoints.
Amazon SNS provides a flexible and scalable architecture for decoupling and distributing messages across different systems or services, making it suitable for building event-driven architectures or sending notifications to multiple recipients.
The other options mentioned are not based on the publish-subscribe model:
A. AWS Lambda: AWS Lambda is a serverless computing service that allows you to run code without provisioning or managing servers. It does not inherently use a combination of publishers and subscribers.
C. Amazon CloudWatch: Amazon CloudWatch is a monitoring and observability service that collects and tracks metrics, logs, and events from various AWS resources. While it can handle events and notifications, it is not centered around the publish-subscribe model.
D. AWS CloudFormation: AWS CloudFormation is a service that allows you to define and provision AWS infrastructure resources in a declarative manner using templates. It does not involve a publish-subscribe model.


---



Q222 is the same as Q221. 


---

Q223. A company has a physical tape library to store data backups. The tape library is running out of space. The company needs to extend the tape library's capacity to the AWS Cloud. Which AWS service should the company use to meet this requirement?

- A) Amazon Elastic File System (Amazon EFS)
- B) Amazon Elastic Block Store (Amazon EBS)
- C) Amazon S3
- [x] D) AWS Storage Gateway

      
https://github.com/justinjiajia/certifications/tree/main/aws/service_img_demo/storage_gateway
 
AWS Storage Gateway provides a solution for extending on-premises storage to the AWS Cloud. It acts as a bridge between an on-premises environment and AWS, allowing you to seamlessly integrate your existing infrastructure with AWS storage services. In this case, the company can use AWS Storage Gateway to extend the tape library's capacity to the AWS Cloud.
AWS Storage Gateway offers different types of gateways, including a Tape Gateway. The Tape Gateway enables you to replace or augment physical tape libraries with virtual tape libraries (VTLs) in the cloud. It provides a scalable and cost-effective solution for storing backup data in the AWS Cloud without the need for physical tapes.
With Tape Gateway, you can create virtual tapes, which are stored as Amazon S3 objects, and attach them to your existing backup infrastructure. The data is uploaded to the cloud, providing off-site backup and disaster recovery capabilities. You can also define retention policies and perform tape-to-tape copies for data migration or long-term archival.
Option A, Amazon Elastic File System (Amazon EFS), is a fully managed file storage service for EC2 instances. It is not the appropriate service for extending the capacity of a physical tape library.

Option B, Amazon Elastic Block Store (Amazon EBS), provides block-level storage volumes for EC2 instances. It is also not the appropriate service for extending the capacity of a physical tape library.
Option C, Amazon S3 (Simple Storage Service), is an object storage service that provides scalable storage for various use cases. While it can be used for backup and long-term storage, it does not directly extend the capacity of a physical tape library.
Therefore, option D, AWS Storage Gateway, is the most suitable AWS service for extending the capacity of a physical tape library to the AWS Cloud.


AWS Storage Gateway is a hybrid cloud storage service that enables seamless integration between on- premises environments and the AWS Cloud. It provides a bridge between on-premises applications and AWS storage services, allowing you to store data securely and durably in the cloud while retaining on- premises access.
With AWS Storage Gateway, you can leverage the Tape Gateway feature, which emulates a virtual tape library (VTL) in the AWS Cloud. This allows you to extend your existing tape-based backup infrastructure to the cloud without the need for physical tapes. You can use the Tape Gateway to store backups in Amazon S3 or Glacier, providing virtually unlimited storage capacity.
By configuring the Tape Gateway, the company can connect their existing physical tape library to the AWS Cloud. It acts as a gateway device that manages the transfer of data between the on-premises tape library and the cloud storage.
 

---


Q224. A systems administrator created a new IAM user for a developer and assigned the user an access key instead of a user name and password. What is the access key used for?

- A) To access the AWS account as the AWS account root user
- B) To access the AWS account through the AWS Management Console
- [x] C) To access the AWS account through a CLI
- D) To access all of a company's AWS accounts




---


Q225. Which AWS service supports the deployment and management of applications in the AWS Cloud?

- A) Amazon CodeGuru
- B) AWS Fargate
- C) AWS CodeCommit
- [x] D) AWS Elastic Beanstalk

AWS Elastic Beanstalk is a fully managed service provided by Amazon Web Services (AWS) that supports the deployment and management of applications in the AWS Cloud. It simplifies the process of deploying and scaling applications by automatically handling the deployment details, such as capacity provisioning, load balancing, and application health monitoring.
With AWS Elastic Beanstalk, developers can simply upload their application code, and the service takes care of the underlying infrastructure and resources needed to run the application. It supports various programming languages and platforms, including Java, .NET, Node.js, Python, Ruby, Go, and more.
The service provides features like automatic scaling, environment configuration management, health monitoring, and application versioning. It allows developers to focus on writing code and application logic, while AWS Elastic Beanstalk handles the deployment, scaling, and management aspects.
 
 
B. AWS Fargate: AWS Fargate is a compute engine for containers that allows users to run containers without managing the underlying infrastructure. It provides serverless container deployment, but it is not specifically designed for application deployment and management.
C. AWS CodeCommit: AWS CodeCommit is a fully managed source control service that hosts private Git repositories. It provides version control for code and collaboration among development teams but does not focus on application deployment and management.



---



Q226. When a user wants to utilize their existing per-socket, per-core, or per-virtual machine software licenses for a Microsoft Windows server running on AWS, which Amazon EC2 instance type is required?

- A) Spot Instances
- B) Dedicated Instances
- [x] C) Dedicated Hosts
- D) Reserved Instances

 
Dedicated Hosts provide physical servers dedicated exclusively to a single customer. With Dedicated Hosts, you have full control over the underlying hardware and can bring your own software licenses, including per-socket, per-core, or per-virtual machine licenses for Microsoft Windows Server. By using Dedicated Hosts, you can run your Windows Server instances on dedicated hardware and utilize your existing software licenses without any software licensing restrictions that might apply to other EC2 instance types.

---


Q227. A company has deployed an Amazon EC2 instance. Which option is an AWS responsibility under the AWS shared responsibility model?

- A) Managing and encrypting application data
- B) Installing updates and security patches of guest operating system
- [x] C) Configuration of infrastructure devices
- D) Configuration of security groups on each instance

 

---

Q228. A company wants to migrate a database from an on-premises environment to Amazon RDS. After the migration is complete, which management task will the company still be responsible for?

- A) Hardware lifecycle management
- [x] B) Application optimization
- C) Server maintenance
- D) Power, network, and cooling provisioning

 

---

> [!IMPORTANT]
> Q229. A company is migrating to the AWS Cloud. The company wants to understand and identify potential security misconfigurations or unexpected behaviors. The company wants to prioritize any protective controls it might need. Which AWS Cloud Adoption Framework (AWS CAF) security perspective capability will meet these requirements?

- A) Identity and access management (security)
- [x] B) Threat detection (security)
- C) Platform engineering (platform)
- D) Availability and continuity management (operations)

 

> The Threat detection capability within the security perspective of the AWS CAF focuses on identifying and mitigating potential security threats and risks in the cloud environment. It involves implementing measures to detect and respond to security incidents, including monitoring and analyzing system logs, network traffic, and other security-relevant data to identify any malicious or unauthorized activities.

> By leveraging threat detection capabilities, the company can gain visibility into security events, monitor for potential misconfigurations or unexpected behaviors, and implement appropriate controls to protect their cloud resources.


---

Q230. Which characteristic of the AWS Cloud helps users eliminate underutilized CPU capacity?

- A) Agility
- [x] B) Elasticity
- C) Reliability
- D) Durability

---


Q231. Which AWS Cloud service can send alerts to customers if custom spending thresholds are exceeded?

- [x] A) AWS Budgets
- B) AWS Cost Explorer
- C) AWS Cost Allocation Tags
- D) AWS Organizations


AWS Budgets is a service that allows customers to set custom spending thresholds and receive alerts when those thresholds are exceeded. It helps customers monitor and control their AWS costs by providing notifications via email or Amazon Simple Notification Service (SNS) when spending exceeds the defined thresholds.

AWS Budgets enables customers to set budgets based on cost, usage, or reservation utilization. They can specify the threshold amount, the time period, and the notification preferences. When the actual costs or usage exceed the defined thresholds, AWS Budgets sends alerts to notify customers so they can take appropriate actions to manage their spending.

The other options do not provide this specific functionality:

B. AWS Cost Explorer is a service that helps customers visualize, analyze, and forecast their AWS costs. While it provides insights into cost usage and trends, it does not have the capability to send alerts for custom spending thresholds.

C. AWS Cost Allocation Tags are used for cost allocation and analysis purposes. They help customers categorize and track costs by different dimensions, such as project, team, or environment. However, they do not have the functionality to send alerts for custom spending thresholds.
 

---

> [!IMPORTANT]
> Q232. A company plans to migrate to the AWS Cloud. The company wants to use the AWS Cloud Adoption Framework (AWS CAF) to define and track business outcomes as part of its cloud transformation journey. Which AWS CAF governance perspective capability will meet these requirements?

- [x] A) Benefits management (governance)
- B) Risk management (governance)
- C) Application portfolio management (governance)
- D) Cloud financial management (governance)


> The Benefits management capability in the AWS CAF governance perspective focuses on defining and tracking the business outcomes that an organization aims to achieve through its cloud transformation journey. It helps the organization identify and articulate the expected benefits, aligning them with specific strategic objectives or goals.

> By leveraging the Benefits management capability, the company can define and document the desired business outcomes it wants to achieve with its migration to the AWS Cloud. It provides a structured approach to identify, measure, and track the realization of these outcomes over time. This capability helps the organization assess the success and impact of its cloud adoption efforts and make informed decisions based on the achieved benefits.

> The other options are not directly related to defining and tracking business outcomes:

> B. Risk management focuses on identifying, assessing, and mitigating risks associated with cloud adoption. While important, it does not specifically address the requirement of defining and tracking business outcomes.
> C. Application portfolio management focuses on assessing and managing the organization's application landscape during cloud adoption. It helps identify applications suitable for migration, retirement, or modernization. While relevant to the cloud transformation journey, it does not specifically address the requirement of defining and tracking business outcomes.
> D. Cloud financial management focuses on managing the financial aspects of cloud adoption, such as cost optimization, budgeting, and resource allocation. While financial management is an important aspect of a cloud transformation journey, it does not specifically address the requirement of defining and tracking business outcomes.

---

> [!IMPORTANT]
> Q233. A company needs to quickly and securely move files over long distances between its client and an Amazon S3 bucket. Which S3 feature will meet this requirement?

- A) S3 Versioning
- [x] B) S3 Transfer Acceleration
- C) S3 ACLs
- D) S3 Intelligent-Tiering

<img width="668" alt="image" src="https://github.com/user-attachments/assets/64ccf60c-3a2e-4c15-aace-830bac130a08" />

Amazon S3 Transfer Acceleration is a bucket-level feature that enables fast, easy, and secure transfers of files over long distances between your client and an S3 general purpose bucket. Transfer Acceleration is designed to optimize transfer speeds from across the world into S3 general purpose buckets. Transfer Acceleration takes advantage of the globally distributed edge locations in Amazon CloudFront. As the data arrives at an edge location, the data is routed to Amazon S3 over an optimized network path.


With S3 Transfer Acceleration, data is routed through the nearest Amazon CloudFront edge location to the client, reducing the latency and improving transfer speeds. It is particularly useful when transferring large files or when there is a significant geographical distance between the client and the S3 bucket.

To use S3 Transfer Acceleration, the client uploads or downloads data to/from a unique URL that is specific to the accelerated transfer. This URL includes the "s3-accelerate" keyword, and Amazon S3 automatically routes the data through the optimized network path.

The other options are not directly related to improving transfer speeds or securely moving files over long distances:

A. S3 Versioning is a feature that allows you to keep multiple versions of an object in an S3 bucket. It does not specifically address the requirement of fast and secure file transfers.

C. S3 ACLs (Access Control Lists) are used to manage access permissions for objects in an S3 bucket. While ACLs are important for securing access to objects, they do not directly address the requirement of fast and secure file transfers.

D. S3 Intelligent-Tiering is a storage class in Amazon S3 that automatically moves objects between different storage tiers based on their access patterns. While it can help optimize storage costs, it does not specifically address the requirement of fast and secure file transfers.


---

Q234. A company needs to continuously run an experimental workload on an Amazon EC2 instance and stop the instance after 12 hours. Which instance purchasing option will meet this requirement MOST cost-effectively?

- [x] A) On-Demand Instances
- B) Reserved Instances
- C) Spot Instances
- D) Dedicated Instances


---

Q235. Which cloud transformation journey phase of the AWS Cloud Adoption Framework (AWS CAF) focuses on demonstrating how the cloud helps accelerate business outcomes?

- A) Scale
- [x] B) Envision
- C) Align
- D) Launch


---


Q236. Which option is a customer responsibility under the AWS shared responsibility model?

- A) Maintenance of underlying hardware of Amazon EC2 instances
- [x] B) Application data security
- C) Physical security of data centers
- D) Maintenance of VPC components

---


Q237. A company wants its Amazon EC2 instances to operate in a highly available environment, even if there is a natural disaster in a particular geographic area. Which approach will achieve this goal?

- [x] A) Use EC2 instances in multiple AWS Regions.
- B) Use EC2 instances in multiple Amazon CloudFront locations.
- C) Use EC2 instances in multiple edge locations.
- D) Use EC2 instances in AWS Local Zones.

https://aws.amazon.com/about-aws/global-infrastructure/localzones/

---


Q238 is the same as Q224.

---

> [!IMPORTANT]
> Q239. A company is moving an on-premises data center to the AWS Cloud. The company must migrate 50 petabytes of file storage data to AWS with the least possible operational overhead. Which AWS service or resource should the company use to meet these requirements?

- [x] A) AWS Snowmobile
- B) AWS Snowball Edge
- C) AWS Data Exchange
- D) AWS Database Migration Service (AWS DMS)


To migrate 50 petabytes of file storage data from an on-premises data center to AWS with the least possible operational overhead, the best AWS service is AWS Snowmobile.

AWS Snowmobile is purpose-built for large-scale data migrations, capable of transferring up to 100 petabytes per Snowmobile truck in a single trip. It is designed for exabyte-scale data transfers and is managed entirely by AWS personnel, minimizing operational overhead for the customer.

AWS Snowball Edge is also a physical data transfer device but is designed for smaller-scale transfers (up to ~80 TB per device), making it impractical for 50 PB migrations compared to Snowmobile.

AWS Data Exchange is for subscribing to and sharing third-party data, not for bulk migration of customer-owned storage.

AWS Database Migration Service (DMS) is tailored for migrating databases, not for bulk file storage.

---

> [!IMPORTANT]
> Q240. A company has an application with robust hardware requirements. The application must be accessed by students who are using lightweight, low-cost laptops. Which AWS service will help the company deploy the application without investing in backend infrastructure or high-end client hardware?

- [x] A) Amazon AppStream 2.0
- B) AWS AppSync
- C) Amazon WorkLink
- D) AWS Elastic Beanstalk


---

Q241. A company wants to query its server logs to gain insights about its customers' experiences. Which AWS service will store this data MOST cost-effectively?

- A) Amazon Aurora
- B) Amazon Elastic File System (Amazon EFS)
- C) Amazon Elastic Block Store (Amazon EBS)
- [x] D) Amazon S3

 
For storing server logs in a way that is most cost-effective and supports querying for customer insights, Amazon S3 is the best option.

Amazon S3 offers extremely low storage costs, with the ability to set lifecycle policies for archiving or deleting old logs, making it highly cost-effective for storing large amounts of log data.

Logs stored in S3 can be queried using tools like Amazon Athena, which allows for serverless querying without moving the data, further reducing operational overhead and costs.
 

---

Q242. A company wants to automatically add and remove Amazon EC2 instances. The company wants the EC2 instances to adjust to varying workloads dynamically. Which service or feature will meet these requirements?

- A) Amazon DynamoDB
- B) Amazon EC2 Spot Instances
- C) AWS Snow Family
- [x] D) Amazon EC2 Auto Scaling


---

> [!IMPORTANT]
> Q243. A company is running a critical workload on an Amazon RDS DB instance. The company needs the DB instance to be highly available with a recovery time of less than 5 minutes. Which solution will meet these requirements?

- A) Create a read replica of the DB instance.
- B) Create a template of the DB instance by using AWS CloudFormation.
- C) Take frequent snapshots of the DB instance. Store the snapshots in Amazon S3.
- [x] D) Modify the DB instance to be a Multi-AZ deployment.


Automatic fail over:

- Amazon RDS Multi-AZ with one standby

  Support high availability for your application with automatic database failover that completes as quickly as 60 seconds with zero data loss and no manual intervention.

  Amazon RDS Multi-AZ with two readable standbys: Automatically failover in typically under 35 seconds with zero data loss and with no manual intervention.

To achieve high availability for a critical Amazon RDS DB instance with a recovery time objective (RTO) of less than 5 minutes, the recommended solution is to modify the DB instance to be a Multi-AZ deployment.

Multi-AZ deployments automatically maintain a synchronous standby replica in a different Availability Zone. In the event of a failure, Amazon RDS will automatically fail over to the standby, minimizing downtime.

Typical failover times for Multi-AZ deployments are between 60–120 seconds (1–2 minutes), well within the 5-minute requirement.

Read replicas are intended for scaling read workloads and do not provide automatic failover; promoting a read replica is a manual process and does not guarantee recovery within 5 minutes.

Creating CloudFormation templates or taking frequent snapshots enables disaster recovery but involves manual intervention and longer recovery times, often exceeding several minutes or even hours


---

> [!IMPORTANT]
> Q244. A company wants to identify Amazon S3 buckets that are shared with another AWS account. Which AWS service or feature will meet these requirements?

- A) AWS Lake Formation
- B) IAM credential report
- C) Amazon CloudWatch
- [x] D) IAM Access Analyzer


<img width="600" alt="image" src="https://github.com/user-attachments/assets/06468373-59b8-4267-a3c7-8c212873b8c4" />

---

Q245. Which AWS service gives users the ability to build interactive business intelligence dashboards that include machine learning insights?
- A) Amazon Athena
- B) Amazon Kendra
- [x] C) Amazon QuickSight
- D) Amazon Redshift


---

> [!IMPORTANT]
> Q246. Which action is a security best practice for access to sensitive data that is stored in an Amazon S3 bucket?
- A) Enable S3 Cross-Region Replication (CRR) on the S3 bucket.
- [x] B) Use IAM roles for applications that require access to the S3 bucket.
- C) Configure AWS WAF to prevent unauthorized access to the S3 bucket.
- D) Configure Amazon GuardDuty to prevent unauthorized access to the S3 bucket.

---

Q247. A company wants to know more about the benefits offered by cloud computing. The company wants to understand the operational advantage of agility. How does AWS provide agility for users?
- A) The ability to ensure high availability by deploying workloads to multiple regions
- B) A pay-as-you-go model for many services and resources
- C) The ability to transfer infrastructure management to the AWS Cloud
- [x] D) The ability to provision and deprovision resources quickly with minimal effort

---


> [!IMPORTANT]
> Q248. Which AWS service should users use to learn about AWS service availability and operations?
- A) Amazon EventBridge
- B) AWS Service Catalog
- C) AWS Control Tower
- [x] D) AWS Health Dashboard

---
 

Q249. Which AWS service or tool can be used to capture information about inbound and outbound traffic in an Amazon VPC?
- [x] A) VPC Flow Logs
- B) Amazon Inspector
- C) VPC endpoint services
- D) NAT gateway

---



> [!IMPORTANT]
> Q250. A company plans to migrate to the AWS Cloud. The company is gathering information about its on-premises infrastructure and requires information such as the hostname, IP address, and MAC address. Which AWS service will meet these requirements?
- A) AWS DataSync
- B) AWS Application Migration Service
- [x] C) AWS Application Discovery Service
- D) AWS Database Migration Service (AWS DMS)

---


Q251. Which of the following describes some of the core functionality of Amazon S3?
- A) Amazon S3 is a high-performance block storage service that is designed for use with Amazon EC2.
- [x] B) Amazon S3 is an object storage service that provides high-level performance, security, scalability, and data availability.
- C) Amazon S3 is a fully managed, highly reliable, and scalable file storage system that is accessible over the industry-standard SMB protocol.
- D) Amazon S3 is a scalable, fully managed elastic NFS for use with AWS Cloud services and on-premises resources.

---

Q252. Which AWS services or features enable users to connect on-premises networks to a VPC? (Choose two.)
- [x] A) AWS VPN
- B) Elastic Load Balancing
- [x] C) AWS Direct Connect
- D) VPC peering
- E) Amazon CloudFront

---


Q253. A user needs to quickly deploy a nonrelational database on AWS. The user does not want to manage the underlying hardware or the database software. Which AWS service can be used to accomplish this?
- A) Amazon RDS
- [x] B) Amazon DynamoDB
- C) Amazon Aurora
- D) Amazon Redshift


---

Q254. Which AWS service or feature can a company use to apply security rules to specific Amazon EC2 instances?
A) Network ACLs
- [x] B) Security groups
C) AWS Trusted Advisor
D) AWS WAF


---


Q255. A company wants to create templates that the company can reuse to deploy multiple AWS resources. Which AWS service or feature can the company use to meet this requirement?

- A) AWS Marketplace
- B) Amazon Machine Image (AMI)
- [x] C) AWS CloudFormation
- D) AWS OpsWorks

---

> [!IMPORTANT]
> Q256. A company is building an application that requires the ability to send, store, and receive messages between application components. The company has another requirement to process messages in first-in, first-out (FIFO) order. Which AWS service should the company use?

- A) AWS Step Functions
- B) Amazon Simple Notification Service (Amazon SNS)
- C) Amazon Kinesis Data Streams
- [x] D) Amazon Simple Queue Service (Amazon SQS)


---


Q257. A company wants to migrate its database to a managed AWS service that is compatible with PostgreSQL. Which AWS services will meet these requirements? (Choose two.)

- A) Amazon Athena
- [x] B) Amazon RDS
- C) Amazon EC2
- D) Amazon DynamoDB
- [x] E) Amazon Aurora


---

Q258. A company hosts an application on multiple Amazon EC2 instances. The application uses Amazon Simple Notification Service (Amazon SNS) to send messages. Which AWS service or feature will give the application permission to access required AWS services?

- A) AWS Certificate Manager (ACM)
- [x] B) IAM roles
- C) AWS Security Hub
- D) Amazon GuardDuty

---

Q259. A user has limited knowledge of AWS services, but wants to quickly deploy a scalable Node.js application in the AWS Cloud. Which service should be used to deploy the application?

- A) AWS CloudFormation
- [x] B) AWS Elastic Beanstalk
- C) Amazon EC2
- D) AWS OpsWorks

---

Q260. A company needs a content delivery network that provides secure delivery of data, videos, applications, and APIs to users globally with low latency and high transfer speeds. Which AWS service meets these requirements?

- [x] A) Amazon CloudFront
- B) Elastic Load Balancing
- C) Amazon S3
- D) Amazon Elastic Transcoder

---


Q261. A company needs fully managed, highly reliable, and scalable file storage that is accessible over the Server Message Block (SMB) protocol. Which AWS service will meet these requirements?

- A) Amazon S3
- B) Amazon Elastic File System (Amazon EFS)
- [x] C) Amazon FSx for Windows File Server
- D) Amazon Elastic Block Store (Amazon EBS)


---


Q262. Which task is a responsibility of AWS, according to the AWS shared responsibility model?

- A) Configure identity and access management for applications.
- B) Manage encryption options for data that is stored on AWS.
- C) Configure security groups for Amazon EC2 instances.
- [x] D) Maintain the physical hardware of the infrastructure.

---

Q263. A company has an Amazon EC2 instance in a private subnet. The company wants to initiate a connection to the internet to pull operating system updates while preventing traffic from the internet from accessing the EC2 instance. Which AWS managed service allows this?

- A) VPC endpoint
- [x] B) NAT gateway
- C) Amazon PrivateLink
- D) VPC peering

---

> [!IMPORTANT]
> Q264. A company is storing data that will not be frequently accessed in the AWS Cloud. If the company needs to access the data, the data needs to be retrieved within 12 hours. The company wants a solution that is cost-effective for storage costs for each gigabyte. Which Amazon S3 storage class will meet these requirements?

- A) S3 Standard
- [x] B) S3 Glacier Flexible Retrieval
- C) S3 One Zone-Infrequent Access (S3 One Zone-IA)
- D) S3 Standard-Infrequent Access (S3 Standard-IA)

---

> [!IMPORTANT]
> Q265. Which AWS service or resource can be used to identify services that have been used by a user within a specified date range?

- A) Amazon S3 access control lists (ACLs)
- B) AWS Certificate Manager (ACM)
- C) Network Access Analyzer
- [x] D) AWS Identity and Access Management Access Analyzer



<img width="1019" alt="image" src="https://github.com/user-attachments/assets/0a0e73df-d3fc-41ee-8dad-3117d4a0e3e3" />

<img width="819" alt="image" src="https://github.com/user-attachments/assets/1dbecc66-203a-4191-948a-d391047e6884" />


Policy Generation via CloudTrail Analysis
IAM Access Analyzer reviews AWS CloudTrail logs to track API calls made by IAM entities (users/roles). It generates a policy template listing:

Services accessed (e.g., Amazon S3, EC2)

Specific actions performed (e.g., s3:GetObject, ec2:StartInstances)

Date range (user-defined, up to 90 days) 42.

Step-by-Step Process:

Specify Date Range: During setup, select a timeframe (e.g., June 1–30, 2025) for analysis 4.

Analyze CloudTrail Events: IAM Access Analyzer scans API activity within the chosen window.

Generate Policy: Produces a least-privilege policy template with services/actions used 4.

Review Findings: View services used in the IAM console (e.g., "Service: s3, Actions: ListBucket, GetObject") 15.

Key Requirements:

A CloudTrail trail must be enabled to log API activity 4.

Permissions for IAM Access Analyzer to access CloudTrail (via a service role) 

https://www.conductorone.com/guides/installing-and-harnessing-aws-iam-access-analyzer/#generating-iam-policies-based-on-aws-cloudtrail-logs

---

> [!IMPORTANT]
> Q266. A company wants to create Amazon QuickSight dashboards every week by using its billing data. Which AWS feature or tool can the company use to meet these requirements?

- A) AWS Budgets
- B) AWS Cost Explorer
- [x] C) AWS Cost and Usage Report
- D) AWS Cost Anomaly Detection

<img width="862" alt="image" src="https://github.com/user-attachments/assets/dc5f0e5a-f34a-44c8-8a66-2fc5ac0440f7" />


<img width="837" alt="image" src="https://github.com/user-attachments/assets/65810e81-5505-41d9-9b35-682cf4c527ca" />


After you create a Cost and Usage Report, AWS sends your report to the Amazon S3 bucket that you specify. AWS updates your report at least once a day until your charges are finalized.

Your report files consist of a .csv file or a collection of .csv files and a manifest file. 
You can choose to configure your report data for integration with  
- Amazon Athena
- Amazon Redshift
- Amazon QuickSight


---

Q267 is the same as Q267. 

---
> [!IMPORTANT]
> Q268. A company needs to plan, schedule, and run hundreds of thousands of computing jobs on AWS. Which AWS service can the company use to meet this requirement?

- A) AWS Step Functions
- B) AWS Service Catalog
- C) Amazon Simple Queue Service (Amazon SQS)
- [x] D) AWS Batch

---


> [!IMPORTANT]
> Q269. Which AWS services or features provide high availability and low latency by enabling failover across different AWS Regions? (Choose two.)

- [x] A) Amazon Route 53
- B) Network Load Balancer
- C) Amazon S3 Transfer Acceleration
- [x] D) AWS Global Accelerator
- E) Application Load Balancer

---


Q270. Which of the following is a way to use Amazon EC2 Auto Scaling groups to scale capacity in the AWS Cloud?

- [x] A) Scale the number of EC2 instances in or out automatically, based on demand.
- B) Use serverless EC2 instances.
- C) Scale the size of EC2 instances up or down automatically, based on demand.
- D) Transfer unused CPU resources between EC2 instances.

---


Q271. Which AWS service allows users to model and provision AWS resources using common programming languages?

- A) AWS CloudFormation
- B) AWS CodePipeline
- [x] C) AWS Cloud Development Kit (AWS CDK)
- D) AWS Systems Manager

---



Q272. Which Amazon EC2 instance pricing model can provide discounts of up to 90%?

- A) Reserved Instances
- B) On-Demand
- C) Dedicated Hosts
- [x] D) Spot Instances

---



Q273. Which of the following acts as an instance-level firewall to control inbound and outbound access?

- A) Network access control list
- [x] B) Security groups
- C) AWS Trusted Advisor
- D) Virtual private gateways

---



Q274. A company must be able to develop, test, and launch an application in the AWS Cloud quickly. Which advantage of cloud computing will meet these requirements?
- A) Stop guessing capacity
- B) Trade fixed expense for variable expense
- C) Achieve economies of scale
- [x] D) Increase speed and agility

---

Q275. A company has teams that have different job roles and responsibilities. The company employees often change teams. The company needs to manage permissions for the employees so that the permissions are appropriate for the job responsibilities. Which IAM resource should the company use to meet this requirement with the LEAST operational overhead?

- [x] A) IAM user groups
- B) IAM roles
- C) IAM instance profiles
- D) IAM policies for individual users

---



Q276. Which AWS service can a company use to securely store and encrypt passwords for a database?
- A) AWS Shield
- [x] B) AWS Secrets Manager
- C) AWS Identity and Access Management (IAM)
- D) Amazon Cognito

---



Q277. What can a cloud practitioner use to retrieve AWS security and compliance documents and submit them as evidence to an auditor or regulator?
- A) AWS Certificate Manager
- B) AWS Systems Manager
- [x] C) AWS Artifact
- D) Amazon Inspector


---


> [!IMPORTANT]
> Q278. Which encryption types can be used to protect objects at rest in Amazon S3? (Choose two.)
- [x] A) Server-side encryption with Amazon S3 managed encryption keys (SSE-S3)
- [x] B) Server-side encryption with AWS KMS managed keys (SSE-KMS)
- C) TLS
- D) SSL
- E) Transparent Data Encryption (TDE)

<img width="737" alt="image" src="https://github.com/user-attachments/assets/f265c665-2c35-42b7-a386-b4721d529542" />

server-side encryption is enforced, and cannot be opted out

---


Q279. A company wants to integrate its online shopping website with social media login credentials. Which AWS service can the company use to make this integration?
- A) AWS Directory Service
- B) AWS Identity and Access Management (IAM)
- [x] C) Amazon Cognito
- D) AWS IAM Identity Center (AWS Single Sign-On)

---

Q280. Which AWS service is used to track, record, and audit configuration changes made to AWS resources?
- A) AWS Shield
- [x] B) AWS Config
- C) AWS IAM
- D) Amazon Inspector

---

> [!IMPORTANT]
> Q281. A customer runs an On-Demand Amazon Linux EC2 instance for 3 hours, 5 minutes, and 6 seconds. For how much time will the customer be billed?
- A) 3 hours, 5 minutes
- [x] B) 3 hours, 5 minutes, and 6 seconds
- C) 3 hours, 6 minutes
- D) 4 hours


Minimum Charge: 60 seconds (even if the instance runs for 5 seconds, you pay for 60 seconds).
No Hourly Rounding: Billing is strictly per second after the first minute.

https://aws.amazon.com/ec2/pricing/
Amazon EC2 usage is billed in one-second increments, with a minimum of 60 seconds. The same is true for provisioned storage for Amazon Elastic Block Store (Amazon EBS) volumes. Per-second billing applies to all purchase options. It's available across all Regions and Availability Zones for these instances:

- Amazon Linux
- Windows
- Red Hat Enterprise Linux
- Ubuntu
- Ubuntu Pro

---

Q282. A company website is experiencing DDoS attacks. Which AWS service can help protect the company website against these attacks?
- A) AWS Resource Access Manager
- B) AWS Amplify
- [x] C) AWS Shield
- D) Amazon GuardDuty

---


Q283. A company wants a customized assessment of its current on-premises environment. The company wants to understand its projected running costs in the AWS Cloud. Which AWS service or tool will meet these requirements?
- A) AWS Trusted Advisor
- B) Amazon Inspector
- C) AWS Control Tower
- [x] D) Migration Evaluator

---


Q284. A company that has multiple business units wants to centrally manage and govern its AWS Cloud environments. The company wants to automate the creation of AWS accounts, apply service control policies (SCPs), and simplify billing processes. Which AWS service or tool should the company use to meet these requirements?
- [x] A) AWS Organizations
- B) Cost Explorer
- C) AWS Budgets
- D) AWS Trusted Advisor

---

> [!IMPORTANT]
> Q285. A company is hosting an application in the AWS Cloud. The company wants to verify that underlying AWS services and general AWS infrastructure are operating normally. Which combination of AWS services can the company use to gather the required information? (Choose two.)
- [x] A) AWS Personal Health Dashboard
- B) AWS Systems Manager
- C) AWS Trusted Advisor
- [x] D) AWS Service Health Dashboard
- E) AWS Service Catalog


<img width="1193" alt="image" src="https://github.com/user-attachments/assets/85b4fa54-e866-4d37-9e8b-908f604e7005" />

<img width="1289" alt="image" src="https://github.com/user-attachments/assets/111e916b-ca42-4d89-b18d-9e226ee341b8" />

> keywords: underlying; general aws infrastructure
---


Q286. A company needs to migrate a PostgreSQL database from on-premises to Amazon RDS. Which AWS service or tool should the company use to meet this requirement?
- A) Cloud Adoption Readiness Tool
- B) AWS Migration Hub
- [x] C) AWS Database Migration Service (AWS DMS)
- D) AWS Application Migration Service

---

Q287. Which cloud concept is demonstrated by using AWS Compute Optimizer?
- A) Security validation
- [x] B) Rightsizing
- C) Elasticity
- D) Global reach

---

Q288. A company hosts a large amount of data in AWS. The company wants to identify if any of the data should be considered sensitive. Which AWS service will meet the requirement?

- A) Amazon Inspector
- [x] B) Amazon Macie
- C) AWS Identity and Access Management (IAM)
- D) Amazon CloudWatch

---

Q289. A user has a stateful workload that will run on Amazon EC2 for the next 3 years. What is the MOST cost-effective pricing model for this workload?

- A) On-Demand Instances
- [x] B) Reserved Instances
- C) Dedicated Instances
- D) Spot Instances


---

> [!IMPORTANT]
> Q290. Who enables encryption of data at rest for Amazon Elastic Block Store (Amazon EBS)?

- A) AWS Support
- [x] B) AWS customers
- C) AWS Key Management Service (AWS KMS)
- D) AWS Trusted Advisor


<img width="626" alt="image" src="https://github.com/user-attachments/assets/9948ad49-1cfc-44f7-90b4-6ed0de17c184" />

not enabled by default

---

Q291. What can a user accomplish using AWS CloudTrail?

- A) Generate an IAM user credentials report.
- [x] B) Record API calls made to AWS services.
- C) Assess the compliance of AWS resource configurations with policies and guidelines.
- D) Ensure that Amazon EC2 instances are patched with the latest security updates.

---

Q292. A company is planning to host its workloads on AWS. Which AWS service requires the company to update and patch the guest operating system?

- A) Amazon DynamoDB
- B) Amazon S3
- [x] C) Amazon EC2
- D) Amazon Aurora

---

> [!IMPORTANT]
> Q293. Which AWS service or feature will search for and identify AWS resources that are shared externally?

- A) Amazon OpenSearch Service
- B) AWS Control Tower
- [x] C) AWS IAM Access Analyzer
- D) AWS Fargate


https://github.com/justinjiajia/certifications/blob/main/aws/service_img_demo/iam/iam_access_analyser/readme.md

---

Q294. A company is migrating its workloads to the AWS Cloud. The company must retain full control of patch management for the guest operating systems that host its applications. Which AWS service should the company use to meet these requirements?

- A) Amazon DynamoDB
- [x] B) Amazon EC2
- C) AWS Lambda
- D) Amazon RDS

---

> [!IMPORTANT]
> Q295. At what support level do users receive access to a support concierge?

- A) Basic Support
- B) Developer Support
- C) Business Support
- [x] D) Enterprise Support

This Concierge agent is your primary point of contact for billing or account inquiries;

enterprise on-ramp: White-glove (Concierge) access to billing issues
enterprise: Proactive support in managing billing, including proactive cost optimization, FinOps support, cost analysis, and prioritized answers to billing questions

---

> [!IMPORTANT]
> Q296. Which AWS service can a company use to visually design and build serverless applications?

- A) AWS Lambda
- B) AWS Batch
- [x] C) AWS Application Composer (now AWS Infrastructure Composer)
- D) AWS App Runner

---

Q297. A company wants to migrate to AWS and use the same security software it uses on premises. The security software vendor offers its security software as a service on AWS. Where can the company purchase the security solution?

- A) AWS Partner Solutions Finder
- B) AWS Support Center
- C) AWS Management Console
- [x] D) AWS Marketplace

---

> [!IMPORTANT]
> Q298. A company wants to migrate its PostgreSQL database to AWS. The company does not use the database frequently. Which AWS service or resource will meet these requirements with the LEAST management overhead?

- A) PostgreSQL on Amazon EC2
- B) Amazon RDS for PostgreSQL
- C) Amazon Aurora PostgreSQL-Compatible Edition
- [x] D) Amazon Aurora Serverless

https://aws.amazon.com/rds/aurora/serverless/
With Aurora Serverless, you create a database, specify the desired database capacity range, and connect your applications. You pay on a per-second basis for the database capacity that you use when the database is active, and migrate between standard and serverless configurations with a few steps in the Amazon Relational Database Service (Amazon RDS) console.

For infrequently used PostgreSQL workloads requiring minimal management, Amazon Aurora Serverless (D) is the optimal solution. It eliminates capacity planning, scales automatically, and reduces costs during idle periods.

---

Q299. A company is using Amazon DynamoDB for its application database. Which tasks are the responsibility of AWS, according to the AWS shared responsibility model? (Choose two.)

- A) Classify data.
- B) Configure access permissions.
- C) Manage encryption options.
- [x] D) Provide public endpoints to store and retrieve data.
- [x] E) Manage the infrastructure layer and the operating system.

---


Q300. A company wants to create a globally accessible ecommerce platform for its customers. The company wants to use a highly available and scalable DNS web service to connect users to the platform. Which AWS service will meet these requirements?

- A) Amazon EC2
- B) Amazon VPC
- [x] C) Amazon Route 53
- D) Amazon RDS


---


Q301. Which maintenance task is the customer responsibility, according to the AWS shared responsibility model?

- A) Physical connectivity among Availability Zones
- B) Network switch maintenance
- C) Hardware updates and firmware patches
- [x] D) Amazon EC2 updates and security patches

---

Q302. A company wants to improve its security posture by reviewing user activity through API calls. Which AWS service will meet this requirement?

- A) AWS WAF
- B) Amazon Detective
- C) Amazon CloudWatch
- [x] D) AWS CloudTrail

---

Q303. A company is migrating to the AWS Cloud and plans to run experimental workloads for 3 to 6 months on AWS. Which pricing model will meet these requirements?

- A) Use Savings Plans for a 3-year term.
- B) Use Dedicated Hosts.
- C) Buy Reserved Instances.
- [x] D) Use On-Demand Instances.

---

> [!IMPORTANT]
> Q304. A company that has AWS Enterprise Support is launching a new version of a popular product in 2 months. The company expects a large increase in traffic to its website. The website is hosted on Amazon EC2 instances. Which action should the company take to assess its readiness to scale for this launch?

- A) Replace the EC2 instances with AWS Lambda functions.
- [x] B) Use AWS Infrastructure Event Management (IEM) support. (AWS countdown)
- C) Submit a request on AWS Marketplace to monitor the event.
- D) Review the coverage reports in the AWS Cost Management console.


> AWS Countdown, formerly known as AWS Infrastructure Event Management (IEM), helps you throughout the project lifecycle to assess cloud operational readiness, identify and mitigate risks, and plan capacity, using proven playbooks developed by AWS experts.
> AWS Countdown is a service designed for a broad range of cloud use cases, including cloud migration services, cloud modernization, product launches, and go-live events.
https://aws.amazon.com/premiumsupport/aws-countdown/

 
---

Q305. A company wants to launch multiple workloads on AWS. Each workload is related to a different business unit. The company wants to separate and track costs for each business unit. Which solution will meet these requirements with the LEAST operational overhead?

- [x] A) Use AWS Organizations and create one account for each business unit.
- B) Use a spreadsheet to control the owners and cost of each resource.
- C) Use an Amazon DynamoDB table to record costs for each business unit.
- D) Use the AWS Billing console to assign owners to resources and track costs.


---


Q306. Which option is a shared control between AWS and the customer, according to the AWS shared responsibility model?

- [x] A) Configuration management
- B) Physical and environmental controls
- C) Data integrity authentication
- D) Identity and access management


---

Q307. A company often does not use all of its current Amazon EC2 capacity to run stateless workloads. The company wants to optimize its EC2 costs. Which EC2 instance type will meet these requirements?

- [x] A) Spot Instances
- B) Dedicated Instances
- C) Reserved Instances
- D) On-Demand Instances

> keywords: stateless

---

Q308. A company wants to store data in Amazon S3. The company rarely access the data, and the data can be regenerated if necessary. The company wants to store the data in the most cost-effective storage class. Which S3 storage class will meet this requirement?

- A) S3 Standard
- B) S3 Intelligent-Tiering
- C) S3 Standard-Infrequent Access (S3 Standard-IA)
- [x] D) S3 One Zone-Infrequent Access (S3 One Zone-IA)

just select the one that is the most cost-effective

---

> [!IMPORTANT]
> Q309. A company has migrated its workloads to AWS. The company wants to adopt AWS at scale and operate more efficiently and securely. Which AWS service or framework should the company use for operational support?

- A) AWS Support
- B) AWS Cloud Adoption Framework (AWS CAF)
- [x] C) AWS Managed Services (AMS)
- D) AWS Well-Architected Framework


> AWS Managed Services (AMS) helps eligible AWS Enterprise Support and Enterprise On-Ramp customers adopt AWS at scale and operate more efficiently and securely. Take the complexity out of cloud management with proactive capabilities that extend your team. AMS is a managed services provider that adapts to your infrastructure and applications, ensuring you get the most out of your AWS investment. Our cloud computing managed services help you scale and operate more efficiently and securely with a suite of operational capabilities that leverage AWS services. AMS is available in English for workloads hosted in eligible AWS regions.


> A) AWS Support:	Reactive support (ticket-based) for technical issues—not proactive operational management 8.
> B) AWS Cloud Adoption Framework (CAF):	A planning framework for cloud migration—focuses on organizational readiness, not daily operations 259.
> D) AWS Well-Architected Framework: An audit tool for architectural best practices—lacks hands-on operational support

---

Q310. Which AWS service allows users to download security and compliance reports about the AWS infrastructure on demand?

- A) Amazon GuardDuty.
- B) AWS Security Hub.
- [x] C) AWS Artifact.
- D) AWS Shield.


 
> AWS Artifact is the service that provides access to various security and compliance reports for the AWS infrastructure. It offers a centralized repository of downloadable documents, including compliance reports, audit reports, and other relevant artifacts.
> Through AWS Artifact, users can access and download reports such as AWS Service Organization Control (SOC) reports, Payment Card Industry Data Security Standard (PCI DSS) reports, ISO certifications, and other compliance-related documents. These reports provide information about the security measures, controls, and practices implemented by AWS to protect customer data and ensure compliance with industry standards.
> Option A, Amazon GuardDuty, is a threat detection service that continuously monitors AWS accounts for malicious activity. While GuardDuty provides security insights and alerts, it does not offer downloadable security and compliance reports about the AWS infrastructure.
> Option B, AWS Security Hub, is a security service that aggregates and organizes security findings from various AWS services. While Security Hub provides centralized visibility into security alerts and compliance status, it does not specifically offer the capability to download security and compliance reports on demand.
> Option D, AWS Shield, is a managed Distributed Denial of Service (DDoS) protection service. It focuses on protecting applications and mitigating DDoS attacks, but it does not provide downloadable security and compliance reports.
> 
---

> [!IMPORTANT]
> Q311. A company has a managed IAM policy that does not grant the necessary permissions for users to accomplish required tasks. How can this be resolved?

- A) Enable AWS Shield Advanced.
- [x] B) Create a custom IAM policy.
- C) Use a third-party web application firewall (WAF) managed rule from the AWS Marketplace.
- D) Use AWS Key Management Service (AWS KMS) to create a customer-managed key




---
Q312 is the same as Q195.

---

Q313. Which of the following is entirely the responsibility of AWS, according to the AWS shared responsibility model?

- A) Security awareness and training (shared)
- B) Development of an IAM password policy
- C) Patching of the guest operating system
- [x] D) Physical and environmental controls


---

Q314. According to the AWS shared responsibility model, the customer is responsible for applying the latest security updates and patches for which of the following?

- A) Amazon DynamoDB
- [x] B) Amazon EC2 instances
- C) Amazon RDS instances
- D) Amazon S3
 
> The AWS shared responsibility model defines the division of security responsibilities between AWS and its customers. It outlines which security aspects are the responsibility of AWS and which aspects are the responsibility of the customer.
> In the case of Amazon EC2 (Elastic Compute Cloud) instances, customers are responsible for managing the security of the applications, operating systems, and configurations running on those instances. This includes applying the latest security updates and patches to ensure the instances are protected against known vulnerabilities.
AWS is responsible for the security of the underlying infrastructure, including network security, physical security, and the hypervisor layer. However, the responsibility for maintaining the security of the applications and operating systems running on EC2 instances falls to the customer.
> Option A, Amazon DynamoDB, is a managed NoSQL database service provided by AWS. The responsibility for patching and updating the DynamoDB service itself, including the underlying infrastructure and software, is handled by AWS. Customers are only responsible for securing their access to DynamoDB and configuring appropriate access controls.
> Option C, Amazon RDS instances, refers to managed relational database instances provided by AWS. Similar to DynamoDB, the responsibility for patching and updating the RDS service, including the database engine and underlying infrastructure, is managed by AWS. Customers are responsible for securing their access to RDS and configuring the appropriate database-level security controls.
> Option D, Amazon S3, is a scalable object storage service provided by AWS. The responsibility for securing the S3 service itself, including the underlying infrastructure, is managed by AWS. However, customers are responsible for configuring and managing access controls, encryption, and other security measures for their specific S3 buckets.
 
---

Q315. A company hosts an application on an Amazon EC2 instance. The EC2 instance needs to access several AWS resources, including Amazon S3 and Amazon DynamoDB. What is the MOST operationally efficient solution to delegate permissions?

- [x] A) Create an IAM role with the required permissions. Attach the role to the EC2 instance
- B) Create an IAM user and use its access key and secret access key in the application
- C) Create an IAM user and use its access key and secret access key to create a CLI profile in the EC2 instance.
- D) Create an IAM role with the required permissions. Attach the role to the administrative IAM user

---
Q316. Who is responsible for managing IAM user access and secret keys according to the AWS shared responsibility model?

- A) IAM access and secret keys are static, so there is no need to rotate them
- [x] B) The customer is responsible for rotating keys
- C) AWS will rotate the keys whenever required
- D) The AWS Support team will rotate keys when requested by the customer

  
IAM access keys and secret keys are used for programmatic access to AWS services. It is the responsibility of the customer to manage and rotate these keys to maintain the security of their AWS environment.
AWS provides the IAM service, which allows customers to create and manage IAM users, groups, and roles. As part of IAM user management, customers are responsible for generating, distributing, and rotating access keys and secret keys for their IAM users.
Option A, stating that IAM access and secret keys are static and do not need to be rotated, is incorrect. Rotating access keys and secret keys periodically is recommended as a security best practice to protect against the compromise of long-lived keys.
Option C, suggesting that AWS will rotate the keys whenever required, is not accurate. While AWS offers services like AWS Secrets Manager and AWS Key Management Service (KMS) for managing secrets and encryption keys, the responsibility for managing IAM user access keys and secret keys specifically lies with the customer.
Option D, stating that the AWS Support team will rotate keys when requested by the customer, is not accurate either. The management and rotation of IAM user access keys and secret keys are within the control and responsibility of the customer, and it is not a task performed by the AWS Support team.
 

---

Q317. Which of the following are features of network ACLs as they are used in the AWS Cloud? (Select TWO.)

- [x] A) They are stateless.
- B) They are stateful.
- C) They evaluate all rules before allowing traffic
- [x] D) They process rules in order, starting with the lowest numbered rule, when deciding whether to allow traffic
- E) They operate at the instance level.



---

Q318. An Amazon EC2 instance previously used for development is inaccessible and no longer appears in the AWS Management Console. Which AWS service should be used to determine what action made this EC2 instance inaccessible?

- A) Amazon CloudWatch Logs
- B) AWS Security Hub
- C) Amazon Inspector
- [x] D) AWS CloudTrail


To determine what action made an Amazon EC2 instance inaccessible, you should use:
D. AWS CloudTrail.
Here's the rationale behind this choice:
AWS CloudTrail is a service that provides a detailed history of actions taken by AWS resources within your AWS account. It records API calls and events, including the identity of the caller, the time of the call, the source IP address, and other details. CloudTrail logs can be used to track and investigate actions that may have affected the accessibility or management of AWS resources.
In this scenario, if an EC2 instance is inaccessible and no longer visible in the AWS Management Console, you can consult the CloudTrail logs to identify the actions that were taken on the instance. By searching for events related to the EC2 instance, you can gather information about the operations performed, such as instance terminations, security group changes, or modifications to IAM policies.
Option A, Amazon CloudWatch Logs, is not the most appropriate service for this scenario. While CloudWatch Logs can provide insights into log data and system events, it primarily focuses on collecting and managing log files from various AWS services and applications. It may not have the specific information needed to determine the cause of the EC2 instance's inaccessibility.
Option B, AWS Security Hub, is a service that provides a comprehensive view of security findings and compliance checks across multiple AWS accounts. While Security Hub can help identify security issues and misconfigurations, it is not the primary service to investigate the disappearance or inaccessibility of an EC2 instance.
Option C, Amazon Inspector, is a security assessment service that helps identify vulnerabilities and security issues in your EC2 instances and applications. However, it is not specifically designed to track actions or events related to the management or accessibility of instances.


---


Q319. A company uses Amazon S3 to store records that can contain personally identifiable information (PII). The company wants a solution that can monitor all S3 buckets for PII and immediately alert staff about vulnerabilities. Which AWS service will meet these requirements?

- A) Amazon GuardDuty
- B) Amazon Detective
- [x] C) Amazon Macie
- D) AWS Shield

 
Amazon Macie is a service specifically designed to discover, classify, and protect sensitive data such as personally identifiable information (PII) in AWS. It uses machine learning and pattern matching techniques to analyze the content of S3 buckets and identify sensitive data like social security numbers, credit card numbers, and other forms of PII.
Macie can monitor all S3 buckets in an AWS account and provide alerts and notifications when it detects potential vulnerabilities or sensitive information. It can generate detailed reports, including the location of the sensitive data and its classification, to help organizations understand and manage their data risks more effectively.
Option A, Amazon GuardDuty, is a threat detection service that focuses on identifying malicious and unauthorized activities in AWS accounts and workloads. While GuardDuty provides valuable security monitoring capabilities, it is not specifically designed to monitor S3 buckets for PII or sensitive data.
Option B, Amazon Detective, is a service that helps analyze, investigate, and visualize security-related data in AWS. It provides insights into potential security issues but does not have the primary functionality to monitor S3 buckets for PII.
Option D, AWS Shield, is a service that provides protection against Distributed Denial of Service (DDoS) attacks. It is not directly related to monitoring S3 buckets for PII or vulnerabilities.
 

---

Q320. Which AWS Cloud Adoption Framework (AWS CAF) capability belongs to the business perspective?

- A) Program and project management (governance)
- [x] B) Data science (business)
- C) Observability (operations)
- D) Change and release management (operations)


---

Q321. A company needs a bridge between technology and business to help evolve to a culture of continuous growth and learning. Which perspective in the AWS Cloud Adoption Framework (AWS CAF) serves as this bridge?

- [x] A) People
- B) Governance
- C) Operations
- D) Security

> culture evolution


---

Q322. Which of the following is a characteristic of the AWS account root user?

- A) The root user is the only user that can be configured with multi-factor authentication (MFA)
- B) The root user is the only user that can access the AWS Management Console
- [x] C) The root user is the first sign-in identity that is available when an AWS account is created
- D) The root user has a password that cannot be changed


---

Q323. Which AWS services are supported by Savings Plans? (Select TWO.)
- [x] A) Amazon EC2
- B) Amazon RDS
- [x] C) Amazon SageMaker
- D) Amazon Redshift
- E) Amazon DynamoDB

>  three types of savings plans: compute (ec2, fargate, lambda); ec2 instance; sagemaker
 
---

Q324 is the same as Q2.

---

Q325. Which of the following is the customer's responsibility under the AWS shared responsibility model? (Select TWO.)
- A) Maintain the configuration of infrastructure devices
- B) Maintain patching and updates within the hardware infrastructure
- [x] C) Maintain the configuration of guest operating systems and applications
- [x] D) Manage decisions involving encryption options
- E) Maintain infrastructure hardware
 

---


Q326. A global company wants to use a managed security service for protection from SQL injection attacks. The service also must provide detailed logging information about access to the company's ecommerce applications. Which AWS service will meet these requirements?
- A) AWS Network Firewall
- B) Amazon RDS for SQL Server
- C) Amazon GuardDuty
- [x] D) AWS WAF

AWS WAF is a managed web application firewall service that helps protect web applications from common web exploits, including SQL injection attacks. It provides rules and filters to inspect incoming HTTP and HTTPS requests and block or allow them based on predefined conditions. AWS WAF helps protect against SQL injection attacks by analyzing the content of requests and blocking any malicious SQL injection attempts.

In addition to protecting against SQL injection attacks, AWS WAF also integrates with AWS CloudTrail to provide detailed logging information about access to web applications. CloudTrail captures detailed API activity logs for AWS services, including AWS WAF. By enabling CloudTrail logging for AWS WAF, you can gain visibility into the requests and actions taken by AWS WAF, allowing you to monitor and audit access to your ecommerce applications.

The other options are not the best fit for the given requirements:

A. AWS Network Firewall: AWS Network Firewall is a managed firewall service that provides network-level protection for resources within a VPC (Virtual Private Cloud). While it can provide network-level security, it does not specifically address SQL injection attacks or provide detailed logging information about access to web applications.

B. Amazon RDS for SQL Server: Amazon RDS (Relational Database Service) for SQL Server is a managed database service. While it can provide security features for SQL Server databases, it focuses on database management and security rather than protection against SQL injection attacks and detailed logging information for web applications.

C. Amazon GuardDuty: Amazon GuardDuty is a threat detection service that uses machine learning and anomaly detection to identify potential security issues within AWS accounts and resources. While it can help detect various types of threats, including unauthorized access attempts, it does not specifically focus on protecting against SQL injection attacks or provide detailed logging information about access to web applications.

---

Q327. A company created an Amazon EC2 instance. The company wants to control the incoming and outgoing network traffic at the instance level. Which AWS resource or service will meet this requirement?
- A) AWS Shield
- [x] B) Security groups
- C) Network Access Analyzer
- D) VPC endpoints

 
Security groups are a fundamental component of Amazon EC2 instances and provide control over inbound and outbound traffic at the instance level. A security group acts as a virtual firewall that regulates traffic based on rules defined by the user.
With security groups, you can specify the allowed inbound and outbound traffic based on protocols, ports, and IP addresses. You can configure security group rules to allow specific traffic to reach the instance and control the traffic flow to and from the instance.
Option A, AWS Shield, is a managed Distributed Denial of Service (DDoS) protection service. While AWS Shield helps protect against DDoS attacks, it is not specifically designed for controlling network traffic at the instance level.
Option C, Network Access Analyzer, is a service that helps analyze network traffic in a VPC (Virtual Private Cloud) and provides insights into network topology, traffic paths, and security group rules. However, it doesn't directly control network traffic at the instance level.
Option D, VPC endpoints, allows you to privately connect your VPC to AWS services without requiring public internet access. VPC endpoints enable you to securely access AWS services such as S3, DynamoDB, or other AWS services, but they do not directly control the network traffic at the instance level.
Therefore, the most appropriate AWS resource or service for controlling incoming and outgoing network traffic at the instance level is B. Security groups.


---

Q328. A developer wants AWS users to access AWS services by using temporary security credentials. Which AWS service or feature should the developer use to provide these credentials?
- A) IAM policies
- B) IAM user groups
- [x] C) AWS Security Token Service (AWS STS)
- D) AWS IAM Identity Center (AWS Single Sign-On)

> keyword: temporary

AWS Security Token Service (STS) is specifically designed to provide temporary security credentials for accessing AWS services. It enables users to request temporary credentials that are valid for a specified duration, typically ranging from a few minutes to a few hours.
With AWS STS, users can assume temporary security roles or federated identities to access AWS resources. These temporary credentials can be used for authentication and authorization purposes, and they help enforce the principle of least privilege by providing users with limited access based on their defined roles and permissions.
Option A, IAM policies, is a feature of AWS Identity and Access Management (IAM) that allows you to define permissions and access controls for users and resources. However, IAM policies alone do not provide temporary security credentials.
Option B, IAM user groups, are used to organize IAM users and manage their permissions collectively. However, they do not directly provide temporary security credentials.
Option D, AWS IAM Identity Center (AWS Single Sign-On), is not a valid AWS service or feature. AWS Single Sign-On (SSO) is a service that simplifies user access management across AWS accounts and business applications but does not specifically provide temporary security credentials.

---

Q329. Which task can a company perform by using security groups in the AWS Cloud?
- [x] A) Allow access to an Amazon EC2 instance through only a specific port
- B) Deny access to malicious IP addresses at a subnet level
- C) Protect data that is cached by Amazon CloudFront
- D) Apply a stateless firewall to an Amazon EC2 instance

 

---


Q330. Which AWS service or tool will monitor AWS resources and applications in real time?
- A) AWS Trusted Advisor
- [x] B) Amazon CloudWatch
- C) AWS CloudTrail
- D) AWS Cost Explorer

Amazon CloudWatch is a monitoring and observability service provided by AWS. It allows you to collect and track metrics, collect and monitor log files, set alarms, and automatically react to changes in AWS resources and applications. CloudWatch provides real-time insights into the performance and health of your AWS infrastructure and applications.
With CloudWatch, you can monitor various AWS resources such as EC2 instances, RDS databases, S3 buckets, Lambda functions, and more. It collects and aggregates data from these resources and provides visualizations, customizable dashboards, and real-time alarms to help you monitor the metrics that are important to your applications.
Option A, AWS Trusted Advisor, is a service that provides recommendations to optimize your AWS infrastructure for cost savings, performance, security, and fault tolerance. While it offers valuable insights and recommendations, it is not primarily focused on real-time monitoring of resources and applications.
Option C, AWS CloudTrail, is a service that provides detailed logs of API calls made to your AWS account. It helps with auditing, compliance, and troubleshooting activities. While CloudTrail provides valuable logging information, it does not provide real-time monitoring capabilities.
Option D, AWS Cost Explorer, is a tool that helps you visualize, understand, and analyze your AWS costs and usage over time. It is focused on cost management and analysis rather than real-time monitoring of resources and applications.


---

Q331. A company wants to allow users to authenticate and authorize multiple AWS accounts by using a single set of credentials. Which AWS service or resource will meet this requirement?
- A) AWS Organizations
- B) IAM user
- [x] C) AWS IAM Identity Center (AWS Single Sign-On)
- D) AWS Control Tower



 
AWS Single Sign-On (SSO) (option C) is a service provided by AWS that enables users to authenticate and access multiple AWS accounts and business applications using a single set of credentials. AWS SSO acts as a centralized identity management solution that simplifies user management and access control across multiple accounts.
Here's how AWS SSO meets the specified requirements:
Authenticate and authorize multiple AWS accounts: With AWS SSO, users can log in once using their credentials and access multiple AWS accounts without the need to enter separate credentials for each account. AWS SSO integrates with AWS Organizations (option A) and allows users to access and manage multiple accounts associated with their organization.
Single set of credentials: AWS SSO allows users to use a single set of credentials, such as their corporate credentials or an identity provider (IdP) of their choice, to authenticate and access multiple AWS accounts. This eliminates the need for managing separate IAM users (option B) in each account.
Option A, AWS Organizations, is not the correct choice for this requirement. AWS Organizations is a service that helps you centrally manage and govern multiple AWS accounts, but it does not provide the specific functionality of allowing users to authenticate and authorize multiple accounts using a single set of credentials.
Option B, IAM user, is not the correct choice either. IAM users are specific to individual AWS accounts and are not designed to allow authentication and authorization across multiple accounts using a single set of credentials.
Option D, AWS Control Tower, is a service that helps you set up and govern a secure multi-account environment, but it does not specifically provide the functionality of allowing users to authenticate and authorize multiple accounts using a single set of credentials.


AWS Single Sign-On (SSO) is a service that simplifies user access management across multiple AWS accounts and business applications. It allows users to sign in once using their existing corporate credentials and access multiple AWS accounts without the need for separate IAM user credentials for each account.
With AWS SSO, you can manage user access centrally, define permissions and access policies based on groups, and provide single sign-on access to AWS accounts and applications. It integrates with existing identity providers (IdPs) such as Microsoft Active Directory, enabling users to leverage their corporate credentials for authentication.
Option A, AWS Organizations, is a service that helps manage and organize multiple AWS accounts. While it provides centralized management and governance of AWS accounts, it does not directly enable single sign-on or authentication across multiple accounts.
Option B, IAM user, refers to individual user accounts within an AWS account. IAM users are typically associated with a single AWS account and do not directly provide the ability to authenticate and authorize across multiple accounts using a single set of credentials.
Option D, AWS Control Tower, is a service that helps set up and govern a secure multi-account AWS environment. While it provides account provisioning and governance capabilities, it does not specifically address the requirement of allowing users to authenticate and authorize multiple AWS accounts using a single set of credentials.

---


> [!IMPORTANT]
> Q332. A company uses AWS security services and tools. The company needs a service to help manage the security alerts and must organize the alerts into a single dashboard. Which AWS service should the company use to meet these requirements?
- A) Amazon GuardDuty
- B) Amazon Inspector
- C) Amazon Macie
- [x] D) AWS Security Hub


> AWS Security Hub is a service that provides a comprehensive view of security alerts and compliance status across multiple AWS accounts. It consolidates and organizes security findings from various AWS services and third-party tools into a single dashboard. Key features of AWS Security Hub include:
> - Centralized View: It provides a unified dashboard that aggregates security findings from multiple sources, including Amazon GuardDuty, Amazon Inspector, AWS Firewall Manager, AWS Macie, and more.
> - Prioritized and Detailed Insights: Security Hub prioritizes findings and provides detailed information about the security issues detected, including recommendations for remediation.
> - Automated Compliance Checks: It performs automated compliance checks against industry standards such as CIS AWS Foundations Benchmark and PCI DSS.
> - Integration with Other Tools: It integrates with other AWS services, such as AWS Config and AWS CloudTrail, to provide a more comprehensive view of the security posture.

> Option A, Amazon GuardDuty, is a threat detection service that continuously monitors AWS accounts for malicious activity. While GuardDuty provides security insights and alerts, it does not offer the capability to organize alerts into a single dashboard.
> Option B, Amazon Inspector, is an automated security assessment service that helps in identifying security vulnerabilities in EC2 instances. Like GuardDuty, Inspector provides alerts but does not offer the centralized dashboard functionality.
> Option C, Amazon Macie, is a security service that focuses on data discovery and data loss prevention (DLP). It helps identify sensitive data and monitor data access, but it does not provide a centralized dashboard for managing security alerts.

---

Q333. A company wants to use application stacks to run a workload in the AWS Cloud. The company wants to use pre-configured instances. Which AWS service will meet these requirements?
- [x] A) Amazon Lightsail
- B) Amazon Athena
- C) AWS Outposts
- D) Amazon EC2
 
Amazon Lightsail is a service provided by AWS that offers pre-configured application stacks running on virtual private servers (VPS). It simplifies the process of deploying and managing applications in the cloud by providing pre-configured templates or blueprints for popular application stacks, such as WordPress, LAMP, MEAN, and more. These application stacks come with pre-installed software and configurations, making it easier to deploy an application quickly.
With Amazon Lightsail, you can choose an application stack that matches your requirements, and Lightsail will provision a pre-configured instance with the necessary resources, including compute, storage, and networking. This allows you to get started with your workload without the need for manual instance configuration.
The other options are not the correct answers for this scenario:
B. Amazon Athena: Amazon Athena is a serverless query service that allows you to analyze data stored in Amazon S3 using standard SQL queries. It is not specifically designed to provide pre-configured instances for running application stacks.
C. AWS Outposts: AWS Outposts is a service that extends AWS infrastructure, services, and tools to customer premises. It enables running AWS services on-premises using hardware provided by AWS. It does not provide pre-configured instances for running application stacks in the cloud.
D. Amazon EC2: Amazon EC2 (Elastic Compute Cloud) is a web service that provides resizable compute capacity in the cloud. While EC2 allows you to create instances and configure them to your requirements, it does not specifically offer pre-configured application stacks like Amazon Lightsail.
 

---

Q334. Which option is a responsibility of AWS under the AWS shared responsibility model?

- A) Application data security
- B) Patch management for applications that run on Amazon EC2 instances
- [x] C) Patch management of the underlying infrastructure for managed services
- D) Application identity and access management
  

---

> [!IMPORTANT]
> Q335. Which complimentary AWS service or tool creates data-driven business cases for cloud planning?

- [x] A) Migration Evaluator
- B) AWS Billing Conductor
- C) AWS Billing Console
- D) Amazon Forecast


> Keywords: complimentary AWS service; data-driven business cases

> Migration Evaluator is an AWS service specifically designed to help customers create data-driven business cases for cloud migration and planning. It provides an automated assessment of on-premises environments to generate insights and recommendations for migrating to the AWS Cloud.

> Migration Evaluator collects and analyzes data from your on-premises environment, including infrastructure configurations, utilization metrics, and application dependencies. It then uses this data to generate a comprehensive report that includes cost estimates, TCO (Total Cost of Ownership) analysis, performance comparisons, and other insights to help you make informed decisions about migrating to AWS.

> Option C, AWS Billing Console, is a web-based interface that allows you to view and manage your AWS billing and usage information. However, it does not specifically create data-driven business cases for cloud planning.
> Option D, Amazon Forecast, is a service that uses machine learning algorithms to generate highly accurate forecasts based on historical data. While it can be used for predictive analytics and forecasting, it is not specifically focused on creating business cases for cloud planning.
 

---

Q336. Which AWS service or resource can provide discounts on some AWS service costs in exchange for a spending commitment?

- A) Amazon Detective
- B) AWS Pricing Calculator
- [x] C) Savinas Plans
- D) Basic Support

> Savinas Plans is a program offered by AWS that provides discounts on AWS service costs in exchange for a spending commitment. It allows customers to commit to a specific amount of usage or expenditure on specific AWS services over a period of time, typically one or three years. In return for this commitment, customers receive a discount on the hourly or usage-based charges for the selected services.
> Option A, Amazon Detective, is a service that helps customers analyze, investigate, and visualize security- related data in their AWS environment. It is not related to providing discounts on AWS service costs.
> Option B, AWS Pricing Calculator, is a tool that allows customers to estimate the costs of using various AWS services based on their usage patterns and requirements. It does not provide discounts on AWS service costs.
> Option D, Basic Support, is the default level of support provided by AWS to all customers and does not provide discounts on AWS service costs.
 

---

Q337. A company has services that run in the AWS Cloud and in an on-premises data center. The company wants to set up a dedicated, high-throughput connection between AWS and the data center. Which AWS service will meet these requirements?

- A) Amazon VPC
- [x] B) AWS Direct Connect
- C) Amazon CloudFront
- D) Amazon API Gateway
 
AWS Direct Connect is the service that provides a dedicated network connection between an on-premises data center and AWS. It allows for a private and secure link with high throughput and low latency.
By using AWS Direct Connect, the company can establish a private connection that bypasses the public internet, providing a more consistent and reliable network performance compared to internet-based connections. This is especially beneficial for workloads that require large data transfers or low latency, such as accessing applications or transferring data between the on-premises data center and AWS.
Option A, Amazon VPC (Virtual Private Cloud), is the networking service that allows customers to provision and manage isolated cloud resources within their own virtual network. While Amazon VPC is used in conjunction with AWS Direct Connect to establish the connectivity, it is not the service responsible for the dedicated, high-throughput connection itself.
Option C, Amazon CloudFront, is a content delivery network (CDN) service that accelerates the delivery of web content and applications to end-users. It does not provide the dedicated, high-throughput connection between the data center and AWS.
Option D, Amazon API Gateway, is a fully managed service for creating, deploying, and managing APIs. It is not directly related to setting up a dedicated, high-throughput connection between AWS and the data center.
 


---
> [!IMPORTANT]
> Q338. A company wants to verify if multi-factor authentication (MFA) is enabled for all users within its AWS accounts. Which AWS service or resource will meet this requirement?

- A) AWS Cost and Usage Report
- [x] B) IAM credential reports
- C) AWS Artifact
- D) Amazon CloudFront reports

 
IAM (Identity and Access Management) credential reports provide detailed information about the IAM users and their security credentials within an AWS account. These reports can be used to verify if multi-factor authentication (MFA) is enabled for all users.
IAM credential reports include information such as the user's access key status, password last used date, password reset required status, and MFA device status. By reviewing the MFA device status in the IAM credential reports, you can determine whether MFA is enabled for each IAM user. Option A, AWS Cost and Usage Report, provides detailed cost and usage information for an AWS account, but it does not provide information about MFA settings or user credentials.
Option C, AWS Artifact, is a service that provides access to AWS compliance reports, including audit reports, certifications, and other compliance-related documents. It does not provide information about MFA settings for IAM users.
Option D, Amazon CloudFront reports, provides detailed reports on the usage and performance of the CloudFront content delivery network service. It does not provide information about MFA settings for IAM users.
 

---
Q339 is the same as Q310. 
 

---
> [!IMPORTANT]
> Q340. An external auditor has requested that a company provide a list of all its IAM users, including the status of users' credentials and access keys. What is the SIMPLEST way to provide this information?

- A) Create an IAM user account for the auditor, granting the auditor administrator permissions
- B) Take a screenshot of each user's page in the AWS Management Console, then provide the screenshots to the auditor
- [x] C) Download the IAM credential report, then provide the report to the auditor
- D) Download the AWS Trusted Advisor report, then provide the report to the auditor
 
 


---

Q341. A company wants to provision and manage its AWS infrastructure by using the common programming languages Typescript, Python, Java, and .NET. Which AWS service will meet this requirement?

- A) AWS CodeBuild
- B) AWS CloudFormation
- C) AWS CLI
- [x] D) AWS Cloud Development Kit (AWS CDK)

 

---

Q342. Which Amazon EC2 pricing model provides the MOST cost savings for an always-up, right-sized database server running for a project that will last 1 year?

- A) On-Demand Instances
- B) Convertible Reserved Instances
- C) Spot Instances
- [x] D) Standard Reserved Instances


Standard Reserved Instances provide the most cost savings for long-term, sustained workloads such as an always-up, right-sized database server running for a year. Here's why Standard Reserved Instances are the best choice:
Long-term commitment: Standard Reserved Instances require a 1-year or 3-year commitment, which aligns with the duration of the project. By committing to a longer-term, you can receive a significant discount compared to On-Demand Instances.
Cost savings: Standard Reserved Instances provide the highest level of cost savings compared to On-Demand Instances and Convertible Reserved Instances. The savings can range from 30% to 75% off the On-Demand price, depending on the instance type and term commitment.
Fixed configuration: Standard Reserved Instances have a fixed configuration throughout the term of the reservation. While they don't offer the flexibility to modify the instance attributes like Convertible Reserved Instances, they are suitable for workloads with consistent requirements.
Option A, On-Demand Instances, provides no upfront commitment or long-term savings. While it offers flexibility and is suitable for short-term or unpredictable workloads, it is not the most cost-effective choice for a one-year project.
Option B, Convertible Reserved Instances, offer flexibility and the ability to modify instance attributes, but they generally provide lower cost savings compared to Standard Reserved Instances.
Option C, Spot Instances, can offer significant cost savings but are not recommended for always-up, critical workloads like a database server. Spot Instances are subject to availability and can be terminated with a short notice if the spot price exceeds the maximum bid. They are suitable for fault-tolerant workloads that can handle interruptions.

---

Q343 is the same as Q223.

---
Q344. A company is using the AWS Free Tier for several AWS services for an application. What will happen if the Free Tier usage period expires or if the application use exceeds the Free Tier usage limits?

- [x] A) The company will be charged the standard pay-as-you-go service rates for the usage that exceeds the Free Tier usage.
- B) AWS Support will contact the company to set up standard service charges.
- C) The company will be charged for the services it consumed during the Free Tier period, plus additional charges for service consumption after the Free Tier period.
- D) The company's AWS account will be frozen and can be restarted after a payment plan is established.

 
When the Free Tier usage period expires or if the application usage exceeds the Free Tier usage limits, the company will no longer be eligible for the free services and usage provided through the Free Tier. Any usage that exceeds the Free Tier limits will be billed at the standard pay-as-you-go service rates.
AWS does not automatically charge for services consumed during the Free Tier period unless the usage exceeds the Free Tier limits. The company will only be charged for the services it consumed during the Free Tier period if they exceed the allocated free limits.
Option B, AWS Support contacting the company to set up standard service charges, is not directly related to the Free Tier usage. AWS Support is a separate service with its own pricing plans.
Option C, charging the company for the services consumed during the Free Tier period, as well as additional charges for service consumption after the Free Tier period, is not accurate. The company will only be charged for usage that exceeds the Free Tier limits after the Free Tier period ends.
Option D, freezing the company's AWS account and requiring a payment plan to restart it, is not how AWS handles Free Tier usage expiration or exceeding Free Tier limits. The account will remain active, and the company will be billed for usage that exceeds the Free Tier limits.
 

---

> [!IMPORTANT]
> Q345. A company wants to monitor its workload performance. The company wants to ensure that the cloud services are delivered at a level that meets its business needs. Which AWS Cloud Adoption Framework (AWS CAF) perspective will meet these requirements?

- A) Business
- B) Governance
- C) Platform
- [x] D) Operations  
 
> The operations perspective focuses on ensuring that cloud services are delivered at a level that is agreed upon with your business stakeholders. Automating and optimizing operations will allow you to effectively scale while improving the reliability of your workloads.

---
Q346. A company wants to migrate its applications to the AWS Cloud. The company plans to identify and prioritize any business transformation opportunities and evaluate its AWS Cloud readiness. Which AWS service or tool should the company use to meet these requirements?

- [x] A) AWS Cloud Adoption Framework (AWS CAF)
- B) AWS Managed Services (AMS)
- C) AWS Well-Architected Framework
- D) AWS Migration Hub


---

Q347. A company need an AWS service that provides a clear baseline of what the company runs in its on-premises data centers. The company needs the projected cost to run its on-premises workloads in the AWS Cloud. What AWS service or tool will meet these requirements?

- A) AWS Compute Optimizer
- B) AWS Cost Explorer
- C) AWS Systems Manager Agent (SSM Agent)
- [x] D) Migration Evaluator

 
> Migration Evaluator is an AWS service that helps organizations assess the potential costs and benefits of migrating their on-premises workloads to the AWS Cloud. It provides a comprehensive analysis of the existing on-premises environment and estimates the projected costs and performance of running those workloads in the AWS Cloud.

> By using Migration Evaluator, the company can:
> - Obtain a Baseline of On-Premises Workloads: Migration Evaluator collects information about the company's on-premises workloads, including infrastructure, applications, and usage patterns. It provides visibility into the current state of the on-premises environment, creating a clear baseline for analysis and comparison.
> - Projected Cost Analysis: Migration Evaluator uses this baseline information to generate a detailed cost analysis for running the on-premises workloads in the AWS Cloud. It estimates the costs associated with AWS services, such as compute, storage, networking, and data transfer, based on the workload characteristics and usage patterns. This analysis helps the company understand the potential cost savings or increases that can be achieved through migration.
> Option A, AWS Compute Optimizer, is a service that analyzes existing EC2 instances and provides recommendations for optimizing their performance and cost. While it can help optimize AWS resources, it does not provide the specific analysis and cost projection for running on-premises workloads in the AWS Cloud.
> Option B, AWS Cost Explorer, is a service that provides cost analysis and visualization of AWS usage. While it can help analyze costs for AWS resources, it does not provide the specific analysis and cost projection for on-premises workloads.
> Option C, AWS Systems Manager Agent (SSM Agent), is an agent that can be installed on EC2 instances to enable integration with AWS Systems Manager. It is not directly related to providing a baseline or projected cost analysis for on-premises workloads.
 

---

Q348. A company acquired another corporation. The company now has two AWS accounts. Which AWS service or tool can the company use to consolidate the billing for these two accounts?

- A) AWS Systems Manager
- [x] B) AWS Organizations
- C) AWS License Manager
- D) Cost Explorer


AWS Organizations is a service that helps manage multiple AWS accounts within an organization. It provides features for centralizing and consolidating billing, as well as managing and governing multiple accounts.
By using AWS Organizations, the company can:
Consolidate Billing: AWS Organizations allows the company to create a single payment method and consolidate billing for multiple AWS accounts. It provides a hierarchical structure where the acquired account can be added as a member account under the main AWS Organizations account. This enables unified billing and cost allocation across the organization.
Establish Governance: AWS Organizations provides features for managing and governing multiple accounts. It allows the company to set up policies and permissions that can be applied across all member accounts. This helps ensure consistent standards and security measures are applied to the acquired account.
Option A, AWS Systems Manager, is a service that helps manage and operate resources in AWS. While it provides features for managing multiple AWS accounts, it does not specifically address billing consolidation.
Option C, AWS License Manager, is a service that helps manage software licenses in AWS. While it can be useful for managing licenses across multiple accounts, it does not specifically address billing consolidation.
Option D, Cost Explorer, is a service that provides cost analysis and visualization of AWS usage. While it can help analyze costs for multiple accounts, it does not provide the specific functionality for consolidating billing.
 

---

Q349. A company wants to set up its workloads to perform their intended functions and recover quickly from failure. Which pillar of the AWS Well-Architected Framework aligns with these goals?

- A) Performance efficiency
- B) Sustainability
- [x] C) Reliability
- D) Security
 
 

---
Q350. A company wants to migrate petabytes of data from its on-premises data center to AWS. The company does not want to use an internet connection to perform the migration. Which AWS service will meet these requirements?

- A) AWS DataSync
- B) Amazon Connect
- [x] C) AWS Snowmobile
- D) AWS Direct Connect

  
 

---


> [!IMPORTANT]
> Q351. How does the AWS Enterprise Support Concierge team help users?

- A) Supporting application development
- B) Providing architecture guidance
- [x] C) Answering billing and account inquiries
- D) Answering questions regarding technical support cases

 
The AWS Enterprise Support Concierge team is a specialized support team that focuses on providing personalized assistance and guidance to AWS Enterprise Support customers. While they may help with various aspects of AWS usage, their primary role is to assist with billing and account-related inquiries.
The team can help users with tasks such as:
Billing Inquiries: The Enterprise Support Concierge team can assist users with questions related to AWS billing, including understanding invoices, cost allocation, and billing reports. They can help users navigate the AWS billing console and provide explanations or clarifications on billing-related topics.
Account Management: The team can assist with account-related inquiries, such as managing account settings, user access, and permissions. They can provide guidance on best practices for organizing accounts within an organization and help with account-related troubleshooting.
While the AWS Enterprise Support Concierge team may provide some level of assistance with application development and architecture guidance, their primary focus is on billing and account-related inquiries. They are not directly responsible for answering questions regarding technical support cases. For technical support, users typically engage with the AWS Support team, which provides different levels of support depending on the support plan.

---

Q352. A company wants to run a simulation for 3 years without interruptions. Which Amazon EC2 instance purchasing option will meet these requirements MOST cost-effectively?

- A) Spot Instances
- [x] B) Reserved Instances
- C) Dedicated Hosts
- D) On-Demand Instances

  

---


Q353. A company wants to use Amazon EC2 instances to provide a static website to users all over the world. The company needs to minimize latency for the users.
Which solution meets these requirements?

- A) Use EC2 instances in multiple edge locations.
- B) Use EC2 instances in the same Availability Zone but in different AWS Regions.
- [x] C) Use Amazon CloudFront with the EC2 instances configured as the source.
- D) Use EC2 instances in the same Availability Zone but in different AWS accounts.

 

---


Q354. A company has decided to adopt Amazon EC2 infrastructure and wants to scale various stateless services for short-term usage. Which EC2 pricing model is MOST cost-efficient to meet these requirements?

- [x] A) Spot Instances
- B) On-Demand Instances
- C) Reserved Instances
- D) Dedicated Hosts


---


> [!IMPORTANT]
> Q355. Which of the following are benefits of AWS Trusted Advisor? (Choose two.)

- A) Access to Amazon Simple Queue Service (Amazon SQS)
- [x] B) Cost optimization recommendations
- C) Hourly refresh of the service limit checks
- [x] D) Security checks
- E) AWS Identity and Access Management (IAM) approval management
 
AWS Trusted Advisor is a service that provides real-time guidance to help optimize AWS environments, improve performance, and enhance security. It offers a range of checks and recommendations to assist users in maximizing the value of their AWS resources.

Refresh check results

You can refresh checks to get the latest results for your account. If you have a Developer or Basic Support plan, you can sign in to the Trusted Advisor console to refresh the checks. If you have a Business, Enterprise On-Ramp, or Enterprise Support plan, Trusted Advisor automatically refreshes the checks in your account on a weekly basis.

---


> [!IMPORTANT]
> Q356. A company wants to save costs by archiving data that is no longer frequently accessed by end users. Which Amazon S3 feature will meet this requirement?

- A) S3 Versioning
- [x] B) S3 Lifecycle
- C) S3 Object Lock
- D) S3 Inventory


<img width="951" alt="image" src="https://github.com/user-attachments/assets/4756e792-a4b7-4bde-9437-57eae67a8d38" />
https://docs.aws.amazon.com/AmazonS3/latest/userguide/configure-inventory.html

You can use Amazon S3 Inventory to help manage your storage. For example, you can use it to audit and report on the replication and encryption status of your objects for business, compliance, and regulatory needs. 
     
> S3 Versioning (option A) enables the management of multiple versions of an object in S3, which might be useful for data versioning and recovery but does not specifically address cost optimization for archiving infrequently accessed data.

> S3 Object Lock (option C) provides an extra layer of protection by allowing users to set retention periods and protect objects from being deleted or modified. While it may be useful for data compliance and protection, it does not directly address cost optimization for archiving data.

> S3 Inventory (option D) allows users to generate a report of objects and their metadata in an S3 bucket. It provides visibility into the objects stored in S3 but does not offer specific cost optimization features for archiving infrequently accessed data.
 


---

Q357. A company wants an AWS service to collect and process 10 TB of data locally and transfer the data to AWS. The company has intermittent connectivity. Which AWS service will meet these requirements?

- A) AWS Database Migration Service (AWS DMS)
- B) AWS DataSync
- C) AWS Backup
- [x] D) AWS Snowball Edge

>  AWS Snowball Edge is a physical device that enables secure data transfer between on-premises environments and AWS. It is designed for scenarios where the data transfer is large, the network connectivity is limited or intermittent, or there are security or compliance requirements that necessitate physical data transport.

> Here's how AWS Snowball Edge meets the specified requirements:

> - Data Transfer: AWS Snowball Edge is a ruggedized device equipped with storage capacity (up to 100 TB) and computing capabilities. The company can use Snowball Edge to locally collect and process the 10 TB of data in an offline or intermittent connectivity environment.
> - Physical Data Transport: Once the data processing is complete, the company can transfer the data from the Snowball Edge device to AWS by shipping the device back to AWS. Snowball Edge devices are designed to be physically transported, and they come with built-in encryption and tamper-evident seals to ensure data security during transit.
> - Integration with AWS: Upon receiving the Snowball Edge device at an AWS facility, AWS can import the data into the desired AWS service (e.g., Amazon S3, Amazon Glacier, Amazon EBS) as specified by the company. This allows for seamless integration of the processed data into AWS for further analysis or storage.
 
> AWS DMS (option A) is a service designed for database migration between on-premises databases and AWS. It is not intended for general-purpose data transfer or intermittent connectivity scenarios.

> AWS DataSync (option B) is a service that facilitates fast and secure data transfer between on-premises storage systems and AWS storage services. While it can handle large data transfers, it relies on continuous network connectivity rather than intermittent connectivity.

> AWS Backup (option C) is a service for backing up and restoring data across various AWS services. While it can help with data management and protection, it does not specifically address the requirements of large-scale data transfer with intermittent connectivity.


---
Q358. A company is migrating its on-premises server to an Amazon EC2 instance. The server must stay active at all times for the next 12 months. Which EC2 pricing option is the MOST cost-effective for the company's workload?

- A) On-Demand
- B) Dedicated Hosts
- C) Spot Instances
- [x] D) Reserved Instances


---

> [!IMPORTANT]
> Q359. A company plans to run a compute-intensive workload that uses graphics processing units (GPUs). Which Amazon EC2 instance type should the company use?

- [x] A) Accelerated computing
- B) Compute optimized
- C) Storage optimized
- D) General purpose

https://aws.amazon.com/ec2/instance-types/
 
> Amazon EC2 offers specialized instance types to cater to various workload requirements. When it comes to workloads that require GPUs for compute-intensive tasks, the "Accelerated computing" instance types are the most appropriate choice. These instance types are specifically designed to provide high-performance GPU capabilities.
Here's why the Accelerated computing instance types are suitable:
GPU Capability: The Accelerated computing instance types are equipped with GPUs, allowing for parallel processing and accelerated performance. This makes them ideal for tasks such as machine learning, deep learning, video rendering, scientific simulations, and other GPU-intensive workloads.
Broad GPU Options: The Accelerated computing instance types offer a range of GPU options, including NVIDIA GPUs. The GPU models and performance capabilities may vary across instance types, allowing businesses to choose the specific GPU configuration that best aligns with their workload requirements.
Option B, Compute optimized, is focused on delivering high compute power for general-purpose workloads. While they offer good CPU performance, they do not provide specialized GPU capabilities required for compute-intensive tasks that rely heavily on GPU processing.
Option C, Storage optimized, is designed for workloads that require high storage performance and throughput. They are not specifically tailored for GPU-intensive tasks and would not be the best fit for compute-intensive workloads that heavily rely on GPUs.
Option D, General purpose, offers a balance of compute, memory, and networking resources for a wide range of workloads but does not provide the specialized GPU capabilities required for compute-intensive tasks.
 

---

Q360. Which Amazon S3 storage class is MOST cost-effective for unknown access patterns?

- A) S3 Standard
- B) S3 Standard-Infrequent Access (S3 Standard-IA)
- C) S3 One Zone-Infrequent Access (S3 One Zone-IA)
- [x] D) S3 Intelligent-Tiering

> keywords: unknown access patterns

---

Q361 is the same as Q71.

---



Q362. Which AWS Cloud benefit gives a company the ability to quickly deploy cloud resources to access compute, storage, and database infrastructures in a matter of minutes?

- A) Elasticity
- B) Cost savings
- [x] C) Agility
- D) Reliability
 
 


---

> [!IMPORTANT]
> Q363. A company's application developers need to quickly provision and manage AWS services by using scripts. Which AWS offering should the developers use to meet these requirements?

- [x] A) AWS CLI
- B) AWS CodeBuild
- C) AWS Cloud Adoption Framework (AWS CAF)
- D) AWS Systems Manager Session Manager

 
AWS Command Line Interface (AWS CLI) allows developers to quickly provision and manage AWS services using scripts. It provides a unified tool to manage AWS services through commands in your command-line shell, enabling automation and scripting capabilities.
The other options do not specifically meet the requirement for quickly provisioning and managing AWS services through scripts:
B. AWS CodeBuild: This is a service for building and testing code, not for managing AWS services directly. C. AWS Cloud Adoption Framework (AWS CAF): This is a framework for guiding cloud adoption strategies and practices, not a tool for provisioning services.
D. AWS Systems Manager Session Manager: This is used for managing and accessing Amazon EC2 instances securely, but it does not provide the general provisioning capabilities that AWS CLI offers.


AWS CLI (option A) is a command-line tool that allows developers to interact with AWS services and resources from a command prompt or shell script. It provides a unified interface to access and manage various AWS services, making it well-suited for automating tasks and scripting AWS resource provisioning and management.
Here's how AWS CLI meets the requirements:
Scripting Capabilities: AWS CLI provides a comprehensive set of commands and options that developers can use to interact with AWS services programmatically. By writing scripts using the AWS CLI commands, developers can automate the provisioning and management of AWS resources, making it faster and more efficient.
Cross-Service Support: AWS CLI supports a wide range of AWS services, such as EC2, S3, RDS, Lambda, and many more. This allows developers to work with multiple services using a single command-line tool, simplifying the management of various AWS resources.
Option B, AWS CodeBuild, is a fully managed build service that compiles source code, runs tests, and produces software packages. While it is useful for building and testing applications, it is not specifically designed for provisioning and managing AWS services using scripts.
Option C, AWS Cloud Adoption Framework (AWS CAF), is a framework that provides guidance and best practices for organizations adopting AWS. It focuses on organizational and operational aspects of cloud adoption, rather than providing scripting capabilities for provisioning and managing AWS services.
Option D, AWS Systems Manager Session Manager, is a service that provides secure and auditable instance management for EC2 instances. It enables users to establish secure shell (SSH) sessions or remote desktop protocol (RDP) sessions to EC2 instances without the need for inbound network access. While it offers remote access capabilities, it is not specifically designed for scripting AWS resource provisioning and management.
 

---
Q364. A development team wants to deploy multiple test environments for an application in a fast, repeatable manner. Which AWS service should the team use?

- A) Amazon EC2
- [x] B) AWS CloudFormation
- C) Amazon QuickSight
- D) Amazon Elastic Container Service (Amazon ECS)

keyword: repeatable

---

> [!IMPORTANT]
> Q365. A company wants to quickly implement a continuous integration/continuous delivery (CI/CD) pipeline. Which AWS service will meet this requirement?

- A) AWS Config
- B) Amazon Cognito
- C) AWS DataSync
- [x] D) AWS CodeStar

>AWS CodeStar Connections is a new feature that allows services like AWS CodePipeline to access third-party code source provider. For example, you can now seamlessly connect your Atlassian Bitbucket Cloud source repository to AWS CodePipeline. This allows you to automate  the build, test, and deploy phases of your release process each time a code change occurs.
>AWS renamed AWS CodeStar Connections to AWS CodeConnections. 


To quickly implement a continuous integration/continuous delivery (CI/CD) pipeline, the AWS service that will meet this requirement is:
D. AWS CodeStar
AWS CodeStar (option D) is a fully managed service that simplifies the development, deployment, and operation of applications on AWS. It provides a CI/CD pipeline solution that enables teams to quickly set up, configure, and manage an end-to-end software release process.
Here's how AWS CodeStar meets the requirement:
CI/CD Pipeline: AWS CodeStar includes AWS CodePipeline, a fully managed continuous delivery service. CodePipeline allows teams to define and automate their CI/CD pipeline stages, including source code repositories, build, test, and deployment steps. It integrates with popular development tools and services, providing a seamless end-to-end pipeline for building, testing, and deploying applications.
Quick Setup: AWS CodeStar provides project templates and pre-configured environments for various programming languages and frameworks. These templates include an opinionated set of AWS resources and configurations, allowing teams to quickly set up a CI/CD pipeline with minimal manual configuration.
Integration with AWS Services: AWS CodeStar integrates with other AWS services, such as AWS CodeCommit, AWS CodeBuild, AWS CodeDeploy, and AWS CodePipeline. This integration allows teams to easily connect their source code repositories, build and test processes, and deployment targets within the CI/CD pipeline.
Option A, AWS Config, is a service that provides resource inventory, configuration history, and configuration change notifications. While it can be used for configuration management and compliance, it does not specifically address the requirements of setting up a CI/CD pipeline.
Option B, Amazon Cognito, is an identity management service that allows users to sign in to applications using social identity providers or their own user pools. While it is useful for authentication and user management, it does not provide the necessary features for implementing a CI/CD pipeline.
Option C, AWS DataSync, is a service for transferring data between on-premises storage and AWS storage services. While it is helpful for data migration and synchronization, it is not designed for implementing a CI/CD pipeline.
Therefore, the correct answer is D. AWS CodeStar.


---


Q366. Which AWS Cloud deployment model uses AWS Outposts as part of the application deployment infrastructure?

- A) On-premises
- B) Serverless
- C) Cloud-native
- [x] D) Hybrid




 
AWS Outposts (option D) is a fully managed service that extends AWS infrastructure, services, APIs, and tools to customer on-premises data centers or co-location facilities. It allows organizations to run AWS services locally on Outposts while seamlessly connecting to the rest of their AWS resources in the cloud.
Here's how AWS Outposts fits into the hybrid deployment model:
Hybrid Deployment Model: In a hybrid deployment model, organizations have a combination of on-premises infrastructure and resources in the cloud. This model allows them to leverage the benefits of both environments, such as maintaining sensitive data on-premises while taking advantage of cloud scalability and services.
AWS Outposts: With AWS Outposts, organizations can deploy AWS services, including compute, storage, and database services, on-premises within their own data centers or co-location facilities. This brings the same APIs, tools, and operational processes available in the AWS Cloud to the on-premises environment.
Seamless Integration: AWS Outposts is tightly integrated with the rest of the AWS ecosystem. It can be managed and monitored through the AWS Management Console, AWS CLI, and other familiar AWS tools. Organizations can use familiar AWS services like AWS Identity and Access Management (IAM), AWS CloudFormation, and AWS Elastic Beanstalk to provision, manage, and automate the resources deployed on Outposts.
 
 


---

Q367. Which of the following is a fully managed graph database service on AWS?

- A) Amazon Aurora
- B) Amazon FSx
- C) Amazon DynamoDB
- [x] D) Amazon Neptune

---


Q368. Which AWS service could an administrator use to provide desktop environments for several employees?

- A) AWS Organizations
- B) AWS Fargate
- C) AWS WAF
- [x] D) AWS WorkSpaces
 
AWS WorkSpaces (option D) is a fully managed desktop-as-a-service (DaaS) solution provided by AWS. It allows administrators to provision and manage cloud-based virtual desktops for multiple users, providing a secure and scalable solution for delivering desktop environments to employees.
Here's some information about AWS WorkSpaces:
Desktop Virtualization: AWS WorkSpaces enables administrators to create virtual desktops in the cloud that can be accessed by users from various devices, including laptops, tablets, and thin clients. Each user is provided with a persistent desktop environment that can be customized and personalized.
Fully Managed Service: WorkSpaces is a fully managed service, which means that AWS handles the underlying infrastructure, maintenance, and security patches. Administrators can focus on managing user access, policies, and configurations without worrying about the underlying infrastructure.
Scalability and Flexibility: WorkSpaces allows administrators to easily provision and manage desktop environments for multiple users. The service supports scaling up or down based on the number of users, and it provides different bundle options with varying hardware configurations to meet the requirements of different users.
Option A, AWS Organizations, is a management service that allows administrators to centrally manage and govern multiple AWS accounts. While it can help in organizing and managing resources across accounts, it does not provide desktop environments for employees.
Option B, AWS Fargate, is a container orchestration service. It allows administrators to run containers without managing the underlying infrastructure. While it can be used for certain types of applications, it is not specifically designed for providing desktop environments.
Option C, AWS WAF (Web Application Firewall), is a web application firewall service that helps protect web applications from common web exploits. It is not related to providing desktop environments for employees.
 


---
Q369. Which AWS service or feature gives users the ability to capture information about network traffic in a VPC?

- [x] A) VPC Flow Logs
- B) Amazon Inspector
- C) VPC route tables
- D) AWS CloudTrail

 
> VPC Flow Logs (option A) is a feature in AWS that allows you to capture information about the IP traffic going to and from network interfaces within a Virtual Private Cloud (VPC). It provides visibility into the network traffic patterns and helps in troubleshooting, monitoring, and security analysis.
Here's some information about VPC Flow Logs:
Network Traffic Capture: VPC Flow Logs capture information about the network traffic within a VPC, including details such as source and destination IP addresses, ports, protocol, and the number of bytes and packets transferred. This information is captured at the network interface level, providing granular visibility into the traffic flow.
Configurable Logging: You can configure VPC Flow Logs to capture specific types of traffic based on your requirements. For example, you can enable logging for all traffic or only specific subnets, network interfaces, or IP addresses. You can also choose to log accepted or rejected traffic or both.
Integration with Other AWS Services: VPC Flow Logs can be configured to stream the captured logs to other AWS services such as Amazon CloudWatch Logs, Amazon S3, or Amazon Kinesis Data Firehose. This allows you to analyze and process the logs using various AWS tools and services.
Option B, Amazon Inspector, is a security assessment service that helps in identifying security vulnerabilities and deviations from best practices in your applications and infrastructure. While it provides security analysis, it does not specifically capture network traffic information.
Option C, VPC route tables, are used to control the traffic flow between subnets within a VPC. They define the rules for routing traffic. While route tables are important for network connectivity, they do not capture information about network traffic.
Option D, AWS CloudTrail, is a service that provides governance, compliance, and audit capabilities for your AWS account. It captures API calls and events related to your AWS resources. While CloudTrail provides insights into API activity, it does not capture specific information about network traffic.
 

---

> [!IMPORTANT]
> Q370. Which type of AWS storage is ephemeral and is deleted when an Amazon EC2 instance is stopped or terminated?

- A) Amazon Elastic Block Store (Amazon EBS)
- [x] B) Amazon EC2 instance store
- C) Amazon Elastic File System (Amazon EFS)
- D) Amazon S3


<img width="764" alt="image" src="https://github.com/user-attachments/assets/c77a14d7-e6f5-42a1-95e6-e133cb67f8b3" />

 Not all EC2 instance types support instance stores. Choose types like m5d, c5d, r5d, i3, or i3en (e.g., i3.large or c5d.xlarge) 
 Storage type
The storage type used for the volume.

EBS volumes are block-level storage volumes that persist independently from the lifetime of an EC2 instance, so you can stop and restart your instance at a later time without losing your data. You can also detach an EBS volume from one instance and attach it to another instance. EBS volumes are billed separately from the instance’s usage cost.

Instance store volumes are physically attached to the host computer. These volumes provide temporary block storage that persists only during the lifetime of the instance. If you stop, hibernate, or terminate an instance, data on instance store volumes is lost. The instance type determines the size and number of the instance store volumes available and the type of hardware used for the instance store volumes. Instance store volumes are included as part of the instance's usage cost.

Root Volume: You cannot boot from an instance store (except for deprecated legacy AMIs). The OS must reside on an EBS volume


---

> [!IMPORTANT]
> Q371. A company wants durable storage for static content and infinitely scalable data storage infrastructure at the lowest cost. Which AWS service should the company choose?

- A) Amazon Elastic Block Store (Amazon EBS)
- [x] B) Amazon S3
- C) AWS Storage Gateway
- D) Amazon Elastic File System (Amazon EFS)

|Service	|Durability	|Scalability	|Cost for Static Content|
|--|--|--|--|
|A) Amazon EBS	|❌ Per-volume (99.8%-99.9%)|	❌ Limited to 16 TiB/volume|	❌ ~$0.08/GB-month (gp3) – 3.5× costlier than S3|
|C) AWS Storage Gateway|	✅ Uses S3 backend	|❌ Hybrid only (on-prem bottleneck)	|❌ +$0.035/GB gateway fee|
|D) Amazon EFS	|✅ Multi-AZ (99.9999%)|	✅ Petabyte-scale	|❌ ~$0.08/GB-month (Standard) – 3× costlier than S3|

 Amazon S3
Durability:

99.999999999% (11 nines) durability – Data is automatically replicated across ≥3 AZs, protecting against hardware failures, disasters, and corruption .

Infinite Scalability:

No capacity limits – Stores any volume of data without provisioning .

Handles unlimited requests – Scales automatically to support any request rate (e.g., millions of requests/sec) .

Lowest Cost for Static Content:

Cost-effective tiers:

S3 Standard: $0.023/GB-month (frequent access) .

S3 Intelligent-Tiering: Auto-moves data to cheaper tiers (e.g., $0.0125/GB for infrequent access) .

S3 Glacier: $0.004/GB-month for archival (retrieval in mins/hours) .

Pay only for used storage – No upfront fees or minimum commitments .


Amazon S3 (Simple Storage Service) (option B) is a highly scalable and durable object storage service provided by AWS. It is designed for storing and retrieving large amounts of data, including static content like images, videos, and documents. S3 offers the following features that align with the company's requirements:
Durability: Amazon S3 provides 99.999999999% (11 nines) of durability for objects stored in it. This means that data stored in S3 is highly protected against data loss. It achieves durability through data replication across multiple Availability Zones within a region.
Scalability: S3 is designed to scale seamlessly as data storage needs grow. It can store virtually unlimited amounts of data and handle high request rates. The storage capacity automatically scales with the amount of data being stored, and performance is maintained even with massive amounts of data.
Lowest Cost: Amazon S3 offers cost-effective pricing options, allowing the company to optimize costs based on their storage requirements. S3 provides different storage classes, such as Standard, Intelligent-Tiering, Glacier, and Glacier Deep Archive, each with different pricing structures to meet specific needs. The company can choose the appropriate storage class based on access frequency and cost sensitivity.
Option A, Amazon Elastic Block Store (Amazon EBS), provides block-level storage volumes that are primarily used for attaching to EC2 instances. While EBS provides durability and scalability, it is not specifically designed for storing static content or infinitely scalable data storage.
Option C, AWS Storage Gateway, is a hybrid storage service that connects on-premises environments with cloud storage. It is not designed for infinitely scalable data storage or storing static content directly.
Option D, Amazon Elastic File System (Amazon EFS), provides scalable, fully managed file storage for EC2 instances. While EFS is highly scalable, it may not be the most cost-effective option for storing static content and infinitely scalable data storage, especially when considering the lowest cost requirement.
 


---

> [!IMPORTANT]
> Q372. An ecommerce company wants to use Amazon EC2 Auto Scaling to add and remove EC2 instances based on CPU utilization. Which AWS service or feature can initiate an Amazon EC2 Auto Scaling action to achieve this goal?

- A) Amazon Simple Queue Service (Amazon SQS)
- B) Amazon Simple Notification Service (Amazon SNS)
- C) AWS Systems Manager
- [x] D) Amazon CloudWatch alarm

cloudwatch alarms will be created automatically by the Auto Scaling group once we specify target tracking scaling policy and enable "group metrics collection within CloudWatch"
https://github.com/justinjiajia/certifications/blob/main/aws/cloud_practitioner/labs/lab6.md

To initiate an Amazon EC2 Auto Scaling action based on CPU utilization, the AWS service or feature that can be used is:
D. Amazon CloudWatch alarm
Amazon CloudWatch (option D) is a monitoring and observability service provided by AWS. It can be used to collect and track metrics, create alarms, and trigger actions based on predefined thresholds. In this case, an Amazon CloudWatch alarm can be set up to monitor the CPU utilization of EC2 instances and initiate scaling actions through Amazon EC2 Auto Scaling.
Here's how it works:
CPU Utilization Metric: Amazon CloudWatch provides a CPU utilization metric for EC2 instances, which indicates the percentage of CPU capacity being used. This metric can be collected and monitored by CloudWatch.
CloudWatch Alarms: With CloudWatch, you can create alarms based on specific conditions. In this case, you can set up a CloudWatch alarm to monitor the CPU utilization metric of your EC2 instances. For example, you can configure the alarm to trigger when the CPU utilization exceeds a certain threshold for a specific period of time.
Scaling Actions: When the CloudWatch alarm is triggered, it can initiate scaling actions through Amazon EC2 Auto Scaling. For example, you can configure the alarm to add more EC2 instances when the CPU utilization exceeds the threshold, and remove instances when the CPU utilization drops below the threshold.
Option A, Amazon Simple Queue Service (Amazon SQS), is a fully managed message queuing service. While it can be used for decoupling and asynchronous communication, it is not directly related to initiating EC2 Auto Scaling actions based on CPU utilization.
Option B, Amazon Simple Notification Service (Amazon SNS), is a messaging service that enables the sending and receiving of messages. While SNS can be used for notification purposes, it does not directly initiate EC2 Auto Scaling actions based on CPU utilization.
Option C, AWS Systems Manager, is a management service that helps in managing EC2 instances and other AWS resources. While it provides various capabilities, it does not specifically initiate EC2 Auto Scaling actions based on CPU utilization.
Therefore, the correct answer is D. Amazon CloudWatch alarm.


---
Q373. A company wants to transform its workforce by attracting and developing a digitally fluent high-performance workforce. The company wants to attract a diverse and inclusive workforce with appropriate mix of technical and non-technical skills. Which AWS Cloud Adoption Framework (AWS CAF) perspective will meet these requirements?

- A) Business
- [x] B) People
- C) Platform
- D) Operations

> Cloud fluency
 

---

> [!IMPORTANT]
> Q374. A company wants to move its on-premises databases to managed cloud database services by using a simplified migration process. Which AWS service or tool can help the company meet this requirement?

- A) AWS Storage Gateway
- B) AWS Application Migration Service
- C) AWS DataSync
- [x] D) AWS Database Migration Service (AWS DMS)


To move on-premises databases to managed cloud database services with a simplified migration process, the AWS service or tool that can help the company meet this requirement is:
D. AWS Database Migration Service (AWS DMS)
AWS Database Migration Service (AWS DMS) (option D) is a fully managed service that enables easy and secure migration of databases to AWS. It supports both homogeneous and heterogeneous migrations, allowing the company to move its on-premises databases to managed cloud database services with minimal downtime and disruption.
Here's how AWS DMS can help with the migration process:
Database Compatibility: AWS DMS supports a wide range of database sources, including popular commercial databases like Oracle, Microsoft SQL Server, MySQL, PostgreSQL, and more. This allows the company to migrate its on-premises databases to compatible managed database services in AWS.
Schema Conversion: AWS DMS can perform schema conversion tasks during the migration process. It can automatically convert schema objects, data types, and database code to match the target database format. This helps ensure compatibility between the source and target databases.
Continuous Data Replication: AWS DMS uses ongoing replication to keep the source and target databases in sync during the migration. The initial data load is performed using a database snapshot, and then changes are continuously replicated to the target database. This minimizes the downtime required for the migration process.
Downtime Minimization: With AWS DMS, the company can migrate databases with minimal downtime or even perform a zero-downtime migration. It allows for testing and validating the migration process before cutting over to the new database environment.
Option A, AWS Storage Gateway, is a hybrid cloud storage service that enables on-premises applications to seamlessly use AWS cloud storage. It is not specifically designed for database migration.
Option B, AWS Application Migration Service, is not an AWS service or tool. There is no known AWS service or tool with this exact name as of my knowledge cutoff in September 2021.
Option C, AWS DataSync, is a data transfer service that simplifies and accelerates the movement of data between on-premises storage and AWS storage services. It is not designed for migrating databases.
 

---


Q375. A company needs a fully managed file server that natively supports Microsoft workloads and file systems. The file server must also support the SMB protocol.
Which AWS service should the company use to meet these requirements?

- A) Amazon Elastic File System (Amazon EFS)
- B) Amazon FSx for Lustre
- [x] C) Amazon FSx for Windows File Server
- D) Amazon Elastic Block Store (Amazon EBS)

>  natively supports Microsoft workloads and file systems; support the SMB protocol

 
Amazon FSx for Windows File Server (option C) is a fully managed file storage service that is designed to provide native support for Microsoft Windows workloads and file systems. It offers a fully compatible Windows file system and supports the Server Message Block (SMB) protocol, making it an ideal choice for hosting Windows-based applications and file shares in the AWS environment.
Here's how Amazon FSx for Windows File Server meets the specified requirements:
Native Support for Microsoft Workloads and File Systems: Amazon FSx for Windows File Server provides a fully compatible Windows file system, which means it supports native Windows file system features and semantics. It integrates well with Microsoft Active Directory, making it easy to manage access control and permissions for Windows users and groups. It also supports features like Windows Access Control Lists (ACLs), Distributed File System (DFS), and File Server Resource Manager (FSRM).
Support for the SMB Protocol: Amazon FSx for Windows File Server natively supports the Server Message Block (SMB) protocol, which is the standard protocol used for file sharing in Windows environments. This allows Windows-based clients and applications to access the file server seamlessly using familiar methods and tools.
Option A, Amazon Elastic File System (Amazon EFS), is a fully managed file storage service that provides scalable and shared file storage for Linux-based workloads. While Amazon EFS is highly compatible with Linux file systems and workloads, it does not natively support Windows file systems or the SMB protocol.
Option B, Amazon FSx for Lustre, is a fully managed high-performance file system designed for compute-intensive workloads. It is optimized for high-speed data processing and is not specifically designed to support Microsoft workloads or file systems.
Option D, Amazon Elastic Block Store (Amazon EBS), provides block-level storage volumes that are primarily used for attaching to EC2 instances. It is not a fully managed file server service and does not provide native support for Microsoft workloads or file systems.
 


---


Q376. A company has been storing monthly reports in an Amazon S3 bucket. The company exports the report data into comma-separated values (.csv) files. A developer wants to write a simple query that can read all of these files and generate a summary report. Which AWS service or feature should the developer use to meet these requirements with the LEAST amount of operational overhead?

-  A) Amazon S3 Select
- [x] B) Amazon Athena
- C) Amazon Redshift
- D) Amazon EC2

 
> Amazon Athena (option B) is an interactive query service that allows you to analyze data directly in Amazon S3 using standard SQL queries. It is a serverless service, meaning you don't need to manage any infrastructure or perform any setup. By using Amazon Athena, the developer can easily query the .csv files stored in the Amazon S3 bucket and generate the desired summary report with minimal operational overhead.
 
Querying .csv Files: Amazon Athena supports querying data stored in various formats, including comma-separated values (.csv) files. The developer can define a table schema that corresponds to the structure of the .csv files and then run SQL queries against this table.
Serverless and Fully Managed: With Amazon Athena, there is no infrastructure to manage. You don't need to provision and configure any servers or databases. The service automatically scales and handles query execution, allowing the developer to focus on writing queries and generating the summary report.
Standard SQL Queries: Amazon Athena uses standard SQL syntax, which makes it easy for developers to write queries. The developer can leverage SQL functions, aggregations, and other capabilities to perform calculations and generate the desired summary report.
> Option A, Amazon S3 Select, allows you to retrieve a subset of data from an object in Amazon S3 using simple SQL expressions. While it can be useful for selective retrieval of data, it does not
provide the full capabilities of running complex queries and generating summary reports.
> Option C, Amazon Redshift, is a fully managed data warehousing service that provides powerful analytics capabilities. While it can handle large-scale data analysis and generate complex reports, it requires more operational overhead compared to Amazon Athena. Redshift requires infrastructure provisioning, setup, and ongoing management.
 
 

---

> [!IMPORTANT]
> Q377. A company needs to search for text in documents that are stored in Amazon S3. Which AWS service will meet these requirements?

- [x] A) Amazon Kendra
- B) Amazon Rekognition
- C) Amazon Polly
- D) Amazon Lex

 
Amazon Kendra (option A) is an intelligent search service powered by machine learning that is designed to provide accurate and efficient search capabilities across an organization's data sources. It supports searching for text in various document formats, including PDF, Word, PowerPoint, and more, which can be stored in Amazon S3.
Here's how Amazon Kendra meets the specified requirements:
Document Search: Amazon Kendra is specifically designed for searching text in documents. It uses natural language processing capabilities to understand the content of documents and provide relevant search results. It can index and search through a wide range of document formats, making it suitable for searching text in documents stored in Amazon S3.
Machine Learning-Powered: Amazon Kendra leverages machine learning algorithms to improve search accuracy and relevance over time. It can automatically extract key information from documents, such as entities, relationships, and more, to enhance search results and provide a more comprehensive search experience.
Integration with Amazon S3: Amazon Kendra can be integrated with Amazon S3 to index and search through documents stored in S3 buckets. It can continuously monitor the S3 bucket for new or updated documents and keep the search index up to date.
Option B, Amazon Rekognition, is a service that provides image and video analysis capabilities, such as object and scene detection, facial analysis, and more. It is not specifically designed for searching text in documents.
Option C, Amazon Polly, is a service that converts text into lifelike speech. It is not designed for searching text in documents.
Option D, Amazon Lex, is a service for building conversational interfaces using chatbots and voicebots. It is not designed for searching text in documents.
 

---

Q378. Which AWS services make use of global edge locations? (Choose two.)

- A) AWS Fargate
- [x] B) Amazon CloudFront
- [x] C) AWS Global Accelerator
- D) AWS Wavelength
- E) Amazon VPC


 
Amazon CloudFront (option B) is a content delivery network (CDN) service that delivers static and dynamic web content, including videos, images, and applications, to end-users with low latency and high transfer speeds. It uses a network of global edge locations to cache and serve content from locations closest to end-users, reducing latency and improving performance.
AWS Global Accelerator (option C) is a networking service that improves the availability and performance of applications for global users. It uses a network of global edge locations to intelligently route user traffic to the nearest AWS edge location, reducing the distance and improving application performance. AWS Global Accelerator also provides features like TCP and UDP acceleration and automatic failover to improve application availability.
Option A, AWS Fargate, is a serverless compute engine for containers. It does not make use of global edge locations as it focuses on running containers in a serverless manner without the need for managing the underlying infrastructure.
Option D, AWS Wavelength, is a service that brings AWS compute and storage services to the edge of the 5G network. While it leverages edge locations, it is specifically designed for 5G network deployments and does not fall under the category of global edge locations used by multiple services.
Option E, Amazon VPC (Virtual Private Cloud), is a service that enables users to create isolated virtual networks within the AWS cloud. While VPC has a global presence for network connectivity, it does not directly make use of global edge locations.
 

---


> [!IMPORTANT]
> Q379. A user needs a relational database but does not have the resources to manage the hardware, resiliency, and replication. Which AWS service option meets the user‘s requirements?

- A) Run MySQL on Amazon Elastic Container Service (Amazon ECS).
- B) Run MySQL on Amazon EC2.
- [x] C) Choose Amazon RDS for MySQL.
- D) Choose Amazon ElastiCache for Redis.



 
Amazon RDS (Relational Database Service) (option C) is a fully managed database service that provides a relational database with automated management, high availability, and scalability. It takes care of the administrative tasks such as hardware provisioning, database setup, patching, backups, and replication, allowing the user to focus on their application and data.
Here's how Amazon RDS for MySQL meets the specified requirements:
Relational Database: Amazon RDS for MySQL provides a fully featured and scalable relational database service based on the popular MySQL database engine. It supports standard MySQL features and is compatible with existing MySQL applications and tools.
Fully Managed: With Amazon RDS, AWS handles the underlying infrastructure management tasks such as hardware provisioning, software patching, backups, and automated software updates. This relieves the user from the burden of managing and maintaining the database infrastructure, allowing them to focus on their application development.
High Availability and Resiliency: Amazon RDS for MySQL offers built-in high availability and resiliency features. It automatically replicates data across multiple Availability Zones (AZs) to provide durability and fault tolerance. In case of a failure, it can automatically failover to a standby replica, minimizing downtime and ensuring data availability.
Option A, running MySQL on Amazon Elastic Container Service (Amazon ECS), is a container orchestration service that allows running applications in containers. While it provides containerization capabilities, it does not handle the management of MySQL itself, including hardware provisioning, replication, and resiliency.
Option B, running MySQL on Amazon EC2, provides full control over the MySQL installation on EC2 instances. However, it requires manual management of the underlying infrastructure, including hardware provisioning, replication setup, patching, and backups.
Option D, Amazon ElastiCache for Redis, is an in-memory data store service that is compatible with the Redis data structure. It is not a relational database and does not provide the same features and capabilities as Amazon RDS for MySQL.
 

---



Q380. A company needs to deploy applications in the AWS Cloud as quickly as possible. The company also needs to minimize the complexity that is related to the management of AWS resources. Which AWS service should the company use to meet these requirements?

- A) AWS Config
- [x] B) AWS Elastic Beanstalk
- C) Amazon EC2
- D) Amazon Personalize

https://github.com/justinjiajia/certifications/blob/main/aws/cloud_security/labs/lab7.md
 
AWS Elastic Beanstalk (option B) is a fully managed service that makes it easy to deploy, run, and scale applications in multiple programming languages such as Java, .NET, Python, Node.js, and more. It abstracts away the underlying infrastructure and automates the deployment process, allowing the company to focus on application development rather than resource management.
Here's how AWS Elastic Beanstalk meets the specified requirements:
Quick Application Deployment: Elastic Beanstalk simplifies the deployment process by providing a platform that automatically handles the deployment of applications. It supports a variety of programming languages and frameworks, allowing the company to quickly deploy their applications without the need for manual setup and configuration.
Resource Management: Elastic Beanstalk handles the management of AWS resources for the application, including Amazon EC2 instances, load balancers, auto-scaling, and more. It abstracts away the complexity of resource management, automatically provisioning and managing the necessary resources based on the application's requirements.
Fully Managed Service: Elastic Beanstalk is a fully managed service, meaning AWS handles the underlying infrastructure, including patching, updates, and maintenance. This reduces the operational complexity for the company, allowing them to focus on application development and deployment.
Option A, AWS Config, is a service that provides resource inventory, configuration history, and configuration change notifications for AWS resources. While it can help with resource management, it does not provide the same level of automation and ease of deployment as Elastic Beanstalk.
Option C, Amazon EC2, is a foundational AWS service that provides virtual servers in the cloud. While it offers flexibility and control over the infrastructure, it requires manual management and configuration of EC2 instances, load balancers, and other resources.
Option D, Amazon Personalize, is a service for creating personalized recommendations for users. It is not specifically designed for deploying applications and does not address the requirement of minimizing resource management complexity.
 


---


Q381. Which mechanism allows developers to access AWS services from application code?

- [x] A) AWS Software Development Kit
- B) AWS Management Console
- C) AWS CodePipeline
- D) AWS Config

 
AWS Software Development Kit (SDK) (option A) is a collection of software tools and libraries that enables developers to interact with AWS services programmatically. The SDK provides APIs (Application Programming Interfaces) and pre-built functions for various programming languages, including Java, Python, .NET, Ruby, and more, allowing developers to easily integrate AWS services into their application code.
Here's how the AWS SDK meets the specified requirement:
Access AWS Services: The AWS SDK provides a set of APIs and libraries that expose the functionality of various AWS services, such as Amazon S3, Amazon EC2, AWS Lambda, Amazon DynamoDB, and many more. Developers can use these APIs to interact with AWS services and perform operations like creating, reading, updating, and deleting resources.
Programming Language Support: The AWS SDK supports multiple programming languages, making it accessible to developers working with different languages. Each SDK provides language-specific APIs and libraries, allowing developers to write code in their preferred programming language.
Option B, AWS Management Console, is a web-based graphical user interface (GUI) provided by AWS for managing and configuring AWS resources. It is not specifically designed for accessing AWS services from application code.
Option C, AWS CodePipeline, is a fully managed continuous integration and continuous delivery (CI/CD) service. While it helps with automating software release pipelines, it is not focused on accessing AWS services from application code.
Option D, AWS Config, is a service that provides resource inventory, configuration history, and configuration change notifications for AWS resources. It is not directly used for accessing AWS services from application code.

---

Q382. A company wants to establish a private network connection between AWS and its corporate network. Which AWS service or feature will meet this requirement?

- A) Amazon Connect
- B) Amazon Route 53
- [x] C) AWS Direct Connect
- D) VPC peering


 
AWS Direct Connect (option C) is a network service that provides a dedicated private connection between an organization's on-premises network and AWS. It allows for a secure and reliable connection that bypasses the public internet, providing a more consistent network experience and better bandwidth capacity for data transfer between the corporate network and AWS resources.
Here's how AWS Direct Connect meets the specified requirement:
Private Network Connection: AWS Direct Connect establishes a private, dedicated network connection between the corporate network and AWS. This connection is separate from the public internet, ensuring a secure and reliable network link.
High Bandwidth and Reliable Data Transfer: With AWS Direct Connect, organizations can provision dedicated network links with high bandwidth capacity, ranging from 1 Gbps to 100 Gbps. This enables faster and more efficient data transfer between the corporate network and AWS services.
Reduced Network Costs: By using AWS Direct Connect, organizations can reduce their data transfer costs by bypassing the need to transfer data over the public internet. This is particularly beneficial for organizations with large data volumes or strict security and compliance requirements.
Option A, Amazon Connect, is a cloud-based contact center service for handling customer interactions. It is not related to establishing a private network connection between AWS and a corporate network.
Option B, Amazon Route 53, is a scalable and highly available domain name system (DNS) web service. While it provides DNS routing capabilities, it is not specifically designed for establishing private network connections.
Option D, VPC peering, is a feature that allows connecting two Virtual Private Clouds (VPCs) within AWS. It is used to establish private connectivity between VPCs, but it does not provide connectivity between an AWS VPC and a corporate network.
 

---

> [!IMPORTANT]
> Q383. Which AWS services or features give users the ability to create a network connection between two VPCs? (Choose two.)

- A) VPC endpoints
- B) Amazon Route 53
- [x] C) VPC peering
- D) AWS Direct Connect
- [x] E) AWS Transit Gateway

VPC peering (option C) allows users to create a private network connection between two VPCs within the same AWS Region. It enables resources in one VPC to communicate with resources in another VPC using private IP addresses, without the need for internet gateways, NAT gateways, or VPN connections.
AWS Transit Gateway (option E) is a fully managed service that simplifies network connectivity and routing between multiple VPCs and on-premises networks. It acts as a hub for connecting multiple VPCs and provides centralized control over network routing, helping to simplify network architecture and reduce complexity.
Option A, VPC endpoints, is a feature that allows secure and private communication between a VPC and AWS services without the need for internet gateways or NAT gateways. It does not establish connectivity between two VPCs.
Option B, Amazon Route 53, is a scalable and highly available domain name system (DNS) web service. While it provides DNS routing capabilities, it is not specifically designed for creating network connections between VPCs.
Option D, AWS Direct Connect, is a network service that establishes a private network connection between an on-premises network and AWS. While it provides connectivity to the corporate network, it is not used for creating connections between VPCs.
 

---


Q384. Which AWS service converts text to lifelike voices?

- A) Amazon Transcribe
- B) Amazon Rekognition
- [x] C) Amazon Polly
- D) Amazon Textract


---


Q385 is the same as Q323.
 
  

---

> [!IMPORTANT]
> Q386. Which AWS service or tool can provide rightsizing recommendations for Amazon EC2 resources at no additional cost?

- A) AWS Well-Architected Tool
- B) Amazon CloudWatch
- [x] C) AWS Cost Explorer
- D) Amazon S3 analytics


Implementation Workflow:

Enable Cost Explorer in the AWS Billing Console.

Navigate to Rightsizing Recommendations to view actionable insights (now this is in legacy page section)

Filter by tags, regions, or instance families for targeted savings

<img width="1083" alt="image" src="https://github.com/user-attachments/assets/ce6d4706-dd8f-4a27-ab89-5935bc1493e0" />


AWS Cost Explorer (option C) is a cost management tool that provides cost visualization, analysis, and forecasting capabilities for AWS resources, including Amazon EC2. It offers a set of features that can help identify cost-saving opportunities, including rightsizing recommendations for EC2 instances.
Here's how AWS Cost Explorer meets the specified requirement:
Rightsizing Recommendations: AWS Cost Explorer analyzes the historical usage and performance metrics of EC2 instances and provides rightsizing recommendations. It identifies instances that are overprovisioned or underutilized and suggests appropriate instance types or sizes to optimize resource utilization and cost.
No Additional Cost: The use of AWS Cost Explorer itself does not incur any additional cost. It is available to AWS customers at no charge and can be accessed through the AWS Management Console.
Option A, AWS Well-Architected Tool, is a service that helps architects and developers review and improve the architecture of their workloads based on AWS best practices. While it provides valuable insights and recommendations, it does not specifically focus on rightsizing recommendations for EC2 resources.
Option B, Amazon CloudWatch, is a monitoring and observability service that provides metrics, logs, and events for AWS resources, including EC2 instances. While CloudWatch can provide insights into EC2 resource utilization, it does not provide specific rightsizing recommendations.
Option D, Amazon S3 analytics, is a feature of Amazon S3 that provides analytics and insights into S3 bucket usage and access patterns. It is not related to providing rightsizing recommendations for EC2 resources.

---

Q387. A company operates a petabyte-scale data warehouse to analyze its data. The company wants a solution that will not require manual hardware and software management. Which AWS service will meet these requirements?

- A) Amazon DocumentDB (with MongoDB compatibility)
- [x] B) Amazon Redshift
- C) Amazon Neptune
- D) Amazon ElastiCache


 > keywords; petabytes of data; data warehouse
>
Amazon Redshift (option B) is a fully managed data warehousing service that is designed for online analytical processing (OLAP) workloads. It provides a scalable and cost-effective solution for analyzing large amounts of data without the need for manual hardware and software management.
Here's how Amazon Redshift meets the specified requirements:
Fully Managed: Amazon Redshift is a fully managed service, meaning that AWS handles the underlying infrastructure, hardware provisioning, software setup, patching, and backups. This eliminates the need for manual management of hardware and software components.
Petabyte-Scale Data Warehouse: Amazon Redshift is designed to handle petabyte-scale data warehouses. It provides high-performance query processing, columnar storage, and parallel query execution to handle large volumes of data efficiently.
Option A, Amazon DocumentDB (with MongoDB compatibility), is a fully managed, highly scalable, and highly available document database service. While it is a suitable choice for managing and querying large amounts of document data, it is not specifically designed for data warehousing and OLAP workloads.
Option C, Amazon Neptune, is a fully managed graph database service. It is optimized for storing and querying highly connected data, such as social networking data or recommendation engines. It is not designed for data warehousing and OLAP workloads.
Option D, Amazon ElastiCache, is a fully managed in-memory data caching service. It is used to improve the performance and scalability of applications by caching frequently accessed data in-memory. It is not designed for data warehousing and analytical processing.
 

---
Q388. Which task is a responsibility of AWS, according to the AWS shared responsibility model?

- A) Encryption of application data
- B) Authentication of application users
- [x] C) Protection of physical network infrastructure
- D) Configuration of firewalls


---

Q389. Which options are AWS Cloud Adoption Framework (AWS CAF) cloud transformation journey recommendations? (Choose two.)

- [x] A) Envision phase
- [x] B) Align phase
- C) Assess phase
- D) Mobilize phase
- E) Migrate and modernize phase

> envision, align, launch, scale
 

---

Q390. A company wants to generate a list of IAM users. The company also wants to view the status of various credentials that are associated with the users, such as password, access keys, and multi-factor authentication (MFA) devices. Which AWS service or feature will meet these requirements?

- [x] A) IAM credential report
- B) AWS IAM Identity Center (AWS Single Sign-On)
- C) AWS Identity and Access Management Access Analyzer
- D) AWS Cost and Usage Report
 
The IAM credential report (option A) is a feature provided by AWS Identity and Access Management (IAM) that allows you to generate a comprehensive report of IAM users in your AWS account. The report includes various details about the users, including their user names, ARNs (Amazon Resource Names), creation dates, password reset status, access key status, MFA device status, and more.
Here's how the IAM credential report meets the specified requirements:
List of IAM users: The IAM credential report provides a list of all IAM users in your AWS account. You can generate the report in CSV format and review the user details.
Status of various credentials: The report includes the status of various credentials associated with the IAM users, such as their password reset status, access key status (active or inactive), and MFA device status (enabled or disabled).
Option B, AWS IAM Identity Center (AWS Single Sign-On), is not the correct choice for this requirement. AWS Single Sign-On (SSO) is a service that simplifies user management and single sign-on across multiple AWS accounts and business applications but does not provide the specific functionality of generating a list of IAM users and viewing their credential status.
Option C, AWS Identity and Access Management Access Analyzer, is a service that helps identify unintended access to resources by analyzing policies. It does not provide the functionality of generating a comprehensive report of IAM users and their credential status.
Option D, AWS Cost and Usage Report, is not relevant to this requirement. The AWS Cost and Usage Report provides detailed cost and usage information for AWS resources, but it does not provide information about IAM users or their credentials.
 

---

> [!IMPORTANT]
> Q391. A company wants to track tags, buckets, and prefixes for its Amazon S3 objects. Which S3 feature will meet this requirement?

- [x] A) S3 Inventory report
- B) S3 Lifecycle
- C) S3 Versioning
- D) S3 ACLs

 
 <img width="987" alt="image" src="https://github.com/user-attachments/assets/239183c0-7135-458c-9a83-d43820f062ab" />

The S3 Inventory report (option A) is a feature provided by Amazon S3 that allows you to track and analyze metadata about your objects stored in S3. This feature generates a daily or weekly report, stored in an S3 bucket, that provides a comprehensive list of objects and their associated metadata, including tags, bucket names, and object prefixes.
Here's how the S3 Inventory report meets the specified requirements:
Track tags: The S3 Inventory report includes information about the tags associated with each object. Tags are key-value pairs that you can assign to your S3 objects to categorize and manage them based on specific attributes.
Track buckets: The S3 Inventory report provides details about the bucket names associated with the objects. This allows you to easily track which objects belong to which buckets.
Track prefixes: The S3 Inventory report provides information about the object prefixes. An object prefix is the key name prefix that you specify when storing objects in S3, allowing you to organize and group objects based on a common prefix.
Option B, S3 Lifecycle, is not the correct choice for this requirement. S3 Lifecycle is a feature that allows you to define rules to automatically transition objects between different storage classes or delete them after a specified period. It does not provide the specific functionality of tracking tags, buckets, and prefixes.
Option C, S3 Versioning, is not relevant to this requirement. S3 Versioning is a feature that allows you to keep multiple versions of an object in S3. It does not provide the functionality of tracking tags, buckets, and prefixes.
Option D, S3 ACLs (Access Control Lists), is a mechanism for managing permissions on S3 objects. While ACLs allow you to control access to S3 objects, they do not provide the specific functionality of tracking tags, buckets, and prefixes.
 

---


Q391 is the same as Q331.
 


---

Q393. A company wants to use the AWS Cloud to deploy an application globally. Which architecture deployment model should the company use to meet this requirement?

- [x] A) Multi-Region
- B) Single-Region
- C) Multi-AZ
- D) Single-AZ

---

> [!IMPORTANT]
> Q394. A company wants a web application to interact with various AWS services. Which AWS service or resource will meet this requirement?

- A) AWS CloudShell
- B) AWS Marketplace
- C) AWS Management Console
- [x] D) AWS CLI

<img width="672" alt="image" src="https://github.com/user-attachments/assets/305254fc-80e2-4b34-b536-e222e45c5005" />

---

Q395. Which options are AWS Cloud Adoption Framework (AWS CAF) governance perspective capabilities? (Choose two.)

- A) Identity and access management (security)
- [x] B) Cloud financial management (governance)
- [x] C) Application portfolio management (governance)
- D) Innovation management (business)
- E) Product management (business)

---

Q396. Which architecture concept describes the ability to deploy resources on demand and release resources when they are no longer needed?

- A) High availability
- B) Decoupled architecture
- C) Resilience
- [x] D) Elasticity

---

> [!IMPORTANT]
> Q397. Which task requires a user to sign in as the AWS account root user?

- A) The deletion of IAM users
- [x] B) The deletion of an AWS account
- C) The creation of an organization in AWS Organizations
- D) The deletion of Amazon EC2 instances
 
The AWS account root user has full administrative access to the AWS account and is the highest level of privilege within the account. Certain actions, such as deleting the entire AWS account, can only be performed by the root user.
Here's why the other options do not require signing in as the root user:
A. The deletion of IAM users: IAM (Identity and Access Management) users can be managed by users with the necessary IAM permissions. The root user can create and delete IAM users, but it is not required to sign in as the root user specifically for deleting IAM users.
C. The creation of an organization in AWS Organizations: The creation of an organization in AWS Organizations does not require signing in as the root user. It can be done by any IAM user with the necessary permissions to create and manage organizations.
D. The deletion of Amazon EC2 instances: The deletion of Amazon EC2 instances can be performed by users with the appropriate EC2 permissions. The root user has full administrative access to EC2 and can delete instances, but it is not required to sign in as the root user specifically for this task.
 


---

Q398. A company needs Amazon EC2 instances for a workload that can tolerate interruptions. Which EC2 instance purchasing option meets this requirement with the LARGEST discount compared to On-Demand prices?

- [x] A) Spot Instances
- B) Convertible Reserved Instances
- C) Standard Reserved Instances
- D) Dedicated Hosts

---

Q399. Which guideline is a well-architected design principle for building cloud applications?

- A) Keep static data closer to compute resources.
- B) Provision resources for peak capacity.
- [x] C) Design for automated recovery from failure.
- D) Use tightly coupled components.

 
Designing for automated recovery from failure is a key guideline in building cloud applications that are resilient and highly available. It involves implementing mechanisms and strategies to automatically detect failures and recover from them without manual intervention.
Here's why the other options are not well-architected design principles:
A. Keeping static data closer to compute resources: While minimizing network latency and optimizing data access is important, the specific guideline of keeping static data closer to compute resources does not directly address the overall architecture and resilience of cloud applications.
B. Provisioning resources for peak capacity: Provisioning resources for peak capacity can be costly and inefficient. A well-architected design principle is to design applications to scale and dynamically provision resources based on demand, rather than overprovisioning for peak capacity.
D. Using tightly coupled components: Tightly coupled components can increase dependencies and reduce flexibility, making it challenging to scale and evolve applications. A well-architected design principle is to design applications with loose coupling, using decoupling mechanisms such as message queues and event-driven architectures.
 

---

Q400. A company needs to move 75 petabytes of data from its on-premises data centers to AWS. Which AWS service should the company use to meet these requirements MOST cost-effectively?

- A) AWS Snowball Edge Storage Optimized
- [x] B) AWS Snowmobile
- C) AWS Direct Connect
- D) AWS Storage Gateway


---


Q401. Which of the following are pillars of the AWS Well-Architected Framework? (Choose two.)

- A) Resource scalability
- [x] B) Performance efficiency
- C) System elasticity
- D) Agile development
- [x] E) Operational excellence

---

> [!IMPORTANT]
> Q402. Which design principles should a company apply to AWS Cloud workloads to maximize sustainability and minimize environmental impact? (Choose two.)

- [x] A) Maximize utilization of Amazon EC2 instances. (maximize utilization)
- B) Minimize utilization of Amazon EC2 instances.
- C) Minimize usage of managed services.
- D) Force frequent application reinstallations by users.
- [x] E) Reduce the need for users to reinstall applications. (reduce the downstream impact of your cloud workloads)

see  Design principles for sustainability in the cloud https://docs.aws.amazon.com/pdfs/wellarchitected/latest/sustainability-pillar/wellarchitected-sustainability-pillar.pdf

---

> [!IMPORTANT]
> Q403. In which ways does the AWS Cloud offer lower total cost of ownership (TCO) of computing resources than on-premises data centers? (Choose two.)

- [x] A) AWS replaces upfront capital expenditures with pay-as-you-go costs.
- B) AWS is designed for high availability, which eliminates user downtime.
- C) AWS eliminates the need for on-premises IT staff.  
- [x] D) AWS uses economies of scale to continually reduce prices.
- E) AWS offers a single pricing model for Amazon EC2 instances.


> C. AWS eliminates the need for on-premises IT staff: While AWS Cloud can reduce the need for managing physical infrastructure, it does not eliminate the need for IT staff entirely. Organizations still require IT staff to manage and optimize their cloud resources, design and deploy applications, and ensure secure and efficient operations.

---

Q404. Which AWS service provides on-premises applications with low-latency access to data that is stored in the AWS Cloud?

- A) Amazon CloudFront
- [x] B) AWS Storage Gateway
- C) AWS Backup
- D) AWS DataSync


 
> AWS Storage Gateway is a hybrid cloud storage service that enables on-premises applications to seamlessly use AWS storage. It provides a range of capabilities, including file, volume, and tape gateway options. The file gateway, in particular, allows on-premises applications to access data stored in Amazon S3 with low-latency performance. It achieves this by caching frequently accessed data on-premises and providing transparent access to the full data set in S3.

> A. Amazon CloudFront: Amazon CloudFront is a content delivery network (CDN) service that accelerates the delivery of content, including static and dynamic web content, to end-users. While CloudFront improves the performance of content delivery, it is not specifically designed for on-premises applications to access data stored in the AWS Cloud.

> C. AWS Backup: AWS Backup is a fully managed backup service that helps automate and centralize the backup of data across AWS services. It is not designed for on-premises applications to access data stored in the AWS Cloud.

> D. AWS DataSync: AWS DataSync is a data transfer service that simplifies and accelerates moving large amounts of data between on-premises storage systems and AWS services. While it facilitates data transfer, it is not specifically designed for on-premises applications to access data in the AWS Cloud with low-latency performance.
Therefore, the correct answer is B. AWS Storage Gateway, as it provides on-premises applications with low-latency access to data stored in the AWS Cloud.


---

Q405. Which architecture design principle describes the need to isolate failures between dependent components in the AWS Cloud?

- A) Use a monolithic design.
- B) Design for automation.
- C) Design for single points of failure.
- [x] D) Loosely couple components.


--- 

Q406. Which benefit of cloud computing gives a company the ability to deploy applications to users all over the world through a network of AWS Regions, Availability Zones, and edge locations?

- A) Economy of scale
- [x] B) Global reach
- C) Agility
- D) High availability

---

> [!IMPORTANT]
> Q407. Which AWS service makes it easier to monitor and troubleshoot application logs and cloud resources?

- A) Amazon EC2
- B) AWS Identity and Access Management (IAM)
- [x] C) Amazon CloudWatch
- D) AWS CloudTrail
 
> Amazon CloudWatch is a monitoring and observability service provided by AWS. It is specifically designed to monitor AWS resources and applications running on AWS. CloudWatch allows you to collect and track metrics, collect and monitor log files, set alarms, and automatically react to changes in your AWS resources.

> With Amazon CloudWatch, you can monitor the performance and health of your applications and infrastructure in real-time. It provides a centralized location to view and analyze logs, metrics, and events generated by your applications and AWS services. CloudWatch also supports the creation of custom dashboards, enabling you to visualize and analyze the collected data.

> While Amazon EC2 (A) is a virtual server offered by AWS and AWS Identity and Access Management (IAM) (B) is a service that helps you manage access to AWS resources, they are not specifically designed for monitoring and troubleshooting application logs and cloud resources.

> AWS CloudTrail (D) is a service that provides governance, compliance, and audit capabilities by logging and tracking API activity in your AWS account. While CloudTrail is useful for auditing and tracking changes to your resources, it is not primarily focused on monitoring and troubleshooting application logs and cloud resources like Amazon CloudWatch.
 


---
Q408. Which AWS service uses AWS Compute Optimizer to provide sizing recommendations based on workload metrics?

- [x] A) Amazon EC2
- B) Amazon RDS
- C) Amazon Lightsail
- D) AWS Step Functions

---

Q409. A company is in the early stages of planning a migration to AWS. The company wants to obtain the monthly predicted total AWS cost of ownership for future Amazon EC2 instances and associated storage. Which AWS service or tool should the company use to meet these requirements?

- [x] A) AWS Pricing Calculator
B) AWS Compute Optimizer
C) AWS Trusted Advisor
D) AWS Application Migration Service

 
> The AWS Pricing Calculator is a service provided by AWS that allows you to estimate and predict the costs of using various AWS services. It provides a web-based interface where you can select the desired AWS services, specify the configuration details (such as instance types, storage options, and data transfer), and input usage patterns to estimate the monthly costs.

> To obtain the monthly predicted total AWS cost of ownership for future Amazon EC2 instances and associated storage, the company can use the AWS Pricing Calculator. They can select the desired EC2 instance types, specify the storage options, and input the anticipated usage patterns to get an estimate of the monthly costs.

 
> B. AWS Compute Optimizer: AWS Compute Optimizer is a service that analyzes the performance metrics of EC2 instances and provides recommendations for optimizing their configuration. It does not provide cost estimates or predictions.

> C. AWS Trusted Advisor: AWS Trusted Advisor is a service that provides recommendations to help optimize your AWS infrastructure in areas such as cost optimization, security, performance, and fault tolerance. While it includes some cost optimization recommendations, it does not specifically provide cost estimates or predictions for EC2 instances and storage.

> D. AWS Application Migration Service: AWS Application Migration Service, also known as AWS Server Migration Service, is a service that helps migrate on-premises applications to AWS infrastructure. It is not designed for cost estimation or predicting the monthly cost of using EC2 instances and associated storage.
Therefore, the correct answer is A. AWS Pricing Calculator as the AWS service or tool that the company should use to obtain the monthly predicted total AWS cost of ownership for future Amazon EC2 instances and associated storage.


---

Q410. Which AWS resource can help a company reduce its costs in exchange for a usage commitment when using Amazon EC2 instances?

- [x] A) Compute Savings Plans
- B) Auto Scaling group
- C) On-Demand Instance
- D) EC2 instance store

---

Q411. Which perspective in the AWS Cloud Adoption Framework (AWS CAF) includes a capability for well-designed data and analytics architecture?

- A) Security
- B) Governance
- C) Operations
- [x] D) Platform

> This is the data architecture capability that belongs to the platform perspective

---

Q412. Which options are AWS Cloud Adoption Framework (AWS CAF) people perspective capabilities? (Choose two.)
- [x] A) Organizational alignment (people)
- B) Portfolio management (business)
- [x] C) Organization design (people)
- D) Risk management (governance)
- E) Modern application development (platform)

> options with the word "organization-" belongs to the people perspective

---

> [!IMPORTANT]
> Q413. Which AWS service or resource can identify and provide reports on IAM resources in one AWS account that is shared with another AWS account?
- A) IAM credential report
- B) AWS IAM Identity Center (AWS Single Sign-On)
- [x] C) AWS Identity and Access Management Access Analyzer
- D) Amazon Cognito user pool
 
> AWS Identity and Access Management (IAM) Access Analyzer is a service that helps identify unintended access to resources within an AWS account. It can also analyze resource policies for resources shared between AWS accounts.

> By using IAM Access Analyzer, you can detect any potential issues with access control and identify any risks associated with the sharing of IAM resources across accounts. It can generate detailed reports that highlight any findings or recommendations related to the resource policies.

> The IAM credential report (option A) is a different feature that provides information on the status and configuration of IAM users, groups, and roles within a single AWS account. It does not specifically focus on the sharing of IAM resources across multiple accounts.

> AWS IAM Identity Center (AWS Single Sign-On) (option B) is a service that simplifies identity and access management for multiple AWS accounts. However, it does not specifically provide reports on IAM resources in one account that is shared with another account.

> Amazon Cognito user pool (option D) is a managed service that provides user sign-up, sign-in, and access control for web and mobile applications. It is not specifically designed to identify and report on IAM resources shared between AWS accounts.
 


---
Q414. Which AWS Well-Architected Framework pillar focuses on structured and streamlined allocation of computing resources?
- A) Reliability
- B) Operational excellence
- [x] C) Performance efficiency
- D) Sustainability

> Performance efficiency: The performance efficiency pillar focuses on structured and streamlined allocation of IT and computing resources. Key topics include selecting resource types and sizes optimized for workload requirements, monitoring performance, and maintaining efficiency as business needs evolve. Performance efficiency design principles include:

> - Democratize advanced technologies
> - Go global in minutes
> - Use serverless architectures
> - Experiment more often
> - Consider mechanical sympathy

---

Q415. Which AWS Cloud Adoption Framework (AWS CAF) capabilities belong to the governance perspective? (Choose two.)
- [x] A) Program and project management (governance)
- B) Product management (business)
- C) Portfolio management (business)
- [x] D) Risk management (governance)
- E) Event management (operations)

---

> [!IMPORTANT]
> Q416. A company wants to use AWS Managed Services (AMS) for operational support and wants to understand the scope of AMS. Which AMS feature will meet these requirements?

- [x] A) Landing zone and network management
- B) Customer application development
- C) DevSecOps pipeline configuration
- D) Application log monitoring

 https://www.youtube.com/watch?v=wtoI49B-wwU
https://www.youtube.com/watch?v=gfRDtRfjok4

AWS Control Tower setup: Set up your well-architected automated landing zone.
 
> AWS Managed Services (AMS) provides operational support for AWS infrastructure and services. It is designed to help simplify the management of AWS resources, allowing organizations to offload operational tasks and focus on their core business activities.

> The "Landing zone and network management" feature of AMS involves setting up and managing a secure and well-architected AWS landing zone. This includes creating a foundational AWS environment with network connectivity, identity and access management (IAM), security controls, and operational tooling. The landing zone provides a standardized and secure foundation for running workloads in the AWS cloud.

> By utilizing AMS for landing zone and network management, the company can benefit from AWS experts who will handle operational tasks such as infrastructure provisioning, monitoring, patching, and backups. AMS provides 24/7 support, incident management, and proactive monitoring to ensure the availability and performance of the AWS resources.

> The other options mentioned are not specific to the scope of AWS Managed Services (AMS):

> B. Customer application development: AMS does not directly provide application development services. It focuses on managing and supporting existing AWS infrastructure and services.

> C. DevSecOps pipeline configuration: While AMS may include certain aspects of DevSecOps practices, it is not a primary feature or capability. DevSecOps pipeline configuration typically involves setting up and managing CI/CD pipelines and security integration, which are outside the scope of AMS.

> D. Application log monitoring: AMS primarily focuses on managing infrastructure and services rather than specific application-level monitoring and logging. Application log monitoring is typically handled by application-specific logging and monitoring tools. 


---

Q417. A company wants to migrate its on-premises NoSQL workload to Amazon DynamoDB. Which AWS service will meet this requirement?

- A) AWS Migration Hub
- [x] B) AWS Database Migration Service (AWS DMS)
- C) Migration Evaluator
- D) AWS Application Migration Service



---

Q418. A company is in the process of finding correct Amazon EC2 instance types and sizes to meet its performance and capacity requirements. The company wants to find the lowest possible cost. Which option accurately characterizes the company's actions?

- A) Auto Scaling
- B) Storage tiering
- [x] C) Rightsizing
- D) Instance scheduling


---

Q419. A company wants to manage sign-in security for workforce users. The company needs to create workforce users and centrally manage their access across all the company's AWS accounts and applications. Which AWS service will meet these requirements?
- A) AWS Audit Manager
- B) Amazon Cognito
- C) AWS Security Hub
- [x] D) AWS IAM Identity Center (AWS Single Sign-On)


---


Q420. A company wants a report that lists the status of multi-factor authentication (MFA) devices that all users in the company's AWS account use.  Which AWS feature or service will meet this requirement?
- A. AWS Cost and Usage Reports
- [x] B. IAM credential reports
- C. Detailed Billing Reports
- D. AWS Cost Explorer reports
 
---


> [!IMPORTANT]
> Q421. A company is launching a mobile app in the AWS Cloud. The company wants the app's users to sign in through social media identity providers (IdPs). Which AWS service will meet this requirement?

- A) AWS Lambda
- [x] B) Amazon Cognito
- C) AWS Secrets Manager
- D) Amazon CloudFront

> keywords: mobile app; social media IdPs

---

Q422. Which cloud concept is demonstrated by using AWS Cost Explorer?

- [x] A) Rightsizing
- B) Reliability
- C) Resilience
- D) Modernization

---

Q423. A company wants to deploy a non-containerized Java-based web application on AWS. The company wants to use a managed service to quickly deploy the application. The company wants the service to automatically provision capacity, load balance, scale, and monitor application health. Which AWS service will meet these requirements?

- A) Amazon Elastic Container Service (Amazon ECS)
- B) AWS Lambda
- C) Amazon Elastic Kubernetes Service (Amazon EKS)
- [x] D) AWS Elastic Beanstalk

---

Q424. A company has deployed a web application to Amazon EC2 instances. The EC2 instances have low usage. Which AWS service or feature should the company use to rightsize the EC2 instances?

- A) AWS Config
- B) AWS Cost Anomaly Detection
- C) AWS Budgets
- [x] D) AWS Compute Optimizer

---

Q425. A company needs to categorize and track AWS usage cost based on business categories. Which AWS service or feature should the company use to meet these requirements?

- [x] A) Cost allocation tags
- B) AWS Organizations
- C) AWS Security Hub
- D) AWS Cost and Usage Report
 
Cost allocation tags are metadata labels that can be applied to AWS resources to categorize and track their costs. These tags enable the company to allocate costs to specific business categories, projects, departments, or any other organizational dimension that they want to track. By assigning relevant tags to AWS resources, the company can gain granular visibility into the cost breakdown and analyze spending patterns based on different business dimensions.
Key features of cost allocation tags include:
Flexibility: Cost allocation tags allow the company to define custom tags that align with their specific business needs. They can create tags such as "Department," "Project," "Environment," or any other relevant category.
Resource-level tagging: Cost allocation tags can be applied to various AWS resources, including EC2 instances, S3 buckets, RDS databases, and more. This allows the company to track costs across different types of resources.
Cost allocation reporting: AWS provides tools such as the Cost Explorer and AWS Cost and Usage Reports that leverage cost allocation tags to generate detailed cost reports. These reports can be filtered and aggregated based on the assigned tags, enabling the company to analyze spending across different business categories.
By using cost allocation tags, the company can gain better visibility into their AWS usage costs and allocate them accurately based on their desired business categories. This helps with cost management, budgeting, and resource optimization efforts.
While the other options (B, C, and D) are AWS services or features, they are not specifically designed for categorizing and tracking AWS usage costs based on business categories:
- AWS Organizations (Option B) is a service that helps centrally manage and govern multiple AWS accounts. While it provides organizational structure and billing consolidation capabilities, it does not directly address cost categorization based on business categories.
- AWS Security Hub (Option C) is a service that provides a comprehensive view of security findings and compliance status across AWS accounts. It focuses on security monitoring and threat detection, rather than cost categorization.
- AWS Cost and Usage Report (Option D) provides detailed cost and usage data in a downloadable CSV format. While it includes cost breakdowns at the resource level, it does not provide the specific categorization and tracking capabilities offered by cost allocation tags. 

- 
---

> [!IMPORTANT]
> Q426. Which AWS service can migrate data between AWS storage services?

- [x] A) AWS DataSync
- B) AWS Direct Connect
- C) AWS Lake Formation
- D) Amazon S3

https://github.com/justinjiajia/certifications/tree/main/aws/service_img_demo/datasync
 
AWS DataSync is the AWS service that can migrate data between AWS storage services. DataSync is designed to simplify and automate the process of transferring data between different storage services, both within AWS and on-premises. It can be used to migrate data from on-premises storage systems to AWS, as well as between various AWS storage services such as Amazon S3, Amazon EFS, Amazon FSx, and Amazon EBS.
Option B, AWS Direct Connect, is a network service that provides dedicated network connections between on-premises environments and AWS. It does not directly perform data migration between storage services.
Option C, AWS Lake Formation, is a service that helps in setting up a secure data lake on AWS, enabling data ingestion, data cataloging, and access control. It does not specifically focus on data migration between storage services.
Option D, Amazon S3 (Simple Storage Service), is an object storage service provided by AWS. While it is commonly used for storing and retrieving data, it does not have built-in capabilities for directly migrating data between other AWS storage services.
Therefore, the correct answer is A. AWS DataSync.

---

Q427. Which statements represent the cost-effectiveness of the AWS Cloud? (Choose two.)

- [x] A) Users can trade fixed expenses for variable expenses.
- B) Users can deploy all over the world in minutes.
- C) AWS offers increased speed and agility.
- D) AWS is responsible for patching the infrastructure.
- [x] E) Users benefit from economies of scale.

---

Q428. A company wants to design its cloud architecture so that it can support development innovations, and continuously improve processes and procedures. This is an example of which pillar of the AWS Well-Architected Framework?

- A) Security
- B) Performance efficiency
- [x] C) Operational excellence
- D) Reliability


> Operational Excellence: The operational excellence pillar focuses on running and monitoring systems, and continually improving processes and procedures.

---

Q429. A company needs to consolidate the billing for multiple AWS accounts. The company needs to use one account to pay on behalf of all the other accounts. Which AWS service or tool should the company use to meet this requirement?

- A) AWS Trusted Advisor
- [x] B) AWS Organizations
- C) AWS Budgets
- D) AWS Service Catalog

---

Q430. A company is moving some of its on-premises IT services to the AWS Cloud. The finance department wants to see the entire bill so it can forecast spending limits. Which AWS service can the company use to set spending limits and receive notifications if those limits are exceeded?

- A) AWS Cost and Usage Reports
- [x] B) AWS Budgets
- C) AWS Organizations consolidated billing
- D) Cost Explorer

---

Q431. Which AWS Support plans provide access to an AWS technical account manager (TAM)? (Choose two.)

- A) AWS Basic Support
- B) AWS Developer Support
- C) AWS Business Support
- [x] D) AWS Enterprise On-Ramp Support
- [x] E) AWS Enterprise Support

> AWS Enterprise On-Ramp Support: A pool of Technical Account Managers to provide proactive guidance, and coordinate access to programs and AWS experts

> AWS Enterprise Support: Designated Technical Account Manager (TAM) to provide consultative architectural and operational guidance delivered in the context of your applications and use-cases to help you achieve the greatest value from AWS

---

> [!IMPORTANT]
> Q432. Where can users find examples of AWS Cloud solution designs?
- A) AWS Marketplace
- B) AWS Service Catalog
- [x] C) AWS Architecture Center
- D) AWS Trusted Advisor

https://aws.amazon.com/architecture/

Users can find examples of AWS Cloud solution designs in the AWS Architecture Center.
The AWS Architecture Center is a resource hub that provides a collection of architectural best practices, whitepapers, reference architectures, and design patterns for building solutions on the AWS Cloud. It offers a wide range of pre-built architectures and design guidance across various industries and use cases.
Key features of the AWS Architecture Center include:
Reference architectures: The Architecture Center provides a library of reference architectures that serve as blueprints for building specific types of solutions on AWS. These reference architectures cover a wide range of scenarios, including web applications, data lakes, serverless architectures, and more.
Whitepapers and guides: The Architecture Center offers in-depth whitepapers and guides on various topics related to cloud architecture and design. These resources provide detailed explanations, best practices, and design considerations for building scalable, secure, and high-performing solutions on AWS.
Solutions by industry: The Architecture Center provides industry-specific solutions and design patterns, catering to the unique requirements of different sectors such as healthcare, finance, media, and more.
While the other options (A, B, and D) are also AWS services or features, they do not specifically provide examples of AWS Cloud solution designs:
- AWS Marketplace (Option A) is a digital catalog of software solutions and services from third-party vendors. While it offers a wide range of products, it is focused on software offerings rather than providing examples of solution designs.
- AWS Service Catalog (Option B) is a service that allows organizations to create and manage catalogs of approved IT services that can be deployed on AWS. It helps with governance and standardization but does not specifically provide examples of solution designs.
- AWS Trusted Advisor (Option D) is a service that provides recommendations to optimize AWS deployments in areas such as cost optimization, performance, security, and fault tolerance. While it offers guidance, it does not primarily focus on providing examples of solution designs. Therefore, among the options provided, the AWS Architecture Center is the most appropriate resource for users to find examples of AWS Cloud solution designs.

---

Q433. Which task is the responsibility of a company that is using Amazon RDS?
- A) Provision the underlying infrastructure.
- [x] B) Create IAM policies to control administrative access to the service.
- C) Install the cables to connect the hardware for compute and storage.
- D) Install and patch the RDS operating system.

---

Q434. Which of the following is an advantage that the AWS Cloud provides to users?
- [x] A) Users eliminate the need to guess about infrastructure capacity requirements.
- B) Users decrease their variable costs by maintaining sole ownership of IT hardware.
- C) Users maintain control of underlying IT infrastructure hardware.
- D) Users maintain control of operating systems for managed services.

---

Q435. Which feature of Amazon RDS provides the ability to automatically create a primary database instance and to synchronously replicate data to an instance in another Availability Zone?
- A) Read replicas
- B) Blue/green deployment
- [x] C) Multi-AZ deployment
- D) Reserved Instances

---

> [!IMPORTANT]
> Q436. A company needs to check for IAM access keys that have not been rotated recently. Which AWS service should the company use to meet this requirement?
- A) AWS WAF
- B) AWS Shield
- C) Amazon Cognito
- [x] D) AWS Trusted Advisor

https://github.com/justinjiajia/certifications/tree/main/aws/service_img_demo/trusted_advisor

one of security checks: IAM Access Key Rotation

---

Q437. A company runs many Amazon EC2 instances in its VPC. The company wants to use a native AWS security resource to control network traffic between certain EC2 instances. Which AWS service or feature will meet this requirement?
- A) Network ACLs
- B) AWS WAF
- C) Amazon GuardDuty
- [x] D) Security groups

---


Q438. Which of the following can be components of a VPC in the AWS Cloud? (Choose two.)
- A) Amazon API Gateway
- B) Amazon S3 buckets and objects
- C) AWS Storage Gateway
- [x] D) Internet gateway
- [x] E) Subnet

---

Q439. A company is building a new application on AWS. The company needs the application to remain available if an individual application component fails. Which design principle should the company use to meet this requirement?
- A) Disposable resources
- B) Automation
- C) Rightsizing
- [x] D) Loose coupling

---

Q440. A company wants to use a managed service to identify and protect sensitive data that is stored in Amazon S3. Which AWS service will meet these requirements?
- A) AWS IAM Access Analyzer
- B) Amazon GuardDuty
- C) Amazon Inspector
- [x] D) Amazon Macie

---

Q441. Which AWS service or feature can a user configure to limit network access at the subnet level?
- A) AWS Shield
- B) AWS WAF
- [x] C) Network ACL
- D) Security group


---

> [!IMPORTANT]
> Q442. Which AWS service can a company use to manage encryption keys in the cloud?
- A) AWS License Manager
- B) AWS Certificate Manager (ACM)
- [x] C) AWS CloudHSM (cloud hardware security module)
- D) AWS Directory Service


---

Q443. A company wants to enhance security by launching a third-party ISP intrusion detection system from its AWS account. Which AWS service or resource should the company use to meet this requirement?
- A) AWS Security Hub
- [x] B) AWS Marketplace
- C) AWS Quick Starts
- D) AWS Security Center

> keywords: third-party

---

Q444. How does the AWS Cloud help companies build agility into their processes and cloud infrastructure?
- A) Companies can avoid provisioning too much capacity when they do not know how much capacity is required.
- B) Companies can expand into new geographic regions.
- [x] C) Companies can access a range of technologies to experiment and innovate quickly.
- D) Companies can pay for IT resources only when they use the resources.

---


> [!IMPORTANT]
> Q445. Which AWS service or tool gives a company the ability to release application changes in an automated way?
- A) Amazon AppFlow
- [x] B) AWS CodeDeploy
- C) AWS PrivateLink
- D) Amazon EKS Distro


 
AWS CodeDeploy is a fully managed deployment service that automates the process of deploying applications to various compute services, including Amazon EC2 instances, on-premises instances, AWS Lambda functions, and more. It enables companies to release application changes in an automated and controlled manner.
Here's how AWS CodeDeploy facilitates automated application releases:
Deployment automation: AWS CodeDeploy provides a set of features and capabilities to automate the deployment process. It allows companies to define deployment configurations, specify deployment groups, and set up deployment rules to control the rollout of application changes.
Flexible deployment strategies: CodeDeploy supports multiple deployment strategies, such as rolling deployments, blue/green deployments, and canary deployments. These strategies enable companies to release updates gradually, minimize downtime, and easily roll back changes if issues occur.
Integration with existing CI/CD pipelines: CodeDeploy integrates seamlessly with popular CI/CD (Continuous Integration/Continuous Deployment) tools and services like AWS CodePipeline, Jenkins, and GitHub Actions. This integration enables companies to incorporate automated deployments into their existing development workflows.
Application health monitoring: During the deployment process, CodeDeploy actively monitors the health of each instance or function being updated. It performs automatic rollback if any deployment-related errors or issues are detected, ensuring the application remains in a healthy state.
By utilizing AWS CodeDeploy, companies can automate the release of application changes, reducing manual effort, minimizing deployment errors, and achieving faster and more reliable deployments.
Let's review the other options to understand why they are not the correct answers:
A. Amazon AppFlow: Amazon AppFlow is a service that enables the integration and transfer of data between various software-as-a-service (SaaS) applications and AWS services. While it facilitates data synchronization and integration, it does not specifically address the automation of application releases.
C. AWS PrivateLink: AWS PrivateLink is a networking feature that allows customers to securely access services hosted on AWS over a private connection. It focuses on enhancing network connectivity and security, rather than automating application releases.
D. Amazon EKS Distro: Amazon EKS Distro is a Kubernetes distribution provided by AWS for running Kubernetes clusters. While it helps with Kubernetes deployments, it does not specifically provide automated application release capabilities.
 


---

Q446. Which AWS Cloud Adoption Framework (AWS CAF) perspective focuses on managing identities and permissions at scale?
- A) Operations
- B) Platform
- C) Governance
- [x] D) Security (identity and access management capability)

> This is the identity and access management capability that belongs to the security perspective.
 
---

> [!IMPORTANT]
> Q447. Which AWS service or feature allows users to securely store encrypted credentials and retrieve these credentials when required?
- A) AWS Encryption SDK
- B) AWS Security Hub
- [x] C) AWS Secrets Manager
- D) AWS Artifact

---

Q448. Which pillar of the AWS Well-Architected Framework aligns with the ability to make frequent, small, and reversible changes to AWS Cloud architecture?
- A) Security
- B) Cost optimization
- [x] C) Operational excellence
- D) Performance efficiency

---

> [!IMPORTANT]
> Q449. Which AWS service or resource can a company use to deploy AWS WAF rules?

- A) Amazon EC2
- [x] B) Application Load Balancer
- C) AWS Trusted Advisor
- D) Network Load Balancer


AWS WAF is a web application firewall service that helps protect web applications from common web exploits and attacks. To deploy AWS WAF rules, a company can leverage an AWS service that acts as a frontend to their web application and supports AWS WAF integration. One such service is the Application Load Balancer (ALB).
Here's how the Application Load Balancer enables the deployment of AWS WAF rules:
Web traffic routing: The Application Load Balancer acts as a load balancer and distributes incoming web traffic across multiple targets, such as Amazon EC2 instances, containers, or Lambda functions. It provides advanced request routing capabilities based on various criteria, including URL path, host, and query parameters.
Integration with AWS WAF: The Application Load Balancer seamlessly integrates with AWS WAF. It allows companies to associate AWS WAF rules with the ALB to inspect and filter incoming web requests. Companies can define WAF rules to identify and block malicious traffic, prevent common web exploits, and enforce security policies.
Rule evaluation and enforcement: When web traffic passes through the Application Load Balancer, the integrated AWS WAF evaluates the associated rules. If a request matches any rule conditions, the WAF takes the specified action, such as allowing, blocking, or diverting the request to another path. This helps protect web applications from various types of attacks, including SQL injection, cross-site scripting (XSS), and more.
By leveraging the Application Load Balancer and its integration with AWS WAF, companies can deploy and enforce WAF rules at the entry point of their web applications. This provides an additional layer of security and helps protect against common web-based attacks.
Let's review the other options to understand why they are not the correct answers:
A. Amazon EC2: Amazon EC2 is a web service that provides resizable compute capacity in the cloud. While it allows companies to deploy and manage virtual servers, it does not have native integration with AWS WAF for deploying WAF rules.
C. AWS Trusted Advisor: AWS Trusted Advisor is a service that provides recommendations to optimize AWS environments for security, cost, performance, and fault tolerance. It offers guidance and best practices but does not directly facilitate the deployment of AWS WAF rules.
D. Network Load Balancer: The Network Load Balancer is another AWS load balancing service that operates at the network layer (Layer 4) and is designed for high-throughput, low-latency traffic. Unlike the Application Load Balancer, the Network Load Balancer does not have native integration with AWS WAF for deploying WAF rules.


---

Q450. A company hosts its website on Amazon EC2 instances. The company needs to ensure that the website reaches a global audience and provides minimum latency to users. Which AWS service should the company use to meet these requirements?

- A) Amazon Route 53
- [x] B) Amazon CloudFront
- C) Elastic Load Balancing
- D) AWS Lambda


---

Q451. Which AWS design principle emphasizes the reduction of interdependencies between components of an application?

- A) Scalability
- [x] B) Loose coupling
- C) Automation
- D) Caching


---

> [!IMPORTANT]
> Q452. A company wants to provide one of its employees with access to Amazon RDS. The company also wants to limit the interaction to only the AWS CLI and AWS software development kits (SDKs).
Which combination of actions should the company take to meet these requirements while following the principles of least privilege? (Choose two.)

- A) Create an IAM user and provide AWS Management Console access only.
- [x] B) Create an IAM user and provide programmatic access only.
- C) Create an IAM role and provide AWS Management Console access only.
- D) Create an IAM policy with administrator access and attach it to the IAM user.
- [x] E) Create an IAM policy with Amazon RDS access and attach it to the IAM user.

---

Q453. A company is running a reporting web server application on Amazon EC2 instances. The application runs once every week and once again at the end of the month. The EC2 instances can be shut down when they are not in use. What is the MOST cost-effective billing model for this use case?

- A) Standard Reserved Instances
- B) Convertible Reserved Instances
- C) On-Demand Capacity Reservations
- [x] D) On-Demand Instances

---

> [!IMPORTANT]
> Q454. A company wants to discover, prepare, move, and integrate data from multiple sources for data analytics and machine learning. Which AWS serverless data integration service should the company use to meet these requirements?

- [x] A) AWS Glue
- B) AWS Data Exchange
- C) Amazon Athena
- D) Amazon EMR

> keywords: severless

AWS Glue is an AWS serverless data integration service that provides capabilities for discovering, preparing, and transforming data from various sources. It is designed to simplify the process of building and managing data pipelines for analytics and machine learning workloads.
Here's how AWS Glue meets the company's requirements:
Data discovery: AWS Glue provides automated data discovery, which helps to identify and catalog data from various sources, such as databases, data warehouses, data lakes, and other storage systems. It can scan and analyze data to infer schemas, metadata, and relationships, making it easier to understand the available data assets.
Data preparation and transformation: AWS Glue offers a visual interface and a code-centric approach for building data transformation workflows. It supports data preparation tasks like cleaning, filtering, aggregating, and joining data from different sources. Glue provides a range of built-in transformations and allows custom transformations using Apache Spark or Python code.
Data movement and integration: AWS Glue integrates with various AWS services and data sources, enabling seamless data movement between different systems. It supports data extraction, transformation, and loading (ETL) operations to move data into data lakes, data warehouses, or other destinations for analytics and machine learning purposes.
Serverless and scalable: AWS Glue is a serverless service, which means it automatically scales to handle varying data volumes and processing requirements. It eliminates the need for provisioning and managing infrastructure, allowing the company to focus on data integration tasks without worrying about the underlying infrastructure.


B. AWS Data Exchange: AWS Data Exchange is a service for finding, subscribing to, and using third-party data sets. It primarily focuses on data acquisition and exchange, rather than data integration and transformation.
C. Amazon Athena: Amazon Athena is a serverless query service for analyzing data stored in Amazon S3 using standard SQL queries. While Athena enables ad-hoc querying of data, it does not provide the comprehensive data integration capabilities required to prepare, transform, and move data from multiple sources.
D. Amazon EMR (Elastic MapReduce): Amazon EMR is a managed big data processing service that uses Apache Hadoop and Apache Spark for processing large amounts of data. While EMR can handle data processing tasks, it is not specifically designed for data integration and preparation.


--- 

Q455. A company is moving its development and test environments to AWS to increase agility and reduce cost. Because these are not production workloads and the servers are not fully utilized, occasional unavailability is acceptable. What is the MOST cost-effective Amazon EC2 pricing model that will meet these requirements?

- A) Reserved Instances
- B) On-Demand Instances
- [x] C) Spot Instances
- D) Dedicated Hosts

--- 


Q456. A company deploys its application on Amazon EC2 instances. The application occasionally experiences sudden increases in demand. The company wants to ensure that its application can respond to changes in demand at the lowest possible cost. Which AWS service or concept will meet these requirements?

- [x] A) AWS Auto Scaling
- B) AWS Compute Optimizer
- C) AWS Cost Explorer
- D) AWS Well-Architected Framework


---


Q457. A company wants to organize its users so that the company can grant permissions to the users as a group. Which AWS service or tool can the company use to meet this requirement?

- A) Security groups
- [x]  B) AWS Identity and Access Management (IAM)
- C) Resource groups
- D) AWS Security Hub


---


Q458. A company wants to build an application that uses AWS Lambda to run Python code. Under the AWS shared responsibility model, which tasks will be the company's responsibility? (Choose two.)

- A) Management of the underlying infrastructure.
- B) Management of the operating system.
- [x] C) Writing the business logic code.
- D) Installation of the computer language runtime.
- [x] E) Providing AWS Identity and Access Management (IAM) access to the Lambda service.

---


Q459. A company needs to identify who accessed an AWS service and what action was performed for a given time period. Which AWS service should the company use to meet this requirement?

- A) Amazon CloudWatch
- [x] B) AWS CloudTrail
- C) AWS Security Hub
- D) Amazon Inspector


---



> [!IMPORTANT]
> Q460. A company wants to use a centralized AWS service to enforce compliance with the organizational business standards. The company wants to use an AWS service that can govern and control who can deploy, manage, and decommission AWS resources. Which AWS service will meet these requirements?

- A) Amazon CloudWatch
- [x] B) AWS Service Catalog
- C) Amazon GuardDuty
- D) AWS Security Hub


---

Q461. What does "security of the cloud" refer to in the AWS shared responsibility model?

- A) Availability of AWS services such as Amazon EC2
- [x] B) Security of the cloud infrastructure that runs all the AWS services
- C) Implementation of password policies for IAM users
- D) Security of customer environments by using AWS Network Firewall partners

---

Q462. A company has an application that produces unstructured data continuously. The company needs to store the data so that the data is durable and easy to query. Which AWS service can the company use to meet these requirements?

- A) Amazon RDS
- B) Amazon Aurora
- C) Amazon QuickSight
- [x] D) Amazon DynamoDB



---

Q463. Which options are AWS Cloud Adoption Framework (AWS CAF) perspectives? (Choose two.)

- A) Cloud fluency (a capability of the people perspective)
- [x] B) Security
- C) Change acceleration (a capability of the peope perspective)
- D) Architecture
- [x] E) Business

---

Q464. A company wants to migrate a company's on-premises container infrastructure to the AWS Cloud. The company wants to prevent unplanned administration and operation cost and adapt to a serverless architecture. Which AWS service will meet these requirements?

- A) Amazon Connect
- [x] B) AWS Fargate
- C) Amazon Lightsail
- D) Amazon EC2


---

Q465. A company wants its Amazon EC2 instances to be in different locations but share the same geographic area. The company also wants to use multiple power grids and independent networking connectivity for the EC2 instances. Which solution meets these requirements?

- A) Use EC2 instances in multiple edge locations in the same AWS Region.
- [x] B) Use EC2 instances in multiple Availability Zones in the same AWS Region.
- C) Use EC2 instances in multiple Amazon Connect locations in the same AWS Region.
- D) Use EC2 instances in multiple AWS Artifact locations in the same AWS Region.


---

Q466. An ecommerce company has deployed a new web application on Amazon EC2 instances. The company wants to distribute incoming HTTP traffic evenly across all running instances. Which AWS service or resource will meet this requirement?

- A) Amazon EC2 Auto Scaling
- [x] B) Application Load Balancer
- C) Gateway Load Balancer
- D) Network Load Balancer


---

Q467. Which AWS service or feature gives users the ability to connect VPCs and on-premises networks to a central hub?

- A) Virtual private gateway
- [x] B) AWS Transit Gateway
- C) Internet gateway
- D) Customer gateway


---

> [!IMPORTANT]
> Q468. A company wants to run CPU-intensive workload across multiple Amazon EC2 instances. Which EC2 instance type should the company use to meet this requirement?

- A) General purpose instances
- [x] B) Compute optimized instances
- C) Memory optimized instances
- D) Storage optimized instances


---

> [!IMPORTANT]
> Q469. A company is connecting multiple VPCs and on-premises networks. The company needs to use an AWS service as a cloud router to simplify peering relationships. Which AWS service can the company use to meet this requirement?

- A) AWS Direct Connect
- [x] B) AWS Transit Gateway
- C) Amazon Connect
- D) Amazon Route 53

>  AWS Transit Gateway helps you design and implement networks at scale by acting as a cloud router. 
---


> [!IMPORTANT]
> Q470. A company stores a large amount of data that auditors access only twice each year. Which Amazon S3 storage class should the company use to store the data with the LOWEST cost?

- A. Amazon S3 Outposts
- [x] B. Amazon S3 Glacier Instant Retrieval
- C. Amazon S3 Standard
- D. Amazon S3 Intelligent-Tiering

https://aws.amazon.com/s3/pricing/

> The three automatic access tiers managed by Amazon S3 Intelligent-Tiering are: 1) Frequent Access, 2) Infrequent Access, and 3) Archive Instant Access. Among these, the Archive Instant Access tier is the most cost-effective, with storage charged at $0.004 per GB per month. If an object is moved out of this tier, it will incur a higher storage rate.

> S3 Glacier Instant Retrieval: For long-lived archive data accessed once a quarter with instant retrieval in milliseconds; All Storage / Month	$0.004 per GB


---

Q471. Which action should a company take to improve security in its AWS account?

- [x] A. Require multi-factor authentication (MFA) for privileged users.
- B. Remove the root user account.
- C. Create an access key for the AWS account root user.
- D. Create an access key for each privileged user.

---

Q472. Which of the following are ways to improve security on AWS? (Choose two.)

- A. Using AWS Artifact
- B. Granting the broadest permissions to all IAM roles
- C. Running application code with AWS Cloud
- [x] D. Enabling multi-factor authentication (MFA) with Amazon Cognito
- [x] E. Using AWS Trusted Advisor security checks

 

---

Q473. A company wants to store its files in the AWS Cloud. Users need to be able to download these files directly using a public URL. Which AWS service or feature will meet this requirement?

- A. Amazon Redshift
- B. Amazon Elastic Block Store (Amazon EBS)
- C. Amazon Elastic File System (Amazon EFS)
- [x] D. Amazon S3

---

> [!IMPORTANT]
> Q474. A company is using AWS for all its IT infrastructure. The company's developers are allowed to deploy applications on their own. The developers want to deploy their applications without having to provision the infrastructure themselves. Which AWS service should the developers use to meet these requirements?

- A. AWS CloudFormation
- B. AWS CodeBuild
- [x] C. AWS Elastic Beanstalk
- D. AWS CodeDeploy

Service	Requires Infrastructure Work	Reason
A. CloudFormation	✅ Yes	Requires developers to write infrastructure-as-code templates (YAML/JSON).
B. CodeBuild	✅ Partial	Only builds code; doesn’t deploy/provision infrastructure.
D. CodeDeploy	✅ Yes	Deploys code to existing infrastructure (must provision EC2/Lambda first).

---

Q475. A company wants to gain insights from its data and build interactive data visualization dashboards. Which AWS service will meet these requirements?

- A. Amazon SageMaker
- B. Amazon Rekognition
- [x] C. Amazon QuickSight
- D. Amazon Kinesis


---


Q476. A cloud engineer wants to store data in Amazon S3. The engineer will access some of the data yearly and some of the data daily. Which S3 storage class will meet these requirements MOST cost-effectively?

- A. S3 Standard
- B. S3 Glacier Deep Archive
- C. S3 One Zone-Infrequent Access (S3 One Zone-IA)
- [x] D. S3 Intelligent-Tiering

> implies unknown or changing access patterns; storage class is specified at the object level

---

Q477. Which of the following are economic benefits of using the AWS Cloud? (Choose two.)

- [x] A. Consumption-based pricing
- B. Perpetual licenses
- [x] C. Economies of scale
- D. AWS Enterprise Support at no additional cost
- E. Bring-your-own-hardware model


---

Q478. A user is moving a workload from a local data center to an architecture that is distributed between the local data center and the AWS Cloud. Which type of migration is this?

- A. On-premises to cloud native
- B. Hybrid to cloud native
- [x] C. On-premises to hybrid
- D. Cloud native to hybrid


---

Q479. A company needs to store infrequently used data for data archives and long-term backups. Which AWS service or storage class will meet these requirements MOST cost-effectively?

- A. Amazon FSx for Lustre
- B. Amazon Elastic Block Store (Amazon EBS)
- C. Amazon Elastic File System (Amazon EFS)
- [x] D. Amazon S3 Glacier Flexible Retrieval


---

Q480. Which AWS service provides users with AWS issued reports, certifications, accreditations, and third-party attestations?

- [x] A. AWS Artifact
- B. AWS Trusted Advisor
- C. AWS Health Dashboard
- D. AWS Config


---

Q481. A company needs to create and publish interactive business intelligence dashboards. The dashboards require insights that are powered by machine learning. Which AWS service or tool will meet these requirements?

- A. AWS Glue Studio
- [x] B. Amazon QuickSight
- C. Amazon Redshift
- D. Amazon Athena


---

> [!IMPORTANT]
> Q482. A company wants to use AWS. The company has stringent requirements about low-latency access to on-premises systems and data residency. Which AWS service should the company use to design a solution that meets these requirements?

- A. AWS Wavelength
- B. AWS Transit Gateway
- C. AWS Ground Station
- [x] D. AWS Outposts


AWS Outposts is a fully managed service that extends AWS infrastructure, services, APIs, and tools to customer premises. It allows customers to run AWS services locally on their own hardware while seamlessly connecting to the rest of their AWS resources in the cloud.
Key features of AWS Outposts that make it suitable for the given requirements are:
Low-Latency Access: AWS Outposts enables organizations to have low-latency access to on-premises systems by deploying AWS services and compute instances directly on their own infrastructure. This allows for fast data transfer and reduced network latency when accessing on-premises systems and data.
Data Residency: With AWS Outposts, organizations can keep sensitive data on-premises, addressing data residency requirements. Data processed and stored on AWS Outposts remains within the customer's own data center, providing control and compliance for workloads that require data to stay on-premises.
Seamless Integration: AWS Outposts is seamlessly integrated with other AWS services and resources in the cloud. It allows organizations to leverage the full range of AWS services, tools, and APIs, ensuring consistency and compatibility with their existing AWS workloads. 

A. AWS Wavelength: AWS Wavelength is a service that provides ultra-low latency for mobile and edge computing applications by placing AWS compute and storage resources closer to the edge of the 5G network. It is not specifically focused on on-premises systems or data residency.
B. AWS Transit Gateway: AWS Transit Gateway is a service that simplifies network connectivity between Amazon Virtual Private Clouds (VPCs) and on-premises networks. While it facilitates connectivity, it does not directly address low-latency access to on-premises systems or data residency.
C. AWS Ground Station: AWS Ground Station is a service that provides satellite communication capabilities. It is not directly related to on-premises systems or data residency.
Therefore, for a solution that meets the requirements of low-latency access to on-premises systems and data residency, the recommended option is AWS Outposts.

---

Q483. A company runs an on-premises contact center for customers. The company needs to migrate to a cloud-based solution that can deliver artificial intelligence features to improve user experience. Which AWS service will meet these requirements?

- A. AWS Wavelength
- B. AWS IAM Identity Center (AWS Single Sign-On)
- C. AWS Direct Connect
- [x] D. Amazon Connect


Amazon Connect is a cloud-based contact center service provided by AWS. It is designed to deliver a seamless customer experience with advanced features and integrations, including artificial intelligence capabilities.
Key features of Amazon Connect that make it suitable for the given requirements are:
Cloud-Based Contact Center: Amazon Connect allows companies to migrate their contact center infrastructure to the cloud, eliminating the need for on-premises hardware and providing scalability, flexibility, and reliability.
Artificial Intelligence Features: Amazon Connect integrates with AWS AI services such as Amazon Lex (for conversational interfaces), Amazon Polly (for text-to-speech), and Amazon Transcribe (for speech recognition). These services enable the use of natural language understanding, automated speech recognition, and other AI capabilities to enhance customer interactions and self-service options.
Interactive Voice Response (IVR): Amazon Connect provides an IVR system that uses AI-powered speech recognition to automate customer interactions. This allows customers to navigate through menus, provide responses, and receive information without the need for agent assistance.
Integration Capabilities: Amazon Connect can integrate with other AWS services, such as Amazon S3 for call recording storage and Amazon CloudWatch for monitoring and analytics. It also supports integration with third-party systems, CRM platforms, and workforce management tools.
Scalability and Flexibility: Amazon Connect offers the ability to scale up or down based on call volumes and business needs. It supports global deployments and provides regional redundancy for high availability.
On the other hand, the other options do not specifically address the requirements of migrating the contact center to a cloud-based solution with artificial intelligence features:
A. AWS Wavelength: AWS Wavelength is a service that provides ultra-low latency for mobile and edge computing applications by placing AWS compute and storage resources closer to the edge of the 5G network. It is not directly related to contact center solutions.
B. AWS IAM Identity Center (AWS Single Sign-On): AWS Single Sign-On (SSO) is an AWS service that simplifies user management and access to multiple AWS accounts and business applications. It is not specifically designed for contact center solutions or artificial intelligence features.
C. AWS Direct Connect: AWS Direct Connect is a network service that provides dedicated network connections between on-premises environments and AWS. While it facilitates connectivity, it does not directly address contact center solutions or artificial intelligence features.
Therefore, for migrating the on-premises contact center to a cloud-based solution with artificial intelligence features, the recommended option is Amazon Connect.


---

Q484. A company needs the ability to acquire resources when the resources are needed. The company also needs the ability to release the resources when the resources are no longer needed.
Which AWS concept represents the company's goals?

- A. Scalability
- B. Sustainability
- [x] C. Elasticity
- D. Operational excellence

---



Q485. A company wants to use Amazon EC2 instances for a stable production workload that will run for 1 year. Which instance purchasing option meets these requirements MOST cost-effectively?

- A. Dedicated Hosts
- [x] B. Reserved Instances
- C. On-Demand Instances
- D. Spot Instances


---

Q486. A company wants to log in securely to Linux Amazon EC2 instances. How can the company accomplish this goal?

- [x] A. Use SSH keys.
- B. Use a VPN.
- C. Use end-to-end encryption.
- D. Use Amazon Route 53.


---

Q487. A company wants to use a serverless compute service for an application. Which AWS service will meet this requirement?

- [x] A. AWS Lambda
- B. AWS CloudFormation
- C. AWS Elastic Beanstalk
- D. Elastic Load Balancing


---


Q488. A company wants a solution that will automatically adjust the number of Amazon EC2 instances that are being used based on the current load. Which AWS offering will meet these requirements?

- A. Dedicated Hosts
- B. Placement groups
- [x] C. Auto Scaling groups
- D. Reserved Instances


---


Q489. A company is building AWS architecture to deliver real-time data feeds from an on-premises data center into an application that runs on AWS. The company needs a consistent network connection with minimal latency. What should the company use to connect the application and the data center to meet these requirements?

- [x] A. AWS Direct Connect
- B. Public internet
- C. AWS VPN
- D. Amazon Connect

---

Q490. A company plans to migrate its custom marketing application and order-processing application to AWS. The company needs to deploy the applications on different types of instances with various configurations of CPU, memory, storage, and networking capacity. Which AWS service should the company use to meet these requirements?

- A. AWS Lambda
- B. Amazon Cognito
- C. Amazon Athena
- [x] D. Amazon EC2


---

Q491. A company wants to monitor and block malicious HTTP and HTTPS requests that its Amazon CloudFront distributions receive. Which AWS service should the company use to meet these requirements?

- A. Amazon GuardDuty
- B. Amazon Inspector
- [x] C. AWS WAF
- D. Amazon Detective

> application level traffic

AWS WAF is a web application firewall service that helps protect web applications from common web exploits and attacks. Here's how AWS WAF meets the requirements:
Monitoring: AWS WAF allows you to define rules and conditions to monitor incoming HTTP and HTTPS requests to your CloudFront distributions. You can specify criteria to match specific patterns, such as IP addresses, request headers, or query strings. When a request matches the defined criteria, AWS WAF logs the request details for monitoring and analysis.
Blocking: AWS WAF provides the capability to block or allow requests based on defined rules. You can create rules to identify and block malicious requests, such as those originating from known malicious IP addresses or containing suspicious patterns in headers or payloads. When a request matches a blocking rule, AWS WAF can either block the request outright or redirect it to a different resource.
Integration with CloudFront: AWS WAF seamlessly integrates with Amazon CloudFront, which is a content delivery network (CDN) service. You can associate AWS WAF rules with your CloudFront distributions to filter and inspect the incoming requests at the edge locations. This helps in minimizing the latency and improving the response time for blocking malicious requests.
Managed Rulesets: AWS WAF offers managed rulesets that include pre-configured rules to detect and block common web-based attacks, such as SQL injection, cross-site scripting (XSS), and more. These managed rulesets provide an additional layer of protection without the need for manual rule creation.
On the other hand, the other options do not specifically address monitoring and blocking malicious HTTP and HTTPS requests:
A. Amazon GuardDuty: Amazon GuardDuty is a threat detection service that uses machine learning and anomaly detection to identify potential malicious activity in AWS accounts and workloads. While it provides overall threat detection, it is not specifically focused on monitoring and blocking HTTP and HTTPS requests to CloudFront.
B. Amazon Inspector: Amazon Inspector is an automated security assessment service that helps identify vulnerabilities and security issues in EC2 instances and applications. It does not directly address monitoring and blocking malicious requests to CloudFront.
D. Amazon Detective: Amazon Detective is a service that analyzes and visualizes data from AWS resources to help identify and investigate potential security issues. It does not have the specific capability to monitor and block malicious requests to CloudFront.


---
Q492. Which AWS services can host PostgreSQL databases? (Choose two.)

- A. Amazon S3
- [x] B. Amazon Aurora
- [x] C. Amazon EC2
- D. Amazon OpenSearch Service
- E. Amazon Elastic File System (Amazon EFS)

---

> [!IMPORTANT]
> Q493. Which AWS service can generate information that can be used by external auditors?

- A. Amazon Cognito
- B. Amazon FSx
- [x] C. AWS Config
- D. Amazon Inspector


> AWS Config is a service that provides a detailed inventory of the AWS resources in an account and tracks changes made to those resources over time. It captures configuration snapshots and configuration change history, which can be used for compliance auditing and governance purposes. AWS Config allows you to assess and evaluate the configuration of your resources against desired configurations, policies, and best practices.

> By enabling AWS Config, you can generate configuration snapshots and logs that provide a comprehensive view of the configuration state of your AWS resources. This information can be utilized by external auditors to assess compliance with regulatory requirements, security standards, and internal policies.


> A. Amazon Cognito: Amazon Cognito is an authentication, authorization, and user management service. While it provides user-related information, it is not specifically designed for generating information for external auditors.

> B. Amazon FSx: Amazon FSx is a fully managed file system service. It provides scalable and durable file storage but does not generate information specifically for external auditors.

> D. Amazon Inspector: Amazon Inspector is an automated security assessment service that helps identify vulnerabilities and security issues in EC2 instances and applications. While it provides security assessment information, it may not be directly suitable for generating information for external auditors.
 


---

> [!IMPORTANT]
> Q494. Which AWS service or feature requires an internet service provider (ISP) and a colocation facility to be implemented?

- A. AWS VPN
- B. Amazon Connect
- [x] C. AWS Direct Connect
- D. Internet gateway
 
AWS Direct Connect is a network service that establishes a dedicated and private connection between an on-premises data center and AWS. It requires the involvement of an ISP and a colocation facility to be implemented. Here's how it works:
- Internet Service Provider (ISP): The ISP is responsible for providing the physical network connectivity between the customer's on-premises data center and the colocation facility where AWS Direct Connect is available. The ISP ensures that the customer's network traffic reaches the colocation facility.
- Colocation Facility: The colocation facility is a third-party data center where AWS Direct Connect is available. It is responsible for providing the physical infrastructure and connectivity to AWS Direct Connect. The customer's network traffic is routed from their on-premises data center to the colocation facility via the ISP.
- Dedicated Connection: With AWS Direct Connect, a dedicated and private connection is established between the customer's network and AWS. This connection bypasses the public internet, providing a more secure and consistent network connection for data transfers between the on-premises data center and AWS.
- High-Speed and Low-Latency Connection: AWS Direct Connect offers high-speed connection options ranging from 1 Gbps to 100 Gbps. It provides low-latency and reliable connectivity, which is particularly useful for applications that require real-time data feeds or low-latency access to AWS services.
On the other hand, the other options mentioned do not require an ISP and a colocation facility for implementation:
A. AWS VPN: AWS VPN allows for secure communication between the customer's network and AWS over the internet. It does not require an ISP and a colocation facility but relies on internet connectivity.
B. Amazon Connect: Amazon Connect is a cloud-based contact center service and does not require an ISP and a colocation facility for implementation.
D. Internet Gateway: The internet gateway is a horizontally scalable and highly available AWS service that provides a connection between an Amazon VPC (Virtual Private Cloud) and the internet. It does not require an ISP and a colocation facility for implementation.
 

---
Q495. Which AWS service allows for file sharing between multiple Amazon EC2 instances?

- A. AWS Direct Connect
- B. AWS Snowball Edge
- C. AWS Backup
- [x] D. Amazon Elastic File System (Amazon EFS)


Amazon Elastic File System (Amazon EFS) is a fully managed, scalable, and shared file storage service in the AWS cloud. It provides file storage that can be accessed by multiple Amazon EC2 instances concurrently. Here's how Amazon EFS enables file sharing:
Shared File System: Amazon EFS allows you to create a file system that can be mounted and accessed by multiple EC2 instances simultaneously. This enables file sharing and collaboration between different instances.
NFS Protocol: Amazon EFS uses the Network File System (NFS) protocol, specifically NFSv4.1, which is a widely supported network file sharing protocol. EC2 instances can mount the Amazon EFS file system using the NFS client and access files and directories stored in the file system.
Elastic Scalability: Amazon EFS is designed to be highly scalable, allowing you to grow or shrink your file system automatically as your storage needs change. It can handle thousands of concurrent connections and provides high throughput and low latency access to files.
Data Durability and Availability: Amazon EFS automatically replicates data across multiple Availability Zones (AZs) within a region, providing high durability and availability for your files. This ensures that your data is protected against hardware failures and provides access even if one AZ becomes unavailable.
On the other hand, the other options mentioned do not specifically provide file sharing capabilities between EC2 instances:
A. AWS Direct Connect: AWS Direct Connect is a network service that establishes a dedicated connection between an on-premises data center and AWS. It is not directly related to file sharing between EC2 instances.
B. AWS Snowball Edge: AWS Snowball Edge is a data transfer and edge computing device. While it can be used for data transfer, it does not offer native file sharing capabilities between EC2 instances.
C. AWS Backup: AWS Backup is a managed backup service that helps you centrally manage and automate backups of your AWS resources. While it deals with backups, it does not provide file sharing capabilities between EC2 instances.


---

Q496. A company needs to manage multiple logins across AWS accounts within the same organization in AWS Organizations. Which AWS service should the company use to meet this requirement?

- A. Amazon VPC
- B. Amazon GuardDuty
- C. Amazon Cognito
- [x] D. AWS IAM Identity Center


AWS IAM Identity Center is a service provided by AWS Identity and Access Management (IAM) that allows organizations to centrally manage multiple AWS accounts within their organization. It provides a unified login experience for users across multiple AWS accounts and enables administrators to manage access and permissions consistently.
Here's how AWS IAM Identity Center helps in managing multiple logins across AWS accounts within the same organization:
Centralized Identity Management: AWS IAM Identity Center allows organizations to create and manage a single identity source for users across multiple AWS accounts. Users can have a single set of credentials (username and password) to access various accounts within the organization.
Single Sign-On (SSO): With AWS IAM Identity Center, users can sign in once and access multiple AWS accounts without the need to re-enter credentials for each account. It provides a seamless and streamlined login experience for users.
Fine-Grained Access Control: Administrators can define and manage permissions for users and groups centrally through AWS IAM Identity Center. This allows for consistent access control across multiple AWS accounts, ensuring that users have the appropriate permissions in each account.
Integration with AWS Organizations: AWS IAM Identity Center integrates with AWS Organizations, which is a service for managing multiple AWS accounts. It allows organizations to create and manage accounts hierarchically and apply policies across the organization. AWS IAM Identity Center complements AWS Organizations by providing centralized identity management for the accounts.
 
> A. Amazon VPC: Amazon VPC (Virtual Private Cloud) is a service that allows you to create a virtual network in the AWS cloud. It does not provide specific features for managing logins across AWS accounts.

> B. Amazon GuardDuty: Amazon GuardDuty is a threat detection service that provides continuous monitoring for malicious activity in AWS accounts. It does not directly address the need for managing multiple logins across accounts.

> C. Amazon Cognito: Amazon Cognito is an authentication and user management service. While it provides user management capabilities, it is not specifically designed for managing logins across multiple AWS accounts within an organization.

---

Q497. A company uses Amazon WorkSpaces. Which task is the responsibility of AWS, according to the AWS shared responsibility model?

- A. Set up multi-factor authentication (MFA) for each WorkSpaces user account.
- [x] B. Ensure the environmental safety and security of the AWS infrastructure that hosts WorkSpaces.
- C. Provide security for WorkSpaces user accounts through AWS Identity and Access Management (IAM).
- D. Configure AWS CloudTrail to log API calls and user activity.

---

Q498. A company is migrating its public website to AWS. The company wants to host the domain name for the website on AWS. Which AWS service should the company use to meet this requirement?

A. AWS Lambda
- [x] B. Amazon Route 53
C. Amazon CloudFront
D. AWS Direct Connect

Amazon Route 53 is a scalable domain name system (DNS) web service provided by AWS. It allows you to manage the domain names for your websites and route incoming user requests to the appropriate resources within your infrastructure. Here's how Amazon Route 53 helps in hosting the domain name:
Domain Name Registration: Amazon Route 53 provides domain name registration services, allowing you to register new domain names or transfer existing domain names to AWS. You can purchase and manage domain names directly within the Amazon Route 53 console.
DNS Management: Amazon Route 53 acts as a DNS service, allowing you to manage the DNS records for your domain. You can configure DNS records such as A records, CNAME records, and MX records to map your domain name to the appropriate resources within your AWS infrastructure.
Traffic Routing: Amazon Route 53 provides advanced routing capabilities, allowing you to route incoming user requests to different resources based on various criteria. For example, you can configure routing policies such as simple routing, weighted routing, latency-based routing, or geolocation routing to distribute traffic across multiple AWS resources or regions.
Health Checks and Failover: Amazon Route 53 offers health check capabilities to monitor the health of resources associated with your domain. You can configure health checks to monitor the availability of your website and automatically route traffic away from unhealthy resources. This helps in achieving high availability and fault tolerance for your website.
On the other hand, the other options mentioned are not specifically designed for hosting domain names:
A. AWS Lambda: AWS Lambda is a serverless compute service that allows you to run your code without provisioning or managing servers. It is not directly related to hosting domain names.
C. Amazon CloudFront: Amazon CloudFront is a content delivery network (CDN) service that accelerates the delivery of your web content to end users. While it can be used for caching and distributing website content, it does not handle domain name hosting.
D. AWS Direct Connect: AWS Direct Connect is a network service that establishes a dedicated and private connection between an on-premises data center and AWS. It is not specifically designed for hosting domain names.

---


Q499. A company uses a third-party identity provider (IdP). The company wants to provide its employees with access to AWS accounts and services without requiring another set of login credentials.
Which AWS service will meet this requirement?

- A. AWS Directory Service
- B. Amazon Cognito
- [x] C. AWS IAM Identity Center
- D. AWS Resource Access Manager (AWS RAM)



---

> [!IMPORTANT]
> Q500. Which combination of AWS services can be used to move a commercial relational database to an Amazon-managed open-source database? (Choose two.)

- [x] A. AWS Database Migration Service (AWS DMS)
- B. AWS software development kits (SDKs)
- [x] C. AWS Schema Conversion Tool
- D. AWS Systems Manager
- E. Amazon EMR


 > AWS Database Migration Service (AWS DMS): AWS DMS is a service that simplifies and automates the process of migrating relational databases, including commercial databases, to AWS. It supports both homogeneous and heterogeneous database migrations, allowing you to migrate from one database engine to another. In this case, you can use AWS DMS to migrate the commercial relational database to the Amazon-managed open-source database.

> AWS Schema Conversion Tool: The AWS Schema Conversion Tool (AWS SCT) is used to convert the schema of the source database to a compatible schema for the target database. It helps in converting the schema objects, such as tables, views, stored procedures, and functions, from the source commercial database to the Amazon-managed open-source database. AWS SCT automates the schema conversion process and provides recommendations for manual code conversion.
 

> B. AWS software development kits (SDKs): AWS SDKs are used by developers to interact with AWS services programmatically. While SDKs are useful for application development and integration with AWS services, they are not directly involved in the database migration process.

> D. AWS Systems Manager: AWS Systems Manager is a management service that helps you automate operational tasks on AWS resources. It provides features such as configuration management, automation, and parameter storage. While it can be used for managing databases, it does not specifically facilitate the migration of a commercial database to an Amazon-managed open-source database.

> E. Amazon EMR: Amazon EMR (Elastic MapReduce) is a service used for big data processing and analytics, particularly for processing large-scale data sets using frameworks like Apache Hadoop and Apache Spark. It is not directly related to migrating a commercial relational database to an Amazon-managed open-source database.


---

Q501. Which AWS service gives users on-demand, self-service access to AWS compliance control reports?

- A. AWS Config
- B. Amazon GuardDuty
- C. AWS Trusted Advisor
- [x] D. AWS Artifact



The AWS service that gives users on-demand, self-service access to AWS compliance control reports is D. AWS Artifact.
AWS Artifact provides customers with access to various AWS compliance and security documents, including compliance reports and certifications. These documents can be accessed on-demand and are available for self-service download.


---


Q502. A company runs a legacy workload in an on-premises data center. The company wants to migrate the workload to AWS. The company does not want to make any changes to the workload. Which migration strategy should the company use?

- A. Repurchase
- B. Replatform
- [x] C. Rehost
- D. Refactor


---

> [!IMPORTANT]
> Q503. A company is planning to migrate applications to the AWS Cloud. During a system audit, the company finds that its content management system (CMS) application is incompatible with cloud environments. Which migration strategies will help the company to migrate the CMS application with the LEAST effort? (Choose two.)

- A. Retire
- B. Rehost
- [x] C. Repurchase  
- [x] D. Replatform
- E. Refactor

C. Repurchase (Drop and Shop):

Replace the incompatible CMS with a cloud-native SaaS solution (e.g., migrating to Drupal, WordPress VIP, or Adobe Experience Manager)  

Effort reduction:

Eliminates code/architecture changes; the vendor handles migration, maintenance, and updates.

Avoids compatibility issues since SaaS platforms are pre-optimized for the cloud  

Use Case: Ideal when business needs align with off-the-shelf SaaS CMS offerings.

D. Replatform (Lift, Tinker, and Shift):

Minor optimizations to make the CMS cloud-compatible without core changes (e.g., moving databases to Amazon RDS, replacing WebLogic with Tomcat, or containerizing the app)  

Effort reduction:

Uses automated tools (e.g., AWS Application Migration Service) for server replication.

Retains the existing CMS while leveraging managed services to reduce operational overhead  

Use Case: Suitable when retaining the CMS is necessary but minimal adjustments are needed for cloud compatibility.

A. Retire	❌ Not applicable	Eliminates the CMS rather than migrating it  
B. Rehost	❌ High risk	CMS is incompatible with cloud environments; "lift-and-shift" may fail or require unexpected fixes  
E. Refactor	❌ Maximum effort	Requires full re-architecture (e.g., monolithic to microservices), which is costly and time-intensive

B. Rehost (lift and shift): The rehost strategy involves moving the application to the cloud without making significant modifications to the application architecture or code. It aims to replicate the existing infrastructure and application environment as closely as possible. This approach allows for a relatively quick migration process and requires minimal changes to the application. By rehosting the CMS application, the company can migrate it to AWS without needing to address the compatibility issues directly.
C. Repurchase: The repurchase strategy involves replacing the existing application with a different commercial off-the-shelf (COTS) software or a different vendor's solution. In this case, the company can consider replacing the incompatible CMS application with a cloud-compatible CMS solution. By adopting a different CMS application that is compatible with cloud environments, the company can migrate to AWS without having to resolve the compatibility issues in the existing application.


A. Retire: The retire strategy involves decommissioning or retiring applications that are no longer needed. It does not address the issue of migrating the incompatible CMS application to the AWS Cloud.
D. Replatform: The replatform strategy involves making some modifications to the application or infrastructure to take advantage of specific cloud-native features or services. While it can help address compatibility issues, it may require more effort compared to the rehost strategy, as it involves modifying the application to make it compatible with the cloud environment.
E. Refactor: The refactor strategy involves making significant changes to the application's architecture or code to optimize it for the cloud environment. This strategy requires substantial effort and is more suitable when there is a need to modernize or optimize the CMS application for the cloud, rather than simply addressing compatibility issues.
Therefore, the migration strategies that will help the company migrate the CMS application with the least effort in this scenario are B. Rehost and C. Repurchase.

---


Q504. Which of the following are AWS best practice recommendations for the use of AWS Identity and Access Management (IAM)? (Choose two.)

- A. Use the AWS account root user for daily access.
- B. Use access keys and secret access keys on Amazon EC2.
- [x] C. Rotate credentials on a regular basis.
- D. Create a shared set of access keys for system administrators.
- [x] E. Configure multi-factor authentication (MFA).


---

Q505. Which option is AWS responsible for under the AWS shared responsibility model?

- A. Network and firewall configuration
- B. Client-side data encryption
- C. Management of user permissions
- [x] D. Hardware and infrastructure

---


Q506. A company wants to run a graph query that provides credit card users' names, addresses, and transactions. The company wants the graph to show if the names, addresses, and transactions indicate possible fraud. Which AWS database service will meet these requirements?

- A. Amazon DocumentDB (with MongoDB compatibility)
- B. Amazon Timestream
- C. Amazon DynamoDB
- [x] D. Amazon Neptune


---

Q507. Which AWS service provides machine learning capability to detect and analyze content in images and videos?

- A. Amazon Connect
- B. Amazon Lightsail
- C. Amazon Personalize
- [x] D. Amazon Rekognition

---

> [!IMPORTANT]
> Q508. A company wants its AWS usage to be more sustainable. The company wants to track, measure, review, and forecast polluting emissions that result from its AWS applications. Which AWS service or tool can the company use to meet these requirements?

- A. AWS Health Dashboard
- [x] B. AWS customer carbon footprint tool
- C. AWS Support Center
- D. Amazon QuickSight


https://us-east-1.console.aws.amazon.com/costmanagement/home?region=us-east-1#/customer-carbon-footprint-tool


The CCFT provides estimated emissions for the full range of AWS products and the carbon estimates are provided in metric tons of carbon dioxide-equivalent (MTCO2e).


The AWS customer carbon footprint tool is a service provided by AWS that allows customers to measure and analyze the carbon emissions associated with their AWS usage. It provides insights into the environmental impact of running workloads and helps customers understand their carbon footprint.
By using the AWS customer carbon footprint tool, the company can monitor and track the emissions resulting from its AWS applications. It provides data on energy consumption and carbon emissions associated with various AWS services, regions, and usage patterns. This information can be used for reporting, analysis, and making informed decisions to optimize resource usage and reduce environmental impact.
The other options mentioned are not directly related to tracking and measuring polluting emissions:
A. AWS Health Dashboard: The AWS Health Dashboard provides status and notifications regarding the AWS services' operational health. It focuses on service disruptions, outages, and other service-related issues, rather than carbon emissions tracking.
C. AWS Support Center: The AWS Support Center is a portal for AWS customers to access support and technical assistance. While it can help with general inquiries and support requests, it does not specifically address tracking or measuring polluting emissions.
D. Amazon QuickSight: Amazon QuickSight is a business intelligence tool that enables users to create visualizations, dashboards, and perform data analysis. While it can help with data visualization and analysis, it does not provide specific capabilities for tracking or measuring polluting emissions.
Therefore, the correct AWS service or tool that the company can use to track, measure, review, and forecast polluting emissions resulting from its AWS applications is B. AWS customer carbon footprint tool.

---


Q509. Which AWS service gives users the ability to deploy highly repeatable infrastructure configurations?

- [x] A. AWS CloudFormation
- B. AWS CodeDeploy
- C. AWS CodeBuild
- D. AWS Systems Manager


AWS CloudFormation is a service that helps automate the deployment and management of AWS resources. It allows users to define infrastructure as code using JSON or YAML templates, which describe the desired state of the resources. These templates can be version-controlled, shared, and reused, providing a highly repeatable and consistent way to deploy infrastructure configurations.
With AWS CloudFormation, users can define a stack, which represents a collection of AWS resources, and then create or update the stack based on the template. CloudFormation takes care of provisioning and configuring the resources in the specified order and handles any dependencies between them.
By using CloudFormation, users can easily replicate and deploy infrastructure configurations across different environments, regions, or accounts. This enables consistent and reliable infrastructure deployments, reduces manual setup and configuration, and helps maintain infrastructure as code practices.
The other options mentioned are not specifically focused on infrastructure deployment:
B. AWS CodeDeploy: AWS CodeDeploy is a service that automates application deployments to various compute instances, including EC2 instances, on-premises servers, and Lambda functions. It is primarily used for deploying application code, not infrastructure configurations.
C. AWS CodeBuild: AWS CodeBuild is a fully managed build service that compiles source code, runs tests, and produces software packages. It is focused on the build and test phase of the software development lifecycle, rather than infrastructure deployment.
D. AWS Systems Manager: AWS Systems Manager provides a unified interface for managing and operating AWS resources. It offers various capabilities, including configuration management, patch management, and automation. While it can assist with managing infrastructure configurations, it does not specifically provide the ability to deploy highly repeatable infrastructure configurations like CloudFormation.

---


Q510. A company needs to provide customer service by using voice calls and web chat features. Which AWS service should the company use to meet these requirements?

- A. Amazon Aurora
- [x] B. Amazon Connect
- C. Amazon WorkSpaces
- D. AWS Organizations


---

Q511. Which AWS service is designed to help users handle large amounts of data in a data warehouse environment?

- A. Amazon RDS
- B. Amazon DynamoDB
- [x] C. Amazon Redshift
- D. Amazon Aurora


---

Q512. A company is building a web application using AWS. Which AWS service will help prevent network layer DDoS attacks against the web application?

- A. AWS WAF
- B. AWS Firewall Manager
- C. Amazon GuardDuty
- [x] D. AWS Shield


--- 

Q513. Which AWS compute service gives users the ability to securely and reliably run containers at scale?

- [x] A. Amazon Elastic Container Service (Amazon ECS)
- B. Amazon Aurora
- C. Amazon Athena
- D. Amazon Polly


---

Q514. Which AWS tool or feature acts as a VPC firewall at the subnet level?

- A. Security group
- [x] B. Network ACL
- C. Traffic Mirroring
- D. Internet gateway


---

Q515. A company runs an application on AWS that performs batch jobs. The application is fault-tolerant and can handle interruptions. The company wants to optimize the cost to run the application.
Which AWS offering will meet these requirements?

- A. Amazon Macie
- B. Amazon Neptune
- [x] C. Amazon EC2 Spot Instances
- D. Amazon EC2 On-Demand Instances

---


Q516. Which AWS service can be used to send alerts when a specific Amazon CloudWatch alarm is invoked?

- A. AWS CloudTrail
- [x] B. Amazon Simple Notification Service (Amazon SNS)
- C. Amazon Simple Queue Service (Amazon SQS)
- D. Amazon EventBridge

https://github.com/justinjiajia/certifications/blob/main/aws/cloud_security/labs/lab6.md

--- 

Q517. A cloud practitioner wants to use a highly available and scalable DNS service for its AWS workload. Which AWS service will meet this requirement?

- [x] A. Amazon Route 53
- B. Amazon Lightsail
- C. AWS Amplify Hosting
- D. Amazon S3

---

Q518. According to the AWS shared responsibility model, which task is the customer's responsibility?

- A. Maintaining the infrastructure needed to run AWS Lambda
- B. Updating the operating system of Amazon DynamoDB instances
- C. Maintaining Amazon S3 infrastructure
- [x] D. Updating the guest operating system on Amazon EC2 instances

---

Q519. A company is learning about its responsibilities that are related to the management of Amazon EC2 instances. Which tasks for EC2 instances are the company's responsibility, according to the AWS shared responsibility model? (Choose two.)

- A. Install and patch the machine hypervisor.
- [x] B. Patch the guest operating system.
- [x] C. Encrypt data at rest on associated storage.
- D. Install the physical hardware and cabling.
- E. Provide physical security for the EC2 instances.

---

> [!IMPORTANT]
> Q520. A company runs MySQL database workloads on self-managed servers in an on-premises data center. The company wants to migrate the database workloads to an AWS managed service. Which migration strategy should the company use?

- A. Rehost
- B. Repurchase
- C. Refactor
- [x] D. Replatform

---

Q521. A company is planning to migrate a monolithic application to AWS. The company wants to modernize the application by splitting it into microservices. The company will deploy the microservices on AWS. Which migration strategy should the company use?

- A. Rehost
- B. Repurchase
- C. Replatform
- [x] D. Refactor


---

Q522. A company wants to implement detailed tracking of its cloud costs by department and project. Which AWS feature or service should the company use?

- A. Consolidated billing
- [x] B. Cost allocation tags
- C. AWS Marketplace
- D. AWS Budgets


---

> [!IMPORTANT]
> Q523. A user wants to invoke an AWS Lambda function when an Amazon EC2 instance enters the stopping state. Which AWS service is appropriate for this use case?

- [x] A. Amazon EventBridge
- B. AWS Config
- C. Amazon Simple Notification Service (Amazon SNS)
- D. AWS CloudFormation

https://github.com/justinjiajia/certifications/blob/main/aws/cloud_practitioner/labs/activity_AWS_Lambda.md


Amazon EventBridge is an event bus service provided by AWS that enables event-driven architectures. It allows you to route events from various AWS services, such as EC2, to event targets like AWS Lambda functions.
To achieve the desired functionality, you can configure an EventBridge rule that triggers when a specific event occurs, in this case, when an EC2 instance enters the stopping state. The EC2 service emits events related to the lifecycle of instances, including state changes.
By creating an EventBridge rule with the appropriate event pattern, you can specify the condition for triggering the rule, which in this case would be an EC2 instance entering the stopping state. As the target of the rule, you can specify the AWS Lambda function that you want to invoke when the event occurs.
When an EC2 instance transitions to the stopping state, the event will be captured by the EventBridge rule, and the specified Lambda function will be invoked. This allows you to perform custom actions or execute code based on the occurrence of the event.
The other options mentioned are not the most appropriate for this specific use case:
B. AWS Config: AWS Config is a service that enables you to assess, audit, and evaluate the configurations of your AWS resources. While it can provide information about the state of EC2 instances, it does not provide the capability to trigger a Lambda function based on state transitions.
C. Amazon Simple Notification Service (Amazon SNS): Amazon SNS is a messaging service that enables pub/sub messaging patterns and can send notifications to various endpoints. However, it is not directly designed to trigger Lambda functions based on EC2 instance state changes.
D. AWS CloudFormation: AWS CloudFormation is a service that provides infrastructure as code capabilities for provisioning and managing AWS resources. While it can be used to define and deploy resources, it does not have built-in capabilities for triggering Lambda functions based on EC2 instance state changes.
Therefore, for the given use case, the appropriate AWS service is A. Amazon EventBridge.

---

Q524. A company has a MariaDB database on premises. The company wants to move the data to the AWS Cloud. Which AWS service will host this database with the LEAST amount of operational overhead?

- [x] A. Amazon RDS

- B. Amazon Neptune

- C. Amazon S3

- D. Amazon DynamoDB


---


Q525. Which AWS service or feature supports governance, compliance, and risk auditing of AWS accounts?

- A. Multi-factor authentication (MFA)
- B. AWS Lambda
- C. Amazon Simple Notification Service (Amazon SNS)
- [x] D. AWS CloudTrail

---

Q526. Which AWS Cloud design principle is a company using when the company implements AWS CloudTrail?

- [x] A. Activate traceability. (Security design principles)
- B. Use serverless compute architectures. (Performance efficiency design principles)
- C. Perform operations as code. (Operational excellence design principles )
- D. Go global in minutes. (Performance efficiency design principles)


---

Q527. A company needs a threat detection service that will continuously monitor its AWS accounts, workloads, and Amazon S3 buckets for malicious activity and unauthorized behavior. Which AWS service meets these requirements?

- A. AWS Shield
- B. AWS Firewall Manager
- [x] C. Amazon GuardDuty
- D. Amazon Inspector

---


> [!IMPORTANT]
> Q528. A company is planning to migrate to the AWS Cloud. The company is conducting organizational transformation and wants to become more responsive to customer inquiries and feedback. Which task should the company perform to meet these requirements, according to the AWS Cloud Adoption Framework (AWS CAF)?

- [x] A. Realign teams to focus on products and value streams.
- B. Create new value propositions with new products and services.
- C. Use a new data and analytics platform to create actionable insights.
- D. Migrate and modernize legacy infrastructure.

---

Q529. Which AWS service can create a private network connection from on premises to the AWS Cloud?

- A. AWS Config
- B. Virtual Private Cloud (Amazon VPC)
- [x] C. AWS Direct Connect
- D. Amazon Route 53

---

Q530. What is the recommended use case for Amazon EC2 On-Demand Instances?

- A. A steady-state workload that requires a particular EC2 instance configuration for a long period of time
- B. A workload that can be interrupted for a project that requires the lowest possible cost
- [x] C. An unpredictable workload that does not require a long-term commitment
- D. A workload that is expected to run for longer than 1 year


---


Q531. A company that operates on-premises servers decides to start a new line of business. The company determines that additional servers are required for the new workloads. Which advantage of cloud computing can helps the company to provision additional infrastructure as quickly as possible?

- A. Benefit from massive economies of scale  
- [x] B. Increase speed and agility  
- C. Trade fixed expense for variable expense  
- D. Go global in minutes  

---

Q532. A company wants to continuously improve processes and procedures to deliver business value. Which pillar of the AWS Well-Architected Framework does this goal represent?

- A. Performance efficiency  
- [x] B. Operational excellence  
- C. Reliability  
- D. Sustainability  

> Operational Excellence: The operational excellence pillar focuses on running and monitoring systems, and continually improving processes and procedures.
---

Q533. A company wants to migrate its on-premises SQL Server database to the AWS Cloud. The company wants AWS to handle the day-to-day administration of the database. Which AWS service will meet the company's requirements?

- A. Amazon EC2 for Microsoft SQL Server  
- B. Amazon DynamoDB  
- [x] C. Amazon RDS  
- D. Amazon Aurora  

> Amazon Aurora is a MySQL- and PostgreSQL-compatible relational database, not SQL Server-compatible.
 
---

Q534. A company wants to provide low latency to its users around the world. Which feature of the AWS Cloud meet this requirement?

- [x] A. Global infrastructure  
- B. Pay as-you-go pricing  
- C. Managed services  
- D. Economy of scale  

---

Q535. An online retail company wants to migrate its on-premises workload to AWS. The company needs to automatically handle a seasonal workload increase in a cost effective manner. Which AWS Cloud features will help the company meet this requirement? (Select TWO.)

- A. Cross-Region workload deployment  
- [x] B. Pay-as-you-go pricing  
- C. Built-in AWS CloudTrail audit capabilities  
- [x] D. Auto Scaling policies  
- E. Centralized logging  

> seasonal in a cost effective way

---

Q536. What is a benefit of using an Elastic Load Balancing (ELB) load balancer with applications running in the AWS Cloud?

- A. An ELB will automatically scale resources to meet capacity needs  
- [x] B. An ELB can balance traffic across multiple compute resources  
- C. An ELB can span multiple AWS Regions  
- D. An ELB can balance traffic between multiple internet gateways  

---

> [!IMPORTANT]
> Q537. What is the total volume of data that can be stored in Amazon S3?

- A. 10 PB  
- B. 50 PB  
- C. 100 PB  
- [x] D. Virtually unlimited  

---

Q538. A company wants the ability to automatically acquire resources as needed and release the resources when they are no longer needed.  Which cloud concept describes this functionality?

- A. Availability  
- [x] B. Elasticity  
- C. Durability  
- D. Reliability  

---

Q539. A company is migrating to the AWS Cloud instead of running its infrastructure on premises. Which of the following are advantages of this migration? (Select TWO.)

- A. Elimination of the need to perform security auditing  
- [x] B. Increased global reach and agility  
- [x] C. Ability to deploy globally in minutes  
- D. Elimination of the cost of IT staff members  
- E. Redundancy by default for all compute services  

---

Q540. A company needs to run some of its workloads on premises to comply with regulatory guidelines. The company wants to use the AWS Cloud to run workloads that are not required to be on premises. The company also wants to be able to use the same API calls for the on-premises workloads and the cloud workloads.  Which AWS service or feature should the company use to meet these requirements?

- A. Dedicated Hosts  
- [x] B. AWS Outposts  
- C. Availability Zones  
- D. AWS Wavelength  

---


Q541. A company wants to organize its users so that the company can grant permissions to the users as a group. Which AWS service or tool can the company use to meet this requirement?

- A. Security groups  
- [x] B. AWS Identity and Access Management (IAM)  
- C. Resource groups  
- D. AWS Security Hub  

---

Q542. A company has a workload that will run continuously for 1 year. The workload cannot tolerate service interruptions. Which Amazon EC2 purchasing option will be MOST cost-effective?

- [x] A. All Upfront Reserved Instances  
- B. Partial Upfront Reserved Instances  
- C. Dedicated Instances  
- D. On-Demand Instances  

---

Q543. A company wants to explore and analyze data in Amazon S3 by using a programming language. Which AWS service will meet these requirements?

- A. Amazon Kendra  
- B. Amazon Athena  
- C. Amazon Comprehend  
- [x] D. Amazon SageMaker  

 Amazon Athena	SQL-only queries (no Python/R support); not designed for iterative analysis.
 SQL is not a programming language

 
---

Q544. A company wants to reduce the amount of file storage the company maintains on premises. The company wants a new storage solution that will connect the on-premises storage to cloud-based storage. Which AWS storage option will meet these requirements?

- A. Amazon Elastic Block Store (Amazon EBS)  
- B. Amazon S3 Intelligent-Tiering  
- C. Amazon S3 Glacier Instant Retrieval  
- [x] D. AWS Storage Gateway  

---

Q545. A company wants to use an AWS networking solution that can act as a centralized gateway between multiple VPCs and on-premises networks. Which AWS service or feature will meet this requirement?

- A. Gateway VPC endpoint  
- B. AWS Direct Connect  
- [x] C. AWS Transit Gateway  
- D. AWS PrivateLink  

---

Q546. Which design principle aligns with performance efficiency pillar of the AWS Well-Architected Framework?

- [x] A. Using serverless architectures  
- B. Scaling horizontally  (reliability)
- C. Measuring the cost of workloads  (cost optimization)
- D. Using managed services  (sustainability)

---

Q547. Which AWS service is a fully managed NoSQL database service?

- A. Amazon RDS  
- B. Amazon Redshift  
- [x] C. Amazon DynamoDB  
- D. Amazon Aurora  

---

Q548. A company needs a managed NFS file system that the company can use with its AWS compute resources. Which AWS service or feature will meet these requirements?

- A. Amazon Elastic Block Store (Amazon EBS)  
- B. AWS Storage Gateway Tape Gateway  
- C. Amazon S3 Glacier Flexible Retrieval  
- [x] D. Amazon Elastic File System (Amazon EFS)  

keywords: NFS file system


---

Q549. A company wants to improve employee productivity by providing a way for employees to search for questions and retrieve specific answers. The company wants to use a single intelligent search interface. Which AWS service will meet these requirements?

- A. Amazon Connect  
- [x] B. Amazon Kendra  
- C. Amazon Lex  
- D. Amazon Comprehend  

---

> [!IMPORTANT]
> Q550. A company has developed a new in-house application. The company does not have a way to determine or predict the usage demand that the application will create. Which AWS Cloud computing benefit is the company seeking?

- A. Easy to use  
- B. Cost-effective  
- C. Secure  
- [x] D. Scalable and high performance  

---

Q551. Which Amazon EC2 Reserved Instances term commitment will give users the MOST cost savings?

- A. 1 year  
- B. 2 years  
- [x] C. 3 years  
- D. 5 years  

---

> [!IMPORTANT]
> Q552. A company's cloud environment includes Amazon EC2 instances and Application Load Balancers. The company wants to improve protections for its cloud resources against DDoS attacks. The company also wants to have real-time visibility into any DDoS attacks.  Which AWS service will meet these requirements?

- A. AWS Shield Standard  
- B. AWS Firewall Manager  
- [x] C. AWS Shield Advanced  
- D. Amazon GuardDuty  

---

Q553. A company wants to develop an accessibility application that will convert text into audible speech.   Which AWS service will meet this requirement?

- A. Amazon MQ  
- [x] B. Amazon Polly  
- C. Amazon Neptune  
- D. Amazon Timestream for LiveAnalytics  

---

> [!IMPORTANT]
> Q554. Which programming languages does AWS Cloud Development Kit (AWS CDK) (currently) support?

- [x] A. Python  
- B. Swift  
- [x] C. TypeScript  
- D. Ruby  
- E. PHP  

supported languages: Python; TypeScript; JavaScript; Java; C#; Go

---

Q555. Which AWS service should a company use to organize, characterize, and search large numbers of images?

- A. Amazon Transcribe  
- [x] B. Amazon Rekognition  
- C. Amazon Aurora  
- D. Amazon QuickSight  

---

> [!IMPORTANT]
> Q556. A company migrated its systems to the AWS Cloud. The systems are rightsized and a security review did not reveal any issues. The company must ensure that additional developments, integrations, changes, and system usage growth do not jeopardize this optimized AWS infrastructure. Which AWS service should the company use to report ongoing optimization and security?

- [x] A. AWS Trusted Advisor  
- B. AWS Health Dashboard  
- C. Amazon Connect  
- D. AWS Systems Manager  

> AWS Systems Manager:	Automates ops tasks (patching, state management) but lacks optimization/security checks.

> AWS Health Dashboard:	Tracks AWS service disruptions (not customer resource optimization/security).


---

> [!IMPORTANT]
> Q557. A company wants to securely access an Amazon S3 bucket from an Amazon EC2 instance without accessing the internet. What should the company use to accomplish this goal?

- A. VPN connection  
- B. Internet gateway  
- [x] C. VPC endpoint  
- D. NAT gateway  

---

Q558. A company wants a cost-effective option when running its applications in an Amazon EC2 instance for short time periods. The applications can be interrupted. Which EC2 instance type will meet these requirements?

- [x] A. Spot Instances  
- B. On-Demand Instances  
- C. Reserved Instances  
- D. Dedicated Instances  

---

> [!IMPORTANT]
> Q559. A company is planning to deploy a gaming application on AWS. Users from around the world will access the application. Which AWS service can help the company efficiently deliver the application to global users?

- [x] A. Amazon CloudFront  
- B. Amazon Cognito  
- C. Amazon VPC Lattice  
- D. Amazon Connect  

---

Q560. A developer needs to use a standardized template to create copies of a company's AWS architecture for development, test, and production environments. Which AWS service should the developer use to meet this requirement?

- A. AWS Cloud Map  
- [x] B. AWS CloudFormation  
- C. Amazon CloudFront  
- D. AWS CloudTrail  

can author CloudFormation templates in JSON or YAML formats.

---

> [!IMPORTANT]
> Q561. A company wants to connect its supported AWS services and VPCs. The company does not want to expose its internal traffic to the public internet. Which AWS service will meet these requirements?

- A. Amazon Inspector  
- [x] B. AWS PrivateLink  
- C. Amazon Connect  
- D. AWS Internet Gateway  

---

Q562. A company is designing workloads in the AWS Cloud. The company wants the workloads to perform their intended function correctly and consistently throughout their lifecycle. Which pillar of the AWS Well-Architected Framework does this goal represent?

- A. Operational excellence  (run and monitor systems; continually improve processes and procedures)
- B. Security  (proect information and systems)
- [x] C. Reliability  (perform intended functions and how to quickly recover from failures to meat demands)
- D. Performance efficiency  (structured and streamlined allocation of IT and compute resources)

---

Q563. A company needs to convert video files and audio files to a format that will play on smartphones. Which AWS service will meet this requirement?

- A. Amazon Comprehend  
- B. Amazon Rekognition  
- [x] C. Amazon Elastic Transcoder  
- D. Amazon Polly  
 
Amazon Elastic Transcoder is a media transcoding service provided by AWS. It allows you to convert media files from one format to another, making them compatible with various devices and platforms. It supports video and audio transcoding, including format conversion, bitrate adjustment, resolution changes, and more.
By using Amazon Elastic Transcoder, the company can specify the desired output format and settings for the video and audio files. The service will then transcode the files accordingly, generating versions that are optimized for playback on smartphones and other devices. This includes ensuring compatibility with popular video and audio codecs supported by smartphones.
Amazon Comprehend (option A) is a natural language processing (NLP) service used for text analysis and understanding. It is not related to video and audio transcoding.
Amazon Rekognition (option B) is a computer vision service used for image and video analysis, including object recognition, facial analysis, and scene detection. It is not designed for video and audio transcoding. Amazon Polly (option D) is a text-to-speech (TTS) service that converts text into lifelike speech. It is not intended for video and audio transcoding.
 


---

Q564. Which AWS service or tool provides users with a graphical interface that they can use to manage AWS services?

- A. AWS Copilot  
- B. AWS CLI  
- [x] C. AWS Management Console  
- D. AWS software development kits (SDKs)
  
---

> [!IMPORTANT]
> Q565. Which AWS service or tool provides a visualization of historical AWS spending patterns and projections of future AWS costs?

- A. AWS Cost and Usage Report  
- B. AWS Budgets  
- [x] C. Cost Explorer  
- D. Amazon CloudWatch  

Cost Explorer is a feature within the AWS Management Console that provides comprehensive insights into AWS costs and usage. It allows users to visualize and analyze their AWS spending patterns over time, as well as forecast future costs.
With Cost Explorer, users can view and analyze their AWS cost and usage data using various pre-built reports and customizable filters. It offers detailed breakdowns of costs by service, region, instance type, and other dimensions to help users understand their cost drivers. Users can also explore historical data, compare trends, and identify cost-saving opportunities.
Additionally, Cost Explorer provides forecasting capabilities to estimate future AWS costs based on historical data. It enables users to project their expected spending and budget accordingly.
AWS Cost and Usage Report (option A) is a detailed report that provides comprehensive cost and usage data in a machine-readable format. While it offers detailed data for analysis, it does not provide visualizations or cost projections like Cost Explorer.
AWS Budgets (option B) is a service that allows users to set budget thresholds and receive alerts when the actual costs exceed those thresholds. While it helps with cost monitoring, it does not provide visualizations of spending patterns or cost projections.
Amazon CloudWatch (option D) is a monitoring service that provides real-time insights into various AWS resources and applications. It includes metrics, logs, and alarms for monitoring purposes but does not offer specific features for visualizing historical spending patterns or projecting future costs.


---

Q566. Which AWS services are serverless? (Select TWO.)

- [x] A. AWS Fargate  
- B. Amazon Managed Streaming for Apache Kafka  
- C. Amazon EMR  
- [x] D. Amazon S3  
- E. Amazon EC2  

---

Q567. Which AWS service uses edge locations to cache content?

- A. Amazon Kinesis  
- B. Amazon Simple Queue Service (Amazon SQS)  
- [x] C. Amazon CloudFront  
- D. Amazon Route 53  

---

Q568. Which AWS services or features form the AWS Cloud global infrastructure? (Select TWO.)

- [x] A. Availability Zones  
- B. Amazon ElastiCache  
- [x] C. AWS Regions  
- D. Amazon S3  
- E. Amazon VPC  

---

Q569. A company wants to centrally manage its employees' access to multiple AWS accounts. Which AWS service or feature should the company use to meet this requirement?

- A. AWS Identity and Access Management Access Analyzer  
- B. AWS Secrets Manager  
- [x] C. AWS IAM Identity Center  
- D. AWS Security Token Service (AWS STS)  


AWS IAM Identity Center is the AWS solution for connecting your workforce users to AWS managed applications such as Amazon Q Developer and Amazon QuickSight, and other AWS resources. You can connect your existing identity provider and synchronize users and groups from your directory, or create and manage your users directly in IAM Identity Center. You can then use IAM Identity Center for either or both of the following:

- User access to applications
- User access to AWS accounts


---


Q570. A company has an on-premises application. The application has processing times of less than 5 minutes and is invoked only a few times each day. The company wants to move the application to the AWS Cloud. Which AWS service will support this application MOST cost-effectively?

- A. Amazon Elastic Container Service (Amazon ECS)  
- [x] B. AWS Lambda  
- C. Amazon Elastic Kubernetes Service (Amazon EKS)  
- D. Amazon EC2  

---

Q571. A company runs an uninterruptible Amazon EC2 workload on AWS 24 hours a day, 7 days a week. The company will require the same instance family and instance type to run the workload for the next 12 months. Which combination of purchasing options should the company choose to MOST optimize costs? (Select TWO.)

- [x] A. Standard Reserved Instance  
- B. Convertible Reserved Instance  
- C. Compute Savings Plan  
- D. Spot Instance  
- [x] E. All Upfront payment  


> pricing comparison

> https://aws.amazon.com/savingsplans/compute-pricing/

> https://aws.amazon.com/ec2/pricing/reserved-instances/pricing/

---

> [!IMPORTANT]
> Q572. An independent software vendor wants to deliver and share its custom Amazon Machine Images (AMIs) to prospective customers.  Which AWS service will meet these requirements?

- [x] A. AWS Marketplace  
- B. AWS Data Exchange  
- C. Amazon EC2  
- D. AWS Organizations  

> You can create an AMI from your Amazon EC2 instances and then use it to launch instances with the same configuration. You can copy an AMI to another AWS Region, and then use it to launch instances in that Region. You can also share an AMI that you created with other accounts so that they can launch instances with the same configuration.
> You can sell your AMI using the AWS Marketplace.

---

Q573. A company wants to migrate all of its on-premises infrastructure to the AWS Cloud. Before migration, the company wants estimate of costs for running its as-is infrastructure. Which AWS service or principle should the company use to meet this requirement?

- [x] A. AWS Pricing Calculator  
- B. AWS Well-Architected Framework  
- C. AWS shared responsibility model  
- D. AWS Cloud Adoption Framework (AWS CAF)  

---


Q574. Which of the following can the AWS Pricing Calculator do?

- [x] A. Project monthly AWS costs  
- B. Calculate historical AWS costs  
- C. Provide in-depth information about AWS pricing strategies  
- D. Provide users with access to their monthly bills  

---

Q575. A company wants to maintain bandwidth throughput and provide a more consistent network experience than public internet-based connections. Which AWS service should the company choose?

- A. AWS VPN  
- [x] B. AWS Direct Connect  
- C. Amazon Connect  
- D. Amazon CloudFront  

---

Q576. A developer needs to interact with AWS by using the AWS CLI.  Which security feature or AWS service must be provisioned in the developer's account to meet this requirement?

- A. User name and password  
- B. AWS Systems Manager  
- C. Root password access  
- [x] D. AWS access key  

---

Q577. Which AWS service provides DNS resolution?

- A. Amazon CloudFront  
- B. Amazon VPC  
- [x] C. Amazon Route 53  
- D. AWS Direct Connect  

---

Q578. A company needs to deploy a PostgreSQL database into Amazon RDS. The database must be highly available and fault tolerant.  Which AWS solution should the company use to meet these requirements?

- A. Amazon RDS with a single Availability Zone  
- B. Amazon RDS snapshots  
- [x] C. Amazon RDS with multiple Availability Zones  
- D. AWS Database Migration Service (AWS DMS)  

https://github.com/justinjiajia/certifications/tree/main/aws/service_img_demo/aurora_rds

---

> [!IMPORTANT]
> Q579. A company is building an application that will receive millions of database queries each second. The company needs the data store for the application to scale to meet these needs.  Which AWS service will meet this requirement?

- [x] A. Amazon DynamoDB  
- B. AWS Cloud9  
- C. Amazon ElastiCache for Memcached  
- D. Amazon Neptune  

Amazon DynamoDB is a fully managed serverless NoSQL database service. DynamoDB stores data in tables. Tables hold items. Items are composed of attributes.
Handles millions of requests/sec with single-digit millisecond latency, automatically partitioning data across servers as traffic grows.
On-demand mode instantly scales to 10M+ read/write requests per second.

 a key-value database that provides sub-millisecond latency on a large scale

---

Q580. Which component must be attached to a VPC to enable inbound internet access?

- A. NAT gateway  
- B. VPC endpoint  
- C. VPN connection  
- [x] D. Internet gateway  

> initiated from the Internet

---


Q581. A company is using multiple AWS accounts for different business teams. The finance team wants to receive one bill for all of the company's accounts. Which AWS service or tool should the finance team use to meet this requirement?

- [x] A. AWS Organizations  
- B. AWS Trusted Advisor  
- C. Cost Explorer  
- D. AWS Budgets  

---

Q582. Which tasks are the responsibility of AWS according to the AWS shared responsibility model? (Select TWO.)

- A. Configure AWS Identity and Access Management (IAM)  
- [x] B. Configure security groups on Amazon EC2 instances  
- C. Secure the access of physical AWS facilities  
- [x] D. Patch applications that run on Amazon EC2 instances  
- E. Perform infrastructure patching and maintenance  



 
---

Q583. Which AWS service supports a company's ability to treat infrastructure as code?

- A. AWS CodeDeploy  
- B. AWS Elastic Beanstalk  
- C. Amazon API Gateway  
- [x] D. AWS CloudFormation  

---



Q584. A company is using AWS Identity and Access Management (IAM). Who can manage the access keys of the AWS account root user?

- A. IAM users in the same account that have been granted permission  
- B. IAM roles in any account that have been granted permission  
- C. IAM users and roles that have been granted permission  
- [x] D. The AWS account owner  

---

Q585. A company needs to use SQL syntax to perform a direct query of objects in an Amazon S3 bucket. Which AWS service can the company use to meet this requirement?

- A. AWS Glue  
- [x] B. Amazon Athena  
- C. AWS Lambda  
- D. Amazon Kinesis  

---

Q586. A food delivery company needs to block users in certain countries from accessing its website. Which AWS service should the company use to meet this requirement?

- [x] A. AWS WAF  
- B. AWS Control Tower  
- C. Amazon Fraud Detector  
- D. Amazon Pinpoint  

---

Q587. An ecommerce company has been monitoring usage of its online store that is hosted on a fleet of Amazon EC2 instances. Surges in traffic occur every weekend day at the same time and last for approximately 4 hours. Which AWS service should the company use to ensure that there are enough instances to meet the surges in demand?

- A. AWS Lambda  
- B. Amazon EventBridge  
- C. Elastic Load Balancing (ELB)  
- [x] D. Amazon EC2 Auto Scaling  

---

> [!IMPORTANT]
> Q588. A company must archive its documents by using a write-once, read-many (WORM) model to meet legal and compliance obligations. Which feature of Amazon S3 can the company use to meet this requirement?

- A. S3 Versioning  
- B. S3 bucket policy  
- [x] C. S3 Glacier Vault Lock  
- D. S3 multi-factor authentication (MFA) delete  


The feature of Amazon S3 that enables a write-once, read-many (WORM) model to meet legal and compliance obligations is S3 Object Lock. However, this option is not listed among your choices. Among the provided options, the correct answer is:

C. S3 Glacier Vault Lock

Explanation:

S3 Glacier Vault Lock allows you to implement a WORM model for data archived in Amazon S3 Glacier. Once a Vault Lock policy is created and locked, it becomes immutable—ensuring that data cannot be changed or deleted, even by the root account. This is ideal for meeting strict compliance and legal data retention requirements.

S3 Object Lock (not listed as an option) is the direct S3 feature for WORM at the object level, but S3 Glacier Vault Lock provides similar WORM protection for data archived in S3 Glacier.

Other options:

A. S3 Versioning allows you to retain multiple versions of objects but does not enforce WORM.

B. S3 bucket policy controls access but does not provide immutability or WORM.

D. S3 multi-factor authentication (MFA) delete adds a layer of protection against accidental deletions but does not enforce WORM.


you first create a vault, complete a Vault Lock policy, and then upload the archives to the vault so the policy will be applied to them.

Locking a vault takes two steps. First, you must initiate a Vault Lock policy, which sets the lock to an in-progress state for 24 hours and returns a lock ID. After you've tested your policy to ensure that it works as intended, you then use the provided lock ID to complete the Vault Lock process. If you don't complete this process within 24 hours, S3 Glacier deletes the Vault Lock policy.



---

Q589. Which statements accurately describe the relationships among components of AWS global infrastructure? (Select TWO.)

- A. There are more AWS Regions than Availability Zones  
- [x] B. There are more edge locations than AWS Regions  
- C. An edge location is an Availability Zone  
- D. There are more AWS Regions than edge locations  
- [x] E. There are more Availability Zones than AWS Regions  

 
---

Q590. A company's application is running on Amazon EC2 instances. The company is planning a partial migration to a serverless architecture in the next year and wants to pay for resources up front.  Which AWS purchasing option will optimize the company's costs?

- A. Convertible Reserved Instances  
- B. Spot Instances  
- C. EC2 Instance Savings Plans  
- [x] D. Compute Savings Plan  


> Convertible RIs are designed specifically for Amazon EC2 instances and related compute resources, allowing you to exchange your reservation for different EC2 instance types, operating systems, or tenancies if your needs change.

> For partial serverless migrations, Compute Savings Plans uniquely balance upfront cost control, maximized discounts, and architectural flexibility. 

> pricing comparison

> https://aws.amazon.com/savingsplans/compute-pricing/

> https://aws.amazon.com/ec2/pricing/reserved-instances/pricing/

---

Q591. A company has batch workloads that need to run for short periods of time on Amazon EC2. The workloads can handle interruptions and can start again from where they ended.   What is the MOST cost-effective EC2 instance purchasing option to meet these requirements?

- A. Reserved Instances  
- [x] B. Spot Instances  
- C. Dedicated Instances  
- D. On-Demand Instances  

---

Q592. A company's compliance officer wants to review the AWS Service Organization Control (SOC) reports. Which AWS service or feature should the compliance officer use to complete this task?

- [x] A. AWS Artifact  
- B. AWS Concierge Support  
- C. AWS Support  
- D. AWS Trusted Advisor  

---

Q593. A company has data lakes designed for high performance computing (HPC) workloads.  Which Amazon EC2 instance type should the company use to meet these requirements?

- A. General purpose instances  
- [x] B. Compute optimized instances  
- C. Memory optimized instances  
- D. Storage optimized instances  

---

> [!IMPORTANT]
> Q594. Which AWS network services or features allow CIDR block notation when providing an IP address range? (Select TWO.)

- [x] A. Security groups  
- B. Amazon Machine Image (AMI)  
- [x] C. Network access control list (network ACL)  
- D. AWS Budgets  
- E. Amazon Elastic Block Store (Amazon EBS)  

---

Q595. A company has a compliance requirement to record and evaluate configuration changes, as well as perform remediation actions on AWS resources. Which AWS service should the company use?

- [x] A. AWS Config  
- B. AWS Secrets Manager  
- C. AWS CloudTrail  
- D. AWS Trusted Advisor  

---

Q596. A company's gaming application has been gaining popularity. There has been high demand for the gaming application in countries where the company does not currently deploy the application. Which advantage of the AWS Cloud can help the company to deploy the application to more countries around the world?

- A. Increase speed and agility  
- [x] B. Go global in minutes  
- C. Trade fixed expense for variable expense  
- D. Benefit from massive economies of scale  

---

Q597. A company needs to host a web server on Amazon EC2 instances for at least 1 year. The web server cannot tolerate interruption. Which EC2 instance purchasing option will meet these requirements MOST cost-effectively?

- A. On-Demand Instances  
- [x] B. Partial Upfront Reserved Instances  
- C. Spot Instances  
- D. No Upfront Reserved Instances  

---

Q598. Which task is the responsibility of AWS, according to the AWS shared responsibility model?

- A. Apply guest operating system patches to Amazon EC2 instances.  
- B. Provide monitoring of human resources information management (HRIM) systems.  
- [x] C. Perform automated backups of Amazon RDS instances.  
- D. Optimize the costs of running AWS services.  

---

Q599. What is a customer responsibility under the AWS shared responsibility model when using AWS Lambda?

- A. Maintenance of the underlying Lambda hardware  
- B. Maintenance of the Lambda networking infrastructure  
- [x] C. The code and libraries that run in the Lambda functions  
- D. The Lambda server software  

---

Q600. A systems administrator wants to monitor the CPU utilization of a company's Amazon EC2 instances.  Which AWS service can provide this information?

- A. AWS Config  
- B. AWS Trusted Advisor  
- C. AWS CloudTrail  
- [x] D. Amazon CloudWatch  

---
 

Q601. Which AWS service provides serverless compute for use with containers?  
- A. Amazon Simple Queue Service (Amazon SQS)  
- [x] B. AWS Fargate  
- C. AWS Elastic Beanstalk  
- D. Amazon SageMaker  

---

> [!IMPORTANT]
> Q602. A company needs to use AWS technology to deploy a static website. Which solution meets this requirement with the LEAST amount of operational overhead?  
- A. Deploy the website on Amazon EC2  
- B. Host the website on AWS Elastic Beanstalk  
- C. Deploy the website with Amazon Lightsail  
- [x] D. Host the website on Amazon S3  

---

Q603. What is the primary use case for Amazon GuardDuty?  
- A. Prevention of DDoS attacks  
- B. Protection against SQL injection attacks  
- [x] C. Automatic monitoring for threats to AWS workloads  
- D. Automatic provisioning of AWS resources  

---



Q604. A company wants to manage access and permissions for its third-party software as a service (SaaS) applications. The company wants to use a portal where end users can access assigned AWS accounts and AWS Cloud applications. Which AWS service should the company use to meet these requirements?  
- A. Amazon Cognito  
- [x] B. AWS IAM Identity Center  
- C. AWS Identity and Access Management (IAM)  
- D. AWS Directory Service for Microsoft Active Directory  

---

Q605. Which group shares responsibility with AWS for security and compliance of AWS accounts and resources?  
- A. Third-party vendors  
- [x] B. Customers  
- C. Reseller partners  
- D. Internet providers  

---

Q606. A company wants to deploy an application in multiple Availability Zones in a single AWS Region. Which benefit will this deployment provide to the company?  
- A. Improved connection performance for global customers  
- [x] B. Resilient architecture and a highly available solution  
- C. Reduced overall data storage costs  
- D. Ability to shut down an Availability Zone during periods of low demand  

---

Q607. Which VPC component can a company use to set up a virtual firewall at the Amazon EC2 instance level?  
- A. Network ACL  
- [x] B. Security group  
- C. Route table  
- D. NAT gateway  


---

Q608. A company needs an event history of which AWS resources the company has created. Which AWS service will provide this information?
- A. Amazon CloudWatch
- [x] B. AWS CloudTrail
- C. Amazon Aurora
- D. Amazon EventBridge
 
 
---

Q609. A company's employees are working from home. The company wants its employees to use their personal devices to connect to a managed workstation in the AWS Cloud. Which AWS service should the company use to provide the remote environment?
- [x] A. Amazon WorkSpaces
- B. AWS Cloud9
- C. AWS Outposts
- D. Amazon Lightsail

---

Q610. Which of the following actions are controlled with AWS Identity and Access Management (IAM)? (Select TWO.)
- [x] A. Control access to AWS service APIs and to other specific resources
- B. Provide intelligent threat detection and continuous monitoring
- [x] C. Protect the AWS environment using multi-factor authentication (MFA)
- D. Grant users access to AWS data centers
- E. Provide firewall protection for applications from common web attacks

---

> [!IMPORTANT]
> Q611. Which benefit is always free of charge with AWS, regardless of a user's AWS Support plan?
- A. AWS Developer Support
- [x] B. AWS Developer Forums
- C. Programmatic case management (available from the business support)
- D. AWS technical account manager (TAM) (available from the enterprise on-ramp support)

---

> [!IMPORTANT]
> Q612. A company wants to rightsize its Amazon EC2 instances. Which configuration change will meet this requirement with the LEAST operational overhead?
- A. Add EC2 instances in another Availability Zone.
- [x] B. Change the size and type of the EC2 instances based on utilization.
- C. Convert the payment method from On-Demand to Savings Plans.
- D. Reprovision the EC2 instances with a larger instance type.

---

Q613. Which AWS service supports user sign-up functionality and authentication to mobile and web applications?
- [x] A. Amazon Cognito
- B. AWS Config
- C. Amazon GuardDuty
- D. AWS Systems Manager

---

Q614. Which benefit of the AWS Cloud helps companies achieve lower usage costs because of the aggregate usage of all AWS users?
- A. No need to guess capacity
- B. Ability to go global in minutes
- [x] C. Economies of scale
- D. Increased speed and agility

---

Q615. Which task is the responsibility of the customer, according to the AWS shared responsibility model?
- A. Patch the Amazon DynamoDB operating system.
- B. Secure Amazon CloudFront edge locations by allowing physical access according to the principle of least privilege.
- C. Protect the hardware that runs AWS services.
- [x] D. Use AWS Identity and Access Management (IAM) according to the principle of least privilege.

---

> [!IMPORTANT]
> Q616. A company wants to manage its cloud resources by using infrastructure as code (IaC) templates. The company needs to meet compliance requirements. Which AWS service should the company use to meet these requirements?
- A. AWS Artifact
- B. AWS Resource Explorer
- C. AWS License Manager
- [x] D. AWS Service Catalog

---

Q617. An AWS user wants to proactively detect when an instance or account might be compromised or if there are threats from attacks. Which AWS service should the user choose?
- [x] A. Amazon GuardDuty
- B. AWS WAF
- C. AWS Shield
- D. Amazon Inspector


---

> [!IMPORTANT]
> Q618. Which AWS Support plan provides the full set of AWS Trusted Advisor checks at the LOWEST cost?
- A. AWS Developer Support
- [x] B. AWS Business Support
- C. AWS Enterprise On-Ramp Support
- D. AWS Enterprise Support


---

Q619. A retail company is building a new mobile app. The company is evaluating whether to build the app at an on-premises data center or in the AWS Cloud.  Which of the following are benefits of building this app in the AWS Cloud? (Choose two.)
- A. A large, upfront capital expense and low variable expenses
- [x] B. Increased speed for trying out new projects
- C. Complete control over the physical security of the infrastructure
- [x] D. Flexibility to scale up in minutes as the application becomes popular
- E. Ability to pick the specific data centers that will host the application servers

---

> [!IMPORTANT]
> Q620. What is the MOST secure way to store passwords on AWS?
- A. Store passwords in an Amazon S3 bucket.
- B. Store passwords as AWS CloudFormation parameters.
- C. Store passwords in AWS Storage Gateway.
- [x] D. Store passwords in AWS Secrets Manager.

---

Q621 is the same as Q589.

---

Q622. A company needs to host an application in a specific geographic area to comply with regulations. Which feature of the AWS global infrastructure will help the company meet this requirement?
- A. Scalability
- [x] B. Global footprint
- C. Availability
- D. Performance

---

Q623. An ecommerce company plans to move its data center workload to the AWS Cloud to support highly dynamic usage patterns. Which benefits make the AWS Cloud cost-effective for the migration of this type of workload? (Choose two.)
- A. Reliability
- B. Security
- [x] C. Elasticity
- [x] D. Pay-as-you-go resource
- E. High availability

> keywords: dynamic usage patterns and cost-effective

---

Q624. When designing AWS workloads to be operational even when there are component failures, what is an AWS best practice?
- A. Perform quarterly disaster recovery tests.
- B. Place the main component on the us-east-1 Region.
- [x] C. Design for automatic failover to healthy resources.
- D. Design workloads to fit on a single Amazon EC2 instance.

---

Q625. Which AWS solution gives companies the ability to use protocols such as NFS to store and retrieve objects in Amazon S3?
- A. Amazon FSx for Lustre
- B. AWS Storage Gateway volume gateway
- [x] C. AWS Storage Gateway file gateway
- D. Amazon Elastic File System (Amazon EFS)

> NFS (Network File System): a distributed file system protocol that allows users on different machines to access files and directories on a remote server as if they were local. 
---

> [!IMPORTANT]
> Q626. A user has been granted permission to change their own IAM user password.  Which AWS services can the user use to change the password? (Choose two.)
- [x] A. AWS Command Line Interface (AWS CLI)
- B. AWS Key Management Service (AWS KMS)
- [x] C. AWS Management Console
- D. AWS Resource Access Manager (AWS RAM)
- E. AWS Secrets Manager


> IAM users with the appropriate permissions can change their own password through the AWS Management Console by navigating to the "Security credentials" section and updating their password.

> Alternatively, users can use the AWS CLI command aws iam change-password to change their own password

> Other options listed (AWS KMS, AWS RAM, AWS Secrets Manager) do not provide functionality for changing IAM user passwords.
---


Q627. Which task is the customer's responsibility, according to the AWS shared responsibility model?
- [x] A. Patch a guest operating system that is deployed on an Amazon EC2 instance.
- B. Control physical access to an AWS data center.
- C. Control access to AWS underlying hardware.
- D. Patch a host operating system that is deployed on Amazon S3.

---

Q628. Which AWS service or feature provides a firewall at the subnet level within a VPC?
- A. Security group
- [x] B. Network ACL
- C. Elastic network interface
- D. AWS WAF

---

Q629. A company wants to use automated video analysis to identify employees that are accessing its offices. Which AWS service will meet this requirement?
- [x] A. Amazon Rekognition
- B. Amazon Polly
- C. Amazon Cognito
- D. AWS Lambda

---

> [!IMPORTANT]
> Q630. Which guidelines are best practices for using AWS Identity and Access Management (IAM)? (Choose two.)
- A. Share access keys.
- [x] B. Create individual IAM users.
- C. Use inline policies instead of customer managed policies.
- D. Grant maximum privileges to IAM users.
- [x] E. Use groups to assign permissions to IAM users.


B. Create individual IAM users.
Creating individual IAM users ensures that each user has their own credentials and permissions, which improves security and accountability. This is consistently recommended in AWS documentation and best practice guides.

E. Use groups to assign permissions to IAM users.
Assigning permissions to groups rather than individual users simplifies management and helps enforce consistent access policies. It is a widely recognized IAM best practice.

Why not the others?

A. Share access keys.
Sharing access keys is a security risk and is explicitly discouraged by AWS.

C. Use inline policies instead of customer managed policies.
Inline policies are harder to manage at scale and are not recommended for most scenarios; customer managed (or AWS managed) policies are preferred for centralized management.

D. Grant maximum privileges to IAM users.
This violates the principle of least privilege, which is a core security best practice for IAM

---

Q631. Which advantage of cloud computing allows users to scale resources up and down based on the amount of load that an application supports?
- A. Go global in minutes
- [x] B. Stop guessing capacity
- C. Benefit from massive economies of scale
- D. Trade fixed expense for variable expense

---

Q632. A company is requesting Payment Card Industry (PCI) reports that validate the operating effectiveness of AWS security controls. How should the company obtain these reports?
- A. Contact AWS Support.
- [x] B. Download reports from AWS Artifact.
- C. Download reports from AWS Security Hub.
- D. Contact an AWS technical account manager (TAM).

---

Q633. An ecommerce company wants to distribute traffic between the Amazon EC2 instances that host its website. Which AWS service or resource will meet these requirements?
- [x] A. Application Load Balancer
- B. AWS WAF
- C. AWS CloudHSM
- D. AWS Direct Connect

---

Q634. According to the AWS shared responsibility model, which of the following are AWS responsibilities? (Choose two.)
- [x] A. Network infrastructure and virtualization of infrastructure
- B. Security of application data
- C. Guest operating systems
- [x] D. Physical security of hardware
- E. Credentials and policies

---


> [!IMPORTANT]
> Q635. A company uses Amazon Aurora as its database service. The company wants to encrypt its databases and database backups. Which party manages the encryption of the database clusters and database snapshots, according to the AWS shared responsibility model?
- A. AWS
- [x] B. The company
- C. AWS Marketplace partners
- D. Third-party partners


<img width="726" alt="image" src="https://github.com/user-attachments/assets/99feabbc-12bb-4650-ac0f-de5257fa8ca7" />
Amazon Aurora (including serverless version): server-side encryption is optional


Question #: 544 
https://www.awslagi.com/course/aws-certified-cloud-practitioner-clf-c02-actual-exam/lessons/clf-c02-part-10/
 

---

> [!IMPORTANT]
> Q636. A company is hosting a web application on Amazon EC2 instances. The company wants to implement custom conditions to filter and control inbound web traffic. Which AWS service will meet these requirements?
- A. Amazon GuardDuty
- [x] B. AWS WAF
- C. Amazon Macie
- D. AWS Shield

---

Q637. A company has temporary workload that is also variable. The company needs to use Amazon EC2 instances for the workload. The EC2 instances need to handle short bursts of work that cannot stop before finishing. Which purchase option will meet these requirements?  
- A. Spot Instances  
- [x] B. On-Demand Instances  
- C. Savings Plan  
- D. Reserved Instances  

---

Q638. A company uses Amazon RDS for a product database. The company wants to ensure the database is highly available. Which feature of Amazon RDS will meet this requirement?  
- A. Read replicas  
- B. Blue/green deployment  
- [x] C. Multi-AZ deployment  
- D. Reserved Instances  

> One of the most powerful features of Amazon RDS is the ability to configure your database
instance for high availability with a Multi-AZ deployment. After a Multi-AZ deployment is
configured, Amazon RDS automatically generates a standby copy of the database instance in
another Availability Zone within the same VPC. After seeding the database copy, transactions are
synchronously replicated to the standby copy. Running a database instance in a Multi-AZ
deployment can enhance availability during planned system maintenance, and it can help protect your databases against database instance failure and Availability Zone disruption. 
---

Q639. A company needs a firewall that will control network connections to and from a single Amazon EC2 instance. This firewall will not control network connections to and from other instances that are in the same subnet. Which AWS service or feature can the company use to meet these requirements?  
- A. Network ACL  
- B. AWS WAF  
- C. Route table  
- [x] D. Security group  

---

Q640. A company is planning to use the Amazon EC2 instances as web servers. Customers from around the world will use the web servers. Most customers will use the web servers only during certain hours of the day. How should the company deploy the EC2 instances to achieve the LOWEST operational cost?  
- A. In multiple Availability Zones  
- [x] B. In an Auto Scaling group  
- C. In a placement group  
- D. In private subnets  

---

Q641. A company uses Amazon EC2 instances to run its application. The application needs to be available and running continuously for three or more years. What type of EC2 instance should the company purchase for a discount on the EC2 pricing?  
- [x] A. Reserved Instances  
- B. Spot Instances  
- C. On-Demand Instances  
- D. EC2 Fleet  

---

Q642. A company needs to perform an audit of recent AWS account activity. The audit will investigate who initiated an event and what actions were performed. Which AWS service should the company use to meet these requirements?  
- A. AWS Config  
- B. Amazon Rekognition  
- [x] C. AWS CloudTrail  
- D. Amazon Simple Notification Service (Amazon SNS)  

---

Q643. Which design principles are included in the reliability pillar of the AWS Well-Architected Framework? (Choose two.)  
- [x] A. Automatically recover from failure.  
- B. Grant everyone access to increase AWS service quotas.  
- [x] C. Stop guessing capacity.  
- D. Design applications to run in a single Availability Zone.  
- E. Plan to increase AWS service quotas first in a secondary AWS Region.  

---

> [!IMPORTANT]
> Q644. Which recommendation can AWS Cost Explorer provide to help reduce cost?  
- A. Use a specific database engine.  
- B. Change the programming language for an application.  
- C. Deploy a specific operating system.  
- [x] D. Terminate an idle instance.  

---

> [!IMPORTANT]
> Q645. Which AWS service can companies use to subscribe to RSS feeds for updates about all AWS service issues?  
- A. Amazon Simple Notification Service (Amazon SNS)  
- [x] B. AWS Health Dashboard  
- C. AWS Config  
- D. AWS CodeCommit  

AWS Health Dashboard allows viewing service health, events, interruptions, subscribing to RSS feeds, and account-specific events.
 
A. Amazon Simple Notification Service (Amazon SNS) is a messaging service that can be used to receive notifications, but it does not provide RSS feeds for AWS service issues.
C. AWS Config is a service that records the configurations of AWS resources, but it does not provide RSS feeds for AWS service issues.
D. AWS CodeCommit is a version control service and is not relevant for receiving updates about AWS service issues.
B. AWS Health Dashboard is the correct service that companies can use to subscribe to RSS feeds for updates about all AWS service issues.
The AWS Health Dashboard provides the following key features:
Real-time updates: The dashboard provides real-time information about ongoing AWS service events and disruptions.
RSS feeds: Companies can subscribe to RSS feeds to receive updates about AWS service issues, including descriptions, status, and projected resolution times.
Personalized views: The dashboard can be customized to show only the AWS services and Regions that are relevant to the company's infrastructure.
By subscribing to the RSS feeds provided by the AWS Health Dashboard, companies can stay informed about any AWS service issues that may impact their applications and infrastructure. This allows them to proactively plan and respond to potential disruptions. 


---


Q646. A company is running big data analytics and massive parallel computations on its AWS test and development servers. The company can tolerate occasional downtime. What is the MOST cost-effective Amazon EC2 purchasing option for the company to use?
- A. On-Demand Instances
- [x] B. Spot Instances
- C. Reserved Instances
- D. Savings Plans

---

Q647. A company runs Amazon EC2 instances in a research lab. The instances run for 3 hours each week and cannot be interrupted. What is the MOST cost-effective instance purchasing option to meet these requirements?
- A. Compute Savings Plan
- [x] B. On-Demand Instances
- C. Convertible Reserved Instances
- D. Spot Instances


Why On-Demand?
No Commitment, No Waste:

Cost: Pay only for actual usage ($0.192/hour for a t4g.micro in us-east-1 = $0.576/week).

No upfront fees or long-term commitments, avoiding wasted spend from reserved capacity (Savings Plans/RIs) for minimal usage.

Guaranteed Availability:

No interruptions (unlike Spot Instances).

Predictability:

Ideal for fixed, short-duration workloads with consistent weekly scheduling.

❌ Why Not Others?
Option	Drawbacks
A. Compute Savings Plan	Requires 1-/3-year commitment. For low usage (12–15 hours/month), savings are minimal vs. On-Demand, and unused hours are forfeited.
C. Convertible RIs	Upfront payment + hourly fees for unused capacity (e.g., $30/month for a reserved t4g.micro vs. $2.30/month On-Demand). Overkill for 12 hours/month.
D. Spot Instances	Interruption risk violates the "cannot be interrupted" requirement.


---

> [!IMPORTANT]
> Q648. A new AWS user needs to interact with AWS Support by using API calls. Which AWS Support plan will meet this requirement MOST cost-effectively?
- A. AWS Basic Support
- B. AWS Developer Support
- [x] C. AWS Business Support
- D. AWS Enterprise Support

> programmatic case management through the AWS Support API: available from AWS Business Support
 

 
---

Q649. A company migrated to the AWS Cloud. Now the company pays for services on an as-needed basis. Which advantage of cloud computing is the company benefiting from?  
- A. Stop spending money running and maintaining data centers  
- B. Increase speed and agility  
- C. Go global in minutes  
- [x] D. Trade fixed expense for variable expense  

---
 
Q650. A company will run a predictable compute workload on Amazon EC2 instances for the next 3 years. The workload is critical for the company. The company wants to optimize costs to run the workload. Which solution will meet these requirements?
- A. Spot Instances
- B. Dedicated Hosts
- [x] C. Savings Plans
- D. On-Demand Instances

---

Q651. A company wants to estimate the cost for its AWS architecture solution before migration. Which AWS service or feature will meet this requirement?
- A. Amazon Detective
- B. AWS Budgets
- C. AWS Resource Explorer
- [x] D. AWS Pricing Calculator

---

Q652. A university receives a grant to conduct research by using AWS services. The research team needs to make sure the grant money lasts for the entire school year. The team has decided on a monthly allocation that adds up to the total grant amount. Which AWS service or feature will notify the team if spending exceeds the planned amount?
- [x] A. AWS Budgets
- B. Cost Explorer
- C. Cost allocation tags
- D. Cost categories

---

> [!IMPORTANT]
> Q653. A company has migrated its workload to the AWS Cloud. The company wants to optimize existing Amazon EC2 resources. Which AWS services or tools provide this functionality? (Choose two.)
- A. AWS Elastic Beanstalk
- [x] B. AWS Cost Explorer
- C. Amazon Detective
- [x] D. AWS Compute Optimizer
- E. AWS Billing Conductor

---

> [!IMPORTANT]
> Q654. A company with multiple accounts and teams wants to set up a new multi-account AWS environment. Which AWS service supports this requirement?
- A. AWS CloudFormation
- [x] B. AWS Control Tower
- C. AWS Config
- D. Amazon Virtual Private Cloud (Amazon VPC)


A. AWS CloudFormation is a service that allows you to define and provision your AWS infrastructure as code, but it does not provide the comprehensive multi-account environment setup that this company requires.
B. AWS Control Tower is the correct answer, as it is designed to provide a streamlined way to set up and govern a secure, compliant, and well-architected multi-account AWS environment.
AWS Control Tower offers the following key features that support the company's requirement:
Account management: It can automatically provision new AWS accounts and apply pre-configured security and compliance guardrails.
Governance: It provides a centralized way to manage and enforce policies across multiple AWS accounts.
Visibility: It offers a dashboard to monitor the health and compliance of the overall AWS environment.
Automated deployment: It can set up a well-architected baseline environment across multiple accounts, including VPCs, IAM, logging, and other core services.
C. AWS Config is a service that helps you track changes to your AWS resources, but it does not provide the comprehensive multi-account environment setup capabilities.
D. Amazon VPC is a networking service that allows you to create and manage virtual networks within AWS, but it does not directly address the need for a multi-account environment setup.

---

Q655. A company needs access to checks and recommendations that help the company follow AWS best practices for cost optimization, security, fault tolerance, performance, and service quotas.  Which combination of an AWS service and AWS Support plan on the AWS account will meet these requirements?  
- A. AWS Trusted Advisor with AWS Developer Support  
- B. AWS Health Dashboard with AWS Enterprise Support  
- [x] C. AWS Trusted Advisor with AWS Business Support  
- D. AWS Health Dashboard with AWS Enterprise On-Ramp Support  

---

> [!IMPORTANT]
> Q656. Which AWS service helps users plan and track their server and application inventory migration data to AWS?  
- A. Amazon CloudWatch  
- B. AWS DataSync  
- [x] C. AWS Migration Hub  
- D. AWS Application Migration Service  

> keywords: plan and track

A. Amazon CloudWatch is a monitoring and observability service, but it does not provide the specific functionality to plan and track server and application inventory migration to AWS.

B. AWS DataSync is a data transfer service that helps move data between on-premises and AWS storage, but it does not cover the broader aspects of server and application migration planning and tracking.

C. AWS Migration Hub is the correct answer. AWS Migration Hub is a service that provides a single place to monitor and track the progress of application migrations to AWS. It helps users plan, track, and automate their server and application migrations to AWS.

D. AWS Application Migration Service (AWS MGN) is a service that helps migrate applications to AWS, but it does not provide the holistic migration planning and tracking capabilities that AWS Migration Hub offers.

AWS Migration Hub acts as a central location to plan, track, and automate the migration of servers, databases, and applications to AWS. It provides visibility into the progress of the overall migration process, which aligns with the requirements described in the question. 

---

> [!IMPORTANT]
> Q657. Which AWS team or offering helps users accelerate cloud adoption through paid engagements in any of several specialty practice areas?  
- A. AWS Enterprise Support  
- B. AWS solutions architects  
- [x] C. AWS Professional Services  
- D. AWS account managers

> keywords:  accelerate cloud adoption; paid engagements; several specialty practice areas

A. AWS Enterprise Support is a paid support plan that provides technical support, but it does not offer the specialized consulting and implementation services described in the question.

B. AWS solutions architects are technical experts who provide architectural guidance, but they do not offer the breadth of specialty practice areas mentioned in the question.

C. AWS Professional Services is the correct answer. AWS Professional Services is a team of AWS experts who provide paid engagements to help customers accelerate their cloud adoption through specialized practice areas such as migration, data and analytics, security, and more.

D. AWS account managers are dedicated points of contact for customers, but they do not directly provide the specialized consulting and implementation services described in the question.

https://aws.amazon.com/professional-services/

AWS Professional Services offers a range of specialty practice areas, such as:
- Migration Services
- Data and Analytics Services
- Security Services
- Modernization Services
- Internet of Things (IoT) Services
- Artificial Intelligence (AI) and Machine Learning (ML) Services

These specialized teams and services help customers rapidly adopt and utilize AWS services to achieve their business objectives.



---

Q658. A company needs to purchase Amazon EC2 instances to support an application that will run continuously for more than 1 year.  Which EC2 instance purchasing option meets these requirements MOST cost-effectively?  
- A. Dedicated Instances  
- B. Spot Instances  
- [x] C. Reserved Instances  
- D. On-Demand Instances  

---

Q659 is the same as Q554. 

---

Q660. A company wants to securely store Amazon RDS database credentials and automatically rotate user passwords periodically. Which AWS service or capability will meet these requirements?  
- A. Amazon S3  
- B. AWS Systems Manager Parameter Store  
- [x] C. AWS Secrets Manager  
- D. AWS CloudTrail  

The correct answer is C. AWS Secrets Manager.
Here's why:
AWS Secrets Manager is specifically designed for securely storing and managing secrets like database credentials, API keys, and other sensitive information. It offers features like:
Secure Storage: Secrets are encrypted at rest and in transit.
Rotation: Secrets Manager can automatically rotate passwords and other credentials on a schedule, improving security.
Access Control: You can define fine-grained access policies to control who can access and manage secrets.
Let's look at why the other options are not suitable:
A. Amazon S3: While S3 is great for object storage, it is not designed for storing sensitive credentials. It lacks the security features and rotation capabilities of Secrets Manager.
B. AWS Systems Manager Parameter Store: Parameter Store is primarily used for storing configuration data, not secrets. While it can be used to store credentials, it doesn't offer the same level of security and rotation features as Secrets Manager.
D. AWS CloudTrail: CloudTrail is a logging and auditing service. It records events in your AWS account, but it doesn't store or manage secrets.
In summary: AWS Secrets Manager is the ideal solution for securely storing and managing Amazon RDS database credentials and automating password rotation.


---

> [!IMPORTANT]
> Q661. A company is planning to migrate to the AWS Cloud. The company is conducting organizational transformation and wants to become more responsive to customer inquiries and feedback.  Which tasks should the company perform to meet these requirements, according to the AWS Cloud Adoption Framework (AWS CAF)? (Select TWO.)  
- [x] A. Realign teams to focus on products and value streams  
- B. Create new value propositions with new products and services  
- [x] C. Use agile methods to rapidly iterate and evolve  
- D. Use a new data and analytics platform to create actionable insights.  
- E. Migrate and modernize legacy infrastructure  

people perspective

The two tasks that align with the AWS Cloud Adoption Framework (AWS CAF) for organizational transformation and responsiveness to customer inquiries and feedback are:
A. Realign teams to focus on products and value streams: The AWS CAF emphasizes aligning teams around products and value streams to improve agility and responsiveness. This means organizing teams to focus on delivering specific customer outcomes rather than traditional functional silos.
C. Use agile methods to rapidly iterate and evolve: Agile methodologies are central to the AWS CAF's approach to cloud adoption. They enable organizations to respond quickly to changing customer needs and market demands by embracing iterative development, continuous feedback, and rapid experimentation.
Let's examine why the other options are less relevant in this context:
B. Create new value propositions with new products and services: While innovation is important, this task is more focused on product development and strategy rather than the organizational transformation needed for customer responsiveness.
D. Use a new data and analytics platform to create actionable insights: Data and analytics are crucial for understanding customer needs, but they are a tool to support the transformation, not the transformation itself.
E. Migrate and modernize legacy infrastructure: This task is essential for cloud adoption but doesn't directly address the company's goal of becoming more responsive to customer inquiries and feedback.
In conclusion: Realigning teams around value streams and adopting agile methodologies are key organizational changes that will enable the company to be more responsive to customer needs and feedback, aligning with the principles of the AWS CAF.


---


> [!IMPORTANT]
> Q662. A company runs its production workload in the AWS Cloud. The company needs to choose one of the AWS Support Plans. Which of the AWS Support Plans will meet these requirements at the LOWEST cost?  
- A. Developer  
- B. Enterprise On-Ramp  
- C. Enterprise  
- [x] D. Business  

> Business: Minimum recommended tier if you have production workloads in AWS
---

> [!IMPORTANT]
> Q663. Which AWS Cloud Adoption Framework (AWS CAF) perspective focuses on organizing an inventory of data products in a data catalog?  
- A. Operations  
- [x] B. Governance  (data curation capability)
- C. Business  
- D. Platform  

---

Q664. Which benefits does a company gain when the company moves from on-premises IT architecture to the AWS Cloud? (Select TWO.)  
- [x] A. Reduced or eliminated tasks for hardware troubleshooting, capacity planning, and procurement.  
- B. Elimination of the need for trained IT staff.  
- C. Automatic security configuration of all applications that are migrated to the cloud.  
- D. Elimination of the need for disaster recovery planning.  
- [x] E. Faster deployment of new features and applications.  

---

Q665. A company needs stateless network filtering for its VPC. Which AWS service, tool, or feature will meet this requirement?  
- A. AWS PrivateLink  
- B. Security group  
- [x] C. Network access control list (ACL).  
- D. AWS WAF  

---

Q666. Which tasks are responsibilities of the customer, according to the AWS shared responsibility model? (Select TWO.)  
- A. Secure the virtualization layer.  
- [x] B. Encrypt data and maintain data integrity.  
- C. Patch the Amazon RDS operating system.  
- [x] D. Maintain identity and access management controls.  
- E. Secure Availability Zones.  

---

Q667. A company that is planning to migrate to the AWS Cloud is based in an isolated area that has limited internet connectivity. The company needs to perform local data processing on premises. The company needs a solution that can operate without a stable internet connection.  Which AWS service will meet these requirements?  
- A. Amazon S3  
- [x] B. AWS Snowball Edge  
- C. AWS Storage Gateway  
- D. AWS Backup  

  

---

> [!IMPORTANT]
> Q668. A company uses Amazon S3 Standard to store records. The company needs a solution to restore objects that were accidentally deleted within the last week. Which AWS service or feature should the company use to meet this requirement?  
- A. Point-in-time recovery for Amazon DynamoDB  
- B. S3 Lifecycle  
- C. Amazon Elastic Block Store (Amazon EBS) snapshots  
- [x] D. AWS Backup  

 
AWS Backup: AWS Backup is a managed service designed to centrally back up and restore your AWS resources, including Amazon S3 objects. It offers a feature called "recovery points" that allows you to restore objects to a specific point in time, including those that have been accidentally deleted. This makes it ideal for recovering deleted S3 objects within the last week.
Let's look at why the other options are not suitable:
A. Point-in-time recovery for Amazon DynamoDB: This feature is specific to Amazon DynamoDB and doesn't apply to Amazon S3.
B. S3 Lifecycle: S3 Lifecycle is used to manage the lifecycle of objects in S3, including transitions between storage classes and object expiration. It doesn't provide point-in-time recovery for deleted objects.
C. Amazon Elastic Block Store (Amazon EBS) snapshots: EBS snapshots are used to back up EBS volumes, not S3 objects.
In summary: AWS Backup is the most appropriate service for restoring accidentally deleted S3 objects within the last week, as it offers point-in-time recovery capabilities for S3 data.


---

Q669. Which of the following is a customer responsibility according to the AWS shared responsibility model?  
- A. Apply security patches for Amazon S3 infrastructure devices.  
- B. Provide physical security for AWS datacenters.  
- C. Install operating system updates on Lambda@Edge  
- [x] D. Implement multi-factor authentication (MFA) for IAM user accounts.  


---


> [!IMPORTANT]
> Q670. A company has an AWS Business Support plan. The company needs to gain access to the AWS DDoS Response Team (DRT) to help mitigate DDoS events. Which AWS service or resource must the company use to meet these requirements?
- A. AWS Shield Standard
- B. AWS Enterprise Support
- C. AWS WAF
- [x] D. AWS Shield Advanced

> real-time visibility into any DDoS attacks

> access to shield response team (SRT) that provides added support for Shield Advanced customers. https://docs.aws.amazon.com/waf/latest/developerguide/ddos-srt-support.html

> AWS Shield Advanced is available to all customers; however, to contact the AWS Shield Response Team, customers will need the Enterprise or Business Support levels of AWS Premium Support.

---

> [!IMPORTANT]
> Q671. A company is planning to migrate to the AWS Cloud. The company needs to understand the existing on-premises usage and configuration. The company does not want to replicate its workloads to AWS yet. Which AWS service or tool will meet these requirements?
- [x] A. AWS Application Discovery Service
- B. AWS Application Migration Service
- C. Cloud Migration Factory
- D. AWS Transfer Family

 
AWS Application Discovery Service: This service is designed to discover, map, and analyze your existing on-premises applications and infrastructure. It gathers information about your applications, dependencies, and configurations, providing a comprehensive view of your current environment. This helps you understand your existing workloads without replicating them to AWS.
Let's look at why the other options are not suitable:
B. AWS Application Migration Service: This service helps you migrate your applications to AWS. It's not designed for understanding existing on-premises usage and configuration without migration.
C. Cloud Migration Factory: Cloud Migration Factory is a set of tools and best practices for migrating to AWS. It's not focused on understanding your existing environment without migration.
D. AWS Transfer Family: AWS Transfer Family is a set of services for transferring data to and from AWS. It's not designed for discovering and analyzing your existing on-premises applications.
In summary: AWS Application Discovery Service is the ideal tool for understanding your existing on- premises environment without migrating workloads to AWS. It provides valuable insights into your applications, dependencies, and configurations, enabling you to plan your cloud migration effectively.

---

> [!IMPORTANT]
> Q672. A company wants to migrate its server-based applications to the AWS Cloud. The company wants to determine the total cost of ownership for its compute resources that will be hosted on the AWS Cloud. Which combination of AWS services or tools will meet these requirements? (Select TWO.)
- [x] A. AWS Pricing Calculator
- [x] B. Migration Evaluator
- C. AWS Support Center
- D. AWS Application Discovery Service
- E. AWS Database Migration Service (AWS DMS)

The two AWS services or tools that will help a company determine the total cost of ownership (TCO) for its compute resources when migrating server-based applications to the AWS Cloud are:

A. AWS Pricing Calculator
The AWS Pricing Calculator is a web-based tool that allows you to create cost estimates for AWS services based on your specific use cases. It helps you model solutions, explore pricing options, and estimate the total cost of ownership for running workloads on AWS.

B. Migration Evaluator
Migration Evaluator is a **complimentary AWS service** that analyzes your current on-premises environment and generates a data-driven business case for migration. It inventories your existing resources, models utilization, and provides cost comparisons between your current state and various AWS deployment scenarios, including TCO projections.

Other options:

C. AWS Support Center is for support cases, not TCO analysis.

D. AWS Application Discovery Service helps collect data about your on-premises environment, but does not itself calculate TCO; it can, however, provide data for use in TCO tools.

E. AWS Database Migration Service (AWS DMS) is for migrating databases, not for TCO analysis.


The two correct answers are:
A. AWS Pricing Calculator: The AWS Pricing Calculator is a powerful tool that allows you to estimate the cost of various AWS services, including compute resources like EC2 instances. You can configure different instance types, operating systems, and usage patterns to get a detailed cost breakdown for your specific requirements.
B. Migration Evaluator: The Migration Evaluator is a tool within the AWS Management Console that helps you assess the feasibility and cost of migrating your on-premises workloads to AWS. It analyzes your existing applications and infrastructure and provides recommendations for migration strategies, including cost estimations for compute resources.
Let's examine why the other options are not suitable:
C. AWS Support Center: The AWS Support Center provides technical support and guidance, but it doesn't offer tools for cost estimation.
D. AWS Application Discovery Service: AWS Application Discovery Service is used for discovering and analyzing your existing on-premises applications and infrastructure. It doesn't provide cost estimations for cloud migration.
E. AWS Database Migration Service (AWS DMS): AWS DMS is a service for migrating databases to AWS. While it can provide cost estimations for database migration, it doesn't cover the overall cost of ownership for compute resources.
In summary: The AWS Pricing Calculator and Migration Evaluator are the most relevant tools for determining the total cost of ownership for compute resources in the AWS Cloud. They provide detailed cost breakdowns and migration assessments, helping you make informed decisions about your cloud migration strategy.


---

> [!IMPORTANT]
> Q673. Which AWS service is used to temporarily provide federated security credentials to access AWS resources?
- A. Amazon GuardDuty
- [x] B. AWS Simple Token Service (AWS STS)
- C. AWS Secrets Manager
- D. AWS Certificate Manager


AWS Simple Token Service (AWS STS): STS is a service that provides temporary security credentials for accessing AWS resources. These credentials are typically used for scenarios where you need to grant limited-time access to AWS resources without sharing long-term credentials. This is often used for:
Federated Identity: Allowing users from external identity providers (like Google, Facebook, or Active Directory) to access AWS resources.
Cross-Account Access: Granting temporary access to resources in another AWS account without sharing permanent credentials.
Assume Role: Allowing users or applications to assume a specific IAM role with specific permissions for a limited time.
Let's look at why the other options are not suitable:
A. Amazon GuardDuty: Amazon GuardDuty is a threat detection service that monitors your AWS environment for malicious activity. It doesn't provide temporary security credentials.
C. AWS Secrets Manager: AWS Secrets Manager is a service for securely storing and managing secrets like database credentials and API keys. It's not designed for providing temporary security credentials.
D. AWS Certificate Manager: AWS Certificate Manager is a service for managing and provisioning SSL/TLS certificates for your AWS resources. It doesn't provide temporary security credentials.
In summary: AWS Simple Token Service (STS) is the primary service for providing temporary security credentials to access AWS resources, enabling secure and controlled access for various use cases.


---

Q674. A company stores data in an Amazon S3 bucket. Which task is the responsibility of AWS?
- A. Configure an S3 Lifecycle policy
- B. Activate S3 Versioning
- C. Configure S3 bucket policies.
- [x] D. Protect the infrastructure that supports S3 storage.

---

Q675. Under the AWS shared responsibility model, which of the following is a responsibility of the customer?
- A. Shred disk drives before they leave a data center.
- B. Prevent customers from gathering packets or collecting traffic at the hypervisor level.
- [x] C. Patch the guest operating system with the latest security patches.
- D. Maintain security systems that provide physical monitoring of data centers.

---

Q676. Which AWS service integrates with other AWS services to provide the ability to encrypt data at rest?
- [x] A. AWS Key Management Service (AWS KMS)
- B. AWS Certificate Manager (ACM)
- C. AWS Identity and Access Management (IAM)
- D. AWS Security Hub


The correct answer is A. AWS Key Management Service (AWS KMS).
Here's why:
AWS Key Management Service (AWS KMS): KMS is a managed service that allows you to create and manage encryption keys. It integrates with other AWS services, like S3, EBS, and RDS, to provide data encryption at rest. You can use KMS to encrypt data before storing it in these services, ensuring that data is protected even if the underlying storage is compromised.
Let's look at why the other options are not suitable:
B. AWS Certificate Manager (ACM): ACM is used for managing and provisioning SSL/TLS certificates for your AWS resources. It's not directly involved in data encryption at rest.
C. AWS Identity and Access Management (IAM): IAM is used for managing user identities and access permissions to AWS resources. It doesn't directly encrypt data.
D. AWS Security Hub: Security Hub is a service that provides a centralized view of security alerts and findings across your AWS environment. It doesn't directly encrypt data.
In summary: AWS KMS is the primary service for managing encryption keys and integrating with other AWS services to provide data encryption at rest. It's a crucial component for ensuring data security in the cloud.

---

> [!IMPORTANT]
> Q677. In which situations should a company create an IAM user instead of an IAM role? (Select TWO.)
- A. When an application that runs on Amazon EC2 instances requires access to other AWS services
- [x] B. When the company creates AWS access credentials for individuals
- C. When the company creates an application that runs on a mobile phone that makes requests to AWS
- [x] D. When the company needs to add users to IAM groups
- E. When users are authenticated in the corporate network and want to be able to use AWS without having to sign in a second time.

 E. a federated user that assumes a role
 
B. When the company creates AWS access credentials for individuals
IAM users are intended for real people who need long-term credentials (like passwords or access keys) to log in to the AWS Management Console or use the AWS CLI.

D. When the company needs to add users to IAM groups
IAM users can be organized into groups, which makes it easier to manage permissions for multiple individuals at once.

Explanation:
IAM users represent individual people or specific services that need persistent credentials and direct access to AWS resources. Roles, on the other hand, are designed for temporary access, cross-account access, or for AWS services and applications to assume permissions as needed


> Key IAM Best Practices

- Use IAM users for humans, not machines.
- Use roles for applications/services.
- Never share credentials (Option B ensures individual accountability).
- Always federate external identities (e.g., Active Directory) to avoid creating IAM users for corporate users.


***Federation with IAM***

While we strongly recommend managing human users in IAM Identity Center, you can enable federated principal access with IAM for human users in short-term, small scale deployments. IAM allows you to use separate SAML 2.0 and Open ID Connect (OIDC) IdPs and use federated principal attributes for access control. With IAM, you can pass user attributes, such as cost center, title, or locale, from your IdPs to AWS, and implement fine-grained access permissions based on these attributes.

A workload is a collection of resources and code that delivers business value, such as an application or backend process. Your workload can require an IAM identity to make requests to AWS services, applications, operational tools, and components. These identities include machines running in your AWS environments, such as Amazon EC2 instances or AWS Lambda functions.

You can also manage machine identities for external parties who need access. *To give access to machine identities, you can use IAM roles*. IAM roles have specific permissions and provide a way to access AWS by relying on temporary security credentials with a role session. Additionally, you might have machines outside of AWS that need access to your AWS environments. 


---

Q678. A company wants to migrate critical on-premises production systems to Amazon EC2 instances. The production instances will be used for at least 3 years. The company wants a pricing option that will minimize cost. Which solution will meet these requirements?
- A. On-Demand Instances
- [x] B. Reserved Instances
- C. Spot Instances
- D. AWS Free Tier

---

Q679. Which AWS service is always available free of charge to users?
- A. Amazon Athena
- [x] B. AWS Identity and Access Management (IAM)
- C. AWS Secrets Manager
- D. Amazon ElastiCache

 
---


> [!IMPORTANT]
> Q680. To assist companies with Payment Card Industry Data Security Standard (PCI DSS) compliance in the cloud, AWS provides:
- A. physical inspections of data centers by appointment.
- B. required PCI compliance certifications for any application running on AWS
- [x] C. an AWS Attestation of Compliance (AOC) report for specific AWS services.
- D. professional PCI compliance services.

 
AWS Attestation of Compliance (AOC) report: AWS provides Attestation of Compliance (AOC) reports for specific AWS services, demonstrating their compliance with various industry standards, including PCI DSS. These reports provide evidence that AWS services meet the security requirements outlined in PCI DSS, helping companies demonstrate compliance in their cloud environment.

Let's examine why the other options are not the primary way AWS assists with PCI DSS compliance:

A. Physical inspections of data centers by appointment: While AWS does have secure data centers, physical inspections are not the primary mechanism for demonstrating PCI DSS compliance. Companies are responsible for securing their data and applications within the AWS environment.

B. Required PCI compliance certifications for any application running on AWS: AWS doesn't require applications running on its platform to have specific PCI compliance certifications. The responsibility for PCI compliance lies with the company using the AWS services.

D. Professional PCI compliance services: AWS may offer professional services related to security and compliance, but they don't provide dedicated PCI compliance services. Companies are typically responsible for engaging with third-party auditors to achieve PCI DSS compliance.
 

---

Q681. Which pillar of the AWS Well-Architected Framework focuses on the ability to recover automatically from service interruptions?
- A. Security
- B. Performance efficiency
- C. Operational excellence
- [x] D. Reliability

---

Q682. A company needs to provision uninterruptible Amazon EC2 instances, when needed, and pay for compute capacity by the second. Which EC2 instance purchasing option will meet these requirements?
- A. Reserved Instances
- B. Spot Instances
- [x] C. On-Demand Instances
- D. Dedicated Instances

> By the second means per second or for each second (of time).

> keywords: uninterruptible; "when needed" means unpredictable usage pattern

---

Q683. A company wants to move from an on-premises database to an Amazon RDS DB instance. Which feature will continue to be managed by the company?
- A. Power, network, and cooling
- B. Operating system installation
- C. Operating system patching
- [x] D. Application optimization

---

Q684. An administrator observed that multiple AWS resources were deleted yesterday. Which AWS service will help identify the cause and determine which user deleted the resources?
- [x] A. AWS CloudTrail
- B. Amazon Inspector
- C. Amazon GuardDuty
- D. AWS Trusted Advisor

---

Q685. A company wants to migrate to the AWS Cloud. The company needs the ability to acquire resources when the resources are necessary. The company also needs the ability to release those resources when the resources are no longer necessary. Which architecture concept of the AWS Cloud meets these requirements?
- [x] A. Elasticity
- B. Availability
- C. Reliability
- D. Durability

---

Q686. Which option is an advantage of AWS Cloud computing that minimizes variable costs?
- A. High availability
- [x] B. Economies of scale
- C. Global reach
- D. Agility

---

> [!IMPORTANT]
> Q687. Which AWS Well-Architected Framework concept represents a system's ability to remain functional when the system encounters operational problems?
- A. Consistency
- B. Elasticity
- [x] C. Durability
- D. Latency

> consistency focuses that data is consistent across multiple copies.

---

> [!IMPORTANT]
> Q688. Which AWS service or tool provides recommendations to help users get rightsized Amazon EC2 instances based on historical workload usage data?
- A. AWS Pricing Calculator
- [x] B. AWS Compute Optimizer
- C. AWS App Runner
- D. AWS Systems Manager

AWS App Runner builds and deploys web applications automatically, load balances traffic with encryption, scales to meet your traffic needs, and allows for the configuration of how services are accessed and communicate with other AWS applications in a private Amazon VPC.


---

Q689. A company needs to run some of its workload in the AWS Cloud. The company needs to keep some of the workload in its own on-site data center due to compliance reasons. Which AWS service will meet these requirements?
- A. AWS Config
- [x] B. AWS Outposts
- C. Amazon Lightsail
- D. Amazon Connect

---

Q690. Which AWS service can be used at no additional cost?
- A. Amazon SageMaker
- B. AWS Config
- [x] C. AWS Organizations
- D. Amazon CloudWatch

---

Q691. Which AWS service or feature gives users the ability to provision AWS infrastructure programmatically?
- [x] A. AWS Cloud Development Kit (AWS CDK)
- B. Amazon CodeGuru
- C. AWS Config
- D. AWS CodeCommit

---

Q692. A company has a website on AWS. The company wants to deliver the website to a worldwide audience and provide low-latency response times for global users. Which AWS service will meet these requirements?
- A. AWS CloudFormation
- [x] B. Amazon CloudFront
- C. Amazon ElastiCache
- D. Amazon DynamoDB

The correct answer is B. Amazon CloudFront.
Here's why:
Amazon CloudFront: CloudFront is a content delivery network (CDN) service that delivers content to users with low latency and high availability. It caches static content (like images, CSS, and JavaScript) at edge locations around the world, allowing users to access content from the nearest location, reducing latency and improving performance.
Let's examine why the other options are not the best fit:
A. AWS CloudFormation: CloudFormation is a service for defining and managing AWS infrastructure. It's not designed for content delivery.
C. Amazon ElastiCache: ElastiCache is a managed in-memory caching service that improves application performance. It's not designed for content delivery.
D. Amazon DynamoDB: DynamoDB is a fully managed NoSQL database service. It's not designed for content delivery.
In summary: Amazon CloudFront is the service that provides a global content delivery network (CDN) to deliver your website content to users worldwide with low latency and high availability, ensuring a fast and reliable experience for users around the globe.


---

Q693. Which AWS service or feature can be used to monitor for potential disk write spikes on a system that is running on Amazon EC2?
- A. AWS CloudTrail
- B. AWS Health Dashboard
- C. AWS Trusted Advisor
- [x] D. Amazon CloudWatch

---

Q694. A company wants to update its online data processing application by implementing container-based services that run for 4 hours at a time. The company does not want to provision or manage server instances. Which AWS service will meet these requirements?
- A. AWS Lambda
- [x] B. AWS Fargate
- C. Amazon EC2
- D. AWS Elastic Beanstalk

> AWS Fargate is a serverless compute engine for containers
 
---

Q695. A company needs to use Amazon S3 to store audio files that are each 5 megabytes in size. The company will rarely access the files, but the company must be able to retrieve the files immediately. Which S3 storage class will meet these requirements MOST cost-effectively?
- A. S3 Standard
- [x] B. S3 Standard-Infrequent Access (S3 Standard-IA)
- C. S3 Glacier Flexible Retrieval
- D. S3 Glacier Deep Archive

> C and D don't allow immediate data retrieval.


---

> [!IMPORTANT]
> Q696. Which AWS service enables users to create copies of resources across AWS Regions?
- A. Amazon ElastiCache
- [x] B. AWS CloudFormation
- C. AWS CloudTrail
- D. AWS Systems Manager

The correct answer is B. AWS CloudFormation.
Here's why:
AWS CloudFormation: CloudFormation is a service for defining and managing AWS infrastructure. It allows you to create templates that describe your infrastructure resources (like EC2 instances, S3 buckets, and VPCs). These templates can be used to create stacks, which are collections of resources. CloudFormation supports cross-region replication, allowing you to create copies of your stacks in different AWS Regions.
Let's examine why the other options are not the best fit:
A. Amazon ElastiCache: ElastiCache is a managed in-memory caching service. It's not designed for cross- region replication of resources.
C. AWS CloudTrail: CloudTrail is a service that records API calls made to your AWS account. It's not designed for replicating resources.
D. AWS Systems Manager: Systems Manager is a service for managing your AWS infrastructure. It includes features for patching, inventory, and automation, but it's not designed for cross-region replication of resources.
 


---

Q697 is the same as Q608. 


---

Q698. A company needs to use dashboards and charts to analyze insights from business data. Which AWS service will provide the dashboards and charts for these insights?
- A. Amazon Macie
- B. Amazon Aurora
- [x] C. Amazon QuickSight
- D. AWS CloudTrail

---

> [!IMPORTANT]
> Q699. A company wants to set up a secure network connection from on premises to the AWS Cloud within 1 week. Which solution will meet these requirements?
- A. AWS Direct Connect
- B. Amazon VPC
- [x] C. AWS Site-to-Site VPN
- D. Edge location

 Site-to-Site VPN creates an encrypted network path between your on-premises network and your AWS Cloud network. This connection uses the internet, so you cannot expect consistency.
 
AWS Site-to-Site VPN: A Site-to-Site VPN establishes a secure, encrypted connection between your on- premises network and your AWS VPC. It's a relatively quick and easy way to set up a connection, typically within a week, making it suitable for the company's timeframe.
Let's examine why the other options are not the best fit for this scenario:
A. AWS Direct Connect: Direct Connect provides a dedicated, private connection between your on- premises network and AWS. While it offers higher bandwidth and lower latency than VPN, it involves a more complex setup and longer lead time, usually not within a week. B. Amazon VPC: VPC is a virtual private cloud that provides a logically isolated environment for your AWS resources. It's not a connection method itself but rather the environment where you establish connections. D. Edge location: Edge locations are points of presence for AWS services like CloudFront. They are not designed for establishing secure connections between on-premises networks and AWS.
In summary: AWS Site-to-Site VPN is the most suitable solution for quickly setting up a secure network connection from on-premises to the AWS Cloud within a week. It offers a balance of security, ease of setup, and speed, making it ideal for this scenario.


---

Q700. A company wants to run relationship databases in the AWS Cloud. The company wants to use a managed service that will install the database and run regular software updates.   Which AWS service will meet these requirements?
- A. Amazon S3
- [x] B. Amazon RDS
- C. Amazon Elastic Block Store (Amazon EBS)
- D. Amazon DynamoDB

---


Q701 is the same as Q582.

---

Q702. A company needs to set up dedicated network connectivity between its on-premises data center and the AWS Cloud. The network cannot use the public internet. Which AWS service or feature will meet these requirements?
- A. AWS Transit Gateway
- B. AWS VPN
- C. Amazon CloudFront
- [x] D. AWS Direct Connect

---

Q703. A company wants to test a new application. Which AWS principle will help the company test the application?
- A. Make long-term commitments in exchange for a cost discount.
- [x] B. Scale up and down when needed without any long-term commitments
- C. Have total control over the application infrastructure
- D. Manage all of the maintenance tasks associated with the cloud

---

Q704. Which AWS service provides a fully managed graph database for highly connected datasets?
- A. Amazon DynamoDB
- B. Amazon RDS
- [x] C. Amazon Neptune
- D. Amazon Aurora

---

Q705. A company needs to have the ability to set up infrastructure for new applications in minutes. Which advantage of cloud computing will help the company meet this requirement?
- A. Trade fixed expense for variable expense
- B. Go global in minutes
- [x] C. Increase speed and agility
- D. Stop guessing capacity

---

Q706. Which AWS service or feature allows a company to have its own logically isolated section of the AWS Cloud?
- A. AWS VPN
- B. Availability Zones
- [x] C. Amazon Virtual Private Cloud (Amazon VPC)
- D. AWS Regions

---

Q707. A company wants to add a conversational chatbot to its website. Which AWS service can the company use to meet this requirement?
- A. Amazon Textract
- [x] B. Amazon Lex
- C. AWS Glue
- D. Amazon Rekognition



---

Q708. A company wants to purchase Amazon EC2 instances before using the EC2 instances for a workload. The company will commit to use the EC2 instances at a particular price over a specific period of time. Which AWS pricing model will meet these requirements MOST cost-effectively?
- A. On-Demand Instances
- B. Dedicated Hosts
- [x] C. Reserved Instances
- D. Spot Instances

---

> [!IMPORTANT]
> Q709. Why are AWS CloudFormation templates used?
- [x] A. To reduce provisioning time by using automation.
- B. To transfer existing infrastructure to another company.
- C. To reuse on-premises infrastructure in the AWS Cloud.
- D. To deploy large infrastructure with no cost implications.
 
 


---

Q710. A developer who has no AWS Cloud experience wants to use AWS technology to build a web application. Which AWS service should the developer use to start building the application?
- A. Amazon SageMaker
- B. AWS Lambda
- [x] C. Amazon Lightsail
- D. Amazon Elastic Container Service (Amazon ECS)


---

Q711. A user needs to perform a one-time backup of an Amazon Elastic Block Store (Amazon EBS) volume that is attached to an Amazon EC2 instance. What is the MOST operationally efficient way to perform this backup?
- A. Attach another EBS volume to the EC2 instance, and copy the contents
- B. Copy the EBS volume to a server that is running outside AWS and is connected with AWS Direct Connect.
- [x] C. Create an EBS snapshot of the volume.
- D. Create a custom script to copy the EBS file contents to Amazon S3

---

> [!IMPORTANT]
> Q712. A company purchased Amazon EC2 Standard Reserved Instances (RIs) for a workload in the AWS Cloud. The company needs to move part of the workload to an instance family that does not match the instance family of these Standard RIs. How can the company take advantage of the Standard RIs that it no longer needs?
- A. Contact the AWS Support team, and ask the team to sell the Standard RIs
- [x] B. Sell the Standard RIs on the Amazon EC2 Reserved Instance Marketplace
- C. Sell the Standard RIs as a third-party seller on the AWS Marketplace
- D. Convert the Standard RIs to Savings Plans

> The Amazon EC2 Reserved Instance Marketplace is a platform that facilitates the sale of unused Standard Reserved Instances from AWS customers and third-party sellers.

 
---

Q713. A company wants to build, train, and deploy machine learning (ML) models. Which AWS service can the company use to meet this requirement?
- A. Amazon Personalize
- B. Amazon Comprehend
- C. Amazon Forecast
- [x] D. Amazon SageMaker

---

> [!IMPORTANT]
> Q714. A company is releasing a business-critical application. Before the release, the company needs strategic planning assistance from AWS. During the release, the company needs AWS infrastructure event management and real-time support. What should the company do to meet these requirements?
- A. Access AWS Trusted Advisor
- B. Contact the AWS Partner Network (APN)
- [x] C. Sign up for AWS Enterprise Support.
- D. Contact AWS Professional Services


> AWS Professional Services is a team of AWS experts who provide paid engagements to help customers accelerate their cloud adoption through specialized practice areas such as migration, data and analytics, security, and more. AWS Professional Services offers consulting and implementation assistance but is typically engaged for project-based work rather than ongoing event management and real-time support.

> AWS Countdown: Plan and execute successful events with AWS Countdown, a service designed for a broad range of cloud use cases, including cloud migration services, cloud modernization, product launches, and go-live events. AWS Countdown, formerly known as AWS Infrastructure Event Management (IEM), ***helps you throughout the project lifecycle*** to assess cloud operational readiness, identify and mitigate risks, and plan capacity, using proven playbooks developed by AWS experts.

> AWS Countdown has replaced AWS IEM and is included with Enterprise Support. 
---

Q715. Which AWS offering can be natively associated with AWS WAF?
- [x] A. Application Load Balancer
- B. Network Load Balancer
- C. Gateway Load Balancer
- D. AWS Lambda

 
Application Load Balancer (ALB): ALBs are designed to handle HTTP and HTTPS traffic. They offer features like path-based routing, sticky sessions, and integration with AWS WAF. This integration allows you to apply WAF rules to protect your web applications running behind the ALB.

B. Network Load Balancer (NLB): NLBs handle TCP, UDP, and TLS traffic at the transport layer. They are optimized for high-throughput, low-latency applications and don't natively integrate with AWS WAF.

C. Gateway Load Balancer (GLB): GLBs are deprecated and are no longer recommended for new deployments.
 


---

Q716. A company wants to visualize and manage AWS Cloud costs and usage for a specific period of time. Which AWS service or feature will meet these requirements?
- [x] A. Cost Explorer
- B. Consolidated billing
- C. AWS Organizations
- D. AWS Budgets

---

Q717. Which type of workload should a company run on Amazon EC2 Spot Instances?
- A. A steady-state workload that requires a particular EC2 instance configuration for a long period of time
- [x] B. A workload that can be interrupted and can control costs
- C. A steady-state workload that does not require a long-term commitment
- D. A workload that cannot be interrupted and can control costs

> can tolerate interruptions
> can control costs

---

> [!IMPORTANT]
> Q718. A company deployed an application in multiple AWS Regions around the world. The company wants to improve the application's performance and availability.  Which AWS service will meet these requirements?
- [x] A. AWS Global Accelerator
- B. Amazon DataZone
- C. AWS Cloud Map
- D. AWS Auto Scaling

The correct answer is A. AWS Global Accelerator.
Here's why:
AWS Global Accelerator: Global Accelerator is a service that provides global traffic routing and load balancing for your applications. It directs traffic to the closest and most available endpoint, regardless of the user's location. This improves application performance by reducing latency and improves availability by distributing traffic across multiple Regions.
 
B. Amazon DataZone: DataZone is a service for managing and sharing data across your organization. It's not designed for improving application performance and availability. 

C. AWS Cloud Map: Cloud Map is a service for discovering and registering services within your AWS environment. It's helpful for service discovery but doesn't provide global traffic routing or load balancing. 

D. AWS Auto Scaling: Auto Scaling automatically adjusts the number of EC2 instances in your application based on demand. While it helps with availability, it doesn't address global traffic routing and performance optimization.

---

> [!IMPORTANT]
> Q719. A company wants to transfer a virtual Windows Server 2022 that is currently running in its own data center to AWS. The company wants to automatically convert the existing server to run directly on AWS infrastructure instead of visualized hardware. Which AWS service will meet these requirements?
- A. AWS DataSync
- B. AWS Database Migration Service (AWS DMS)
- C. AWS Application Discovery Service
- [x] D. AWS Application Migration Service

> rehost

 AWS Application Migration Service is the most appropriate service for automatically converting your existing Windows Server 2022 to run directly on AWS infrastructure. It provides the tools and features needed for a seamless and efficient migration process.
 
AWS Application Migration Service (AWS Migrations): AWS Migrations is designed specifically for migrating on-premises applications and workloads to AWS. It offers a variety of features, including:
Server migration: AWS Migrations can automatically convert your existing virtual servers (like Windows Server 2022) to run directly on AWS infrastructure.
Application discovery: It can inventory your on-premises applications and dependencies to help plan your migration.
Migration tools: It provides tools for migrating databases, applications, and other components.


A. AWS DataSync: DataSync is a service for transferring data between AWS storage services and on- premises locations. It's not designed for migrating entire servers or applications. B. AWS Database Migration Service (AWS DMS): DMS is specifically designed for migrating databases to AWS. While it can handle some application components, it's not a comprehensive solution for migrating entire servers.

C. AWS Application Discovery Service: Application Discovery Service helps you inventory your on- premises applications and dependencies. It's a useful tool for planning your migration but doesn't handle the actual migration process.
 


---

Q720. A company wants an Amazon S3 solution that provides access to object storage within single-digit milliseconds. Which solution will meet these requirements?
- [x] A. S3 Express One Zone
- B. S3 Standard
- C. S3 Glacier Flexible Retrieval
- D. S3 Glacier Instant Retrieval

---

Q721. For which use case are Amazon EC2 On-Demand Instances MOST cost-effective?
- A. Compute-intensive video transcoding that can be restarted if necessary
- [x] B. An instance in continual use for 1 month to conduct quality assurance tests
- C. An instance that runs a web server that will run for 1 year
- D. An instance that runs a database that will run for 3 years

---

Q722. A company has multiple AWS accounts. The company needs to receive a consolidated bill from AWS and must centrally manage security and compliance. Which AWS service or feature should the company use to meet these requirements?
- A. AWS Cost and Usage Report
- [x] B. AWS Organizations
- C. AWS Config
- D. AWS Security Hub

---

> [!IMPORTANT]
> Q723. A company wants to track the monthly cost and usage of all Amazon EC2 instances in a specific AWS environment. Which AWS service or tool will meet these requirements?
- A. AWS Cost Anomaly Detection
- [x] B. AWS Budgets
- C. AWS Compute Optimizer
- D. AWS Trusted Advisor
 
A. AWS Cost Anomaly Detection	Detects unexpected spending spikes but does not provide detailed cost/usage reports for EC2 instances  
B. AWS Budgets	Tracks overall spending against targets and alerts on thresholds but lacks granular EC2 instance-level cost/usage breakdowns 
C. AWS Compute Optimizer	Recommends resource rightsizing (e.g., EC2 instance types) but cannot track costs or usage metrics 
D. AWS Trusted Advisor	Identifies cost optimization opportunities (e.g., idle instances) but does not provide monthly cost/usage reports 

The Actual Solution: AWS Cost Explorer
Though not listed in the options, AWS Cost Explorer is the only AWS-native tool that meets all requirements:

Instance-Level Cost Tracking:

Filter by Service = Amazon EC2 and Dimension = Resource to view costs per EC2 instance ID 14.

Includes metrics like Blended Cost and Usage Hours 514.

Monthly Granularity: View data for up to 13 months with monthly/daily/hourly breakdowns 24.

Usage Metrics: Track compute hours, data transfer, and storage alongside costs 213.

Tag-Based Analysis: Group costs by tags (e.g., Environment=Production) to isolate specific environments

---

Q724. Which AWS service should a cloud engineer use to view API calls to AWS services?
- A. Amazon CloudWatch
- [x] B. AWS CloudTrail
- C. AWS Config
- D. AWS Artifact

---

Q725. Which of the following are best practices in AWS Identity and Access Management (IAM)? (Select TWO.)
- A. Create shared access keys.
- [x] B. Use roles to delegate permissions.
- C. Disable multi-factor authentication (MFA).
- D. Avoid the use of policy conditions.
- [x] E. Use groups to assign permissions to IAM users.

---

Q726. A company is migrating to the AWS Cloud. The company wants to understand and identify potential security misconfigurations or unexpected behaviors. The company wants to prioritize any protective controls it might need. Which AWS Cloud Adoption Framework (AWS CAF) security perspective capability will meet these requirements?
- A. Identity and access management (security)
- [x] B. Threat detection  (security)
- C. Platform engineering  (platform)
- D. Availability and continuity management (operations)

---

Q727. A company is creating a web application that requires a relational database to store customer data. Which AWS service should the company use to host the database?
- [x] A. Amazon Aurora
- B. Amazon DynamoDB
- C. Amazon ElastiCache
- D. Amazon Redshift

---

Q728. A company wants to avoid unnecessary charges and run workloads at the lowest price point. Which pillar of the AWS Well-Architected Framework includes these goals?
- A. Security
- B. Reliability
- C. Sustainability
- [x] D. Cost optimization

---

Q729. A company has a goal to run and monitor systems to deliver business value while continually improving support processes and procedures. Which pillar of the AWS Well-Architected Framework does this goal meet?
- A. Reliability
- B. Security
- [x] C. Operational excellence
- D. Performance efficiency


---

Q730. A company needs to connect multiple VPCs and on-premises networks through a single network connection to the AWS Cloud. Which solution meets this requirement?  
- [x] A. AWS Transit Gateway  
- B. AWS Direct Connect  
- C. VPC peering  
- D. AWS Client VPN  

---

Q731. Which feature of Amazon S3 can restore accidentally deleted or overwritten objects?  
- A. S3 Access Points  
- B. S3 Block Public Access  
- [x] C. S3 Versioning  
- D. S3 Object Lock  

---

Q732. A company needs an AWS Support plan that provides programmatic case management through the AWS Support API. Which support plan will meet this requirement MOST cost-effectively?  
- [x] A. AWS Business Support  
- B. AWS Basic Support  
- C. AWS Developer Support  
- D. AWS Enterprise Support  

---

Q733. A company needs an AWS design solution for a distributed system. The system's components need to be set up so that one system component cannot negatively impact another component. Which AWS architectural best practice will meet this requirement?  
- A. Use request throttling  
- B. Use a stateful service  
- C. Implement automatic data backups  
- [x] D. Implement loose coupling  

---

Q734. A company wants a list of all users in its AWS account, the status of all of the users' access keys, and if multi-factor authentication (MFA) has been configured. Which AWS service or feature will meet these requirements?  
- A. AWS Key Management Service (AWS KMS)  
- B. IAM Access Analyzer  
- [x] C. IAM credential report  
- D. Amazon CloudWatch  

---

> [!IMPORTANT]
> Q735. Which AWS service can automate patching of operating systems that run on Amazon EC2 instances?  
- A. Amazon Inspector  
- B. AWS License Manager  
- C. AWS Config  
- [x] D. AWS Systems Manager  

 
AWS Systems Manager provides a set of tools to automate operational tasks, including the patching of operating systems running on Amazon EC2 instances. Using Systems Manager Patch Manager, you can automate the process of patching and ensure that your instances are up-to-date with the latest security and software updates.
The other options do not specifically focus on automating operating system patching:
A. Amazon Inspector: This service is used for automated security assessments of applications running on EC2, but it does not handle patch management.
B. AWS License Manager: This service helps manage software licenses but does not automate patching. C. AWS Config: This service monitors and records AWS resource configurations and compliance but does not perform patching of operating systems.

---

Q736. A company needs to create an encrypted network connection between two offices in different countries. The connection must be over the public internet.  Which AWS service should the company use to meet these requirements?  
- A. AWS Direct Connect  
- B. Amazon VPC Lattice  
- [x] C. AWS Site-to-Site VPN  
- D. AWS Cloud WAN  

---

Q737. Which AWS Cloud Adoption Framework (AWS CAF) capability is included in the governance perspective?  
- A. Organization design  (people)
- [x] B. Application portfolio management (governance)
- C. Application management  (operations)
- D. Application security  (security)

---

> [!IMPORTANT]
> Q738. A company is migrating its on-premises data center infrastructure to the AWS Cloud. The company needs to determine its computer asset inventory, plan the migration, and track the migration. Which AWS service will meet these requirements?
- A. AWS Mainframe Modernization
- B. AWS Schema Conversion Tool (AWS SCT)
- [x] C. AWS Migration Hub
- D. AWS Transfer Family
 
 
AWS Migration Hub provides a central location to track the progress of application migrations across multiple AWS and partner solutions. It helps organizations to determine their compute asset inventory, plan their migration strategy, and monitor the migration process effectively.
The other options do not meet all the specified requirements:
A. AWS Mainframe Modernization: This service is focused on modernizing mainframe workloads but does not specifically track migrations across various environments. B. AWS Schema Conversion Tool (AWS SCT): This tool helps convert database schemas but does not track the overall migration process or asset inventory.
D. AWS Transfer Family: This service facilitates transferring files into and out of AWS but is not focused on migration planning or tracking.

  
---
Q739 is the same as Q363. 

---

Q740. A company needs to run a workload for several batch image rendering applications. It is acceptable for the workload to experience downtime. Which Amazon EC2 pricing model would be MOST cost-effective in this situation?  
- A. On-Demand Instances  
- B. Reserved Instances  
- C. Dedicated Instances  
- [x] D. Spot Instances  

---


Q741. A company needs a graph database service that is scalable and highly available. Which AWS service meets these requirements?  
- A. Amazon Aurora  
- B. Amazon Redshift  
- C. Amazon DynamoDB  
- [x] D. Amazon Neptune  

---

Q742. Which option routes inbound traffic from the internet to resources in a VPC?  
- A. AWS Fargate  
- [x] B. Internet gateway  
- C. VPC peering connection  
- D. AWS WAF  

---

> [!IMPORTANT]
> Q743. A software engineer wants to launch a virtual machine (VM) and MySQL database on AWS. Which AWS service will meet these requirements with the LEAST operational effort?  
- A. Amazon Elastic Container Service (Amazon ECS)  
- B. AWS Elastic Beanstalk  
- [x] C. Amazon Lightsail  
- D. Amazon EC2  


https://www.youtube.com/watch?v=CQ94kSUun8w
 
Amazon Lightsail is designed to make it easy to launch and manage virtual machines (VMs) and includes built-in support for databases like MySQL. It provides a simplified interface and predictable pricing, reducing the operational effort needed for management compared to other services.
The other options require more operational input:
A. Amazon Elastic Container Service (Amazon ECS): This service is focused on container orchestration and would require more setup and management for a VM and database. B. AWS Elastic Beanstalk: This service is great for deploying applications but may be more complex than necessary for simply launching a VM and a database.
D. Amazon EC2: While it can launch VMs and databases, it requires more operational effort to manage instances and configure the environment compared to Lightsail.


---

Q744. Which Reserved Instance (RI) provides the HIGHEST average cost savings compared to an On-Demand Instance?  
- A. 1-year, No Upfront, Standard RI  
- B. 1-year, All Upfront, Convertible RI  
- [x] C. 3-year, All Upfront, Standard RI  
- D. 3-year, No Upfront, Convertible RI  

---

> [!IMPORTANT]
> Q745. What is the MINIMUM AWS Support plan that is required to access Support Automation Workflows that are maintained by AWS Support?  
- A. AWS Enterprise Support  
- B. AWS Enterprise On-Ramp Support  
- C. AWS Business Support  
- [x] D. AWS Developer Support  

https://aws.amazon.com/premiumsupport/technology/saw/
I guess there's a recent change:
currently
Developer Support: Includes basic SAW (AWSSupport-*) but lacks advanced runbooks and 24/7 support.
Business Support: Expands to premium runbooks (AWSPremiumSupport-*) with faster response times

>Support Automation Workflows (SAW) are automation runbooks written and maintained by the AWS Support team. These runbooks help you troubleshoot common issues with your AWS resources, proactively monitor and identify network issues, collect and analyze logs, and more.

> SAW runbooks use the AWSSupport prefix. For example, AWSSupport-ActivateWindowsWithAmazonLicense.

> Additionally, AWS Enterprise and Business Support customers also have access to runbooks that use the AWSPremiumSupport prefix. For example, AWSPremiumSupport-TroubleshootEC2DiskUsage.

> AWS Support Automation Workflows enable you to diagnose and resolve common Support issues following AWS best practices. Access to Support Automation Workflows with prefix AWSSupport is included with Developer Support.

> Developer Support provides access to a subset of Support Automation Workflows maintained by AWS Support (those with the prefix AWSSupport-). Higher-tier plans provide access to additional, more advanced workflows ( with the prefix AWSPremiumSupport-), but Developer Support is the minimum required for the basic set

---

> [!IMPORTANT]
> Q746. Which AWS service gives users the ability to use standard SQL to directly query AWS Cost and Usage Report data?  
- A. Amazon Aurora  
- [x] B. Amazon Athena  
- C. Amazon DynamoDB  
- D. Amazon CloudWatch  

> Cost and Usage Report data can be integrated to Amazon Athena, Amazon Redshift, and Amazon QuickSight

---

Q747. A company needs to apply security rules to specific Amazon EC2 instances. Which AWS service or feature provides this functionality?  
- A. AWS WAF  
- B. Network ACLs  
- C. Amazon VPC  
- [x] D. Security groups  



---


> [!IMPORTANT]
> Q748. A company's application uses Amazon EC2 instances, AWS Lambda functions, and AWS Fargate tasks that are deployed in multiple AWS Regions. The company needs to optimize cost across Regions by using a single purchasing option. Which purchasing option will meet these requirements MOST cost-effectively?  
- [x] A. Compute Savings Plans  
- B. EC2 Instance Savings Plans  
- C. On-Demand Instances  
- D. Reserved Instances  

---

> [!IMPORTANT]
> Q749. A company needs to invoke an AWS Step Functions workflow each time an Amazon EC2 instance state changes to RUNNING. Which AWS service can the company use to meet this requirement?  
- A. Amazon SageMaker  
- B. Amazon Connect  
- [x] C. Amazon EventBridge  
- D. AWS Fargate  


Amazon EventBridge can be used to monitor events from various sources, including changes in the state of Amazon EC2 instances. You can create an EventBridge rule that listens for EC2 state change events (such as transitioning to the RUNNING state) and triggers an AWS Step Functions workflow whenever this event occurs.
The other options do not fulfill this requirement:
A. Amazon SageMaker: This is a machine learning service and not designed for event-driven workflows. B. Amazon Connect: This is a cloud contact center service and does not relate to monitoring EC2 instance states.
D. AWS Fargate: This is a serverless compute engine for containers and does not directly handle events or workflows based on EC2 state changes.


---

Q750. Which AWS compute service automatically scales resources up or down to meet application workload demands?  
- A. Amazon Simple Queue Service (Amazon SQS)  
- B. Amazon EC2  
- C. Amazon Aurora  
- [x] D. AWS Lambda  
 



---

Q751. A cloud engineer needs to track AWS costs. The cloud engineer also needs to receive event-driven alerts when costs exceed specific thresholds. Which AWS tool provides this functionality?  
- A. AWS Cost Explorer  
- [x] B. AWS Budgets  
- C. Cost allocation tags  
- D. AWS Cost and Usage Reports  

---

> [!IMPORTANT]
> Q752. Which AWS service or tool does AWS Control Tower use to create resources?  
- [x] A. AWS CloudFormation  
- B. AWS Trusted Advisor  
- C. AWS Directory Service  
- D. AWS Cost Explorer  

 
AWS Control Tower uses AWS CloudFormation to create and manage the resources needed for setting up and governing a multi-account environment. CloudFormation allows Control Tower to automate the deployment of AWS resources according to predefined templates, ensuring that resources are provisioned consistently and efficiently.
The other options do not serve this purpose:
B. AWS Trusted Advisor: This is a service that provides real-time guidance to help you provision your resources following AWS best practices but does not create resources. C. AWS Directory Service: This service provides directory services for AWS resources but is not used by Control Tower to create resources.
D. AWS Cost Explorer: This tool helps you analyze your AWS spending but does not create or manage resources.

---

Q753. A company wants to run an application on Amazon EC2 instances. The application has short-term, irregular workloads that cannot be interrupted. Which will be the MOST cost-effective pricing model for this workload?  
- [x] A. On-Demand Instances  
- B. Dedicated Instances  
- C. Reserved Instances  
- D. Savings Plans  

---

> [!IMPORTANT]
> Q754. A company needs to receive rightsizing recommendations that help identify cost-saving opportunities for Amazon EC2 instances. Which AWS service or tool will provide these recommendations?  
- A. AWS Config  
- [x] B. AWS Cost Explorer  
- C. Amazon Inspector  
- D. Amazon Lightsail  

---

Q755. Which statement is an AWS Cloud best practice that focuses on the elasticity and agility of cloud computing?  
- A. Provision capacity based on past usage and theoretical peaks.  
- [x] B. Dynamically scale to meet usage demands.  
- C. Build the application and infrastructure in a data center that grants physical access.  
- D. Break apart the application into loosely coupled components.  


---

Q756. A company needs to continuously monitor its environment to analyze network and account activity and identify potential security threats. Which AWS service should the company use to meet these requirements?  
- A. AWS Artifact  
- B. Amazon Macie  
- C. AWS Identity and Access Management (IAM)  
- [x] D. Amazon GuardDuty  

---

Q757. A company plans to deploy its application globally. The company wants to cache content at edge locations and deliver the content to users with the lowest possible latency. Which AWS service will meet these requirements?  
- A. AWS Global Accelerator  
- B. AWS Outposts  
- C. Amazon Route 53  
- [x] D. Amazon CloudFront  

 
Amazon CloudFront is a content delivery network (CDN) service that caches content at edge locations around the world. It is designed to deliver content to users with the lowest possible latency by serving it from the nearest edge location. This makes it ideal for globally deployed applications that require fast content delivery.
 
A. AWS Global Accelerator: This service improves the availability and performance of applications by ***directing user traffic to the optimal endpoint*** ***but does not cache content***. B. AWS Outposts: This service extends AWS infrastructure to on-premises environments, but it does not focus on content delivery or caching.
C. Amazon Route 53: This is a scalable domain name system (DNS) web service but does not cache or deliver content.

---

> [!IMPORTANT]
> Q758. A company has an application workload that is mostly consistent. However, the workload requires access to additional capacity during unpredictable peaks in demand. The workload must run for 1 year and cannot be interrupted. Which purchasing option will meet these requirements MOST cost-effectively?  
- A. Use Spot Instances for the entire workload.  
- B. Use On-Demand Instances for the entire workload.  
- C. Use On-Demand Instances for consistent baseline compute capacity. Use Spot Instances for additional burst capacity.  
- [x] D. Use Compute Savings Plans for consistent baseline compute capacity. Use On-Demand Instances for additional burst capacity.  

---

Q759. In the AWS shared responsibility model, which tasks are the responsibility of AWS? (Select TWO.)  
- A. Patch an Amazon EC2 instance operating system.  
- B. Configure a security group.  
- [x] C. Monitor the health of an Availability Zone.  
- [x] D. Protect the infrastructure that runs Amazon EC2 instances.  
- E. Manage access to the data in an Amazon S3 bucket.  

---

Q760. A company is migrating a relational database server to the AWS Cloud. The company wants to minimize administrative overhead of database maintenance tasks. Which AWS service will meet these requirements?  
- A. Amazon DynamoDB  
- B. Amazon EC2  
- C. Amazon Redshift  
- [x] D. Amazon RDS  

---

Q761. A company wants to perform sentiment analysis on customer service email messages that it receives. The company wants to identify whether the customer service engagement was positive or negative. Which AWS service should the company use to perform this analysis?  
- A. Amazon Textract  
- B. Amazon Translate  
- [x] C. Amazon Comprehend  
- D. Amazon Rekognition  

---

Q762. A company needs to set up a user-defined isolated environment in the AWS Cloud. Which of the following can the company use to meet this requirement?  
- A. AWS VPN  
- [x] B. Amazon VPC  
- C. AWS Regions  
- D. Availability Zones  

---

> [!IMPORTANT]
> Q763. A company wants to securely rehost databases to AWS with minimal downtime. Which AWS service will meet these requirements?  
- [x] A. AWS Database Migration Service (AWS DMS)  
- B. AWS Snow Family  
- C. AWS DataSync  
- D. AWS Mainframe Modernization  

  
AWS Database Migration Service (AWS DMS) is specifically designed for migrating databases to AWS with minimal downtime. It supports both homogenous (same database type) and heterogeneous (different database types) migrations, allowing you to securely rehost your databases while keeping the source database operational during the migration process.
 
B. AWS Snow Family: This is used for transferring large amounts of data when network bandwidth is limited but is not specifically tailored for database migrations. C. AWS DataSync: This service is intended for data transfer between on-premises storage and AWS but is not specifically designed for database migration.
D. AWS Mainframe Modernization: This service is focused on modernizing mainframe applications and does not specifically address database migration needs.

AWS Database Migration Service (AWS DMS) is a web service you can use to migrate data from your database that is 
 - on-premises,
 - on an Amazon Relational Database Service (Amazon RDS) DB instance,
 - or in a database on an Amazon Elastic Compute Cloud (Amazon EC2) instance

to a database on an AWS service. These services can include:

- a database on Amazon RDS
- or a database on an Amazon EC2 instance. 

You can also migrate a database from an AWS service to an on-premises database. 

---

Q764. Which AWS service or feature can migrate data files to the AWS Cloud from an on-premises site with no internet connection?  
- A. AWS Outposts servers  
- [x] B. AWS Snowball Edge compute optimized devices  
- C. AWS Storage Gateway  
- D. Amazon File Cache  


---

Q765. Which AWS service gives users the ability to download compliance reports from third-party auditors?
- A. AWS Lambda
- B. AWS Trusted Advisor
- [x] C. AWS Artifact
- D. AWS Audit Manager

 
AWS Artifact is a service that provides access to compliance reports and security documentation from third-party auditors. It acts as a central resource for managing compliance-related documents, allowing users to download and review these reports to ensure compliance with various standards and regulations.
The other options do not provide this functionality:
A. AWS Lambda: This is a serverless compute service and does not deal with compliance reports. B. AWS Trusted Advisor: This service provides real-time guidance to help you provision your resources according to AWS best practices but does not offer compliance reports. 
D. AWS Audit Manager: This service helps you continuously audit your AWS usage and manage compliance but does not provide direct access to third-party compliance reports like AWS Artifact does.


---

Q766. A company is deploying a mobile app on AWS. Thousands of users will access the app. Which AWS service should the company use to create a directory to manage sign-in for the users?
- A. AWS Directory Service
- B. AWS IAM Identity Center
- [x] C. Amazon Cognito
- D. AWS Identity and Access Management (IAM)

 
Amazon Cognito is specifically designed for managing user sign-up, sign-in, and access control for mobile and web applications. It provides a scalable user directory that can handle thousands of users, allowing you to manage user identities and authentication efficiently.
The other options do not serve this purpose as effectively:
A. AWS Directory Service: This service is primarily for integrating with Microsoft Active Directory and is more suited for enterprise applications rather than mobile apps. B. AWS IAM Identity Center: This service is focused on managing access to AWS accounts and applications for users within an organization, rather than for external users of a mobile app. D. AWS Identity and Access Management (IAM): While IAM is crucial for managing permissions and access to AWS resources, it is not designed for user authentication and management for mobile applications.


---

Q767. Which AWS service or feature can a company use to apply security rules to a subnet for Amazon EC2 instances?
- A. AWS WAF
- B. AWS Shield
- [x] C. Network ACLs
- D. Security groups

---

> [!IMPORTANT]
> Q768. A company wants to automatically set up and govern a multi-account AWS environment. Which AWS service provides this functionality?
- A. AWS IAM Identity Center
- B. AWS Systems Manager
- C. AWS Config
- [x] D. AWS Control Tower
 
AWS Control Tower is designed to automatically set up and govern a multi-account AWS environment. It provides best practices for account management, security, and compliance, making it easier to manage multiple accounts in a structured way. Control Tower helps organizations implement governance controls and automates the setup of accounts according to AWS best practices.
The other options do not provide the same level of functionality:
A. AWS IAM Identity Center: This service is focused on managing user access to AWS accounts and applications but does not govern a multi-account setup.
B. AWS Systems Manager: This service helps manage AWS resources and automate operational tasks but is not specifically designed for multi-account governance. C. AWS Config: This service monitors the configuration of AWS resources and evaluates compliance but does not set up multi-account environments.


---

Q769. A company needs to put its AWS resources into groups and then determine the cost for each group. Which AWS service or feature can the company use to group the resources?
- [x] A. Cost allocation tags
- B. AWS Budgets
- C. AWS Billing Conductor
- D. AWS Identity and Access Management (IAM)

---

Q770. A company needs to securely store important credentials that an application uses to connect users to a database. Which AWS service can meet this requirement with the MINIMAL amount of operational overhead?
- A. AWS Key Management Service (AWS KMS)
- B. AWS Config
- [x] C. AWS Secrets Manager
- D. Amazon GuardDuty

---

Q771. Which AWS service keeps track of SSL/TLS certificates, creates new certificates, and processes renewals?
- A. AWS Identity and Access Management (IAM)
- [x] B. AWS Certificate Manager (ACM)
- C. AWS Config
- D. AWS Trusted Advisor

 
AWS Certificate Manager (ACM) is the service that manages SSL/TLS certificates for your AWS-based applications. It provides functionalities for creating, managing, and renewing certificates easily, allowing you to deploy secure connections without the operational overhead of manual certificate management.
The other options do not provide this functionality:
A. AWS Identity and Access Management (IAM): While IAM can manage some types of certificates, it is not focused on SSL/TLS certificate management.
C. AWS Config: This service monitors and evaluates the configurations of your AWS resources but does not manage certificates.
D. AWS Trusted Advisor: This service provides best practice recommendations for AWS accounts but does not manage or track SSL/TLS certificates.

---

Q772. A company wants to manage access and permissions for its third-party software as a service (SaaS) applications. The company wants to use a portal where end users can access assigned AWS accounts and AWS Cloud applications. Which AWS service should the company use to meet these requirements?
- A. Amazon Cognito
- [x] B. AWS IAM Identity Center (AWS Single Sign-On)
- C. AWS Identity and Access Management (IAM)
- D. AWS Directory Service for Microsoft Active Directory

 
A. Amazon Cognito - Amazon Cognito is a user identity and data synchronization service that enables you to create and manage user identities in your applications. It primarily focuses on user sign-up, sign-in, and access control with a heavy emphasis on mobile and web applications. It is not tailored for managing access to multiple AWS accounts and third-party SaaS applications through a single portal.
B. AWS IAM Identity Center (AWS Single Sign-On) - AWS IAM Identity Center (formerly AWS Single Sign-On, or AWS SSO) enables you to manage access to multiple AWS accounts and business applications from one place. It centralizes authentication and allows users to access resources in AWS and third-party applications using a single set of credentials. This service meets the requirement of managing access and permissions for both AWS and third-party SaaS applications through a portal.
C. AWS Identity and Access Management (IAM) - AWS IAM is a robust service for managing access to AWS services and resources securely. However, it focuses primarily on AWS resources and does not have a built-in capability to manage access to third-party SaaS applications through a single portal.
D. AWS Directory Service for Microsoft Active Directory - AWS Directory Service provides managed Microsoft Active Directory, AD Connector, and Simple AD services. It is primarily used to integrate Microsoft Active Directory with AWS, enabling single sign-on and access control for on-premises and AWS resources. While it can be part of a larger identity and access management solution, it does not meet the requirement of managing access to third-party SaaS applications through a single portal.
 

---

Q773. Which AWS service is designed for users running workloads that include a NoSQL database?
- A. Amazon RDS
- B. Amazon S3
- C. Amazon Redshift
- [x] D. Amazon DynamoDB

---

Q774. A company has applications that control on-premises factory equipment. Which AWS service should the company use to run these applications with the LEAST latency?
- [x] A. AWS Outposts
- B. Amazon EC2
- C. AWS Lambda
- D. AWS Fargate

To determine which AWS service would provide the LEAST latency for running applications that control on-premises factory equipment, let's evaluate each option:
A. AWS Outposts - AWS Outposts is a fully managed service that extends AWS infrastructure, AWS services, APIs, and tools to your on-premises environments. By deploying AWS Outposts, you can run the same AWS services in your data center that you run in the AWS Cloud, offering low-latency access to your on-premises factory equipment. This is because AWS Outposts brings the cloud to your data center, minimizing the distance between the applications and the equipment they control.
B. Amazon EC2 - Amazon Elastic Compute Cloud (EC2) provides scalable computing capacity in the AWS Cloud. While EC2 is a powerful service, it operates within the AWS Cloud infrastructure, which would likely result in higher latency for controlling on-premises factory equipment compared to AWS Outposts.
C. AWS Lambda - AWS Lambda is a serverless compute service that lets you run code without provisioning or managing servers. Lambda functions execute in response to events and automatically manage the underlying compute resources. However, Lambda functions run in the AWS Cloud, resulting in higher latency for controlling on-premises factory equipment.
D. AWS Fargate - AWS Fargate is a serverless compute engine for containerized applications that allows you to run containers without managing servers or clusters. Like Lambda, Fargate operates within the AWS Cloud infrastructure, which would also result in higher latency for controlling on-premises factory equipment.
 

---

> [!IMPORTANT]
> Q775. A company plans to perform a one-time migration of a large dataset with millions of files from its on-premises data center to the AWS Cloud. Which AWS service should the company use for the migration?
- A. AWS Database Migration Service (AWS DMS)
- [x] B. AWS DataSync
- C. AWS Migration Hub
- D. AWS Application Migration Service

To determine which AWS service is best suited for a one-time migration of a large dataset with millions of files from an on-premises data center to the AWS Cloud, let's evaluate each option:
A. AWS Database Migration Service (AWS DMS) - AWS DMS is designed to migrate relational databases, such as MySQL, PostgreSQL, Oracle, SQL Server, and others, to AWS. It is primarily focused on database migration and might not be the best choice for migrating large datasets that include millions of files, especially if those files are not structured as database records.
B. AWS DataSync - AWS DataSync is a managed data transfer service that simplifies, automates, and accelerates moving and replicating large amounts of data between on-premises storage and AWS storage services, or between AWS storage services. It is specifically designed to handle large-scale data migrations and can efficiently transfer millions of files. DataSync optimizes data transfer for both network performance and cost, making it an excellent choice for a one-time migration of a large dataset.
C. AWS Migration Hub - AWS Migration Hub provides a single place to track and manage your application migrations across multiple AWS services. It does not itself perform data migrations but rather provides a centralized view and management of migration processes.
D. AWS Application Migration Service - This is not a specific AWS service. AWS offers a variety of tools and services for application migration, but none is named "AWS Application Migration Service." Instead, services like AWS Server Migration Service (SMS) and AWS CloudEndure Migration can be used for migrating applications, but they typically focus on entire servers or virtual machines rather than large datasets with millions of files.
 


---

Q776. A company wants to migrate its on-premises infrastructure to the AWS Cloud. Which advantage of cloud computing will help the company reduce upfront costs?
- A. Go global in minutes
- B. Increase speed and agility
- C. Benefit from massive economies of scale
- [x] D. Trade fixed expense for variable expense

---

> [!IMPORTANT]
> Q777. A company plans to migrate to the AWS Cloud. The company wants to gather information about its on-premises data center. Which AWS service should the company use to meet these requirements?
- [x] A. AWS Application Discovery Service
- B. AWS DataSync
- C. AWS Storage Gateway
- D. AWS Database Migration Service (AWS DMS)
 
A. AWS Application Discovery Service - AWS Application Discovery Service automatically discovers on-premises servers that are running in your data center or on your corporate network. It helps you to identify the applications running on those servers, the connections between them, and the performance metrics associated with them. This information is crucial for planning a migration to the AWS Cloud.
B. AWS DataSync - AWS DataSync is a managed data transfer service that simplifies, automates, and accelerates moving and replicating large amounts of data between on-premises storage and AWS storage services, or between AWS storage services. It is not used for gathering information about the on-premises data center but rather for data migration.
C. AWS Storage Gateway - AWS Storage Gateway is a hybrid storage service that enables you to seamlessly connect your on-premises IT environment to the AWS storage infrastructure. It provides you with the flexibility to store your data in AWS while maintaining low-latency access to your data from your on-premises applications. However, it is not used for gathering information about the on-premises data center.
D. AWS Database Migration Service (AWS DMS) - AWS DMS helps you migrate databases to AWS with minimal downtime. It supports homogeneous and heterogeneous migrations and can replicate data continuously to AWS so that you can perform cutover when you are ready. This service is focused on database migration rather than gathering information about the on-premises data center.
 


---

Q778. Which AWS service uses speech-to-text conversion to help users create meeting notes?
- A. Amazon Polly
- B. Amazon Textract
- C. Amazon Rekognition
- [x] D. Amazon Transcribe

---

> [!IMPORTANT]
> Q779. A company wants an AWS service that can automate software deployment in Amazon EC2 instances and on-premises instances. Which AWS service will meet this requirement?
- A. AWS CodeCommit
- B. AWS CodeBuild
- [x] C. AWS CodeDeploy
- D. AWS CodePipeline

To determine which AWS service can automate software deployment in Amazon EC2 instances and on-premises instances, let's evaluate each option:
A. AWS CodeCommit - AWS CodeCommit is a fully-managed source control service that hosts secure, private Git repositories. It is used for storing and managing code, but it does not automate software deployment.
B. AWS CodeBuild - AWS CodeBuild is a fully managed continuous integration service that compiles and tests your code whenever you push changes to your source control repository. It builds and tests your applications automatically, but it does not directly deploy them.
C. AWS CodeDeploy - AWS CodeDeploy is a fully managed deployment service that automates application deployments to various environments such as Amazon EC2 instances, on-premises instances, Lambda, and Amazon ECS services. It automates the deployment process, making it easier to quickly and reliably deploy applications.
D. AWS CodePipeline - AWS CodePipeline is a continuous integration and continuous delivery (CI/CD) service that builds and tests your code every time you make a change to your source code. It automates the build, test, and deploy processes, but it relies on other AWS services (like AWS CodeDeploy) to handle the actual deployment.
Based on the evaluation, the AWS service that will meet the requirement to automate software deployment in Amazon EC2 instances and on-premises instances is:
C. AWS CodeDeploy

---

Q780. A company needs to run some of its workloads on premises to comply with regulatory guidelines. The company wants to use the AWS Cloud to run workloads that are not required to be on premises. The company also wants to be able to use the same API calls for the on-premises workloads and the cloud workloads. Which AWS service or feature should the company use to meet these requirements?
- A. Dedicated Hosts
- [x] B. AWS Outposts
- C. Availability Zones
- D. AWS Wavelength

---

Q781. A company hosts a web application on AWS. The company has improved the availability of its application by provisioning multiple Amazon EC2 instances. The company wants to distribute its traffic across the EC2 instances while providing a single point of contact to the web clients. Which AWS service can distribute the traffic to multiple EC2 instances as targets?
- A. VPC endpoints
- [x] B. Application Load Balancer
- C. NAT gateway
- D. Internet gateway

---

Q782. Which design principle is related to the reliability pillar according to the AWS Well-Architected Framework?
- [x] A. Test recovery procedures 
- B. Experiment more often  (performance)
- C. Go global in minutes (performance)
- D. Analyze and attribute to expenditure (cost optimization)

---

Q783. A company wants to build graph queries for real-time fraud pattern detection. Which AWS service will meet this requirement?
- [x] A. Amazon Neptune
- B. Amazon DynamoDB
- C. Amazon Timestream
- D. Amazon Forecast

The AWS service that will meet the requirement of building graph queries for real-time fraud pattern detection is A. Amazon Neptune.
Here's why Amazon Neptune is the correct choice:
Graph Database: Amazon Neptune is a fast, fully managed graph database service that makes it easy to build and run applications that work with highly connected data. It is designed for graph workloads and provides fast query performance and low latency.
Graph Query Language: Amazon Neptune supports open graph APIs such as Apache TinkerPop (Gremlin) and W3C's RDF, SPARQL, and property graph query languages. This allows you to build complex graph queries to detect fraud patterns in real-time.
Real-Time Fraud Detection: By using Amazon Neptune, you can store and query highly connected data, such as transaction networks, user behavior patterns, and other relevant information, to identify fraud patterns in real-time. This helps in promptly addressing fraudulent activities and minimizing losses.
The other options provided are not suitable for this requirement:
B. Amazon DynamoDB: DynamoDB is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability. However, it is not designed for graph workloads and does not support graph query languages.
C. Amazon Timestream: Timestream is a fast, scalable, fully managed time series database service that makes it easy to analyze and query trillions of time series data points per second. It is primarily used for time series analysis and is not suitable for graph queries.
D. Amazon Forecast: Forecast is a fully managed service that uses machine learning to deliver highly accurate and scalable predictions. It is designed for forecasting future events based on historical data, but it does not support graph queries for real-time fraud pattern detection.
Therefore, Amazon Neptune is the most suitable AWS service for building graph queries for real-time fraud pattern detection.

---

> [!IMPORTANT]
> Q784. A company wants to deploy a web application as a containerized application. The company wants to use a managed service that can automatically create container images from source code and deploy the containerized application. Which AWS service will meet these requirements?
- A. AWS Elastic Beanstalk
- B. Amazon Elastic Container Service (Amazon ECS)
- [x] C. AWS App Runner
- D. Amazon EC2

  
Containerized Application Deployment: AWS App Runner is a fully managed service that makes it easy to deploy and operate scalable web applications and APIs at any scale. It automatically builds and deploys container images from source code repositories or container images stored in Amazon ECR.
Fully Managed Service: AWS App Runner abstracts away the underlying infrastructure, allowing you to focus on writing code and configuring your application. It automatically scales your application up or down based on incoming traffic.
Source-to-URL: AWS App Runner supports a source-to-URL workflow, where you can provide a link to your source code repository (e.g., GitHub), and it will automatically build and deploy your application as a containerized service.
 
A. AWS Elastic Beanstalk: Elastic Beanstalk is a platform as a service (PaaS) that provides an environment in which you can deploy and manage scalable web applications. However, it does not automatically build container images from source code and deploy them as containerized applications. Instead, it supports multiple deployment environments, including EC2 instances and Docker containers, but it requires more manual configuration and management.
B. Amazon Elastic Container Service (Amazon ECS): ECS is a highly scalable, fast, container management service that supports Docker containers. However, it requires you to manually build and push container images to Amazon ECR, and then deploy them to ECS clusters. It does not provide an automated source-to-URL workflow.
D. Amazon EC2: EC2 is a virtual computing environment that provides scalable computing capacity in the AWS Cloud. It allows you to run applications on Amazon-provided infrastructure. However, it does not provide a managed service for automatically building and deploying container images from source code. You would need to manually set up and manage EC2 instances, Docker containers, and other infrastructure components.
Therefore, AWS App Runner is the most suitable AWS service for deploying a containerized application, automatically creating container images from source code, and deploying the containerized application as a managed service.

---

Q785. A company has moved all its infrastructure to the AWS Cloud. To plan ahead for each quarter, the finance team wants to track the cost and usage data of all resources from previous months. The finance team wants to automatically generate reports that contains the data.  Which AWS service or feature should the finance team use to meet these requirements?  
- A. Amazon Detective  
- B. AWS Pricing Calculator  
- [x] C. AWS Budgets  
- D. AWS Savings Plans  

---

> [!IMPORTANT]
> Q786. Which AWS Cloud Adoption Framework (AWS CAF) perspective focuses on real-time insights and answers questions about strategy?  
- A. Operations  
- B. People  
- [x] C. Business  (business insights)
- D. Platform  

---

Q787. A company has multiple SQL-based databases located in a data center. The company needs to migrate all database servers to the AWS Cloud to reduce the cost of operating physical servers. Which AWS service or resource will meet these requirements with the LEAST operational overhead?  
- A. Amazon EC2 instances  
- [x] B. Amazon RDS  
- C. Amazon DynamoDB  
- D. OpenSearch



---


Q788 is the same as Q713. 


---

> [!IMPORTANT]
> Q789. A company needs to run an application on Amazon EC2 instances without interruption. Which EC2 instance purchasing option will meet this requirement MOST cost-effectively?  
- [x] A. Standard Reserved Instances  
- B. Convertible Reserved Instances  
- C. On-Demand Instances  
- D. Spot Instances  

without other constraints


---

> [!IMPORTANT]
> Q790. A company wants a fully managed service that centralizes and automates data protection across AWS services and hybrid workloads. Which AWS service will meet these requirements?  
- A. AWS Artifact  
- [x] B. AWS Backup  
- C. AWS Batch  
- D. AWS Shield

 
A. AWS Artifact:
AWS Artifact is a centralized repository that provides access to third-party software licenses, contracts, and other documents. It is primarily used for managing software agreements and does not relate to data protection.
B. AWS Backup:
AWS Backup is a fully managed backup service that automates the backup of AWS resources and on-premises workloads. It centralizes the backup process, enabling customers to create, manage, and automate backups across AWS services such as EC2, RDS, DynamoDB, and EFS, as well as hybrid workloads. AWS Backup provides a unified view of backups, simplifies compliance, and reduces operational overhead.
C. AWS Batch:
AWS Batch is a fully managed service that enables developers, scientists, and engineers to run batch computing workloads on AWS. It automates the allocation and management of the underlying compute resources required for running these workloads at any scale. AWS Batch is not related to data protection.
D. AWS Shield:
AWS Shield is a managed DDoS protection service that provides continuous DDoS mitigation for AWS customers. It is designed to protect against the most sophisticated DDoS attacks and reduce the risk of downtime. AWS Shield does not provide data protection services.
Based on the analysis, the AWS service that meets the requirements for a fully managed service that centralizes and automates data protection across AWS services and hybrid workloads is B. AWS Backup. It offers a unified approach to managing backups, ensuring data protection across a wide range of AWS resources and hybrid workloads.


---

> [!IMPORTANT]
> Q791. A company plans to migrate its application from on premises to the AWS Cloud. The company needs to gather usage and configuration data for the application components. Which AWS service will meet these requirements?  
- A. AWS Database Migration Service (AWS DMS)  
- B. AWS Transfer Family  
- [x] C. AWS Application Discovery Service  
- D. AWS Global Accelerator  

---

Q792. Which AWS offering can analyze a company AWS environment to discover security vulnerabilities on Amazon EC2 instances?  
- [x] A. Amazon Inspector  
- B. Amazon Macie  
- C. AWS Shield Standard  
- D. Security groups  

---

Q793. A company plans to onboard new employees that will be working remotely. The company needs to set up Windows virtual desktops to create a working environment for the new employees. The employees must be able access the working environment from anywhere and by using their computer or a web browser. Which AWS service or feature will meet these requirements?  
- A. Dedicated Hosts  
- B. AWS Global Accelerator  
- [x] C. Amazon Workspaces  
- D. Amazon CloudFront  

---

Q794. Which AWS service supports MySQL database engines?  
- A. Amazon DynamoDB
- [x] B. Amazon RDS  
- C. Amazon DocumentDB (with MongoDB compatibility)  
- D. Amazon ElastiCache  

 


---


Q795 is the same as Q712.

---

Q796. A company wants to run its application's code without having to provision and manage servers. Which AWS service will meet this requirement?
- A. AWS Glue
- [x] B. AWS Lambda
- C. AWS CodeDeploy
- D. Amazon CodeGuru

---

> [!IMPORTANT]
> Q797. A company wants to allow its employees to work remotely from home. The company's employees use Windows or Linux desktops. The company's employees need access from anywhere and at anytime by using any supported devices. Which AWS service will meet these requirements?
- [x] A. Amazon Workspaces
- B. Amazon AppStream 2.0
- C. Amazon Keyspaces (for Apache Cassandra)
- D. AWS Cloud9

To address the company's requirements for allowing employees to work remotely from home using Windows or Linux desktops, with access anywhere and anytime via any supported devices, the most suitable AWS service is:
A. Amazon WorkSpaces
Here's why Amazon WorkSpaces meets these requirements:
Remote Desktop Access: Amazon WorkSpaces provides a managed, secure desktop-as-a-service (DaaS) solution that runs on AWS. Employees can access their virtual Microsoft Windows desktops from any supported device, anytime and anywhere.
Platform Support: Amazon WorkSpaces supports both Windows and Linux desktops, accommodating the company's employee preferences.
Flexibility and Scalability: The service can be easily scaled to meet the company's growing needs, providing a flexible solution for remote work.
Security: Amazon WorkSpaces offers built-in security features, including encryption and network isolation, ensuring that sensitive company data remains protected.
 
Amazon AppStream 2.0: While this service also allows for streaming applications to any device with a web browser, it is primarily designed for streaming desktop applications rather than full desktops. It may not provide the same level of control and customization as Amazon WorkSpaces.
Amazon Keyspaces (for Apache Cassandra): This service is a managed NoSQL database service that is fully compatible with Apache Cassandra. It is not suitable for providing remote desktop access to employees.
AWS Cloud9: AWS Cloud9 is a cloud-based integrated development environment (IDE) that lets developers write, run, and debug their code with just a browser. It is primarily designed for development work and does not meet the requirements for providing remote desktop access to employees.
Therefore, Amazon WorkSpaces is the most appropriate AWS service to meet the company's remote work requirements.


---

Q798. A company plans to launch an ecommerce website that contains many images for a product catalog. The company wants to keep the cost of running the website within a specific budget. Which AWS service or tool should the company use to monitor the ongoing costs of the website?
- [x] A. AWS Cost Explorer
- B. AWS SDKs
- C. EC2 Image Builder
- D. AWS CloudFormation

---

> [!IMPORTANT]
> Q799. A company has deployed several public applications behind Application Load Balancers. The company wants to improve the performance of the applications. Which AWS service will meet these requirements?
- [x] A. AWS Global Accelerator
- B. Amazon Connect
- C. Amazon ElastiCache
- D. Amazon CloudWatch

each Application Load Balancers serves as the single point of contact for clients


AWS Global Accelerator leverages the AWS global network to direct user traffic to the optimal AWS endpoint, reducing latency and improving throughput for your applications. It provides a global fixed entry point and intelligently routes traffic to the closest healthy Application Load Balancer, resulting in significant performance improvements for users worldwide. This service is specifically designed to enhance both the availability and speed of applications accessed over the internet.

Other options:

B. Amazon Connect is a cloud contact center service, not related to application performance.

C. Amazon ElastiCache improves performance for data access and caching, but not for global network routing or load balancer traffic.

D. Amazon CloudWatch is for monitoring and observability, not for directly improving application performance

---

Q800. A company is learning about the perspectives of the AWS Cloud Adoption Framework (AWS CAF). Which perspective of the AWS CAF addresses the strategy management capability?
- [x] A. Business perspective
- B. People perspective
- C. Governance perspective
- D. Operations perspective

---

Q801. A company wants to consolidate its call centers to improve the customer voice and chat experience with call center agents. Which AWS service or tool will meet these requirements?
- A. Amazon Simple Notification Service (Amazon SNS)
- B. AWS Support Center
- C. Amazon Cognito
- [x] D. Amazon Connect

---

> [!IMPORTANT]
> Q802. Which AWS service can migrate Amazon EC2 instances from one AWS Region to another?
- [x] A. AWS Application Migration Service
- B. AWS Database Migration Service (AWS DMS)
- C. AWS DataSync
- D. AWS Migration Hub
 
Automated Migration: AWS MGN is a highly automated direct migration (re-hosting) service that simplifies, accelerates, and reduces the cost of migrating applications to AWS. It allows for the direct migration of a large number of physical, virtual, or cloud servers without compatibility issues, performance interruptions, or excessive conversion windows.
Cross-Region Migration: MGN supports the migration of EC2 instances across different AWS regions. This is particularly useful for organizations that need to optimize their infrastructure for latency, cost, or regulatory requirements.
Comprehensive Migration Management: MGN provides a comprehensive set of tools and features for managing the migration process, including assessment, replication, synchronization, testing, and cutover. This ensures a smooth and seamless migration experience.
Now, let's consider the other options:
AWS Database Migration Service (AWS DMS): AWS DMS is a web service that helps you migrate databases to AWS. It supports migrations between various database engines and platforms, but it is primarily focused on database migration rather than EC2 instance migration.
AWS DataSync: AWS DataSync is a service that automates and accelerates data transfer to and from AWS Storage services. It is useful for moving large amounts of data between different storage solutions, but it is not designed for migrating EC2 instances.
AWS Migration Hub: AWS Migration Hub provides a centralized place to track and manage your migration projects. It integrates with various AWS migration services and tools to provide a comprehensive view of your migration activities. However, it does not perform the actual migration of EC2 instances.
In summary, AWS Application Migration Service (MGN) is the AWS service that can migrate Amazon EC2 instances from one AWS Region to another.



---

Q803. A company needs to block SQL injection attacks. Which AWS service or feature provides this functionality?
- [x] A. AWS WAF
- B. Network ACLs
- C. Security groups
- D. AWS Trusted Advisor


---

Q804. A company wants to run its application on Amazon EC2 instances. The company needs to keep the application on-premises to meet a compliance requirement. Which AWS offering will meet these requirements?
- A. Dedicated Instances
- B. Amazon CloudFront
- C. AWS Fargate
- [x] D. AWS Outposts

---

Q805. Which AWS service can manage permissions for AWS resources by using policies?
- A. Amazon Inspector
- B. Amazon Detective
- [x] C. AWS Identity and Access Management (IAM)
- D. Amazon GuardDuty

---

Q806. A company wants to deploy an application that stores data in a relational database. The company wants database tasks, such as automated backups and database snapshots, to be managed by AWS. Which AWS service will meet these requirements?
- A. Amazon DocumentDB
- [x] B. Amazon RDS
- C. Amazon Elastic Block Store (Amazon EBS)
- D. Amazon S3

<img width="847" alt="image" src="https://github.com/user-attachments/assets/21a20243-3826-43d8-aca1-342fc59b7634" />

---

Q807. Which AWS service or feature can be used to create a virtual network that is private and isolated in the AWS Cloud?
- A. AWS VPN
- B. AWS Regions
- C. Availability Zones
- [x] D. Amazon Virtual Private Cloud (Amazon VPC)

---

Q808. Which AWS Cloud Adoption Framework (AWS CAF) perspective includes the risk management capability?
- [x] A. Governance
- B. Business
- C. Operations
- D. People

---

Q809. A company needs an automated vulnerability management service that continually scans AWS workloads for software vulnerabilities. Which AWS service will meet these requirements?
- A. Amazon GuardDuty
- [x] B. Amazon Inspector
- C. AWS Security Hub
- D. AWS Shield


Amazon Inspector is an automated vulnerability management service that continually scans AWS workloads for software vulnerabilities and unexpected network exposures. It can scan Amazon Elastic Compute Cloud (EC2) instances, AWS Lambda functions, container images in Amazon Elastic Container Registry (ECR), and software in continuous integration and continuous delivery (CI/CD) tools. Amazon Inspector provides nearly real-time vulnerability results and helps prioritize responses by providing highly contextualized and meaningful risk scores for each finding.
 
A. Amazon GuardDuty - This is a threat detection service that continuously monitors for malicious or unauthorized behavior in your AWS environment. It does not focus on vulnerability management.
C. AWS Security Hub - AWS Security Hub provides you with a comprehensive view of your security alerts and compliance status across your AWS accounts. While it can integrate with vulnerability scanning tools like Amazon Inspector, it does not itself perform vulnerability scanning.
D. AWS Shield - AWS Shield is a DDoS protection service that provides protection against distributed denial-of-service (DDoS) attacks. It does not focus on vulnerability management.
 

---

Q810. A company needs to launch an Amazon EC2 instance. Which of the following can the company use during the launch process to configure the root volume of the EC2 instance?
- A. Amazon EC2 Auto Scaling
- B. Amazon Data Lifecycle Manager (Amazon DLM)
- [x] C. Amazon Machine Image (AMI)
- D. Amazon Elastic Block Store (Amazon EBS) volume

---

> [!IMPORTANT]
> Q811. A company needs to store data across multiple Availability Zones in an AWS Region. The data will not be accessed regularly but must be immediately retrievable. Which Amazon Elastic File System (Amazon EFS) storage class meets these requirements MOST cost-effectively?
- A. EFS Standard
- [x] B. EFS Standard-Infrequent Access (EFS Standard-IA)
- C. EFS One Zone
- D. EFS One Zone-Infrequent Access (EFS One Zone-IA)

https://docs.aws.amazon.com/efs/latest/ug/features.html#storage-classes
https://aws.amazon.com/efs/pricing/

---

> [!IMPORTANT]
> Q812. A company needs DDoS protection for its AWS resources. The company also needs proactive mitigation assistance from AWS if a DDoS attack occurs. Which AWS service will meet these requirements?
- A. Amazon GuardDuty
- B. AWS Network Firewall
- [x] C. AWS Shield Advanced
- D. AWS WAF
 
 real-time visibility into any DDoS attacks
access to shied response team
proactive mitigation assistance if a DDoS attack occurs

https://aws.amazon.com/shield/features/#topic-2
For higher levels of protection against attacks targeting your applications running on Amazon Elastic Compute Cloud (EC2), Elastic Load Balancing (ELB), Amazon CloudFront, AWS Global Accelerator, and Amazon Route 53 resources, you can subscribe to AWS Shield Advanced. 

In addition to the network and transport layer protections that come with Standard, Shield Advanced provides 
- additional detection and mitigation against large and sophisticated DDoS attacks,
- near real-time visibility into attacks,
- and integration with AWS WAF, a web application firewall.
- Shield Advanced also gives you 24/7 access to the AWS Shield Response Team (SRT) and protection against DDoS-related spikes in your EC2, ELB, CloudFront, Global Accelerator, and Route 53 charges.
- AWS Shield Advanced offers proactive engagement from the SRT when a DDoS event is detected. When you activate proactive engagement, the SRT will directly contact you if a Route 53 health check associated with your protected resource becomes unhealthy during a DDoS event.

---

Q813. Which AWS solution provides the ability for a company to run AWS services in the company's on-premises data center?
- A. AWS Direct Connect
- [x] B. AWS Outposts
- C. AWS Systems Manager hybrid activations
- D. AWS Storage Gateway

---

> [!IMPORTANT]
> Q814. Which AWS Trusted Advisor check category includes the AWS CloudTrail logging check?
- A. Service limits
- [x] B. Security
- C. Performance
- D. Fault tolerance

> CloudTrail increases traceability, which is a design principle of the security pillar
> AWS CloudTrail Logging
> AWS CloudTrail Management Event Logging
---

Q815. A company wants to reduce the cost of its Amazon EC2 instances. The applications that run on the instances cannot tolerate interruptions. The instances must remain in operation for at least 1 year. Which purchasing options should the company use to meet these requirements? (Select TWO.)
- [x] A. Reserved Instances
- B. Spot Instances
- C. AWS Marketplace subscriptions
- [x] D. Savings Plans
- E. Dedicated Hosts

---

Q816. Which Amazon EC2 instance purchasing option offers the LARGEST discount compared to the price of EC2 On-Demand Instances?
- A. Savings Plans
- [x] B. Spot Instances
- C. Reserved Instances
- D. Dedicated Hosts

---

Q817. A company needs a secure, encrypted connection between its data center workload and the AWS Cloud. The connection needs to use the public internet. Which AWS service will meet these requirements?
- A. AWS Direct Connect
- B. Amazon Connect
- [x] C. AWS Site-to-Site VPN
- D. AWS Client VPN

---

> [!IMPORTANT]
> Q818. Which AWS service, feature, or tool uses machine learning to continuously monitor cost and usage for unusual cloud spending?
- A. Amazon Lookout for Metrics
- B. AWS Budgets
- C. Amazon CloudWatch
- [x] D. AWS Cost Anomaly Detection

 
AWS Cost Anomaly Detection uses machine learning to continuously monitor your AWS cost and usage patterns. It automatically detects unusual spending and alerts you to potential anomalies, helping you manage and control your cloud costs effectively.
The other options do not specifically focus on anomaly detection for cost:
A. Amazon Lookout for Metrics: This service is designed for detecting anomalies in various metrics but is not specifically focused on AWS cost and usage.
B. AWS Budgets: This tool allows you to set budgets for your AWS costs and usage but does not use machine learning to detect anomalies.
C. Amazon CloudWatch: This service monitors AWS resources and applications but primarily focuses on performance and operational metrics, rather than specific cost anomalies.

---

Q819. A company wants to continuously monitor its AWS accounts and workloads for malicious activity. The company also wants to receive detailed security findings for visibility and remediation. Which AWS service should the company use to meet these requirements?
- [x] A. Amazon GuardDuty
- B. AWS Shield
- C. AWS WAF
- D. AWS CloudTrail

 
Amazon GuardDuty is a threat detection service that continuously monitors AWS accounts and workloads for malicious activity. It uses machine learning, anomaly detection, and integrated threat intelligence to identify potential security threats and provides detailed security findings, which helps organizations gain visibility and take remediation actions.
 
B. AWS Shield: This service provides DDoS protection but does not focus on continuous monitoring for malicious activity.
C. AWS WAF: The AWS Web Application Firewall helps protect web applications from common web exploits but does not provide continuous monitoring or detailed findings about malicious activity across AWS accounts.
D. AWS CloudTrail: This service logs AWS account activity for auditing and compliance but is not primarily focused on real-time security threat detection or providing security findings.

---

Q820. Which AWS service can provide the documents?
- A. AWS Trusted Advisor
- [x] B. AWS Artifact
- C. AWS Well-Architected Tool
- D. AWS Systems Manager

---

> [!IMPORTANT]
> Q821. Which of the following are benefits of Amazon EC2 Auto Scaling? (Select TWO.)
- [x] A. Improved health and availability of applications
- B. Reduced network latency
- [x] C. Optimized performance and costs
- D. Automated snapshots of data
- E. Cross-Region Replication.

>  can be cross-zone but not cross-region


B. Reduced network latency - While scaling can potentially help distribute load and improve response times, it doesn't specifically reduce network latency. Latency is often influenced by factors such as geographical proximity and network infrastructure.
 


---

Q822. A company needs to collect performance metrics about its Amazon RDS instances and Amazon EC2 instances. Which AWS service meets this requirement?
- A. AWS CloudTrail
- [x] B. Amazon CloudWatch
- C. Amazon Inspector
- D. AWS Config

---

Q823. A cloud practitioner needs to design a NoSQL database that is highly scalable, is durable, and requires minimal maintenance. Which AWS service meets these requirements?
- A. Amazon RDS for MySQL
- B. Microsoft SQL Server on Amazon EC2
- [x] C. Amazon DynamoDB
- D. Amazon Redshift

---

> [!IMPORTANT]
> Q824. A company is planning a migration to AWS. The company wants to modernize its applications by refactoring the applications to microservices. Which AWS service or feature should the company use to achieve this goal?
- [x] A. AWS Migration Hub Refactor Spaces
- B. AWS Application Migration Service
- C. AWS Database Migration Service (AWS DMS)
- D. AWS Compute Optimizer


> AWS Application Migration Service (MGN) is a highly automated lift-and-shift (rehost) solution 
---

Q825. Which AWS service gives a company the ability to use a private, dedicated connection between a VPC and an on-premises data center?
- [x] A. AWS Direct Connect
- B. Amazon API Gateway
- C. AWS Systems Manager
- D. AWS CloudFormation

---

> [!IMPORTANT]
> Q826. What are some advantages of using Amazon EC2 instances to host applications in the AWS Cloud instead of on premises? (Select TWO.)
- A. EC2 includes operating system patch management.
- [x] B. EC2 integrates with Amazon VPC, AWS CloudTrail, and AWS Identity and Access Management (IAM).
- C. EC2 has a 100% service level agreement (SLA).
- [x] D. EC2 has a flexible, pay-as-you-go pricing model.
- E. EC2 has automatic storage cost optimization.

> Not 100% SLA; can guarantee 99.99% availability for certain instance types in a specific AZ. 
> doesn't have automatic storage cost optimization. customers are resposible for managing their storage costs
---

Q827. A company needs to request temporary, limited-privilege credentials for IAM users and for the federated users that the company authenticates. Which AWS service will provide these credentials?
- A. Amazon GuardDuty
- B. AWS Key Management Service (AWS KMS)
- [x] C. AWS Security Token Service (AWS STS)
- D. AWS Identity and Access Management Access Analyzer

---

> [!IMPORTANT]
> Q828. A company needs centralized storage to manage the configuration data and passwords for its applications. Which AWS service or capability will meet these requirements?
- A. AWS CodeArtifact
- B. AWS Config
- C. AWS Security Hub
- [x] D. AWS Systems Manager Parameter Store

 
AWS Systems Manager Parameter Store provides a centralized, secure, and scalable way to manage configuration data, secrets, and passwords across your applications and services. It allows you to store parameters as plain text or securely encrypted values, and it integrates with AWS Identity and Access Management (IAM) to provide fine-grained access control.
Let's look at the other options:
A. AWS CodeArtifact
AWS CodeArtifact is a fully managed repository service that makes it easy for you to share packages with your team and consume packages from public and third-party repositories. It supports popular package formats such as Maven, npm, and PyPI. CodeArtifact does not provide centralized storage for configuration data and passwords.
B. AWS Config
AWS Config is a service that enables you to assess, audit, and evaluate the configurations of your AWS resources. It provides you with a detailed view of the configuration of your resources and allows you to track changes over time. AWS Config does not provide centralized storage for configuration data and passwords.
C. AWS Security Hub
AWS Security Hub is a comprehensive security and compliance management service that provides you with a unified view of your security alerts and compliance checks across AWS accounts. It integrates with a variety of AWS services and third-party security tools to aggregate, prioritize, and take action on security findings. AWS Security Hub does not provide centralized storage for configuration data and passwords.
Therefore, the correct answer for this question is D, AWS Systems Manager Parameter Store.

---

> [!IMPORTANT]
> Q829. A company manages global applications that require static IP addresses. Which AWS service would enable the company to improve the availability and performance of its applications?
- A. Amazon CloudFront
- [x] B. AWS Global Accelerator
- C. Amazon S3 Transfer Acceleration
- D. Amazon API Gateway

> static IP addresses
 
AWS Global Accelerator directs traffic to optimal endpoints across multiple AWS Regions, improving the availability and performance of your applications. It provides static IP addresses that you can use to route traffic to your application across AWS Regions. Global Accelerator automatically routes traffic to the optimal endpoint based on health, latency, and other metrics.
Let's look at the other options:
A. Amazon CloudFront
Amazon CloudFront is a global content delivery network (CDN) service that accelerates delivery of your websites, APIs, video content, or other assets. It integrates with other AWS services to provide a secure, highly scalable, and low-latency global content delivery solution. However, CloudFront does not provide static IP addresses for routing traffic.
C. Amazon S3 Transfer Acceleration
Amazon S3 Transfer Acceleration enables faster transfers of files over long distances between your client and an S3 bucket. It uses the AWS global network to route transfers through an optimized path, which can result in faster data transfer speeds compared to transfers over the public internet. However, S3 Transfer Acceleration is specifically for S3 buckets and does not provide static IP addresses for routing traffic to other types of applications.
D. Amazon API Gateway
Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. It provides a way to create RESTful APIs, WebSocket APIs, and HTTP APIs that act as the "front door" for applications to access data, business logic, or functionality from your backend services. However, API Gateway does not provide static IP addresses for routing traffic to your applications.
Therefore, the correct answer for this question is B, AWS Global Accelerator.

---

Q830. Which capabilities are in the operations perspective of the AWS Cloud Adoption Framework (AWS CAF)? (Select TWO.)
- [x] A. Observability (operations)
- B. Portfolio management (business)
- C. Incident response (security)
- D. Data governance (governance)
- [x] E. Configuration management (operations)

---

> [!IMPORTANT]
> Q831. Which AWS service or resource can distribute TCP and UDP traffic?
- A. Amazon API Gateway
- B. Application Load Balancer
- [x] C. Network Load Balancer
- D. Gateway Load Balancer

 
Network Load Balancer (NLB): This load balancer operates at the transport layer (Layer 4) of the OSI model and is specifically designed to route TCP and UDP traffic. It is capable of distributing network traffic to multiple targets, such as Amazon EC2 instances or IP addresses, and is highly effective for handling large volumes of traffic.
Amazon API Gateway: While API Gateway is a powerful service for creating, publishing, maintaining, monitoring, and protecting APIs, it is primarily focused on managing API traffic at the application layer (Layer 7). It does not distribute raw TCP or UDP traffic.
Application Load Balancer (ALB): ALB also operates at the application layer and is optimized for HTTP and HTTPS traffic. It provides advanced routing features, such as path-based routing and host-based routing, which are not relevant for raw TCP or UDP traffic.
Gateway Load Balancer: This option is not a valid AWS service name. AWS offers several types of load balancers, but "Gateway Load Balancer" is not one of them. In summary, if you need to distribute TCP and UDP traffic in AWS, you should use a Network Load Balancer.

---

Q832. A financial company needs to centrally manage its AWS accounts and use consolidated billing. Which AWS service or feature should the company use?
- A. AWS Cost Explorer
- [x] B. AWS Organizations
- C. AWS Billing and Cost Management
- D. AWS Budgets

---

Q833. A company is using Amazon EC2 instances to test an application. The company needs to run uninterrupted tests for 1 month. Which EC2 instance purchasing option will meet these requirements MOST cost-effectively?
- [x] A. On-Demand Instances
- B. Spot Instances
- C. Reserved Instances
- D. Compute Savings Plan

---

Q834. Which AWS service will turn text into lifelike speech?
- [x] A. Amazon Polly
- B. Amazon Rekognition
- C. Amazon Connect
- D. Amazon Kendra

---

> [!IMPORTANT]
> Q835. A company needs to collect and assess on-premises server and application inventory data before moving its infrastructure to AWS. Which AWS service provides this functionality?
- A. Amazon AppFlow
- [x] B. AWS Migration Hub
- C. Amazon QuickSight
- D. AWS Step Functions
 
AWS Migration Hub is a centralized service that provides a single place to track the migration status of applications, servers, and databases being moved to AWS. It integrates with a variety of AWS and third- party migration tools and services, offering a comprehensive view of migration activities and progress.
Here's a brief analysis of the other options:
A. Amazon AppFlow - Amazon AppFlow is a fully managed service that enables secure and scalable data transfers between AWS services and third-party applications. It automates data flows and supports data synchronization and replication across multiple data sources and destinations. However, it is not specifically designed for collecting and assessing on-premises server and application inventory data before migration.
C. Amazon QuickSight - Amazon QuickSight is a business intelligence (BI) service that makes it easy to build visual analytics and dashboards in the cloud. It allows users to create interactive dashboards and perform data analysis using a variety of data sources. While it can be used for data visualization and analysis, it is not used for collecting and assessing on-premises server and application inventory data before migration.
D. AWS Step Functions - AWS Step Functions is a serverless workflow service that lets you coordinate the steps of distributed applications and microservices using visual workflows. It enables you to build and run complex workflows that combine multiple AWS services and third-party APIs. However, it is not used for collecting and assessing on-premises server and application inventory data before migration.
In summary, AWS Migration Hub is the AWS service that provides the functionality to collect and assess on-premises server and application inventory data before moving the infrastructure to AWS.


---

Q836. A company's user base needs to remotely access virtual desktop computers from the internet. Which AWS service provides this functionality?
- A. Amazon Connect
- B. Amazon Cognito
- [x] C. Amazon WorkSpaces
- D. Amazon AppStream 2.0

---

Q837. Which AWS services and features are provided to all customers at no charge? (Select TWO.)
- A. Amazon Aurora
- [x] B. VPC
- C. Amazon SageMaker
- [x] D. AWS Identity and Access Management (IAM)
- E. Amazon Polly

---

> [!IMPORTANT]
> Q838. Which AWS services can a company use to transfer on-premises data to the AWS Cloud? (Select TWO.)
- [x] A. AWS Snowcone
- B. AWS Transit Gateway
- [x] C. AWS DataSync
- D. AWS Backup
- E. Amazon Connect


  
A. AWS Snowcone - AWS Snowcone is a rugged, tamper-evident, and portable data transfer device that allows companies to securely transfer large amounts of data into and out of AWS. It is designed for environments with limited network bandwidth, such as remote offices or edge locations. With AWS Snowcone, companies can physically transport data to AWS using a secure device.
C. AWS DataSync - AWS DataSync is a fully managed data transfer service that simplifies, automates, and accelerates moving and replicating data between on-premises storage and AWS storage services, as well as between AWS storage services. It uses high-speed data transfer protocols and intelligent data deduplication to optimize data transfer performance and reduce costs. With AWS DataSync, companies can transfer data over the network without the need for physical devices.
The other options, B, D, and E, are not designed for transferring on-premises data to the AWS Cloud:
B. AWS Transit Gateway - AWS Transit Gateway is a network transit hub that connects Amazon VPCs, on- premises networks, and remote networks using BGP. It provides optimized routing and redundancy, but it is not a data transfer service.
D. AWS Backup - AWS Backup is a centralized backup service that helps companies automate and manage backups across AWS services. It is not designed for transferring data between on-premises and AWS.
E. Amazon Connect - Amazon Connect is an omnichannel cloud contact center service that helps companies deliver better customer service. It is not a data transfer service.
In summary, the AWS services that a company can use to transfer on-premises data to the AWS Cloud are AWS Snowcone and AWS DataSync.


The AWS services that a company can use to transfer on-premises data to the AWS Cloud are:
A. AWS Snowcone - AWS Snowcone is a small, rugged, and secure data transfer device that allows customers to transfer large amounts of data into and out of AWS. It is designed for customers who need to move data that is too large to move over the internet or who have limited connectivity.
C. AWS DataSync - AWS DataSync is a fully managed data transfer service that simplifies, automates, and accelerates moving and replicating data between on-premises storage and AWS storage services. It provides a simple, scalable, and cost-effective way to transfer data at high speeds and with high reliability.
Here's a brief analysis of the other options:
B. AWS Transit Gateway - AWS Transit Gateway is a network transit hub that allows customers to connect their Amazon VPCs and on-premises networks to a single, centralized gateway. While it provides a way to connect on-premises networks to AWS, it is not used for data transfer itself.
D. AWS Backup - AWS Backup is a centralized and automated backup service that makes it easy to protect data across AWS services. It provides a unified view of backups and enables point-in-time recovery for many AWS services. However, it is not used for transferring on-premises data to AWS.
E. Amazon Connect - Amazon Connect is a cloud-based contact center solution that provides an easy-to- use interface for building customer service and support operations. It is designed for handling customer interactions and is not used for transferring on-premises data to AWS.
In summary, AWS Snowcone and AWS DataSync are the AWS services that a company can use to transfer on-premises data to the AWS Cloud.


---

Q839. A company wants to control the protection of its AWS resources. The company wants to block SQL injection attacks and cross-site scripting. Which AWS service or feature meets these requirements?
- A. Amazon GuardDuty
- [x] B. AWS WAF
- C. Security groups
- D. AWS Shield

---

Q840. Which capabilities are in the platform perspective of the AWS Cloud Adoption Framework (AWS CAF)? (Select TWO.)
- A. Data protection (security)
- B. Data governance (governance)
- [x] C. Data architecture (platform)
- [x] D. Data engineering (platform)
- E. Data science (business)

---


Q841. A company needs to gain data insights by using natural language to ask questions about its data.  Which AWS service provides this functionality?
- A. AWS Glue
- B. Amazon SageMaker
- [x] C. Amazon QuickSight
- D. AWS Panorama
 
Amazon QuickSight is an interactive, serverless business analytics service in the AWS Cloud that makes it easy to build visualizations, perform ad-hoc analysis, and quickly get business insights from your data. One of its key features is the ability to use natural language queries to ask questions about your data and receive visual answers.
Here's a brief explanation of the other options:
AWS Glue is a serverless data integration service that makes it easy to discover, prepare, and combine data for analytics. It is not used for querying data using natural language. 


AWS Panorama is a fully managed service that makes it easy to deploy computer vision applications at the edge. It uses AWS IoT Greengrass to run applications on edge devices, and it does not support natural language querying of data.
 
 
---

Q842. Which option is the responsibility of AWS, according to the AWS shared responsibility model?
- A. Management of guest operating systems
- B. Firewall configuration changes
- [x] C. Hardware for compute resources
- D. Identity and access management

---

Q843. A company runs a web application on Amazon EC2 instances. The application has consistent usage and is expected to run indefinitely. Which EC2 instance purchasing option will meet these requirements MOST cost-effectively?
- A. 1-year All Upfront Reserved Instances
- B. 1-year No Upfront Reserved Instances
- [x] C. 3-year All Upfront Reserved Instances
- D. 3-year No Upfront Reserved Instances

---

Q844. Which option is a pillar of the AWS Well-Architected Framework?
- A. Patch management
- [x] B. Cost optimization
- C. Business technology strategy
- D. Physical and environmental controls

---

Q845. A company needs to create and manage a portfolio of IT workloads that the company approves for use on AWS.  Which AWS service provides this functionality?
- A. AWS Config
- [x] B. AWS Service Catalog
- C. AWS Systems Manager
- D. AWS CloudFormation

---

Q846. A company uses AWS and has a VPC that includes two public subnets. The company needs to allow and deny specific inbound and outbound traffic for each public subnet. Which AWS service or tool can the company use to meet this requirement?
- [x] A. Network ACL
- B. AWS WAF
- C. VPC route table entry
- D. Security group

---

> [!IMPORTANT]
> Q847. Which AWS service should a user use to change an AWS account root user password?
- A. AWS IAM Identity Center
- [x] B. AWS Management Console
- C. AWS Secrets Manager
- D. AWS Security Hub
 
AWS IAM Identity Center (formerly AWS Single Sign-On (SSO)) is primarily used for managing and controlling access to multiple AWS accounts and applications through a single sign-on experience. It doesn't directly allow changing the root user password.

AWS Management Console is the web-based interface provided by AWS for managing AWS services. Users can log in to the AWS Management Console with their root user credentials and change the root user password through the IAM (Identity and Access Management) service settings. 

AWS Secrets Manager is a service that helps you manage, retrieve, and rotate API keys, passwords, certificates, and other secrets securely. It's not used for changing root user passwords. 

AWS Security Hub provides a comprehensive view of your security alerts and compliance status across your AWS accounts. It integrates with AWS security services and third-party products to provide unified insights and recommendations to improve your security posture. It does not provide functionality to change root user passwords.
Thus, the AWS Management Console is the correct choice for changing an AWS account root user password.

---

Q848. Which tasks are the responsibility of AWS, according to the AWS shared responsibility model? (Select TWO.)
- [x] A. Patch AWS network devices.
- B. Set user password rules.
- [x] C. Provide physical security for compute resources.
- D. Configure security groups.
- E. Patch the operating system of an Amazon EC2 instance.

---

> [!IMPORTANT]
> Q849. A company needs to automate operations to update its applications in production. The company must use automated deployments and rollbacks. Which AWS service provides this functionality?
- A. Amazon CodeGuru
- B. AWS CodePipeline
- [x] C. AWS CodeDeploy
- D. AWS CodeBuild
 
AWS CodeDeploy is a service that automates the deployment of applications to Amazon EC2 instances, on-premises instances, or serverless compute services like AWS Lambda. It supports various deployment methods, including in-place updates, blue/green deployments, and canary releases. CodeDeploy also allows for automated rollbacks in case of deployment failures, ensuring that the application can quickly revert to a stable state.

Amazon CodeGuru is a service that provides machine learning-based recommendations for improving the quality and performance of code. It helps developers identify issues, such as potential bugs, and suggests optimizations, but it does not handle deployment automation. 

AWS CodePipeline is a continuous integration and continuous delivery (CI/CD) service that automates the build, test, and deployment phases of application development. While it can orchestrate the entire CI/CD workflow, it relies on other services like CodeDeploy for the actual deployment and rollback functionality. 

AWS CodeBuild is a fully managed build service that compiles and tests your source code and produces artifacts that you can deploy. It can be integrated with CodePipeline for automated builds, but it does not handle deployments or rollbacks.
 

---

> [!IMPORTANT]
> Q850. A company needs to perform a one-time migration of 50 TB of data from on-premises storage to AWS. Which AWS service will meet this requirement with the LEAST operational overhead?
- A. Amazon S3
- [x] B. AWS Snowball Edge
- C. AWS Database Migration Service (AWS DMS)
- D. Amazon Elastic Block Store (Amazon EBS)

---
Q851. Which AWS services can help reduce application latency and improve performance by using edge locations? (Select TWO.)
- A. Amazon Route 53
- [x] B. AWS Global Accelerator
- C. AWS Direct Connect
- D. Amazon Connect
- [x] E. Amazon CloudFront

---

> [!IMPORTANT]
> Q852. A web developer wants to use machine learning to classify images that are uploaded to a website. Which AWS service or feature will meet these requirements?
- [x] A. Amazon Rekognition
- B. Amazon SageMaker Clarify
- C. Amazon Mechanical Turk
- D. Amazon Transcribe

The AWS service that will meet the requirements for a web developer to use machine learning to classify images that are uploaded to a website is:
A. Amazon Rekognition
Here's why:
Amazon Rekognition is a fully managed service that uses machine learning to analyze images and video. It can identify objects, scenes, activities, people, text, and more in images and video. For the use case of classifying images uploaded to a website, Amazon Rekognition can be used to detect and label objects in the images, or to recognize specific faces or scenes.

Amazon SageMaker Clarify is a feature of Amazon SageMaker, a fully managed service that provides every developer and data scientist with the ability to build, train, and deploy machine learning models at any scale. SageMaker Clarify helps you understand the biases and fairness of your machine learning models, but it is not a service for image classification.

Amazon Mechanical Turk is a web service that provides an on-demand, scalable workforce to perform Human Intelligence Tasks (HITs). While it can be used for various tasks, such as image labeling, it is not a fully managed machine learning service for image classification.
 

---

Q853 is the same as Q3.

---

> [!IMPORTANT]
> Q854. Which AWS service provides automated backups of data by default?
- A. Amazon S3
- [x] B. Amazon Aurora
- C. Amazon ElastiCache (Memcached)
- D. Amazon Elastic File System (Amazon EFS)

B. Amazon Aurora (Answer)	✅ Yes	- Automatic daily backups during the backup window (1-35 days retention).
- Continuous incremental backups to S3 with point-in-time recovery (PITR).
- Enabled by default with no additional configuration needed.
A. Amazon S3	❌ No	- Requires manual enablement of versioning for object recovery.
- Cross-region replication must be explicitly configured.
C. Amazon ElastiCache (Memcached)	❌ No	- Memcached engines do not support persistence or backups.
- Data is purely in-memory and volatile.
D. Amazon EFS	❌ No	- Backups must be manually initiated via EFS-to-EFS backup or AWS Backup.
- No automatic backup schedule unless configured.

  
---

Q855. A company needs steady and predictable performance from its Amazon EC2 instances at the lowest possible cost. The company also needs the ability to scale resources to ensure that it has the right resources available at the right time. Which AWS service or resource will meet these requirements?
- A. Amazon CloudWatch
- B. Application Load Balancer
- C. AWS Batch
- [x] D. Amazon EC2 Auto Scaling

---

Q856. A company needs to set up a petabyte-scale data warehouse in the AWS Cloud. Which AWS service will meet this requirement?
- A. Amazon DynamoDB
- B. Amazon RDS
- [x] C. Amazon Redshift
- D. Amazon ElastiCache

---

Q857. A company wants to deploy its critical application on AWS and maintain high availability. How should the company deploy the application to meet these requirements?
- A. In a single Availability Zone
- B. On AWS Direct Connect
- C. On Reserved Instances
- [x] D. In multiple Availability Zones

---

Q858. Which AWS service requires the customer to be fully responsible for applying operating system patches?
- A. Amazon DynamoDB
- B. AWS Lambda
- C. AWS Fargate
- [x] D. Amazon EC2

---

Q859. A company needs to store data in an Amazon S3 bucket. The company will rarely access the data and can recreate the data if necessary. Which S3 storage class will meet the requirements for this data MOST cost-effectively?
- A. S3 Express One Zone
- [x] B. S3 One Zone-Infrequent Access (S3 One Zone-IA)
- C. S3 Standard
- D. S3 Standard-Infrequent Access (S3 Standard-IA)

---

Q860. A company runs critical workloads on AWS. The company needs a response from AWS technical support within 15 minutes if a critical system goes down. Which AWS Support plan offers this response time?
- A. AWS Basic Support
- B. AWS Business Support
- [x] C. AWS Enterprise Support
- D. AWS Developer Support

> AWS Enterprise Support: Business-critical system down: < 15 minutes

---

> [!IMPORTANT]
> Q861. A company needs to analyze more than 200,000 financial records that are generated each day. The company must use containerized applications to perform the analysis and automate the process. Which AWS service will meet these requirements?
- A. Amazon Athena
- B. AWS Database Migration Service (AWS DMS)
- [x] C. AWS Batch
- D. AWS Systems Manager

 
AWS Batch is a fully managed service that enables developers, scientists, and engineers to run batch computing workloads on AWS. It dynamically allocates the compute resources required for the batch jobs, optimizes the workload for cost and speed, and scales the compute resources up or down automatically based on the requirements of the workload. With AWS Batch, the company can use containerized applications to perform the analysis of financial records and automate the process.
 
A. Amazon Athena - Amazon Athena is an interactive query service that makes it easy to analyze data directly in Amazon S3 using standard SQL. It is not designed for running batch computing workloads or containerized applications.
B. AWS Database Migration Service (AWS DMS) - AWS DMS helps you migrate databases to AWS. It supports homogeneous and heterogeneous migrations and can replicate your data continuously with minimal downtime. However, it is not designed for running batch computing workloads or containerized applications.
D. AWS Systems Manager - AWS Systems Manager provides a unified view of your AWS resources, including EC2 instances, on-premises servers, and virtual machines. It enables you to automate operations, secure and manage your resources, and gain insights into your applications. However, it is not specifically designed for running batch computing workloads or containerized applications.
 

---

Q862 is the same as Q838. 

---

> [!IMPORTANT]
> Q863. A company needs a low-code, visual workflow service that developers can use to build distributed applications. Which AWS service is designed to meet these requirements?
- [x] A. AWS Step Functions
- B. AWS Config
- C. AWS Lambda
- D. Amazon CloudWatch

keywords: low-code; visual

---

> [!IMPORTANT]
> Q864. Which AWS Cloud Adoption Framework (AWS CAF) perspective helps a company achieve confidentiality and integrity of its data?
- A. Business
- [x] B. Security
- C. Governance
- D. Operations

---

Q865. Which AWS service tracks API calls and user activity?
- A. AWS Organizations
- B. AWS Config
- C. Amazon CloudWatch
- [x] D. AWS CloudTrail

---

> [!IMPORTANT]
> Q866. A company needs to publish and manage web services by using a digital interface. Which AWS service provides this functionality?
- A. AWS App Mesh
- [x] B. Amazon API Gateway
- C. AWS Lambda
- D. AWS Cloud Map

 
Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. It provides a way to create RESTful APIs, WebSocket APIs, and HTTP APIs that act as the "front door" for applications to access data, business logic, or functionality from your backend services.
Let's review the other options:
A. AWS App Mesh is a service mesh that provides application-level networking to make microservices easier to build and operate. It is not used for publishing and managing web services via a digital interface. 

C. AWS Lambda is a compute service that lets you run code without provisioning or managing servers. While Lambda can be integrated with API Gateway to handle API requests, it does not provide the functionality to publish and manage web services.
D. AWS Cloud Map is a service discovery solution that makes it easy for microservices, containers, and applications to discover and connect to each other across multiple environments. It is not used for publishing and managing web services via a digital interface. Therefore, the correct answer is B. Amazon API Gateway, as it provides the functionality to publish and manage web services by using a digital interface.

---

Q867. Which statement describes a characteristic of the AWS global infrastructure?
- A. Edge locations contain multiple AWS Regions.
- B. AWS Regions contain multiple Regional edge caches.
- [x] C. Availability Zones contain multiple data centers.
- D. Each data center contains multiple edge locations.

---

> [!IMPORTANT]
> Q868. A company owns per-core software licenses. Which Amazon EC2 instance purchasing option must the company use for this license type?
- A. Reserved Instances
- [x] B. Dedicated Hosts
- C. Spot Instances
- D. Dedicated Instances

---

Q869. A company needs to deploy Amazon EC2 instances from a component that defines the operating system and includes pre-installed applications. Which AWS service or feature should the company use to meet this requirement?
- A. Security group
- B. Elastic network interface
- C. Amazon Elastic Block Store (Amazon EBS)
- [x] D. Amazon Machine Image (AMI)

---

Q870. A company is building an application in the AWS Cloud. The company wants to use temporary credentials for the application to access other AWS resources. Which AWS service will meet these requirements?
- A. AWS Key Management Service (AWS KMS)
- B. AWS CloudHSM
- C. Amazon Cognito
- [x] D. AWS Security Token Service (AWS STS)

---

> [!IMPORTANT]
> Q871. A security engineer wants a single-tenant AWS solution to create, control, and manage their own cryptographic keys to meet regulatory compliance requirements for data security.  
Which AWS service should the engineer use?
- A. AWS Key Management Service (AWS KMS)
- B. AWS Certificate Manager (ACM)
- [x] C. AWS CloudHSM
- D. AWS Systems Manager
 
> AWS CloudHSM: Manage single-tenant hardware security modules (HSMs) on AWS

> AWS KMS has a multi-tenant design 

---

Q872. A company needs to establish a connection between two VPCs. The VPCs are located in two different AWS Regions. The company wants to use the existing infrastructure of the VPCs for this connection. Which AWS service or feature can be used to establish this connection?
- A. AWS Client VPN
- [x] B. VPC peering
- C. AWS Direct Connect
- D. VPC endpoints


A. AWS Client VPN	Connects user devices to VPCs—not VPC-to-VPC. Requires client software.
C. AWS Direct Connect	Physically connects on-premises data centers to AWS—not for VPC-to-VPC. Requires dedicated network circuits.
D. VPC Endpoints	Privately connects VPC resources to AWS services (e.g., S3)—not other VPCs.

---

Q873. A company needs to host a highly available application in the AWS Cloud. The application runs infrequently for short periods of time. Which AWS service will meet these requirements with the LEAST amount of operational overhead?
- A. Amazon EC2
- B. AWS Fargate
- [x] C. AWS Lambda
- D. Amazon Aurora

---

> [!IMPORTANT]
> Q874. A company wants to use machine learning to identify suspicious activities in its AWS account. Which AWS service provides this functionality?
- A. AWS Shield
- B. Amazon Macie
- [x] C. Amazon Detective
- D. AWS WAF

Amazon Detective helps you quickly analyze and investigate security events across one or more AWS accounts by generating data visualizations that represent the ways your resources behave and interact over time. Detective creates visualizations of GuardDuty findings.

Detective ingests finding details for all finding types, and provides access to the entity profiles to investigate different entities that are involved with the finding. An entity can be an AWS account, an AWS resource within an account, or an external IP Address that has interacted with your resources. The GuardDuty console supports pivoting to Amazon Detective from the following entities, depending on finding type: AWS account, IAM role, user, or role session, user agent, federated user, Amazon EC2 instance, or IP address.

---

Q875. Which option is the responsibility of AWS, according to the AWS shared responsibility model?
- A. Management of guest operating systems
- B. Firewall configuration changes
- [x] C. Hardware for compute resources
- D. Identity and access management

---

Q876 is the same as Q66.

---

Q877. Which AWS service or feature gives a company the ability to control incoming traffic and outgoing traffic for Amazon EC2 instances?
- [x] A. Security groups
- B. Amazon Route 53
- C. AWS Direct Connect
- D. Amazon VPC

---

> [!IMPORTANT]
> Q878. A company wants to use the AWS Cloud to provide secure access to desktop applications that are running in a fully managed environment. Which AWS service should the company use to meet this requirement?
- A. Amazon S3
- [x] B. Amazon AppStream 2.0
- C. AWS AppSync
- D. AWS Outposts

  
A. Amazon S3 - Amazon Simple Storage Service (S3) is an object storage service that offers industry- leading scalability, data availability, security, and performance. It is primarily used for storing and retrieving any amount of data from anywhere in the world via the web. It is not suitable for providing access to desktop applications.

B. Amazon AppStream 2.0 - Amazon AppStream 2.0 is a fully managed, scalable application streaming service that lets you stream desktop applications to users without rewriting applications. It enables users to access applications instantly across various devices, including Chromebooks, iOS, and Android tablets and phones, as well as Windows and macOS desktops and laptops. This service meets the requirement of providing secure access to desktop applications in a fully managed environment.

C. AWS AppSync - AWS AppSync is a fully managed GraphQL service that provides real-time and offline capabilities for mobile and web applications. It allows you to create and run GraphQL APIs that can be used to query, mutate, and subscribe to data from your backend data sources. It is not designed for streaming desktop applications.

D. AWS Outposts - AWS Outposts is a fully managed service that extends AWS infrastructure, AWS services, APIs, and tools to your on-premises locations. It allows you to run workloads on AWS-managed infrastructure that is located on your premises or in a colocation environment. While it provides a way to bring AWS services closer to your data, it does not directly address the requirement of streaming desktop applications.
 

---

> [!IMPORTANT]
> Q879. A company uses AWS Organizations. The company wants to apply security best practices from the AWS Well-Architected Framework to all of its AWS accounts.  Which AWS service will meet these requirements?
- A. Amazon Macie
- B. Amazon Detective
- [x] C. AWS Control Tower
- D. AWS Secrets Manager

 
A. Amazon Macie - Amazon Macie is a fully managed data security and data privacy service that uses machine learning and pattern matching to discover and protect sensitive data in AWS. It helps identify and classify sensitive data and monitor access to that data. While it enhances data security, it does not directly address the requirement of applying Well-Architected Framework best practices across all accounts.
B. Amazon Detective - Amazon Detective is an interactive, visual investigation tool that enables you to analyze and quickly identify the root cause of potential security issues or suspicious activities. It helps you analyze data from AWS CloudTrail and Amazon GuardDuty to trace the activity across your AWS accounts and resources. Detective focuses on incident response rather than proactive security best practices implementation.
C. AWS Control Tower - AWS Control Tower is a fully managed service that provides pre-configured landing zones on AWS. It helps you quickly set up a secure, multi-account AWS environment by automating the creation and configuration of AWS accounts and resources. It aligns with the AWS Well-Architected Framework by providing a set of security, operational, and compliance best practices. It is designed to simplify the setup and management of AWS Organizations and ensure that all accounts are configured according to best practices.
D. AWS Secrets Manager - AWS Secrets Manager helps you manage, rotate, and retrieve database credentials, API keys, and other secrets throughout their lifecycle. It provides secure storage and rotation of credentials, which are essential for security but do not address the broader requirement of applying Well- Architected Framework best practices across all accounts.
 

---

Q880 is the same as Q420. 


---


> [!IMPORTANT]
> Q881. How does AWS CloudFormation help users operate in the AWS Cloud?
- A. It supports the simple coding of cloud applications.
- B. It monitors the cloud environment.
- C. It automates responses to threats, reducing remediation time and recovery time.
- [x] D. It provides the ability to model and provision the resources that applications need.

> resources rather than applications

---

Q882. A company needs to set up alerts that occur when the actual or forecasted costs of AWS services exceed a defined threshold. Which AWS service or tool should the company use to meet this requirement?
- A. AWS Cost Explorer
- [x] B. AWS Budgets
- C. AWS Cost and Usage Report
- D. AWS CloudTrail

---

Q883. Which AWS offering can provide discounts on some AWS service costs in exchange for a spending commitment?
- A. Amazon Detective
- B. AWS Pricing Calculator
- [x] C. Savings Plans
- D. AWS Basic Support

---

Q884. A company wants to build an application that consists entirely of microservices. Which AWS Cloud architecture design principle supports this goal?
- A. Think parallel.
- B. Implement elasticity.
- C. Stop guessing capacity.
- [x] D. Decouple components.

---

Q885. Which AWS service or feature can a company use to determine which business unit is using specific AWS resources?
- [x] A. Cost allocation tags
- B. Key pairs
- C. Amazon Inspector
- D. AWS Trusted Advisor

---

Q886. A cloud engineer wants to know the percentage of the allocated compute units that are in use for a specific Amazon EC2 instance. Which AWS service can provide this information?
- A. AWS CloudTrail
- B. AWS Config
- [x] C. Amazon CloudWatch
- D. AWS Artifact

---

Q887. Which design principle is included in the operational excellence pillar of the AWS Well-Architected Framework?
- A. Create annotated documentation.
- [x] B. Anticipate failure.
- C. Ensure performance efficiency.
- D. Optimize costs.

---

Q888. Which pillar of the AWS Well-Architected Framework includes a design principle about measuring the overall efficiency of workloads in terms of business value?
- A. Operational excellence
- B. Security
- C. Reliability
- [x] D. Cost optimization

---

Q889. A media production company wants to automatically generate time-stamped subtitles from the audio track of a video and display the subtitles with the video content. Which AWS service should the company use for this functionality?
- A. Amazon Rekognition
- B. Amazon Textract
- [x] C. Amazon Transcribe
- D. Amazon Comprehend

---

> [!IMPORTANT]
> Q890. Which Amazon Route 53 routing policy can a company use to route traffic to multiple resources in specified proportions?
- [x] A. Weighted routing policy
- B. Multivalue answer routing policy
- C. Failover routing policy
- D. Latency routing policy
 
A. Weighted routing policy
Weighted routing allows you to associate multiple resources with a single domain name or subdomain name and choose how much traffic is routed to each resource. You assign each resource a relative weight that corresponds to the proportion of traffic you want to send to it. Amazon Route 53 then distributes traffic to the resources based on these weights. This policy is useful for various purposes, including load balancing and testing new versions of software.
The other options are not suitable for routing traffic to multiple resources in specified proportions:
B. Multivalue answer routing policy - This policy returns up to eight healthy records in response to a DNS query, selected at random. It is primarily used to improve availability and fault tolerance by providing multiple IP addresses for clients to choose from.
C. Failover routing policy - This policy is used to configure active-passive failover. It routes traffic to a primary resource and switches to a secondary resource if the primary resource becomes unavailable. D. Latency routing policy - This policy routes traffic to the resource that provides the best latency based on the user's location. It is useful for global applications where minimizing latency is critical. Therefore, the correct answer is A. Weighted routing policy.


---

Q891. A company has a web application that has users all over the world. The company is moving the application to AWS to improve speed for the users. The company needs an AWS service that delivers the application content through data centers around the world. Which AWS service or feature will meet these requirements?  
- A. Amazon Connect  
- B. AWS Config  
- C. AWS AppSync  
- [x] D. Edge locations

 
  
The correct answer is:
D. Edge locations
Explanation:
Edge locations are part of the AWS content delivery network (CDN) service known as Amazon CloudFront. Edge locations are data centers located around the world that cache copies of your application content, allowing for faster delivery to users based on their geographic location. This improves the speed and performance of the web application for users globally.
A. Amazon Connect: This is a cloud-based contact center service and is not related to content delivery.
B. AWS Config: This service is used for assessing, auditing, and evaluating the configurations of AWS resources; it does not deliver content.
C. AWS AppSync: This is a managed service that simplifies the process of developing GraphQL APIs but does not specifically address content delivery across the globe.
Summary:
Recommended service for delivering application content globally: Edge locations (part of Amazon CloudFront)

Edge locations are part of Amazon CloudFront, which is a global content delivery network (CDN) service that accelerates delivery of your websites, APIs, video content, or other assets to your users with low latency and high transfer speeds. CloudFront caches your content in multiple edge locations across the globe, which enables it to serve your content to users with high speed and reliability, regardless of their location.
The other options are not suitable for this purpose:
A. Amazon Connect - This is a contact center as a service (CCaaS) solution that enables you to quickly and easily set up a scalable cloud contact center.
B. AWS Config - This service enables you to assess, audit, and evaluate the configurations of your AWS resources.
C. AWS AppSync - This service provides a fully managed GraphQL service that makes it easy to create and run scalable applications that use real-time and offline capabilities. Edge locations, through Amazon CloudFront, are the best fit for delivering web application content to users around the world with low latency and high transfer speeds.


---

Q892. Which AWS service or tool inspects a user's AWS environment and makes recommendations for cost savings and system performance improvements?  
- A. Cost Explorer  
- [x] B. AWS Trusted Advisor  
- C. Amazon Inspector  
- D. AWS Budgets

 
AWS Trusted Advisor provides real-time guidance to help you provision your resources following AWS best practices. It inspects your AWS environment and offers recommendations in five categories: cost optimization, security, fault tolerance, performance, and service limits. These recommendations can help you save money, improve system performance, and increase the reliability and security of your applications.
The other options are not suitable for this purpose:
A. Cost Explorer - This tool enables you to visualize your AWS costs and usage over different time periods, and to understand your spending by service, region, account, or tag. C. Amazon Inspector - This automated security assessment service helps you improve the security and compliance of your Amazon EC2 instances and applications by automatically assessing vulnerabilities and configurations.
D. AWS Budgets - This service helps you plan and track your AWS costs by setting custom budgets and receiving alerts when your usage exceeds, or is forecasted to exceed, your budgeted amounts.
 

---

> [!IMPORTANT]
> Q893. A company needs to reserve a certain amount of Amazon EC2 compute resources in a specific Availability Zone within an AWS Region. Which purchasing option should the company use to meet this requirement?  
- A. EC2 Instance Savings Plans  
- B. Compute Savings Plans  
- C. Regional Reserved Instances  
- [x] D. Zonal Reserved Instances  

When you purchase a Reserved Instance, you determine the scope of the Reserved Instance. The scope is either regional or zonal.

Regional: When you purchase a Reserved Instance for a Region, it's referred to as a regional Reserved Instance.

Zonal: When you purchase a Reserved Instance for a specific Availability Zone, it's referred to as a zonal Reserved Instance.

The scope does not affect the price. You pay the same price for a regional or zonal Reserved Instance.

---

Q894. A company needs to centrally manage workforce identity access and permissions across AWS accounts and applications. Which AWS service provides this functionality?  
- A. Amazon Cognito  
- B. AWS Control Tower  
- [x] C. AWS IAM Identity Center  
- D. AWS IAM Roles Anywhere  

---

> [!IMPORTANT]
> Q895. A company wants to host workloads on Amazon EC2 instances. The workloads require a balance of compute, memory, and networking resources. Which EC2 instance type should the company use to host the workloads?  
- [x] A. General purpose instances  
- B. Compute optimized instances  
- C. Memory optimized instances  
- D. Storage optimized instances  

 
---

Q896. A company needs to store its files in the AWS Cloud. Users must be able to download the files directly by using a public URL. Which AWS service provides this functionality?  
- A. Amazon Redshift  
- B. Amazon Elastic Block Store (Amazon EBS)  
- C. Amazon Elastic File System (Amazon EFS)  
- [x] D. Amazon S3  

---

Q897. What is the scope of a VPC within the AWS network?  
- A. A VPC can span all Availability Zones globally.  
- B. A VPC must span at least two subnets in each AWS Region.  
- C. A VPC must span at least two edge locations in each AWS Region.  
- [x] D. A VPC can span all Availability Zones within an AWS Region.  

---

Q898. A company needs to encrypt data at rest in the AWS Cloud by using an encryption key that the company controls. Which AWS service should the company use to meet this requirement?  
- A. AWS Certificate Manager (ACM)  
- B. Amazon Cognito  
- [x] C. AWS Key Management Service (AWS KMS)  
- D. AWS Trusted Advisor  

---

Q899. Which AWS Cloud benefit describes the ability to acquire resources as they are needed and release resources when they are no longer needed?  
- A. Economies of scale  
- [x] B. Elasticity  
- C. Agility  
- D. Security  

---
 
Q900. Which AWS service can a company use to build conversational chatbots for customer service?  
- [x] A. Amazon Lex  
- B. AWS Amplify  
- C. Amazon Comprehend  
- D. Amazon Polly  

---

Q901. A cloud engineer needs to download AWS security and compliance documents for an upcoming audit. Which AWS service can provide the documents?  
- A. AWS Trusted Advisor  
- [x] B. AWS Artifact  
- C. AWS Well-Architected Tool  
- D. AWS Systems Manager  

---

> [!IMPORTANT]
> Q902. A company wants to migrate its containerized workload from an on-premises data center to a managed container service in the AWS Cloud. Which AWS services should the company use? (Select TWO.)  
- A. Amazon EC2  
- [x] B. Amazon Elastic Kubernetes Service (Amazon EKS)  
- C. Amazon Elastic Container Registry (Amazon ECR)  
- [x] D. Amazon Elastic Container Service (Amazon ECS)  
- E. AWS Lambda  

Amazon ECS is AWS’s container orchestration service, while EKS is a managed Kubernetes service that allows you to run Kubernetes on AWS.
1. Image Creation:
Developers create container images using tools like Docker and then push them to ECR. 
2. Task/Pod Definition:
In ECS, you define a task that specifies the container image from ECR and other settings. In EKS, you define a pod that also references the container image. 
3. Deployment:
ECS and EKS use these definitions to deploy and manage the containers, pulling the images from ECR as needed. 
4. Scaling and Management:
The container orchestration services handle scaling, updates, and other operational tasks, ensuring the containers are running efficiently and reliably. 
In short, ECR is the storage, ECS and EKS are the orchestrators, and they work together to deploy and manage containerized applications on AWS
---

Q903. A company wants to migrate its on-premises application to the AWS Cloud. The company is legally obligated to retain certain data in its on-premises data center. Which AWS service or feature will support this requirement?  
- A. AWS Wavelength  
- B. AWS Local Zones  
- C. VMware Cloud on AWS  
- [x] D. AWS Outposts  

---

Q904. A company plans to move its test workloads to Amazon EC2. The test workloads can be interrupted and are not required to start at a particular time. Which EC2 instance purchasing option is MOST cost-effective for this use case?  
- A. On-Demand Instances  
- [x] B. Spot Instances  
- C. Reserved Instances  
- D. Dedicated Hosts  

---

> [!IMPORTANT]
> Q905. A company's project team needs to simultaneously mount a file system on multiple Amazon EC2 Linux instances. The file system also will be shared across multiple Availability Zones. Which AWS service will meet these requirements?  
- [x] A. Amazon Elastic File System (Amazon EFS)  
- B. Amazon S3  
- C. Amazon Elastic Block Store (Amazon EBS)  
- D. Amazon FSx for Windows File Server  

 
- Amazon EFS is a fully managed, scalable file storage service that can be mounted on multiple EC2 instances simultaneously and is designed for high availability across multiple Availability Zones.
Summary of Other Options:
B. Amazon S3: While S3 is a storage service that can be accessed by multiple instances, it is not a file system and does not support mounting in the same way as EFS.
C. Amazon Elastic Block Store (Amazon EBS): EBS volumes can only be attached to a single EC2 instance at a time (with some exceptions for multi-Attach), making it unsuitable for this requirement.
D. Amazon FSx for Windows File Server: This service is designed for Windows-based applications and file sharing but is not optimized for Linux instances as EFS is.
Final Answer:
A. Amazon Elastic File System (Amazon EFS)

---

Q906. A company is designing an application. For the data persistence layer, the company wants to use a NoSQL database. Which AWS service should the company use for the database?  
- A. Amazon Redshift  
- B. AWS DataSync  
- C. Amazon Athena  
- [x] D. Amazon DynamoDB  

---

> [!IMPORTANT]
> Q907. A company runs workloads on AWS to provide real-time gaming and augmented virtual reality platforms to users. The company wants to ensure that the users can run apps with single-digit millisecond latencies on their mobile devices. Which AWS solution can the company use for deployment to meet these requirements?  
- A. Provisioned IOPS  
- B. AWS Graviton processors  
- [x] C. AWS Wavelength  
- D. AWS Outposts
 
A. Provisioned IOPS
Provisioned IOPS (Input/Output Operations Per Second) is an Amazon Elastic Block Store (EBS) volume type designed for workloads that require consistent, predictable performance at any scale. While it offers high-performance storage, it is not specifically tailored for low-latency mobile applications.
B. AWS Graviton processors
AWS Graviton processors are custom-built Arm-based processors designed to deliver high performance and cost efficiency for workloads running on AWS. They can help reduce costs and improve performance for certain types of workloads, but they are not specifically optimized for low-latency mobile applications, especially for real-time gaming and augmented virtual reality platforms.
C. AWS Wavelength
AWS Wavelength is an edge computing service that extends AWS's compute, storage, and other services to the edge of mobile networks. It is designed to provide ultra-low latency for applications running on mobile devices by placing AWS compute resources closer to users. This service is ideal for applications that require real-time interactions, such as gaming, augmented reality, and virtual reality.
D. AWS Outposts
AWS Outposts is a fully managed service that extends AWS infrastructure, services, APIs, and tools to on- premises environments. While it provides a consistent hybrid cloud experience, it is not specifically designed for low-latency mobile applications and is more suited for organizations that want to run AWS services in their own data centers.
Given the company's requirements for single-digit millisecond latencies on mobile devices for real-time gaming and augmented virtual reality platforms, AWS Wavelength is the most suitable solution. It is specifically designed for edge computing scenarios and can provide ultra-low latency by placing AWS compute resources closer to users. This makes it ideal for applications that require real-time interactions and high performance, such as those in the gaming and augmented reality industries.
 

---

> [!IMPORTANT]
> Q908. A company needs a portable solution to collect data and run computations. Which AWS service provides the MOST compact solution to meet these requirements?  
- [x] A. AWS Snowcone  
- B. AWS Snowball Edge  
- C. Amazon S3  
- D. AWS Outposts  

> keyword: "most compact"; "portable"
>
To determine the most compact AWS service that meets the requirements of a portable solution for collecting data and running computations, let's evaluate each option provided:
A. AWS Snowcone
AWS Snowcone is a small, rugged, and secure data transfer device designed for moving large amounts of data into and out of AWS. It is portable and compact, making it suitable for environments with limited connectivity or capacity. It can be used for data migration, disaster recovery, and content distribution, and it supports local compute capabilities for running applications and data processing tasks.
B. AWS Snowball Edge
AWS Snowball Edge is a larger, more powerful data transfer device compared to Snowcone. It offers high- capacity storage options and on-device compute capabilities for data preprocessing, machine learning inference, and data transformation. While it is also portable, it is physically larger and more suited for larger data volumes and more complex computations.
C. Amazon S3
Amazon S3 (Simple Storage Service) is an object storage service that offers scalable storage for internet applications. It is not a portable solution but rather a cloud-based storage service. It does not support local data collection or computations and is therefore not suitable for the requirements specified.
D. AWS Outposts
AWS Outposts is a fully managed service that extends AWS infrastructure, services, APIs, and tools to your on-premises environments. It provides a consistent hybrid experience but is not a portable solution. It is designed for organizations that want to run AWS services in their own data centers or on-premises facilities. Given the requirements for a portable solution to collect data and run computations, AWS Snowcone is the most compact option that meets these needs. It is small, rugged, and secure, making it easy to transport and deploy in various environments. Additionally, its local compute capabilities allow for data processing and application execution on the device itself, making it an ideal solution for scenarios where on-site data collection and computation are required.
Therefore, the correct answer is:
A. AWS Snowcone

---

> [!IMPORTANT]
> Q909. Which options are benefits of using third-party software from AWS Marketplace? (Select TWO.)  
- A. The software's data encryption is managed by a third-party vendor.  
- [x] B. The software has been evaluated by vendors to ensure that it will run on AWS.  
- C. Users do not need to upgrade to newer software versions.  
- D. Users do not need to conduct security testing on the software.  
- [x] E. Users can launch preconfigured software in only a few steps.

When considering the benefits of using third-party software from AWS Marketplace, it's important to understand what AWS Marketplace offers and how it can benefit users.
Let's analyze the options provided:
A. The software's data encryption is managed by a third-party vendor.
This is not necessarily a benefit. While third-party vendors may have their own encryption practices, AWS Marketplace itself does not guarantee the encryption or security of the software. Users should still be aware of and comfortable with the encryption and security measures in place. B. The software has been evaluated by vendors to ensure that it will run on AWS.
This is a benefit. AWS Marketplace partners ensure that their software is compatible with AWS services and infrastructure. This means that users can trust that the software will run smoothly on AWS without extensive troubleshooting or configuration.
C. Users do not need to upgrade to newer software versions.
This is not a benefit. In fact, it could be a drawback. Software that is not regularly updated may become outdated, contain security vulnerabilities, or lack new features and improvements. Users should always be aware of and consider upgrading to newer software versions as needed. D. Users do not need to conduct security testing on the software.
This is not a benefit. While AWS Marketplace partners may have conducted their own security testing, users should still conduct their own security assessments and testing to ensure that the software meets their security requirements and standards.
E. Users can launch preconfigured software in only a few steps.
This is a benefit. AWS Marketplace offers preconfigured software images that can be launched quickly and easily with minimal configuration. This can save users time and effort, allowing them to get started with the software more quickly.
Given the requirement to select two benefits of using third-party software from AWS Marketplace, the most appropriate options are:
B. The software has been evaluated by vendors to ensure that it will run on AWS. E. Users can launch preconfigured software in only a few steps.
These options highlight the compatibility and ease of use of third-party software from AWS Marketplace, making it a valuable resource for users looking to deploy and manage software on AWS.


---

> [!IMPORTANT]
> Q910. A company has only basic knowledge of AWS technologies. Which AWS service provides the SIMPLEST way for the company to establish a website on AWS?  
- A. Amazon Elastic File System (Amazon EFS)  
- B. AWS Elastic Beanstalk  
- C. AWS Lambda  
- [x] D. Amazon Lightsail  

---

Q911. A company notices suspicious network activity against an application that is running on a fleet of Amazon EC2 instances. The suspicious activity is coming from a single IP address. Which AWS service should the company use to block access from this IP address?  
- A. AWS Shield  
- B. AWS Config  
- C. Amazon GuardDuty  
- [x] D. AWS WAF  

---

Q912. A company needs to establish a dedicated network connection from on premises to AWS. The connection must provide consistent, low-latency network performance. Which AWS service should the company use to meet this requirement?  
- [x] A. AWS Direct Connect  
- B. AWS Site-to-Site VPN  
- C. AWS Directory Service  
- D. AWS Transit Gateway  

---

Q913. Which AWS service scans for software vulnerabilities and unintended network exposure?  
- [x] A. Amazon Inspector  
- B. AWS Security Hub  
- C. AWS Shield  
- D. AWS Trusted Advisor  

---

Q914. Which AWS service offers object storage?  
- A. Amazon RDS  
- B. Amazon Elastic File System (Amazon EFS)  
- [x] C. Amazon S3  
- D. Amazon DynamoDB  

---

Q915 is the same as Q891. 

---

Q916. A company has an application that runs periodically in an on-premises environment. The application runs for a few hours most days, but runs for 8 hours a day for a week at the end of each month. Which AWS service or feature should be used to host the application in the AWS Cloud?  
- A. Amazon EC2 Standard Reserved Instances  
- [x] B. Amazon EC2 On-Demand Instances  
- C. AWS Wavelength  
- D. Application Load Balancer  

---

> [!IMPORTANT]
> Q917. A company is operating several factories where it builds products. The company needs the ability to process data, store data, and run applications with local system interdependencies that require low latency. Which AWS service should the company use to meet these requirements?  
- [x] A. AWS IoT Greengrass  
- B. AWS Lambda  
- C. AWS Outposts  
- D. AWS Snowball Edge  

> keywords: factories;  local system interdependencies

https://docs.aws.amazon.com/greengrass/v2/developerguide/how-it-works.html

https://docs.aws.amazon.com/greengrass/v2/developerguide/what-is-iot-greengrass.html

https://docs.aws.amazon.com/prescriptive-guidance/latest/iot-greengrass-golden-images/introduction.html
 
A. AWS IoT Greengrass
AWS IoT Greengrass allows you to run local compute, messaging, data caching, and machine learning inference capabilities on connected devices. It is designed for scenarios where low latency is required and can process data locally, making it suitable for factory environments with local system interdependencies.

B. AWS IAMbda: This is a serverless compute service but is not specifically designed for local processing in edge environments.

C. AWS Outposts: While it provides a way to run AWS infrastructure on-premises, it may be more complex and costly if only local processing is needed.

D. AWS Snowball Edge: This is primarily used for data transfer and edge computing but is not specifically intended for continuous processing of data in a factory setting.

---

Q918. A company needs to mount a file share across multiple Amazon EC2 instances as a mapped drive by using the SMB protocol. Which AWS service will meet these requirements?  
- [x] A. Amazon FSx for Windows File Server  
- B. Amazon Elastic File System (Amazon EFS)  
- C. Amazon S3  
- D. AWS DataSync  


both Amazon S3 File Gateway and Amazon FSx for Windows File Server support (Server Message Block) protocol

The correct answer is:
A. Amazon FSx for Windows File Server
Explanation:
Amazon FSx for Windows File Server provides a fully managed Windows file system that supports the SMB protocol. This service allows you to easily create file shares that can be mounted across multiple Amazon EC2 instances, making it the ideal choice for your requirement to use SMB for a mapped drive.
B. Amazon Elastic File System (Amazon EFS): While EFS supports NFS and is suitable for Linux-based workloads, it does not natively support SMB.
C. Amazon S3: This is an object storage service and does not support mounting as a file share using SMB. D. AWS DataSync: This service is used for transferring data between on-premises storage and AWS but is not a file storage solution itself.
Summary:
Recommended service for SMB file sharing: Amazon FSx for Windows File Server


---

Q919. A company's application is gaining popularity. The company needs to set up a phone number to manage the increasing volume of calls that the company's support staff receives. Which AWS service should the company use to meet this requirement?  
- [x] A. Amazon Connect  
- B. Amazon CloudFront  
- C. AWS Direct Connect  
- D. AWS Trusted Advisor  

---

Q920. Which of the following are customer responsibilities under the AWS shared responsibility model? (Select TWO.)  
- A. Physical security of AWS facilities  
- [x] B. Configuration of security groups  
- [x] C. Encryption of customer data on AWS  
- D. Management of AWS Lambda infrastructure  
- E. Management of network throughput of each AWS Region  

---

Q921. A cloud practitioner wants a repeatable way to deploy identical AWS resources by using infrastructure templates. Which AWS service will meet these requirements?  
- [x] A. AWS CloudFormation  
- B. AWS Directory Service  
- C. Amazon Lightsail  
- D. AWS CodeDeploy  

---

Q922. Which task is a responsibility of AWS, according to the AWS shared responsibility model?  
- A. Client-side encryption of objects that are stored in Amazon S3  
- B. Configuration of security groups that are associated with Amazon EC2 instances  
- C. Patch management of guest operating systems of Amazon EC2 instances  
- [x] D. Configuration of the AWS Nitro Enclaves Nitro Hypervisor  

---

Q923 is the same as Q895.


---

Q924. A company wants to secure its consumer web application by using SSL/TLS to encrypt traffic. Which AWS service can the company use to meet this goal?  
- A. AWS WAF  
- B. AWS Shield  
- C. Amazon VPC  
- [x] D. AWS Certificate Manager (ACM)  

SSL (Secure Sockets Layer) and TLS (Transport Layer Security) 

---

Q925. Which AWS service or feature can a company use to capture information about incoming and outgoing traffic in VPC infrastructure?  
- A. AWS Config  
- [x] B. VPC Flow Logs  
- C. AWS Trusted Advisor  
- D. AWS CloudTrail  

---

Q926. A company needs a serverless data integration service to discover, prepare, and combine data for analytics. Which AWS service will meet these requirements?  
- A. Amazon EMR  
- B. Amazon Redshift  
- [x] C. AWS Glue  
- D. AWS Step Functions  

> severless; ETL workloads
---

Q927. Which AWS service gives companies the ability to create graph applications that can analyze billions of relationships between data points in milliseconds?  
- A. Amazon Redshift  
- [x] B. Amazon Neptune  
- C. Amazon DocumentDB (with MongoDB compatibility)  
- D. Amazon ElastiCache  

---

Q928. A company wants to minimize network latency between its Amazon EC2 instances. The EC2 instances do not need to be highly available. Which solution meets these requirements?  
- [x] A. Use EC2 instances in a single Availability Zone.  
- B. Use EC2 instances in multiple edge locations.  
- C. Use EC2 instances in the same Availability Zone but in different AWS Regions.  
- D. Use EC2 instances in the same edge location and the same AWS Region.  

---

Q929. A company needs to apply security rules to a subnet for Amazon EC2 instances. Which AWS service or feature provides this functionality?  
- [x] A. Network ACLs  
- B. Security groups  
- C. AWS Certificate Manager (ACM)  
- D. AWS Config  

---

> [!IMPORTANT]
> Q930. A company is building a business intelligence solution that uses Amazon Redshift. The company wants to use an AWS service to create interactive dashboards and not pay any upfront costs for it. Which service should the company use?  
- A. Amazon CloudWatch  
- B. AWS Health Dashboard  
- C. AWS Service Catalog  
- [x] D. Amazon QuickSight  

> keywords: interactive dashboards; serverless; no upfront costs; natural language queries; machine Learning Integration

Amazon QuickSight is a scalable, **serverless** business intelligence (BI) service that allows users to create interactive dashboards and visualizations. It operates on a pay-as-you-go pricing model, meaning there are no upfront costs, making it a suitable choice for companies looking to build BI solutions without initial investment.


A. Amazon CloudWatch: This service is primarily for monitoring resources and applications, not for creating interactive dashboards for business intelligence.
B. AWS Health Dashboard: This provides insights into the health of AWS services but is not designed for building custom dashboards for business intelligence.
C. AWS Service Catalog: This service helps organizations create and manage catalogs of IT services but does not provide BI dashboard capabilities.
 

---

Q931 is the same as Q900.

---

Q932. A company needs to schedule the rotation of database credentials in the AWS Cloud. Which AWS service should the company use to perform this task?  
- A. AWS Identity and Access Management (IAM)  
- B. AWS Managed Services (AMS)  
- C. Amazon RDS  
- [x] D. AWS Secrets Manager  

---

> [!IMPORTANT]
> Q933. Which AWS service or feature should a company use between two microservices to ensure that messages are sent and received in exact order?  
- A. Amazon Simple Email Service (Amazon SES)  
- B. Amazon Simple Notification Service (Amazon SNS)  
- C. Amazon S3 Event Notifications  
- [x] D. Amazon Simple Queue Service (Amazon SQS) FIFO queues  
 
 

Amazon SNS (Simple Notification Service) and Amazon SQS (Simple Queue Service) are complementary AWS messaging services that decouple microservices. Here's how they interact:

🔄 Core Relationship: Pub/Sub + Queueing
SNS (Publisher):

A topic-based pub/sub system that broadcasts messages to multiple subscribers (e.g., SQS queues, Lambda, HTTP endpoints).

Does not store messages—delivers immediately or discards if no subscribers.

SQS (Subscriber):

A message queue that stores messages until consumers process them.

Acts as a subscriber to SNS topics to receive messages asynchronously.
 
 
A. Amazon SES	Email service—no message queuing or ordering capabilities.
B. Amazon SNS	Standard topics offer best-effort ordering (no guarantees). FIFO topics exist but require pairing with SQS FIFO queues for strict ordering.
C. S3 Event Notifications	Events are not ordered (e.g., object PUT may arrive before DELETE).


The Amazon SNS service will attempt to deliver messages from the publisher in the order they were published into the topic. However, network issues could potentially result in out-of-order messages at the subscriber end.

Similar to standard SNS topics, SNS FIFO topics allow users to publish a message to a topic, so it can be delivered to a series of subscribing endpoints. When the delivery of those messages to subscribers must be in order (first-in-first-out), and once only, and you want SNS to take care of it, SNS FIFO topics is the way to go. Amazon SNS FIFO topics can deliver ordered messages to Amazon Simple Queue Service (Amazon SQS) FIFO queues to provide consistent end-to-end message ordering for distributed applications. You can now reduce the effort required to process your high throughput, consistently ordered transactions and simplify your messaging architecture. When strict ordering is not necessary, Amazon FIFO topics can also deliver messages to Amazon SQS standard queues, offering flexibility in how you design your applications. Example use cases include bank transaction logs, stock tickers, flight trackers, price updates, news broadcasting, and inventory management.


---

Q934. Which AWS service or feature can a company use to create a private, secured, and scalable network environment in the AWS Cloud?  
- A. Amazon Elastic Container Service (Amazon ECS)  
- B. Amazon S3
- [x] C. Amazon VPC  
- D. Route tables  

---

> [!IMPORTANT]
> Q935. A company needs to set up user authentication for a new application. Users must be able to sign in directly with a username and password, or through a third-party provider. Which AWS service should the company use to meet these requirements?  
- A. AWS IAM Identity Center  
- B. AWS Signer  
- [x] C. Amazon Cognito  
- D. AWS Directory Service  


---

Q936. A company is preparing for an audit and wants documentation that AWS complies with the Payment Card Industry Data Security Standard (PCI DSS). Where can the company find this documentation?  
- [x] A. AWS Artifact  
- B. AWS Organizations  
- C. AWS Trusted Advisor  
- D. AWS Support Center  

---

Q937. Which AWS service provides a scalable data warehouse solution?  
- A. Amazon S3  
- B. Amazon DynamoDB  
- C. Amazon Kinesis Data Streams  
- [x] D. Amazon Redshift

 
Amazon Redshift is a fully managed, scalable data warehouse solution designed for online analytical processing (OLAP). It allows you to run complex queries and perform analytics on large amounts of structured data, making it suitable for business intelligence and reporting.
Summary of Other Options:
A. Amazon S3: This is an object storage service, not a data warehouse. B. Amazon DynamoDB: This is a managed NoSQL database service, which is not specifically designed as a data warehouse.
C. Amazon Kinesis Data Streams: This service is used for real-time data streaming but does not provide data warehousing capabilities.
Final Answer:
D. Amazon Redshift


---

Q938. Which AWS service monitors AWS accounts for security threats?  
- [x] A. Amazon GuardDuty  
- B. AWS Secrets Manager  
- C. Amazon Cognito  
- D. AWS Certificate Manager (ACM)  

---

Q939. A company is running Amazon EC2 instances in a private subnet in a VPC. Which AWS service or feature can provide the EC2 instances with network connections to the internet?  
- A. Gateway endpoint  
- [x] B. NAT gateway  
- C. Network Load Balancer  
- D. Amazon Route 53  

---

Q940. Treating infrastructure as code in the AWS Cloud allows users to:  
- A. automate migration of on-premises hardware to AWS data centers.  
- B. let a third party automate an audit of the AWS infrastructure.  
- C. turn over application code to AWS so it can run on the AWS infrastructure.  
- [x] D. automate the infrastructure provisioning process.  


---

> [!IMPORTANT]
> Q941. Which AWS feature or resource is a deployable Amazon EC2 instance template that is prepackaged with software and security requirements?
- A. Amazon Elastic Block Store (Amazon EBS) volume  
- B. AWS CloudFormation template  
- C. Amazon Elastic Block Store (Amazon EBS) snapshot  
- [x] D. Amazon Machine Image (AMI)  
 

---

Q942. According to the AWS shared responsibility model, which activities are the customer's responsibility for security in the AWS Cloud? (Select TWO.)
- A. Hardware maintenance  
- [x] B. Amazon EC2 operating system patching  
- [x] C. API access control for AWS resources  
- D. Configuration management of infrastructure devices  
- E. Maintenance of an Availability Zone  

 
---

> [!IMPORTANT]
> Q943. Which task can an IAM user perform without AWS account root user credentials?
- A. Change to a different AWS Support plan.  
- B. Close an AWS account.  
- [x] C. View the AWS Billing console.  
- D. Activate access to the AWS Billing console.  

> To change your support plan, you must have AWS Identity and Access Management (IAM) permissions or sign in to your account as a root user. https://docs.aws.amazon.com/awssupport/latest/user/changing-support-plans.html

---

Q944. A company needs to use an offline transfer strategy to move petabytes of databases, backups, and data records from on premises to the AWS Cloud. Which solution will meet this requirement with the MOST operational efficiency?
- [x] A. AWS Snowball Edge compute-optimized devices  
- B. AWS Snowcone devices  
- C. AWS Storage Gateway  
- D. AWS DataSync

> keywords: offline

---

Q945. Which AWS services can a company use to deploy a database on AWS? (Select TWO.)
- A. Elastic Load Balancing (ELB)  
- B. AWS CloudTrail  
- [x] C. Amazon RDS  
- [x] D. Amazon EC2  
- E. Amazon Elastic File System (Amazon EFS)  

 

---

> [!IMPORTANT]
> Q946. A company needs to lift and shift many applications to AWS without long cutover windows. Which AWS service provides this functionality?
- A. AWS Application Discovery Service  
- [x] B. AWS Application Migration Service  
- C. AWS Migration Hub  
- D. AWS DataSync  

 

---

> [!IMPORTANT]
> Q947. Which AWS service or feature gives users the ability to access AWS resources from any location by using an encrypted connection?
- A. Amazon CloudFront  
- [x] B. AWS Client VPN  
- C. AWS Direct Connect  
- D. AWS PrivateLink  

> keywords: any location

Client VPN is a managed client-based VPN service that gives you the ability to securely access your AWS resources and the resources in your on-premises network. With Client VPN, you can access your resources from any location through an OpenVPN-based VPN client. You would use Client VPN to connect individual laptops to AWS



---

Q948. Which tasks are the customer's responsibility in the AWS Cloud? (Select TWO.)
- [x] A. Configure VPC subnets.  
- [x] B. Configure security groups for Amazon EC2 instances.  
- C. Manage and maintain AWS Regions.  
- D. Patch and maintain Amazon CloudFront.  
- E. Patch the operating system in Amazon DynamoDB.  
 

---

Q949. Which AWS service provides recommendations to help users reduce the cost of Amazon EC2 instances?
- A. AWS AppConfig  
- B. AWS Control Tower  
- C. AWS AppSync  
- [x] D. AWS Compute Optimizer  

 
---

> [!IMPORTANT]
> Q950. A company needs a solution that provides recommended steps for migration to the AWS Cloud. Which AWS service or tool will meet this requirement?
- A. AWS CloudFormation  
- B. AWS Application Discovery Service  
- [x] C. AWS Cloud Readiness Assessment  
- D. Amazon CloudWatch  

 

---

Q951. A company's IT administrator needs to configure the AWS CLI for programmatic access to AWS services for the company's employees. Which combination of credential components must the IT administrator use to meet this requirement? (Select TWO.)
- A. public key  
- [x] B. A secret access key  
- C. An IAM role  
- [x] D. An access key ID  
- E. A private key  
 

---

> [!IMPORTANT]
> Q952. A company plans to migrate on-premises Internet Small Computer Systems Interface (iSCSI) storage to AWS. The company needs low-latency access to the stored data. The company also must minimize infrastructure changes to workloads that use the storage. Which AWS storage solution will meet these requirements?
- A. Amazon Elastic Block Store (Amazon EBS)  
- B. Amazon S3 File Gateway  
- C. AWS Storage Gateway Tape Gateway  
- [x] D. AWS Storage Gateway Volume Gateway  
 
---

> [!IMPORTANT]
> Q953. Which AWS service can assess and gather information about a company's on-premises servers and databases before a migration to AWS?
- [x] A. AWS Application Discovery Service  
- B. AWS Application Migration Service  
- C. AWS Database Migration Service (AWS DMS)  
- D. AWS Mainframe Modernization  


---

Q954. A company is planning to migrate to the AWS Cloud. The company wants to identify measurable business outcomes that will explain the value of the company's decision to migrate. Which phase of the cloud transformation journey includes these activities?
- [x] A. Envision  
- B. Align  
- C. Scale  
- D. Launch   
---

Q955. A company is designing an application. For the data persistence layer, the company wants to use a NoSQL database. Which AWS service should the company use for the database?
- A. Amazon Redshift  
- B. AWS DataSync  
- C. Amazon Athena  
- [x] D. Amazon DynamoDB  

 

---

> [!IMPORTANT]
> Q956. For which task does AWS Trusted Advisor provide guidance?
- A. Auditing of AWS account activity  
- B. Troubleshooting of connectivity issues  
- [x] C. Elimination of unused and idle resources  
- D. Implementation of migration assessments  

https://docs.aws.amazon.com/awssupport/latest/user/cost-optimization-checks.html#ec2-cost-opt-for-instances
https://docs.aws.amazon.com/cost-management/latest/userguide/coh-optimization-strategies.html

---

Q957. A company seeks cost savings in exchange for a commitment to use a specific amount of an AWS service or category of AWS services for 1 year or 3 years. Which AWS pricing model or offering will meet these requirements?
- A. Pay-as-you-go pricing  
- [x] B. Savings Plans  
- C. AWS Free Tier  
- D. Volume discounts  

 
---

Q958. Which AWS service gives users the ability to simplify costs and take advantage of quantity discounts with a single bill?
- A. Service Quotas  
- B. AWS Service Catalog  
- C. AWS Control Tower  
- [x] D. AWS Organizations  

---

Q959. A company needs to create graphs that show historical and current costs for the company's AWS account. Which AWS service or tool provides this functionality?
- A. AWS Config  
- B. AWS Cost and Usage Report  
- C. AWS Budgets  
- [x] D. AWS Cost Explorer  


 
AWS Cost Explorer provides visualization tools and cost reports with graphical representations of historical and current AWS costs, making it the best choice for creating cost graphs. The other options serve different purposes:
- AWS Config tracks resource configurations
- Cost and Usage Report provides detailed billing data (but not visualizations)
- AWS Budgets helps set and monitor cost thresholds 

---




