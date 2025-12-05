SAA-C03 Part 1

https://www.awslagi.com/course/aws-certified-solutions-architect-associate-saa-c03-practice-exam/lessons/saa-c03-part-1/


Question 1: A company hosts a web application on multiple Amazon EC2 instances. The EC2 instances are in an Auto Scaling group that scales in response to user demand. The company wants to optimize cost savings without making a long-term commitment. Which EC2 instance purchasing option should a solutions architect recommend to meet these requirements?
  - A. Dedicated Instances only
  - B. On-Demand Instances only
  - C. A mix of On-Demand Instances and Spot Instances
  - D. A mix of On-Demand Instances and Reserved Instances

---

Question 2: A company is building a mobile app on AWS. The company wants to expand its reach to millions of users. The company needs to build a platform so that authorized users can watch the company’s content on their mobile devices. What should a solutions architect recommend to meet these requirements?
  - A. Publish content to a public Amazon S3 bucket. Use AWS Key Management Service (AWS KMS) keys to stream content.
  - B. Set up IPsec VPN between the mobile app and the AWS environment to stream content.
  - [x] C. Use Amazon CloudFront. Provide signed URLs to stream content.
  - D. Set up AWS Client VPN between the mobile app and the AWS environment to stream content.

---
Question 3: A company is designing the network for an online multi-player game. The game uses the UDP networking protocol and will be deployed in eight AWS Regions. 
The network architecture needs to minimize latency and packet loss to give end users a high-quality gaming experience. Which solution will meet these requirements?
  - A. Setup a transit gateway in each Region. Create inter-Region peering attachments between each transit gateway.
  - [x] B. Set up AWS Global Accelerator with UDP listeners and endpoint groups in each Region.
  - C. Set up Amazon CloudFront with UDP turned on. Configure an origin in each Region.
  - D. Set up a VPC peering mesh between each Region. Turn on UDP for each VPC.

Option B (AWS Global Accelerator with UDP Listeners):
This is the best solution. Global Accelerator uses static anycast IPs to route user traffic to the nearest AWS edge location. From there, traffic travels over the AWS backbone (optimized for low latency/packet loss) to the closest healthy game server in one of the eight regions.

UDP Support: Explicitly supports UDP listeners.

Latency Reduction: Shortens the public internet path via edge locations.

Packet Loss Mitigation: Traffic uses AWS's reliable backbone and includes health checks for failover.

Simplicity: No complex peering mesh; endpoint groups direct traffic to regional resources (e.g., NLB, EC2).

Option C (CloudFront with UDP):
CloudFront is a CDN for HTTP(S)/WebSocket traffic and does not support UDP. It is unsuitable for real-time UDP game traffic.

---

Question 4: A company hosts a serverless application on AWS. The application uses Amazon API Gateway, AWS Lambda, and an Amazon RDS for PostgreSQL database. The company notices an increase in application errors that result from database connection timeouts during times of peak traffic or unpredictable traffic. The company needs a solution that reduces the application failures with the least amount of change to the code. What should a solutions architect do to meet these requirements?

  - A. Reduce the Lambda concurrency rate.
  - [x] B. Enable RDS Proxy on the RDS DB instance.
  - C. Resize the RDS DB instance class to accept more connections.
  - D. Migrate the database to Amazon DynamoDB with on-demand scaling.

https://aws.amazon.com/rds/proxy/

Many applications, including those built on modern serverless architectures, can have a large number of open connections to the database server and may open and close database connections at a high rate, exhausting database memory and compute resources. Amazon RDS Proxy allows applications to pool and share connections established with the database, improving database efficiency and application scalability. With Amazon RDS Proxy, failover times for Amazon Aurora and Amazon RDS databases are reduced by up to 66% and database credentials, authentication, and access can be managed through integration with AWS Secrets Manager and AWS Identity and Access Management (IAM).


---

Question 5: A company has a Java application that uses Amazon Simple Queue Service (Amazon SQS) to parse messages. The application cannot parse messages that are larger than 256 KB in size. The company wants to implement a solution to give the application the ability to parse messages as large as 50 MB. Which solution will meet these requirements with the FEWEST changes to the code?

- [x] A. Use the Amazon SQS Extended Client Library for Java to host messages that are larger than 256 KB in Amazon S3.
- B. Use Amazon EventBridge to post large messages from the application instead of Amazon SQS.
- C. Change the limit in Amazon SQS to handle messages that are larger than 256 KB.
- D. Store messages that are larger than 256 KB in Amazon Elastic File System (Amazon EFS). Configure Amazon SQS to reference this location in the messages.


https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-s3-messages.html

Use the Amazon SQS Extended Client Library for Java with Amazon S3 to manage large Amazon SQS messages, particularly for payloads ranging from 256 KB to 2 GB. The library stores the message payload in an Amazon S3 bucket and sends a message containing a reference to the stored object in the Amazon SQS queue.

- With the Amazon SQS Extended Client Library for Java, you can:
- Specify whether messages are always stored in Amazon S3 or only when the size of a message exceeds 256 KB
- Send a message that references a single message object stored in an S3 bucket
- Retrieve the message object from an Amazon S3 bucket
- Delete the message object from an Amazon S3 bucket

Why Other Options Fail:
B. Use EventBridge:
Requires rewriting the entire messaging layer (EventBridge doesn’t natively support large payloads; needs manual S3 integration).

C. Change SQS Limit:
Impossible—SQS has a fixed 256 KB message limit.

D. Use EFS:
Requires manual file I/O logic to read/write messages, VPC configuration, and filesystem mounting. Significantly more code changes.


---


Question 6: A transaction processing company has weekly scripted batch jobs that run on Amazon EC2 instances. The EC2 instances are in an Auto Scaling group. The number of transactions can vary, but the baseline CPU utilization that is noted on each run is at least 60%. The company needs to provision the capacity 30 minutes before the jobs run. Currently, engineers complete this task by manually modifying the Auto Scaling group parameters. The company does not have the resources to analyze the required capacity trends for the Auto Scaling group counts. The company needs an automated way to modify the Auto Scaling group's desired capacity. Which solution will meet these requirements with the LEAST operational overhead?

- A. Create a dynamic scaling policy for the Auto Scaling group. Configure the policy to scale based on the CPU utilization metric. Set the target value for the metric to 60%.
- B. Create a scheduled scaling policy for the Auto Scaling group. Set the appropriate desired capacity, minimum capacity, and maximum capacity. Set the recurrence to weekly. Set the start time to 30 minutes before the batch jobs run.
- [x] C. Create a predictive scaling policy for the Auto Scaling group. Configure the policy to scale based on forecast. Set the scaling metric to CPU utilization. Set the target value for the metric to 60%. In the policy, set the instances to pre-launch 30 minutes before the jobs run.
- D. Create an Amazon EventBridge event to invoke an AWS Lambda function when the CPU utilization metric value for the Auto Scaling group reaches 60%. Configure the Lambda function to increase the Auto Scaling group's desired capacity and maximum capacity by 20%.

---

Question 7

A company has an aging network-attached storage (NAS) array in its data center. The NAS array presents SMB shares and NFS shares to client workstations. The company does not want to purchase a new NAS array. The company also does not want to incur the cost of renewing the NAS array's support contract. Some of the data is accessed frequently, but much of the data is inactive. A solutions architect needs to implement a solution that migrates the data to Amazon S3, uses S3 Lifecycle policies, and maintains the same look and feel for the client workstations. The solutions architect has identified AWS Storage Gateway as part of the solution. Which type of storage gateway should the solutions architect provision to meet these requirements?

- A. Volume Gateway
- B. Tape Gateway
- C. Amazon FSx File Gateway
- [x] D. Amazon S3 File Gateway


---

Question 8

A company has an application that is running on Amazon EC2 instances. A solutions architect has standardized the company on a particular instance family and various instance sizes based on the current needs of the company. The company wants to maximize cost savings for the application over the next 3 years. The company needs to be able to change the instance family and sizes in the next 6 months based on application popularity and usage. Which solution will meet these requirements MOST cost-effectively?
- [x] A. Compute Savings Plan
- B. EC2 Instance Savings Plan
- C. Zonal Reserved Instances
- D. Standard Reserved Instances

> Standard and zonal reserved instances don't allow changes to an instance family
> EC2 Instance Savings Plans provide the lowest prices, offering savings up to 72% in exchange for commitment to usage of individual instance families in a Region

https://github.com/justinjiajia/certifications/blob/main/aws/cloud_practitioner/concepts.md#31-standard-ris

---

Question 9

A company collects data from a large number of participants who use wearable devices. The company stores the data in an Amazon DynamoDB table and uses applications to analyze the data. The data workload is constant and predictable. The company wants to stay at or below its forecasted budget for DynamoDB. Which solution will meet these requirements MOST cost-effectively?
- A. Use provisioned mode and DynamoDB Standard-Infrequent Access (DynamoDB Standard-IA). Reserve capacity for the forecasted workload.
- [x] B. Use provisioned mode. Specify the read capacity units (RCUs) and write capacity units (WCUs).
- C. Use on-demand mode. Set the read capacity units (RCUs) and write capacity units (WCUs) high enough to accommodate changes in the workload.
- D. Use on-demand mode. Specify the read capacity units (RCUs) and write capacity units (WCUs) with reserved capacity.


https://aws.amazon.com/dynamodb/pricing/provisioned/

When you select provisioned capacity mode, you specify the read and write capacity that you expect your application to require. You can use auto scaling to automatically adjust your table’s capacity based on the specified utilization rate to ensure application performance while reducing costs. DynamoDB charges one WCU for each write per second (up to 1 KB) and two WCUs for each transactional write per second. For reads, DynamoDB charges one RCU for each strongly consistent read per second, two RCUs for each transactional read per second, and one-half of an RCU for each eventually consistent read per second (up to 4 KB). You will be charged for the throughput capacity (reads and writes) you provision in your Amazon DynamoDB table, even if you do not fully utilize the provisioned capacity. The price for provisioned capacity depends on your table class. The actual reads and writes performance of your DynamoDB tables may vary and may be less than the throughput capacity that you provision.


https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/provisioned-capacity-mode.html

For provisioned mode tables, you specify throughput requirements in terms of capacity units. These units represent the amount of data your application needs to read or write per second. You can modify these settings later, if needed, or enable DynamoDB auto scaling to modify them automatically.

For an item up to 4 KB, one read capacity unit (RCU) represents one strongly consistent read operation per second, or two eventually consistent read operations per second. 

A write capacity unit (WCU) represents one write per second for an item up to 1 KB.


 The **DynamoDB Standard-IA table class** is ideal for use cases that require long-term storage of data that is infrequently accessed, such as application logs, old social media posts, ecommerce order history, and past gaming achievements.

The DynamoDB Standard-IA table class offers lower storage costs than the DynamoDB Standard tables, making it the most cost-effective option for tables with storage as the dominant table cost. The DynamoDB Standard table class offers lower throughput costs than the DynamoDB Standard-IA table class.


**DynamoDB auto scaling** actively manages provisioned throughput capacity for tables and global secondary indexes. With auto scaling, you define a range (upper and lower limits) for read and write capacity units. You also define a target utilization percentage within that range. DynamoDB auto scaling seeks to maintain your target utilization, even as your application workload increases or decreases.


---

Question 10

A company hosts a three-tier web application on Amazon EC2 instances in a single Availability Zone. The web application uses a self-managed MySQL database that is hosted on an EC2 instance to store data in an Amazon Elastic Block Store (Amazon EBS) volume. The MySQL database currently uses a 1 TB Provisioned IOPS SSD (io2) EBS volume. The company expects traffic of 1,000 IOPS for both reads and writes at peak traffic. The company wants to minimize any disruptions, stabilize performance, and reduce costs while retaining the capacity for double the IOPS. The company wants to move the database tier to a fully managed solution that is highly available and fault tolerant. Which solution will meet these requirements MOST cost-effectively?

- A. Use a Multi-AZ deployment of an Amazon RDS for MySQL DB instance with an io2 Block Express EBS volume.
- [x] B. Use a Multi-AZ deployment of an Amazon RDS for MySQL DB instance with a General Purpose SSD (gp2) EBS volume.
- C. Use Amazon S3 Intelligent-Tiering access tiers.
- D. Use two large EC2 instances to host the database in active-passive mode.

https://aws.amazon.com/ebs/pricing/
https://aws.amazon.com/ebs/provisioned-iops/
https://aws.amazon.com/blogs/aws/amazon-ebs-io2-block-express-volumes-with-amazon-ec2-r5b-instances-are-now-generally-available/

> io2 Block Express is a high-performance EBS volume supporting very high IOPS and throughput, but it is expensive and typically used for extreme performance needs. Likely over-provisioned and costly for 2,000 IOPS requirement.

> D. is a self-managed solution.

> C. is not relevant for database storage.

---

Question 11

A company is migrating an old application to AWS. The application runs a batch job every hour and is CPU intensive. The batch job takes 15 minutes on average with an on-premises server. The server has 64 virtual CPU (vCPU) and 512 GiB of memory. Which solution will run the batch job within 15 minutes with the LEAST operational overhead?

- A. Use AWS Lambda with functional scaling.
- B. Use Amazon Elastic Container Service (Amazon ECS) with AWS Fargate.
- C. Use Amazon Lightsail with AWS Auto Scaling.
- [x] D. Use AWS Batch on Amazon EC2.



AWS Batch is a fully managed batch computing service that plans, schedules, and runs your containerized batch ML, simulation, and analytics workloads across the full range of AWS compute offerings, such as Amazon ECS, Amazon EKS, AWS Fargate, and Spot or On-Demand Instances.


AWS Batch can automatically provision an EC2 instance with 64 vCPUs and 512 GiB RAM (e.g., c6i.32xlarge or similar). This matches the on-premises server specs, ensuring the job completes in 15 minutes. No resource constraints (unlike Lambda/Fargate).

AWS Batch manages infrastructure: Automatically launches EC2 instances when jobs are submitted; Terminates instances after job completion; Handles job queueing, retries, and scaling.

Only requires defining the job (Docker container or script) and resource requirements.



https://docs.aws.amazon.com/lambda/latest/dg/configuration-memory.html

Lambda runs your code for a set amount of time before timing out. Timeout is the maximum amount of time in seconds that a Lambda function can run. The default value for this setting is 3 seconds, but you can adjust this in increments of 1 second up to a maximum value of 900 seconds (15 minutes).

Lambda allocates CPU power in proportion to the amount of memory configured. Memory is the amount of memory available to your Lambda function at runtime. You can increase or decrease the memory and CPU power allocated to your function using the Memory setting. You can configure memory between 128 MB and 10,240 MB in 1-MB increments. At 1,769 MB, a function has the equivalent of one vCPU (one vCPU-second of credits per second). ( Resource Limits: Max 10 GB RAM and 6 vCPUs )

Amazon ECS task definition parameters for the Fargate launch type:
https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_definition_parameters.html#task_size

maximum values for vCPUs : 16vCPU

and memory: Between 32 GB and 120 GB in 8 GB increments


---


Question 12

A company stores its data objects in Amazon S3 Standard storage. A solutions architect has found that 75% of the data is rarely accessed after 30 days. The company needs all the data to remain immediately accessible with the same high availability and resiliency, but the company wants to minimize storage costs. Which storage solution will meet these requirements?

- A. Move the data objects to S3 Glacier Deep Archive after 30 days.
- [x] B. Move the data objects to S3 Standard-Infrequent Access (S3 Standard-IA) after 30 days.
- C. Move the data objects to S3 One Zone-Infrequent Access (S3 One Zone-IA) after 30 days.
- D. Move the data objects to S3 One Zone-Infrequent Access (S3 One Zone-IA) immediately.

---

Question 13

A gaming company is moving its public scoreboard from a data center to the AWS Cloud. The company uses Amazon EC2 Windows Server instances behind an Application Load Balancer to host its dynamic application. The company needs a highly available storage solution for the application. The application consists of static files and dynamic server-side code. Which combination of steps should a solutions architect take to meet these requirements? (Choose two.)

- [x] A. Store the static files on Amazon S3. Use Amazon CloudFront to cache objects at the edge.
- B. Store the static files on Amazon S3. Use Amazon ElastiCache to cache objects at the edge.
- C. Store the server-side code on Amazon Elastic File System (Amazon EFS). Mount the EFS volume on each EC2 instance to share the files.
- [x] D. Store the server-side code on Amazon FSx for Windows File Server. Mount the FSx for Windows File Server volume on each EC2 instance to share the files.
- E. Store the server-side code on a General Purpose SSD (gp2) Amazon Elastic Block Store (Amazon EBS) volume. Mount the EBS volume on each EC2 instance to share the files.


> servers: windows server instances

> Amazon EFS supports the Network File System version 4 (NFSv4.1 and NFSv4.0) protocol.

---

Question 14

A social media company runs its application on Amazon EC2 instances behind an Application Load Balancer (ALB). The ALB is the origin for an Amazon CloudFront distribution. The application has more than a billion images stored in an Amazon S3 bucket and processes thousands of images each second. The company wants to resize the images dynamically and serve appropriate formats to clients. Which solution will meet these requirements with the LEAST operational overhead?

- A. Install an external image management library on an EC2 instance. Use the image management library to process the images.
- B. Create a CloudFront origin request policy. Use the policy to automatically resize images and to serve the appropriate format based on the User-Agent HTTP header in the request.
- [x] C. Use a Lambda@Edge function with an external image management library. Associate the Lambda@Edge function with the CloudFront behaviors that serve the images.
- D. Create a CloudFront response headers policy. Use the policy to automatically resize images and to serve the appropriate format based on the User-Agent HTTP header in the request.


https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/lambda-at-the-edge.html

Lambda@Edge is an extension of AWS Lambda. Lambda@Edge is a compute service that lets you execute functions that customize the content that Amazon CloudFront delivers. 


After you create the function, you can add triggers using the Lambda console or CloudFront console so that the functions run in AWS locations that are closer to the viewer, without provisioning or managing servers

Lambda@Edge can inspect requests, resize images on the fly, serve appropriate formats, and cache results in CloudFront. Serverless and scalable.

origin request policies:
https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/controlling-origin-requests.html
https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/understanding-how-origin-request-policies-and-cache-policies-work-together.html

response headers policies

https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/understanding-response-headers-policies.html

---

Question 15

A hospital needs to store patient records in an Amazon S3 bucket. The hospital's compliance team must ensure that all protected health information (PHI) is encrypted in transit and at rest. The compliance team must administer the encryption key for data at rest. Which solution will meet these requirements?

- A. Create a public SSL/TLS certificate in AWS Certificate Manager (ACM). Associate the certificate with Amazon S3. Configure default encryption for each S3 bucket to use server-side encryption with AWS KMS keys (SSE-KMS). Assign the compliance team to manage the KMS keys.
- B. Use the aws:SecureTransport condition on S3 bucket policies to allow only encrypted connections over HTTPS (TLS). Configure default encryption for each S3 bucket to use server-side encryption with S3 managed encryption keys (SSE-S3). Assign the compliance team to manage the SSE-S3 keys.
- [x] C. Use the aws:SecureTransport condition on S3 bucket policies to allow only encrypted connections over HTTPS (TLS). Configure default encryption for each S3 bucket to use server-side encryption with AWS KMS keys (SSE-KMS). Assign the compliance team to manage the KMS keys.
- D. Use the aws:SecureTransport condition on S3 bucket policies to allow only encrypted connections over HTTPS (TLS). Use Amazon Macie to protect the sensitive data that is stored in Amazon S3. Assign the compliance team to manage Macie.

https://docs.aws.amazon.com/AmazonS3/latest/userguide/security-best-practices.html

"You can use HTTPS (TLS) to help prevent potential attackers from eavesdropping on or manipulating network traffic by using person-in-the-middle or similar attacks. We recommend allowing only encrypted connections over HTTPS (TLS) by using the aws:SecureTransport condition in your Amazon S3 bucket policies. "

https://docs.aws.amazon.com/AmazonS3/latest/userguide/example-bucket-policies.html#example-bucket-policies-HTTP-HTTPS

---

Question 16

A company uses Amazon API Gateway to run a private gateway with two REST APIs in the same VPC. The BuyStock RESTful web service calls the CheckFunds RESTful web service to ensure that enough funds are available before a stock can be purchased. The company has noticed in the VPC flow logs that the BuyStock RESTful web service calls the CheckFunds RESTful web service over the internet instead of through the VPC. A solutions architect must implement a solution so that the APIs communicate through the VPC. Which solution will meet these requirements with the FEWEST changes to the code?
  - A. Add an X-API-Key header in the HTTP header for authorization.
  - B. Use an interface endpoint.
  - C. Use a gateway endpoint.
  - D. Add an Amazon Simple Queue Service (Amazon SQS) queue between the two REST APIs.
---
Question 17: A company stores confidential data in an Amazon Aurora PostgreSQL database in the ap-southeast-3 Region. The database is encrypted with an AWS Key Management Service (AWS KMS) customer managed key. The company was recently acquired and must securely share a backup of the database with the acquiring company’s AWS account in ap-southeast-3. What should a solutions architect do to meet these requirements?
  - A. Create a database snapshot. Copy the snapshot to a new unencrypted snapshot. Share the new snapshot with the acquiring company’s AWS account.
  - B. Create a database snapshot. Add the acquiring company’s AWS account to the KMS key policy. Share the snapshot with the acquiring company’s AWS account.
  - C. Create a database snapshot that uses a different AWS managed KMS key. Add the acquiring company’s AWS account to the KMS key alias. Share the snapshot with the acquiring company’s AWS account.
  - D. Create a database snapshot. Download the database snapshot. Upload the database snapshot to an Amazon S3 bucket. Update the S3 bucket policy to allow access from the acquiring company’s AWS account.

---

Question 18: A company uses a 100 GB Amazon RDS for Microsoft SQL Server Single-AZ DB instance in the us-east-1 Region to store customer transactions. The company needs high availability and automatic recovery for the DB instance. The company must also run reports on the RDS database several times a year. The report process causes transactions to take longer than usual to post to the customers’ accounts. The company needs a solution that will improve the performance of the report process. Which combination of steps will meet these requirements? (Choose two.)
  - A. Modify the DB instance from a Single-AZ DB instance to a Multi-AZ deployment.
  - B. Take a snapshot of the current DB instance. Restore the snapshot to a new RDS deployment in another Availability Zone.
  - C. Create a read replica of the DB instance in a different Availability Zone. Point all requests for reports to the read replica.
  - D. Migrate the database to RDS Custom.
  - E. Use RDS Proxy to limit reporting requests to the maintenance window.

---

Question 19: A solutions architect is designing a company’s disaster recovery (DR) architecture. The company has a MySQL database that runs on an Amazon EC2 instance in a private subnet with scheduled backup. The DR design needs to include multiple AWS Regions. Which solution will meet these requirements with the LEAST operational overhead?
  - A. Migrate the MySQL database to multiple EC2 instances. Configure a standby EC2 instance in the DR Region. Turn on replication.
  - B. Migrate the MySQL database to Amazon RDS. Use a Multi-AZ deployment. Turn on read replication for the primary DB instance in the different Availability Zones.
  - C. Migrate the MySQL database to an Amazon Aurora global database. Host the primary DB cluster in the primary Region. Host the secondary DB cluster in the DR Region.
  - D. Store the scheduled backup of the MySQL database in an Amazon S3 bucket that is configured for S3 Cross-Region Replication (CRR). Use the data backup to restore the database in the DR Region.

---

Question 20: A company wants to restrict access to the content of one of its main web applications and to protect the content by using authorization techniques available on AWS. The company wants to implement a serverless architecture and an authentication solution for fewer than 100 users. The solution needs to integrate with the main web application and serve web content globally. The solution must also scale as the company’s user base grows while providing the lowest login latency possible. Which solution will meet these requirements MOST cost-effectively?
  - A. Use Amazon Cognito for authentication. Use Lambda@Edge for authorization. Use Amazon CloudFront to serve the web application globally.
  - B. Use AWS Directory Service for Microsoft Active Directory for authentication. Use AWS Lambda for authorization. Use an Application Load Balancer to serve the web application globally.
  - C. Use Amazon Cognito for authentication. Use AWS Lambda for authorization. Use Amazon S3 Transfer Acceleration to serve the web application globally.
  - D. Use AWS Directory Service for Microsoft Active Directory for authentication. Use Lambda@Edge for authorization. Use AWS Elastic Beanstalk to serve the web application globally.
---

Question 21: A company is moving its data management application to AWS. The company wants to transition to an event-driven architecture. The architecture needs to be more distributed and to use serverless concepts while performing the different aspects of the workflow. The company also wants to minimize operational overhead. Which solution will meet these requirements?
  - A. Build out the workflow in AWS Glue. Use AWS Glue to invoke AWS Lambda functions to process the workflow steps.
  - B. Build out the workflow in AWS Step Functions. Deploy the application on Amazon EC2 instances. Use Step Functions to invoke the workflow steps on the EC2 instances.
  - C. Build out the workflow in Amazon EventBridge. Use EventBridge to invoke AWS Lambda functions on a schedule to process the workflow steps.
  - D. Build out the workflow in AWS Step Functions. Use Step Functions to create a state machine. Use the state machine to invoke AWS Lambda functions to process the workflow steps.

Question 22: A company hosts a multiplayer gaming application on AWS. The company wants the application to read data with sub-millisecond latency and run one-time queries on historical data. Which solution will meet these requirements with the LEAST operational overhead?
  - A. Use Amazon RDS for data that is frequently accessed. Run a periodic custom script to export the data to an Amazon S3 bucket.
  - B. Store the data directly in an Amazon S3 bucket. Implement an S3 Lifecycle policy to move older data to S3 Glacier Deep Archive for long-term storage. Run one-time queries on the data in Amazon S3 by using Amazon Athena.
  - C. Use Amazon DynamoDB with DynamoDB Accelerator (DAX) for data that is frequently accessed. Export the data to an Amazon S3 bucket by using DynamoDB table export. Run one-time queries on the data in Amazon S3 by using Amazon Athena.
  - D. Use Amazon DynamoDB for data that is frequently accessed. Turn on streaming to Amazon Kinesis Data Streams. Use Amazon Kinesis Data Firehose to read the data from Kinesis Data Streams. Store the records in an Amazon S3 bucket.

Question 23: A company uses a payment processing system that requires messages for a particular payment ID to be received in the same order that they were sent. Otherwise, the payments might be processed incorrectly. Which actions should a solutions architect take to meet this requirement? (Choose two.)
  - A. Write the messages to an Amazon DynamoDB table with the payment ID as the partition key.
  - B. Write the messages to an Amazon Kinesis data stream with the payment ID as the partition key.
  - C. Write the messages to an Amazon ElastiCache for Memcached cluster with the payment ID as the key.
  - D. Write the messages to an Amazon Simple Queue Service (Amazon SQS) queue. Set the message attribute to use the payment ID.
  - E. Write the messages to an Amazon Simple Queue Service (Amazon SQS) FIFO queue. Set the message group to use the payment ID.

Question 24: A company is building a game system that needs to send unique events to separate leaderboard, matchmaking, and authentication services concurrently. The company needs an AWS event-driven system that guarantees the order of the events. Which solution will meet these requirements?
  - A. Amazon EventBridge event bus
  - B. Amazon Simple Notification Service (Amazon SNS) FIFO topics
  - C. Amazon Simple Notification Service (Amazon SNS) standard topics
  - D. Amazon Simple Queue Service (Amazon SQS) FIFO queues

Question 25: A hospital is designing a new application that gathers symptoms from patients. The hospital has decided to use Amazon Simple Queue Service (Amazon SQS) and Amazon Simple Notification Service (Amazon SNS) in the architecture. A solutions architect is reviewing the infrastructure design. Data must be encrypted at rest and in transit. Only authorized personnel of the hospital should be able to access the data. Which combination of steps should the solutions architect take to meet these requirements? (Choose two.)
  - A. Turn on server-side encryption on the SQS components. Update the default key policy to restrict key usage to a set of authorized principals.
  - B. Turn on server-side encryption on the SNS components by using an AWS Key Management Service (AWS KMS) customer managed key. Apply a key policy to restrict key usage to a set of authorized principals.
  - C. Turn on encryption on the SNS components. Update the default key policy to restrict key usage to a set of authorized principals. Set a condition in the topic policy to allow only encrypted connections over TLS.
  - D. Turn on server-side encryption on the SQS components by using an AWS Key Management Service (AWS KMS) customer managed key. Apply a key policy to restrict key usage to a set of authorized principals. Set a condition in the queue policy to allow only encrypted connections over TLS.
  - E. Turn on server-side encryption on the SQS components by using an AWS Key Management Service (AWS KMS) customer managed key. Apply an IAM policy to restrict key usage to a set of authorized principals. Set a condition in the queue policy to allow only encrypted connections over TLS.

Question 26: A company runs a web application that is backed by Amazon RDS. A new database administrator caused data loss by accidentally editing information in a database table. To help recover from this type of incident, the company wants the ability to restore the database to its state from 5 minutes before any change within the last 30 days. Which feature should the solutions architect include in the design to meet this requirement?
  - A. Read replicas
  - B. Manual snapshots
  - C. Automated backups
  - D. Multi-AZ deployments

Question 27: A company’s web application consists of an Amazon API Gateway API in front of an AWS Lambda function and an Amazon DynamoDB database. The Lambda function handles the business logic, and the DynamoDB table hosts the data. The application uses Amazon Cognito user pools to identify the individual users of the application. A solutions architect needs to update the application so that only users who have a subscription can access premium content. Which solution will meet this requirement with the LEAST operational overhead?
  - A. Enable API caching and throttling on the API Gateway API.
  - B. Set up AWS WAF on the API Gateway API. Create a rule to filter users who have a subscription.
  - C. Apply fine-grained IAM permissions to the premium content in the DynamoDB table.
  - D. Implement API usage plans and API keys to limit the access of users who do not have a subscription.

Question 28: A company is using Amazon Route 53 latency-based routing to route requests to its UDP-based application for users around the world. The application is hosted on redundant servers in the company’s on-premises data centers in the United States, Asia, and Europe. The company’s compliance requirements state that the application must be hosted on premises. The company wants to improve the performance and availability of the application. What should a solutions architect do to meet these requirements?
  - A. Configure three Network Load Balancers (NLBs) in the three AWS Regions to address the on-premises endpoints. Create an accelerator by using AWS Global Accelerator, and register the NLBs as its endpoints. Provide access to the application by using a CNAME that points to the accelerator DNS.
  - B. Configure three Application Load Balancers (ALBs) in the three AWS Regions to address the on-premises endpoints. Create an accelerator by using AWS Global Accelerator, and register the ALBs as its endpoints. Provide access to the application by using a CNAME that points to the accelerator DNS.
  - C. Configure three Network Load Balancers (NLBs) in the three AWS Regions to address the on-premises endpoints. In Route 53, create a latency-based record that points to the three NLBs, and use it as an origin for an Amazon CloudFront distribution. Provide access to the application by using a CNAME that points to the CloudFront DNS.
  - D. Configure three Application Load Balancers (ALBs) in the three AWS Regions to address the on-premises endpoints. In Route 53, create a latency-based record that points to the three ALBs, and use it as an origin for an Amazon CloudFront distribution. Provide access to the application by using a CNAME that points to the CloudFront DNS.

Question 29: A solutions architect wants all new users to have specific complexity requirements and mandatory rotation periods for IAM user passwords. What should the solutions architect do to accomplish this?
  - A. Set an overall password policy for the entire AWS account.
  - B. Set a password policy for each IAM user in the AWS account.
  - C. Use third-party vendor software to set password requirements.
  - D. Attach an Amazon CloudWatch rule to the Create_newuser event to set the password with the appropriate requirements.

Question 30: A company has migrated an application to Amazon EC2 Linux instances. One of these EC2 instances runs several 1-hour tasks on a schedule. These tasks were written by different teams and have no common programming language. The company is concerned about performance and scalability while these tasks run on a single instance. A solutions architect needs to implement a solution to resolve these concerns. Which solution will meet these requirements with the LEAST operational overhead?
  - A. Use AWS Batch to run the tasks as jobs. Schedule the jobs by using Amazon EventBridge (Amazon CloudWatch Events).
  - B. Convert the EC2 instance to a container. Use AWS App Runner to create the container on demand to run the tasks as jobs.
  - C. Copy the tasks into AWS Lambda functions. Schedule the Lambda functions by using Amazon EventBridge (Amazon CloudWatch Events).
  - D. Create an Amazon Machine Image (AMI) of the EC2 instance that runs the tasks. Create an Auto Scaling group with the AMI to run multiple copies of the instance.

Question 31: A company runs a public three-tier web application in a VPC. The application runs on Amazon EC2 instances across multiple Availability Zones. The EC2 instances that run in private subnets need to communicate with a license server over the internet. The company needs a managed solution that minimizes operational maintenance. Which solution meets these requirements?
  - A. Provision a NAT instance in a public subnet. Modify each private subnet’s route table with a default route that points to the NAT instance.
  - B. Provision a NAT instance in a private subnet. Modify each private subnet’s route table with a default route that points to the NAT instance.
  - C. Provision a NAT gateway in a public subnet. Modify each private subnet’s route table with a default route that points to the NAT gateway.
  - D. Provision a NAT gateway in a private subnet. Modify each private subnet’s route table with a default route that points to the NAT gateway.

Question 32: A company needs to create an Amazon Elastic Kubernetes Service (Amazon EKS) cluster to host a digital media streaming application. The EKS cluster will use a managed node group that is backed by Amazon Elastic Block Store (Amazon EBS) volumes for storage. The company must encrypt all data at rest by using a customer managed key that is stored in AWS Key Management Service (AWS KMS). Which combination of actions will meet this requirement with the LEAST operational overhead? (Choose two.)
  - A. Use a Kubernetes plugin that uses the customer managed key to perform data encryption.
  - B. After creation of the EKS cluster, locate the EBS volumes. Enable encryption by using the customer managed key.
  - C. Enable EBS encryption by default in the AWS Region where the EKS cluster will be created. Select the customer managed key as the default key.
  - D. Create the EKS cluster. Create an IAM role that has a policy that grants permission to the customer managed key. Associate the role with the EKS cluster.
  - E. Store the customer managed key as a Kubernetes secret in the EKS cluster. Use the customer managed key to encrypt the EBS volumes.

Question 33: A company wants to migrate an Oracle database to AWS. The database consists of a single table that contains millions of geographic information systems (GIS) images that are high resolution and are identified by a geographic code. When a natural disaster occurs, tens of thousands of images get updated every few minutes. Each geographic code has a single image or row that is associated with it. The company wants a solution that is highly available and scalable during such events. Which solution meets these requirements MOST cost-effectively?
  - A. Store the images and geographic codes in a database table. Use Oracle running on an Amazon RDS Multi-AZ DB instance.
  - B. Store the images in Amazon S3 buckets. Use Amazon DynamoDB with the geographic code as the key and the image S3 URL as the value.
  - C. Store the images and geographic codes in an Amazon DynamoDB table. Configure DynamoDB Accelerator (DAX) during times of high load.
  - D. Store the images in Amazon S3 buckets. Store geographic codes and image S3 URLs in a database table. Use Oracle running on an Amazon RDS Multi-AZ DB instance.

Question 34: A company has an application that collects data from IoT sensors on automobiles. The data is streamed and stored in Amazon S3 through Amazon Kinesis Data Firehose. The data produces trillions of S3 objects each year. Each morning, the company uses the data from the previous 30 days to retrain a suite of machine learning (ML) models. Four times each year, the company uses the data from the previous 12 months to perform analysis and train other ML models. The data must be available with minimal delay for up to 1 year. After 1 year, the data must be retained for archival purposes. Which storage solution meets these requirements MOST cost-effectively?
  - A. Use the S3 Intelligent-Tiering storage class. Create an S3 Lifecycle policy to transition objects to S3 Glacier Deep Archive after 1 year.
  - B. Use the S3 Intelligent-Tiering storage class. Configure S3 Intelligent-Tiering to automatically move objects to S3 Glacier Deep Archive after 1 year.
  - C. Use the S3 Standard-Infrequent Access (S3 Standard-IA) storage class. Create an S3 Lifecycle policy to transition objects to S3 Glacier Deep Archive after 1 year.
  - D. Use the S3 Standard storage class. Create an S3 Lifecycle policy to transition objects to S3 Standard-Infrequent Access (S3 Standard-IA) after 30 days, and then to S3 Glacier Deep Archive after 1 year.

Question 35: A company is running several business applications in three separate VPCs within the us-east-1 Region. The applications must be able to communicate between VPCs. The applications also must be able to consistently send hundreds of gigabytes of data each day to a latency-sensitive application that runs in a single on-premises data center. A solutions architect needs to design a network connectivity solution that maximizes cost-effectiveness. Which solution meets these requirements?
  - A. Configure three AWS Site-to-Site VPN connections from the data center to AWS. Establish connectivity by configuring one VPN connection for each VPC.
  - B. Launch a third-party virtual network appliance in each VPC. Establish an IPsec VPN tunnel between the data center and each virtual appliance.
  - C. Set up three AWS Direct Connect connections from the data center to a Direct Connect gateway in us-east-1. Establish connectivity by configuring each VPC to use one of the Direct Connect connections.
  - D. Set up one AWS Direct Connect connection from the data center to AWS. Create a transit gateway, and attach each VPC to the transit gateway. Establish connectivity between the Direct Connect connection and the transit gateway.

Question 36: An ecommerce company is building a distributed application that involves several serverless functions and AWS services to complete order-processing tasks. These tasks require manual approvals as part of the workflow. A solutions architect needs to design an architecture for the order-processing application. The solution must be able to combine multiple AWS Lambda functions into responsive serverless applications. The solution also must orchestrate data and services that run on Amazon EC2 instances, containers, or on-premises servers. Which solution will meet these requirements with the LEAST operational overhead?
  - A. Use AWS Step Functions to build the application.
  - B. Integrate all the application components in an AWS Glue job.
  - C. Use Amazon Simple Queue Service (Amazon SQS) to build the application.
  - D. Use AWS Lambda functions and Amazon EventBridge events to build the application.

Question 37: A company has launched an Amazon RDS for MySQL DB instance. Most of the connections to the database come from serverless applications. Application traffic to the database changes significantly at random intervals. At times of high demand, users report that their applications experience database connection rejection errors. Which solution will resolve this issue with the LEAST operational overhead?
  - A. Create a proxy in RDS Proxy. Configure the users’ applications to use the DB instance through RDS Proxy.
  - B. Deploy Amazon ElastiCache for Memcached between the users’ applications and the DB instance.
  - C. Migrate the DB instance to a different instance class that has higher I/O capacity. Configure the users’ applications to use the new DB instance.
  - D. Configure Multi-AZ for the DB instance. Configure the users’ applications to switch between the DB instances.

Question 38: A company recently deployed a new auditing system to centralize information about operating system versions, patching, and installed software for Amazon EC2 instances. A solutions architect must ensure all instances provisioned through EC2 Auto Scaling groups successfully send reports to the auditing system as soon as they are launched and terminated. Which solution achieves these goals MOST efficiently?
  - A. Use a scheduled AWS Lambda function and run a script remotely on all EC2 instances to send data to the audit system.
  - B. Use EC2 Auto Scaling lifecycle hooks to run a custom script to send data to the audit system when instances are launched and terminated.
  - C. Use an EC2 Auto Scaling launch configuration to run a custom script through user data to send data to the audit system when instances are launched and terminated.
  - D. Run a custom script on the instance operating system to send data to the audit system. Configure the script to be invoked by the EC2 Auto Scaling group when the instance starts and is terminated.

Question 39: A company is developing a real-time multiplayer game that uses UDP for communications between the client and servers in an Auto Scaling group. Spikes in demand are anticipated during the day, so the game server platform must adapt accordingly. Developers want to store gamer scores and other non-relational data in a database solution that will scale without intervention. Which solution should a solutions architect recommend?
  - A. Use Amazon Route 53 for traffic distribution and Amazon Aurora Serverless for data storage.
  - B. Use a Network Load Balancer for traffic distribution and Amazon DynamoDB on-demand for data storage.
  - C. Use a Network Load Balancer for traffic distribution and Amazon Aurora Global Database for data storage.
  - D. Use an Application Load Balancer for traffic distribution and Amazon DynamoDB global tables for data storage.

Question 40: A company hosts a frontend application that uses an Amazon API Gateway API backend that is integrated with AWS Lambda. When the API receives requests, the Lambda function loads many libraries. Then the Lambda function connects to an Amazon RDS database, processes the data, and returns the data to the frontend application. The company wants to ensure that response latency is as low as possible for all its users with the fewest number of changes to the company’s operations. Which solution will meet these requirements?
  - A. Establish a connection between the frontend application and the database to make queries faster by bypassing the API.
  - B. Configure provisioned concurrency for the Lambda function that handles the requests.
  - C. Cache the results of the queries in Amazon S3 for faster retrieval of similar datasets.
  - D. Increase the size of the database to increase the number of connections Lambda can establish at one time.

