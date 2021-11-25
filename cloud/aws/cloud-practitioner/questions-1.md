Question 1Correct**Domain:** Security

Which AWS service provides infrastructure security optimization recommendations?

*   A. AWS Application Programming Interface(API)
*   B. Reserved Instances
*   C. AWS Trusted Advisorright
*   D. Amazon Elastic Compute Cloud (Amazon EC2) SpotFleet

###### Explanation:

Answer – C

The AWS documentation mentions the following:

 An online resource to help you reduce cost, increase performance, and improve security by optimizing your AWS environment, Trusted Advisor provides real time guidance to help you provision your resources following AWS best practices

For more information on the AWS Trusted Advisor, please refer to the below URL:

*   [https://aws.amazon.com/premiumsupport/trustedadvisor/](https://aws.amazon.com/premiumsupport/trustedadvisor/)

Choices A, B, and D are incorrect. They are not related to infrastructure security optimization.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 2Correct**Domain:** Technology

A file-sharing service uses Amazon S3 to store files uploaded by users. Files are accessed with random frequency. Popular ones are downloaded every day whilst others not so often and some rarely. What is the most cost-effective Amazon S3 object storage class to implement?

*   A. Amazon S3 Standard
*   B. Amazon S3 Glacier
*   C. Amazon S3 One Zone-Infrequently Accessed
*   D. Amazon S3 Intelligent-Tieringright

###### Explanation:

**Correct Answer – D**

S3 Intelligent-Tiering is a new Amazon S3 storage class designed for customers who want to optimize storage costs automatically when data access patterns change, without performance impact or operational overhead. S3 Intelligent-Tiering is the first cloud object storage class that delivers automatic cost savings by moving data between two access tiers — frequent access and infrequent access — when access patterns change, and is ideal for data with unknown or changing access patterns.

S3 Intelligent-Tiering stores objects in two access tiers: one tier optimized for frequent access and another lower-cost tier optimized for infrequent access. For a small monthly monitoring and automation fee per object, S3 Intelligent-Tiering monitors access patterns and moves objects that have not been accessed for 30 consecutive days to the infrequent access tier. There are no retrieval fees in S3 Intelligent-Tiering. If an object in the infrequent access tier is accessed later, it is automatically moved back to the frequent access tier. No additional tiering fees apply when objects are moved between access tiers within the S3 Intelligent-Tiering storage class. S3 Intelligent-Tiering is designed for 99.9% availability and 99.999999999% durability, and offers the same low latency and high throughput performance of S3 Standard.

[https://aws.amazon.com/about-aws/whats-new/2018/11/s3-intelligent-tiering/](https://aws.amazon.com/about-aws/whats-new/2018/11/s3-intelligent-tiering/)

*   **Option A is incorrect** because Amazon S3 Standard would be an inefficient class for storing those objects that will be accessed rarely.
*   **Option B is incorrect** because storing objects that are frequently accessed in Amazon S3 Glacier would present operational bottlenecks since these objects would not be available instantly.
    *   [https://aws.amazon.com/s3/storage-classes/](https://aws.amazon.com/s3/storage-classes/)
*   **Option C is incorrect** because storing those objects that are rarely accessed and those that would be accessed frequently in Amazon S3 One Zone-Infrequently Accessed would be inefficient.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 3Correct**Domain:** Technology

Which AWS service can be deployed to enhance read performance for applications while reading data from NoSQL database?

*   A. Amazon Route 53
*   B. Amazon DynamoDB Acceleratorright
*   C. Amazon CloudFront
*   D. AWS Greengrass

###### Explanation:

**Correct Answer – B**

Amazon DynamoDB Accelerator (DAX) is a caching service for DynamoDB which can be deployed in VPC in a region where DynamoDB is deployed. For read-heavy applications, DAX can be deployed to increase throughput by providing in-memory caching.

*   **Option A is incorrect** becauseAmazon Route 53 is an AWS DNS service and cannot improve the performance of DynamoDB.
*   **Option C is incorrect **because Amazon CloudFront is a global content delivery network that cannot be applied to a DynamoDB table.
*   **Option D is incorrect **becauseAWS Greengrass is data caching software for connected devices.

For more information on caching solutions with AWS, refer to the following URL:

*   [https://aws.amazon.com/caching/aws-caching/](https://aws.amazon.com/caching/aws-caching/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 4Correct**Domain:** Technology0

An organization utilizes a software suite that consists of a multitude of underlying microservices hosted on the cloud. The application is frequently giving runtime errors. Which service will help in the troubleshooting process?

*   A. AWS CloudTrail
*   B. AWS CloudWatch
*   C. AWS X-Rayright
*   D. Amazon OpenSearch Service

###### Explanation:

**Correct Answer – C**

AWS X-Ray is a service that collects data about requests that your application serves and provides tools that you can use to view, filter, and gain insights into that data to identify issues and opportunities for optimization. AWS X-Ray helps developers analyze and debug production, distributed applications, such as those built using a microservices architecture.

[https://aws.amazon.com/xray/](https://aws.amazon.com/xray/)

**Option A is INCORRECT** because AWS CloudTrail primarily records user or API activity, ‘who has done what.’ It logs, continuously monitors, and retains account activity related to actions across AWS infrastructure. CloudTrail provides event history in the AWS account activity but NOT that of the interaction of software microservices within a suite.

[https://aws.amazon.com/cloudtrail/](https://aws.amazon.com/cloudtrail/)

**Option B is INCORRECT** because AWS CloudWatch does the primary function of monitoring and NOT debugging. It collates data and actionable insights to monitor applications. It also responds to system-wide performance changes, optimizes resource utilization, and gets a unified view of operational health. However, the service does neither debug nor logs errors that occur amongst software microservices within a suite.

[https://aws.amazon.com/cloudwatch/](https://aws.amazon.com/cloudwatch/)

**Option D is INCORRECT** because Amazon OpenSearch Service is a managed service that makes it easy to deploy, operate, and scale OpenSearch clusters in the AWS Cloud. It automatically detects and replaces failed OpenSearch Service nodes, reducing the overhead associated with self-managed infrastructures. 

[https://docs.aws.amazon.com/opensearch-service/latest/developerguide/what-is.html](https://docs.aws.amazon.com/opensearch-service/latest/developerguide/what-is.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 5Correct**Domain:** Cloud Concepts

According to the AWS, what is the benefit of Elasticity?

*   A. Minimize storage requirements by reducing logging and auditing activities
*   B. Create systems that scale to the required capacity based on changes in demandright
*   C. Enable AWS to automatically select the most cost-effective services.
*   D. Accelerate the design process because recovery from failure is automated, reducing the need for testing

###### Explanation:

Answer – B

The concept of Elasticity is the means of an application having the ability to scale up and scale down based on demand. An example of such a service is the Autoscaling service

For more information on AWS Autoscaling service, please refer to the below URL:

*   [https://aws.amazon.com/autoscaling/](https://aws.amazon.com/autoscaling/)

A, C and D are incorrect. Elasticity will not have positive effects on storage, cost or design agility.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 6Correct**Domain:** Billing and Pricing

Which tool can you use to forecast your AWS spending?

*   A. AWS Organizations
*   B. Amazon Dev Pay
*   C. AWS Trusted Advisor
*   D. AWS Cost Explorerright

###### Explanation:

Answer – D

The AWS Documentation mentions the following.

Cost Explorer is a free tool that you can use to view your costs. You can view data up to the last 12 months. You can forecast how much you are likely to spend for the next 12 months and get recommendations for what Reserved Instances to purchase. You can use Cost Explorer to see patterns in how much you spend on AWS resources over time, identify areas that need further inquiry, and see trends that you can use to understand your costs. You also can specify time ranges for the data and view time data by day or by month.

For more information on the AWS Cost Explorer, please refer to the below URL:

*   [http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/cost-explorer-what-is.html](http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/cost-explorer-what-is.html)

A, B and C are incorrect. These services do not relate to billing and cost.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 7Incorrect**Domain:** Security

Which of the following is an optional Security layer attached to a subnet within a VPC for controlling traffic in & out of the VPC?

*   A. VPC Flow Logs
*   B. Web Application Firewall
*   C. Security Groupwrong
*   D. Network ACLright

###### Explanation:

**Correct Answer – D**

Network ACL can be additionally configured on subnet level to control traffic in & out of the VPC.

*   **Option A is incorrect. **VPC Flow Logs will capture information about IP traffic in & out of VPC. This will not be used for controlling purposes.
*   **Option B is incorrect. **Web Application Firewall (WAF) can be configured to protect web applications from common security threats. It can be deployed on devices such as Amazon CloudFront, Application Load Balancer and Amazon API Gateway.
*   **Option C is incorrect.** Security Groups are attached at instance level & not at the subnet level.

For more information on security within VPC, refer to the following URL:

*   [https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Security.html#VPC_Security_Comparison](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Security.html#VPC_Security_Comparison)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 8Correct**Domain:** Security

Which of the following is a customer responsibility under AWS Shared Responsibility Model?

*   A. Patching of host OS deployed on Amazon S3.
*   B. Logical Access controls for underlying infrastructure.
*   C. Physical security of the facilities.
*   D. Patching of guest OS deployed on Amazon EC2 instance.right

###### Explanation:

**Correct Answer – D**

Under the AWS shared responsibility model, AWS takes care of infrastructure configuration & management while customers must take care of the resources they launched within AWS.

*   **Option A is incorrect. **Amazon S3 is part of the infrastructure layer & Patching of host OS/Configuration for Amazon S3 is responsibility of AWS.
*   **Option B is incorrect.** AWS has the responsibility for the Logical Access controls for the underlying infrastructure.
*   **Option C is incorrect.** Physical Security of the facilities is AWS responsibility.

For more information on Shared responsibility model, refer to the following URL:

*   [https://aws.amazon.com/compliance/shared-responsibility-model](https://aws.amazon.com/compliance/shared-responsibility-model/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 9Correct**Domain:** Technology

What is the AWS feature that enables fast, easy and secure transfers of files over long distances between your client and your Amazon S3 bucket?

*   A. File Transfer
*   B. HTTP Transfer
*   C. Amazon S3 Transfer Accelerationright
*   D. S3 Acceleration

###### Explanation:

Answer – C

The AWS Documentation mentions the following.

Amazon S3 Transfer Acceleration enables fast, easy, and secure transfers of files over long distances between your client and an S3 bucket. Transfer Acceleration takes advantage of Amazon CloudFront’s globally distributed edge locations. As the data arrives at an edge location, data is routed to Amazon S3 over an optimized network path.

For more information on S3 transfer acceleration, please visit the Link:

*   [http://docs.aws.amazon.com/AmazonS3/latest/dev/transfer-acceleration.html](http://docs.aws.amazon.com/AmazonS3/latest/dev/transfer-acceleration.html)

Options A, B and D are incorrect. These features deal with transferring data but not between clients and an S3 bucket.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 10Incorrect**Domain:** Technology

Which of the following services can be used to optimize performance for global users to transfer large-sized data objects to a centralized Amazon S3 bucket in us-west-1 region?

*   A. Enable S3 Transfer Acceleration on Amazon S3 bucket.right
*   B. Use Amazon CloudFront Put/Post commands
*   C. Use Multipart uploadwrong
*   D. Use Amazon ElastiCache

###### Explanation:

**Correct Answer – A**

S3 Transfer Acceleration can optimise performance for data transfer between users & objects in Amazon S3 bucket. Transfer acceleration uses CloudFront edge location to provide accelerated data transfer to users.

*   **Option B is incorrect** as Amazon CloudFront Put/Post commands can be used for small-sized objects but for large-sized data objects, S3 Transfer Acceleration provides better performance.
*   **Option C is incorrect** as users should use Multipart uploads for all data objects exceeding 100 megabytes. But for better performance, S3 transfer acceleration should be enabled.
*   **Option D is incorrect** as for global users accessing S3 bucket, S3 Transfer Acceleration is a better choice.. 

For more information on Amazon S3 Transfer Acceleration, refer to the following URLs:

*   [https://aws.amazon.com/s3/faqs/#s3ta](https://aws.amazon.com/s3/faqs/#s3ta)
*   [https://docs.aws.amazon.com/AmazonS3/latest/dev/optimizing-performance.html](https://docs.aws.amazon.com/AmazonS3/latest/dev/optimizing-performance.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 11Correct**Domain:** Technology

There is a requirement to store objects. The objects must be downloadable via a URL. Which storage option would you choose?

*   A. Amazon S3right
*   B. Amazon Glacier
*   C. Amazon Storage Gateway
*   D. Amazon EBS

###### Explanation:

Answer - A

Amazon S3 is the perfect storage option. It also provides the facility of assigning a URL to each object which can be used to download the object.

*   For more information on AWS S3, please visit the Link:
    *   [https://aws.amazon.com/s3/](https://aws.amazon.com/s3/)
*   B is incorrect. Glacier is for archival and long-term storage.

This question is to check the user understanding of AWS S3 service terminology and use cases. Objects are stored in S3 and should be downloadable via a URL. It's not possible with EBS.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 12Correct**Domain:** Billing and Pricing

There is a requirement to host a database server for a minimum period of one year. Which of the following would result in the least cost?

*   A. Spot Instances
*   B. On-Demand
*   C. No Upfront costs Reserved
*   D. Partial Upfront costs Reservedright

###### Explanation:

Answer - D

If the database is going to be used for a minimum of one year at least, it is better to get Reserved Instances. You can save on costs if you use partial upfront options.

*   For more information on AWS Reserved Instances, please visit the Link:
    *   [https://aws.amazon.com/ec2/pricing/reserved-instances/](https://aws.amazon.com/ec2/pricing/reserved-instances/)

*   **A is incorrect**. Spot instances can be terminated with fluctuations in market prices. Unless the question specifies a use case where high availability is not a requirement, this cannot be assumed.
*   **B is incorrect**. On-Demand is not the most cost-efficient solution.
*   **C is incorrect**. No upfront payment is required. However, it's a costlier option than Partial/All upfront payment.

*   For more information on the Reserved Instances Payment option, please check below AWS Docs:
    *   [https://docs.aws.amazon.com/aws-technical-content/latest/cost-optimization-reservation-models/reserved-instance-payment-options.html](https://docs.aws.amazon.com/aws-technical-content/latest/cost-optimization-reservation-models/reserved-instance-payment-options.html)

**Note:**

*   Reserved Instances do not renew automatically. When they expire, you can continue using the EC2 instance without interruption. But you are charged On-Demand rates. In the above example, when the Reserved Instances that cover the T2 and C4 instances expire, you go back to paying the On-Demand rates until you terminate the instances or purchase new Reserved Instances that match the instance attributes.
    *   [https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-reserved-instances.html](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-reserved-instances.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 13Correct**Domain:** Security

During an organization’s information systems audit, the administrator is requested to provide a dossier of security and compliance reports and online service agreements between the organization and AWS. Which service can they utilize to acquire this information?

*   A. AWS Artifactright
*   B. AWS Resource Center
*   C. AWS Service Catalog
*   D. AWS Directory Service

###### Explanation:

**Correct Answer – A**

AWS Artifact is a comprehensive resource center to have access to the AWS’ auditor-issued reports and security and compliance documentation from several renowned independent standard organizations.

[https://aws.amazon.com/artifact/](https://aws.amazon.com/artifact/)

*   **Option B is INCORRECT.** AWS Resource Center is a  repository of tutorials, whitepapers, digital training, and project use cases that aid in learning the core concepts of Amazon Web Services.

[https://aws.amazon.com/getting-started/](https://aws.amazon.com/getting-started/)

*   **Option C is INCORRECT.** AWS Service Catalog allows organizations to create and save their own IT service catalogs for further use. But they have to be approved by AWS. IT service catalogs can be multi-tiered application architectures.

[https://docs.aws.amazon.com/servicecatalog/latest/adminguide/introduction.html](https://docs.aws.amazon.com/servicecatalog/latest/adminguide/introduction.html)

*   **Option D is INCORRECT.** AWS Directory Service is an AWS tool that provides multiple ways to use Amazon Cloud Directory and Microsoft Active Directory with other AWS services.

[https://docs.aws.amazon.com/directoryservice/latest/admin-guide/what_is.html](https://docs.aws.amazon.com/directoryservice/latest/admin-guide/what_is.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 14Correct**Domain:** Security

A new department has recently joined the organization and the administrator needs to compose access permissions for the group of users. Given that they have various roles and access needs, what is the best-practice approach when granting access?

*   A. After gathering information on their access needs, the administrator should allow every user to access the most common resources and privileges on the system.
*   B. The administrator should grant all users the same permissions and then grant more upon request. 
*   C. The administrator should grant all users the least privilege and add more privileges to only to those who need it.right
*   D. Users should have no access and be granted temporary access on the occasions that they need to execute a task.

###### Explanation:

**Correct Answer – C**

The best-practice for AWS Identity Access Management (IAM) is to grant the least amount of permissions on the system only to execute the required tasks of the user’s role. Additional permissions can be granted per user according to the tasks they wish to perform on the system.

[https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege)

*   **Option A is incorrect** because granting users access to the most common resources presents security vulnerabilities, especially from those who have access to resources they do not need.
*   **Option B is incorrect** because granting users the same privileges on the system means other users might get access to resources they do not need to carry out their job functions. This presents a security risk.
*   **Option D is incorrect** because the users are part of the organisation; it will be cumbersome for the administrator to create temporal access passes for internal staff constantly.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 15Correct**Domain:** Security0

There is an external audit being carried out on your company. The IT auditor needs to have a log of 'who made the requests' to the AWS resources in the company’s account. Which of the below services can assist in providing these details?

*   A. AWS Cloudwatch
*   B. AWS CloudTrailright
*   C. AWS EC2
*   D. AWS SNS

###### Explanation:

**Answer - B**

Using CloudTrail, one can monitor all the API activity conducted on all AWS services.

The AWS Documentation additionally mentions the following.

AWS CloudTrail is a service that enables governance, compliance, operational auditing, and risk auditing of your AWS account. With CloudTrail, you can log, continuously monitor, and retain account activity related to actions across your AWS infrastructure. CloudTrail provides event history of your AWS account activity, including actions taken through the AWS Management Console, AWS SDKs, command line tools, and other AWS services. This event history simplifies security analysis, resource change tracking, and troubleshooting.

For more information on AWS Cloudtrail, please refer to the below URL:

*   [https://aws.amazon.com/cloudtrail/](https://aws.amazon.com/cloudtrail/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 16Incorrect**Domain:** Technology

Which of the following features can be used to preview changes to be made to an AWS resource which will be deployed using the AWS CloudFormation template?

*   A. AWS CloudFormation Drift Detectionwrong
*   B. AWS CloudFormation Change Setsright
*   C. AWS CloudFormation Stack Sets
*   D. AWS CloudFormation Intrinsic Functions

###### Explanation:

**Correct Answer – B**

AWS CloudFormation Change Set can be used to preview changes to AWS resources when a stack is executed.

*   **Option A is incorrect** as AWS CloudFormation Drift Detection is used to detect any changes made to resources outside of CloudFormation templates. It would not be able to preview changes that will be made by CloudFormation Templates.
*   **Option C is incorrect** as these are groups of stacks that are managed together.
*   **Option D is incorrect** as these Intrinsic Functions are used for assigning values to properties in CloudFormation templates.

For more information on AWS CloudFormation, refer to the following URL:

*   [https://aws.amazon.com/cloudformation/features/](https://aws.amazon.com/cloudformation/features/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 17Correct**Domain:** Security0

Which of the following is the responsibility of the customer to ensure the availability and backup of the EBS volumes?

*   A. Delete the data and create a new EBS volume.
*   B. Create EBS snapshots.right
*   C. Attach new volumes to EC2 Instances.
*   D. Create copies of EBS Volumes.

###### Explanation:

**Answer – B**

Snapshots are _incremental_ backups, which means that only the blocks on the device that have changed after your most recent snapshot are saved.   
When you create an EBS volume based on a snapshot, the new volume begins as an exact replica of the original volume that was used to create the snapshot. The replicated volume loads data in the background so that you can begin using it immediately.

**Option A is incorrect** because there is no need for backup of the volumes if data is already deleted.

**Option C is incorrect** because attaching more EBS volumes doesn't ensure availability, if there is no snapshot then the volume cannot be available to a different availability zone.

**Option D is incorrect** EBS volumes cannot be copied, they can only be replicated using snapshots.

For more information on EBS Snapshots, please refer to the below URL:

*   [https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSSnapshots.html](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSSnapshots.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 18Correct**Domain:** Cloud Concepts

When designing a highly available architecture, what is the difference between vertical scaling (scaling-up) and horizontal scaling (scaling-out)?

*   A. Scaling up provides for high availability whilst scaling out brings fault-tolerance.
*   B. Scaling out is not cost-effective compared to scaling up.
*   C. Scaling up adds more resources to an instance, scaling out adds more instances.right
*   D. Autoscaling groups require scaling up whilst launch configurations use scaling out.

###### Explanation:

Correct Answer – C

In high availability architectures, Autoscaling is used to give elasticity to the design. Horizontal scaling (scaling-out) uses Autoscaling groups to increase processing capacity in response to changes in preset threshold parameters. It could involve adding more EC2 instances of a web server. Vertical scaling (scaling-up), which can create a single point of failure, involves adding more resources to a particular instance to meet demand.

*   [https://docs.aws.amazon.com/autoscaling/plans/userguide/what-is-aws-auto-scaling.html](https://docs.aws.amazon.com/autoscaling/plans/userguide/what-is-aws-auto-scaling.html)
*   **Option A is INCORRECT.** Scaling-up does not provide high availability. Adding more resources to one instance is often not a best-practice in architecture design.
*   **Option B is INCORRECT.** Scaling-out is cost-effective since it involves adding more resources in response to demand and reducing resources (scaling down) when demand is low.
*   **Option D is INCORRECT.** All Autoscaling groups require a launch configuration based on what resources would be provisioned or deprovisioned to meet predefined parameters.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 19Correct**Domain:** Billing and Pricing

Your company is planning to move to the AWS Cloud. You need to give a presentation on the cost perspective when moving existing resources to the AWS Cloud. Considering Amazon EC2, which of the following is an advantage from the cost perspective?

*   A. Having the ability of automated backups of the EC2 instance, so that you don’t need to worry about the maintenance costs.
*   B. The ability to choose low cost AMI’s to prepare the EC2 Instances.
*   C. The ability to only pay for what you use.right
*   D. Ability to tag instances to reduce the overall cost.

###### Explanation:

Answer - C

One of the advantages of EC2 Instances is the per-second billing concept. This is also given in the AWS documentation.

With per-second billing, you pay for only what you use. It takes the cost of unused minutes and seconds in an hour off of the bill. So, you can focus on improving your applications instead of maximizing usage to the hour especially if you manage instances running for irregular periods of time, such as dev/testing, data processing, analytics, batch processing and gaming applications.

For more information on EC2 Pricing, please refer to the below URL:

*   [https://aws.amazon.com/ec2/pricing/](https://aws.amazon.com/ec2/pricing/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 20Correct**Domain:** Cloud Concepts

When designing a system, you use the principle of “design for failure and nothing will fail”. Which of the following services/features of AWS can assist in supporting this design principle? Choose 3 answers from the options given below.

*   A. Availability Zonesright
*   B. Regionsright
*   C. Elastic Load Balancerright
*   D. Pay as you go

###### Explanation:

Answer – A, B and C

Each AZ is a set of one or more data centers. By deploying your AWS resources to multiple Availability zones, you are designing with failure in mind. So if one AZ were to go down, the other AZ’s would still be up and running. Hence your application would be more fault-tolerant.

For disaster recovery scenarios, one can move or make resources run in other regions.

And finally, one can use the Elastic Load Balancer to distribute load to multiple backend instances within a particular region.

For more information on AWS Regions and AZ’s, please refer to the below URL:

*   [http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html](http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 21Correct**Domain:** Cloud Concepts

Your design team is planning to design an application that will be hosted on the AWS Cloud. One of their main non-functional requirements is given below:

*   Reduce inter-dependencies so failures do not impact other components.

Which of the following concepts does this requirement relate to?

*   A. Integration
*   B. Decouplingright
*   C. Aggregation
*   D. Segregation

###### Explanation:

Answer – B

The entire concept of decoupling components ensures that the different components of applications can be managed and maintained separately. If all components are tightly coupled, the entire application would go down when one component goes down. Hence it is always a better practice to decouple application components.

For more information on a decoupled architecture, please refer to the below URL:

*   [http://whatis.techtarget.com/definition/decoupled-architecture](http://whatis.techtarget.com/definition/decoupled-architecture)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 22Correct**Domain:** Security

Which of the following security requirements are managed by AWS? Select 3 answers from the options given below.

*   A. Password Policies
*   B. User permissions
*   C. Physical securityright
*   D. Disk disposalright
*   E. Hardware patchingright

###### Explanation:

Answer – C, D and E

As per the Shared Responsibility Model, the Patching of the underlying hardware and physical security of AWS resources is the responsibility of AWS.

For more information on AWS Shared Responsibility Model, please refer to the below URL-

*   [https://aws.amazon.com/compliance/shared-responsibility-model/](https://aws.amazon.com/compliance/shared-responsibility-model/)

Disk disposal-

Storage Device Decommissioning: When a storage device has reached the end of its useful life, AWS procedures include a decommissioning process designed to prevent customer data from being exposed to unauthorized individuals. AWS uses the techniques detailed in DoD 5220.22-M (“National Industrial Security Program Operating Manual “) or NIST 800-88 (“Guidelines for Media Sanitization”) to destroy data as part of the decommissioning process. All decommissioned magnetic storage devices are degaussed and physically destroyed in accordance with industry-standard practices.

For more information on Disk disposal, please refer to the below URL-

*   [https://d0.awsstatic.com/whitepapers/aws-security-whitepaper.pdf](https://d0.awsstatic.com/whitepapers/aws-security-whitepaper.pdf)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 23Correct**Domain:** Technology

You are planning on deploying a video-based application onto the AWS Cloud. Users across the world will access these videos. Which of the below services can help efficiently stream the content to the users across the globe?

*   A. Amazon SES
*   B. Amazon Cloudtrail
*   C. Amazon CloudFrontright
*   D. Amazon S3

###### Explanation:

Answer – C

The AWS Documentation mentions the following:

Amazon CloudFront is a web service that gives businesses and web application developers an easy and cost-effective way to distribute content with low latency and high data transfer speeds. Like other AWS services, Amazon CloudFront is a self-service, pay-per-use offering, requiring no long term commitments or minimum fees. With CloudFront, your files are delivered to end-users using a global network of edge locations.

For more information on CloudFront, please visit the link:

*   [https://aws.amazon.com/cloudfront/](https://aws.amazon.com/cloudfront/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 24Incorrect**Domain:** Security0

Which of the following AWS services can be used to retrieve configuration changes made to AWS resources causing operational issues?

*   A. Amazon Inspectorwrong
*   B. AWS CloudFormation
*   C. AWS Trusted Advisor
*   D. AWS Configright

###### Explanation:

**Correct Answer – D**

AWS Config can be used to audit, evaluate configurations of AWS resources. If there are any operational issues, AWS config can be used to retrieve configurational changes made to AWS resources that may have caused these issues.

*   **Option A is incorrect** as Amazon Inspector can be used to analyze potential security threats for an Amazon EC2 instance against an assessment template with predefined rules. It does not provide historical data for configurational changes done to AWS resources.
*   **Option B is incorrect** as AWS CloudFormation provided templates to provision and configure resources in AWS.
*   **Option C is incorrect** as AWS Trusted Advisor can help optimize resources with AWS cloud with respect to cost, security, performance, fault tolerance, and service limits. It does not provide historical data for configurational changes done to AWS resources.

For more information on AWS Config, refer to the following URL:

*   [https://docs.aws.amazon.com/config/latest/developerguide/WhatIsConfig.html](https://aws.amazon.com/config/faq/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 25Incorrect**Domain:** Security

An organization runs several EC2 instances inside a VPC using three subnets, one for Development, one for Test and one for Production. The Security team has some concerns about the VPC configuration. It requires to restrict the communication across the EC2 instances using Security Groups.

Which of the following options is true for Security Groups?

*   A. You can change a Security Group associated to an instance if the instance state is stopped or running.right
*   B. You can change a Security Group associated to an instance if the instance state is stopped but not if the instance state is running.wrong
*   C. You can change a Security Group only if there are no instances associated to it.
*   D. The only Security Group you can change is the Default Security Group.
*   E. None of the above

###### Explanation:

**Answer:** A

*   **Option A is CORRECT** because the AWS documentation mentions it in the section called  “Changing an Instance’s Security Group” using the following sentence: “After you launch an instance into a VPC, you can change the security groups that are associated with the instance. You can change the security groups for an instance when the instance is in the running or stopped state.”
*   **Option B, C, D and E are INCORRECT** as a consequence of A.

**Diagram:** none

**References:**

[https://docs.aws.amazon.com/en_pv/vpc/latest/userguide/VPC_SecurityGroups.html](https://docs.aws.amazon.com/en_pv/vpc/latest/userguide/VPC_SecurityGroups.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 26Incorrect**Domain:** Billing and Pricing

Your company is planning to pay for an AWS Support plan. They have the following requirements as far as the support plan goes:

*   24x7 access to Cloud Support Engineers via email, chat & phone
*   Response time of less than 15 minutes for any business-critical system faults

Which of the following plans will suffice to keep in mind the above requirement?

*   A. Basic
*   B. Developer
*   C. Businesswrong
*   D. Enterpriseright

###### Explanation:

Answer – D

As per the AWS document, there is no critical support available for Basic, Developer and Business plans.   

Enterprise plan has critical support within 15 minutes. The question mentions less than 15 minutes for critical faults. Hence the correct answer is Enterprise. 

For more information on the support plans, please refer to the following Link:

*   [https://aws.amazon.com/premiumsupport/compare-plans/![](https://s3.amazonaws.com/media.whizlabs.com/learn/2019/01/22/questions_dgdbva.png)](https://aws.amazon.com/premiumsupport/compare-plans/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 27Correct**Domain:** Technology

Your company wants to move an existing Oracle database to the AWS Cloud. Which of the following services can help facilitate this move?

*   A. AWS Database Migration Serviceright
*   B. AWS VM Migration Service
*   C. AWS Inspector
*   D. AWS Trusted Advisor

###### Explanation:

Answer - A

The AWS Documentation mentions the following.

AWS Database Migration Service helps you migrate databases to AWS quickly and securely. The source database remains fully operational during the migration, minimizing downtime to applications that rely on the database. The AWS Database Migration Service can migrate your data to and from the most widely used commercial and open-source databases.

For more information on AWS Database migration, please refer to the below URL:

*   [https://aws.amazon.com/dms/](https://aws.amazon.com/dms/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 28Incorrect**Domain:** Security

On which of the following resources does Amazon Inspector perform network accessibility checks?

*   A. Amazon CloudFront
*   B. Amazon VPN
*   C. Amazon EC2 instanceright
*   D. Amazon VPCwrong

###### Explanation:

**Correct Answer – C**

Amazon Inspector provides two types of packages. Network reachability rules package checks network accessibility checks on Amazon EC2 instance. Host assessment rules package checks vulnerabilities on Amazon EC2 instance.

*   **Options A, B & D are incorrect** as Amazon Inspector performs network accessibility checks on Amazon EC2 instance, not on Amazon CloudFront, Amazon VPN or Amazon VPC.

For more information on Amazon Inspector, refer to the following URL:

*   [https://aws.amazon.com/inspector/faqs/](https://aws.amazon.com/inspector/faqs/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 29Correct**Domain:** Cloud Concepts

Which of the following services helps to achieve the computing elasticity in AWS?

*   A. AWS RDS
*   B. VPC Endpoint
*   C. AWS EC2 Auto Scaling Groupright
*   D. Amazon S3

###### Explanation:

Answer – C

AWS EC2 Auto Scaling Group achieves the computing elasticity by scaling up/down the EC2 instances based on demand.

For more information on the AWS Autoscaling service, please refer to the below URL:

*   [https://aws.amazon.com/autoscaling/](https://aws.amazon.com/autoscaling/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 30Correct**Domain:** Cloud Concepts

A live online game uses DynamoDB instances in the backend to store real-time scores of the participants as they compete against each other from various parts of the world. Which data consistency option is the most appropriate to implement?

*   A. Strongly consistentright
*   B. Eventually consistent
*   C. Strong Eventual consistency
*   D. Optimistic consistency

###### Explanation:

**Correct Answer – A**

Since the gamers are from geographically distinct locations, the data will need to be immediately readable within a second as soon as it is written. Therefore strongly consistency is needed.

[https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html)

*   **Option B is INCORRECT** because the scenarios outline that the participants of the game are live. It will not suffice if any of them get updates on scores in less than real-time.
*   **Option C is INCORRECT **because strong eventual consistency is not applicable in DynamoDB.
*   **Option D is INCORRECT **because only two data consistency models are available with the DynamoDB service. Optimistic consistency is not supported.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 31Incorrect**Domain:** Security

Which of the following services allows you to analyze EC2 Instances against pre-defined security templates to check for vulnerabilities?

*   A. AWS Trusted Advisor
*   B. AWS Inspectorright
*   C. AWS WAF
*   D. AWS Shieldwrong

###### Explanation:

Answer – B

The AWS Documentation mentions the following.

Amazon Inspector enables you to analyze the behavior of your AWS resources and helps you to identify potential security issues. Using Amazon Inspector, you can define a collection of AWS resources that you want to include in an assessment target. You can then create an _assessment template_ and launch a security _assessment run_ of this target.

For more information on AWS Inspector, please refer to the below URL:

*   [https://docs.aws.amazon.com/inspector/latest/userguide/inspector_introduction.html](https://docs.aws.amazon.com/inspector/latest/userguide/inspector_introduction.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 32Correct**Domain:** Cloud Concepts

You are planning to serve a web application on the AWS Platform by using EC2 Instances. Which of the below principles would you adopt to ensure that even if some of the EC2 Instances crash, you still have a working application?

*   A. Using a scalable system
*   B. Using an elastic system
*   C. Using a regional system
*   D. Using a fault tolerant systemright

###### Explanation:

Answer - D

A fault-tolerant system is one that ensures that the entire system works as expected, even there are issues.

For more information on designing fault-tolerant applications in AWS, please refer to the below URL:

[https://d1.awsstatic.com/whitepapers/aws-building-fault-tolerant-applications.pdf?did=wp_card&trk=wp_card](https://d1.awsstatic.com/whitepapers/aws-building-fault-tolerant-applications.pdf?did=wp_card&trk=wp_card)

[https://aws.amazon.com/premiumsupport/knowledge-center/autoscaling-fault-tolerance-load-balancer/](https://aws.amazon.com/premiumsupport/knowledge-center/autoscaling-fault-tolerance-load-balancer/)

[https://aws.amazon.com/whitepapers/?whitepapers-main.sort-by=item.additionalFields.sortDate&whitepapers-main.sort-order=desc](https://aws.amazon.com/whitepapers/?whitepapers-main.sort-by=item.additionalFields.sortDate&whitepapers-main.sort-order=desc)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 33Correct**Domain:** Cloud Concepts

Which of the following are best practices when designing cloud-based systems? Choose 2 answers from the options below.

*   A. Build Tightly-coupled components.
*   B. Build loosely-coupled components.right
*   C. Assume everything will fail.right
*   D. Use as many services as possible.

###### Explanation:

**Answer – B and C**

Always build components that are loosely coupled. This is so that even if one component does fail, the entire system does not fail.

If you build with the assumption that everything will fail, you will ensure that the right measures are taken to build a highly available and fault-tolerant system.

**Option D is incorrect** because using multiple services increases cost and operational burden, rather use less and efficient services like serverless storage services and serverless compute services.

For more information on a well-architected framework, please refer to the below URL:

*   [https://d0.awsstatic.com/whitepapers/architecture/AWS_Well-Architected_Framework.pdf](https://d0.awsstatic.com/whitepapers/architecture/AWS_Well-Architected_Framework.pdf)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 34Correct**Domain:** Technology

Which services allow the customer to retain full administrative privileges of the underlying virtual infrastructure?

*   A. Amazon EC2right
*   B. Amazon S3
*   C. Amazon Lambda
*   D. Amazon DynamoDB

###### Explanation:

Answer – A

All of the other services are all managed by AWS as serverless components. Only you have complete control over the EC2 service. For more information on AWS EC2, please refer to the below URL:

*   [https://aws.amazon.com/ec2/](https://aws.amazon.com/ec2/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 35Incorrect**Domain:** Cloud Concepts

You have a mission-critical application that must be globally available at all times. If this is the case, which of the below deployment mechanisms would you employ?

*   A. Deployment to multiple edge locations
*   B. Deployment to multiple Availability Zoneswrong
*   C. Deployment to multiple Data Centers
*   D. Deployment to multiple Regionsright

###### Explanation:

Answer – D

Regions represent different geographical locations and are suitable for hosting your application across multiple regions for disaster recovery.

For more information on AWS Regions, please refer to the below URL:

*   [https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 36Correct**Domain:** Security

Which of the following can be used to protect against DDoS attacks? Choose 2 answers from the options given below.

*   A. AWS EC2
*   B. AWS RDS
*   C. AWS Shieldright
*   D. AWS Shield Advancedright

###### Explanation:

Answer – C and D

The AWS Documentation mentions the following:

AWS Shield - All AWS customers benefit from the automatic protections of AWS Shield Standard, at no additional charge. AWS Shield Standard defends against most common, frequently occurring network and transport layer DDoS attacks that target your web site or applications

AWS Shield Advanced - For higher levels of protection against attacks targeting your web applications running on Amazon EC2, Elastic Load Balancing (ELB), CloudFront, and Route 53 resources, you can subscribe to AWS Shield Advanced. AWS Shield Advanced provides expanded DDoS attack protection for these resources.

For more information on AWS Shield, please refer to the below URL:

*   [https://docs.aws.amazon.com/waf/latest/developerguide/ddos-overview.html](https://docs.aws.amazon.com/waf/latest/developerguide/ddos-overview.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 37Correct**Domain:** Cloud Concepts

Which of the following is a serverless compute offering from AWS?

*   A. AWS EC2
*   B. AWS Lambdaright
*   C. AWS SNS
*   D. AWS SQS

###### Explanation:

Answer – B

The AWS Documentation mentions the following:

AWS Lambda is a compute service that lets you run code without provisioning or managing servers. AWS Lambda executes your code only when needed and scales automatically, from a few requests per day to thousands per second.

For more information on AWS Lambda, please refer to the below URL:

*   [https://docs.aws.amazon.com/lambda/latest/dg/welcome.html](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 38Incorrect**Domain:** Security

Which of the following security services can be used to detect users' personal credit card numbers from data stored in Amazon S3?

*   A. Amazon Macieright
*   B. Amazon GuardDutywrong
*   C. Amazon Inspector
*   D. AWS Shield

###### Explanation:

**Correct Answer – A**

Explanation: Amazon Macie is a managed security service which can be used to detect personally identifiable information (PII) such as names, password, Credit card numbers from large amounts of data stored in Amazon S3 bucket.

*   **Option B is incorrect** as Amazon GuardDuty is used to identify threats by analyzing events from AWS CloudTrail, VPC Flow Logs, and DNS Logs. It cannot be used to detect PII from data stored in the Amazon S3 bucket.
*   **Option C is incorrect** as Amazon Inspector can analyze potential security threats for an Amazon EC2 instance against an assessment template with predefined rules.
*   **Option D is incorrect** as AWS Shield provides protection against DDOS attacks.

For more information on Amazon Macie, refer to the following URLs:

*   [https://aws.amazon.com/macie/features/](https://aws.amazon.com/macie/features/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 39Incorrect**Domain:** Technology

An online streaming company is prohibited from broadcasting its content in certain countries and regions in the world. Which Amazon Route 53 routing policy would be the most suitable in guaranteeing their compliance?

*   A. Geoproximitywrong
*   B. Geolocationright
*   C. Multi-value answer
*   D. Failover

###### Explanation:

**Correct Answer – B**

Amazon Route 53 geolocation routing policy makes it possible for different types of content to be served depending on the browser's geographical location. In this use case, the streaming company can serve a restriction message if Amazon Route 53 detects origin requests from prohibited countries.

[https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html#routing-policy-geo](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html#routing-policy-geo)

*   **Option A is INCORRECT** because geo-proximity allows for DNS traffic to be routed in accordance with a bias or preset preference rule. This allows the user to be served with content from resources closest to their geographical location. This routing manipulates DNS traffic flow only. This routing policy is not the most suitable.
    *   [https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html#routing-policy-geoproximity](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html#routing-policy-geoproximity)
*   **Option C is INCORRECT** because a multi-value answer primarily addresses the quality of service and resources queried in DNS requests. This routing policy is not the most suitable.
    *   [https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html#routing-policy-multivalue](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html#routing-policy-multivalue)
*   **Option D is INCORRECT** because failover allows for the automatic switch to healthy DNS resources if another becomes unavailable. It will not allow for the preferential serving of content based on the geographical location. This routing policy is not the most suitable.
    *   [https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html#routing-policy-multivalue](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html#routing-policy-multivalue)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 40Correct**Domain:** Cloud Concepts

Which AWS service provides a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability?

*   A. AWS RDS
*   B. DynamoDBright
*   C. Oracle RDS
*   D. Elastic Map Reduce

###### Explanation:

Answer: - B

DynamoDB is a fully managed NoSQL offering provided by AWS. It is now available in most regions for users to consume.

For more information on AWS DynamoDB, please refer to the below URL:

*   [http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html](http://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Introduction.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 41Incorrect**Domain:** Billing and Pricing

In the AWS Billing and Management service, which tool can provide usage-based forecasts of estimated billing costs and usage for the coming months?

*   A. AWS Cost Explorerright
*   B. AWS Bills
*   C. AWS Reports
*   D. Cost & Usage Reportswrong

###### Explanation:

**Correct Answer – A**

AWS Cost Explorer can create user-defined custom forecasts for future usage patterns.

[https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/ce-forecast.html](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/ce-forecast.html)

[https://aws.amazon.com/about-aws/whats-new/2019/07/usage-based-forecasting-in-aws-cost-explorer/](https://aws.amazon.com/about-aws/whats-new/2019/07/usage-based-forecasting-in-aws-cost-explorer/)

*   **Option B is INCORRECT** because AWS Bills will list the historical costs that would have been incurred over the past month with granular options. The tool will not give the usage-based forecasts as specified in the question.
*   **Option C is INCORRECT** because AWS Reports will give a composite overview of costs and usage. The tool gives a granular perspective of usage and billing but without usage-based forecasts.
*   **Option D is INCORRECT** because AWS Reports and Cost & Usage Reports are the same tool. Option C. explanation outlines why it is inaccurate as a response to the question.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 42Correct**Domain:** Technology

Which of the following AWS managed database service provides processing power that is up to 5X faster than a traditional MySQL database?

*   A. MariaDB
*   B. Auroraright
*   C. PostgreSQL
*   D. DynamoDB

###### Explanation:

Answer – B

The AWS Documentation mentions the following:

Amazon Aurora (Aurora) is a fully managed, MySQL- and PostgreSQL-compatible, relational database engine. It combines the speed and reliability of high-end commercial databases with the simplicity and cost-effectiveness of open-source databases. It delivers up to five times the throughput of MySQL and up to three times the throughput of PostgreSQL without requiring changes to most of your existing applications.

For more information on AWS Aurora, please refer to the below URL:

*   [https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Aurora.Overview.html](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Aurora.Overview.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 43Correct**Domain:** Cloud Concepts

In the AWS Well-Architected Framework, which of the following is NOT a Security design principle to design solutions in AWS?

*   A. Apply Security only at the edge of the network.right
*   B. Protect Data at rest & in transit.
*   C. Implement a strong Identity foundation.
*   D. Enable Traceability.

###### Explanation:

**Correct Answer: A**

Security needs to be applied at all network layers, like edge of network, VPC, all instances & application with the VPC. Applying Security controls at the edge of the network is not an efficient security control & against security design principles.

As per AWS Well-Architected Framework, the following are the design principles for security in the cloud:

·         Implement a strong identity foundation.

·         Enable traceability.

·         Apply security at all layers.

·         Automate security best practices.

·         Protect data in transit and at rest.

·         Keep people away from data.

·         Prepare for security events.

*   **Options B, C, & D are incorrect** as these are part of security design principles that need to be followed while implementing security controls in the cloud.

For more information on Security Design Principle with AWS Well-Architected Framework, refer to the following URL:

*   [https://docs.aws.amazon.com/wellarchitected/latest/framework/sec-design.html](https://docs.aws.amazon.com/wellarchitected/latest/framework/sec-design.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 44Correct**Domain:** Technology

Which of the following options is TRUE for AWS Database Migration Service (AWS DMS)?

*   A. AWS DMS can migrate databases from on-premise to AWS.
*   B. AWS DMS can migrate databases from AWS to on-premise.
*   C. AWS DMS can migrate databases from EC2 to Amazon RDS.
*   D. AWS DMS can have Amazon Redshift and Amazon DynamoDB as target databases.
*   E. All the aboveright

###### Explanation:

**Answer: E**

All the options are CORRECT.

Options are clearly described in the AWS DMS documentation at the link below.

*   **Option A is TRUE** and is the “most common” way to use AWS DMS.
*   **Option B is TRUE** and can be used to create a copy (or migrate) a database from AWS to the on-premise data center.
*   **Option C is TRUE** and can be used to migrate the IaaS solution (e.g., generated from a lift-and-shift wave) to a managed service like Amazon RDS.
*   **Option D is TRUE,** according to AWS documentation.

**Diagram:** none

**References:**

*   [https://aws.amazon.com/dms/](https://aws.amazon.com/dms/)
*   [https://aws.amazon.com/dms/faqs/](https://aws.amazon.com/dms/faqs/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 45Correct**Domain:** Security

Which of the following services helps in governance, compliance, and risk auditing in AWS?

*   A. AWS CloudFormation
*   B. AWS CloudTrailright
*   C. AWS CloudWatch
*   D. AWS SNS

###### Explanation:

Answer - B

The AWS Documentation mentions the following:

AWS CloudTrail is a service that enables governance, compliance, operational auditing, and risk auditing of your AWS account. With CloudTrail, you can log, continuously monitor, and retain account activity related to actions across your AWS infrastructure. CloudTrail provides event history of your AWS account activity, including actions taken through the AWS Management Console, AWS SDKs, command line tools, and other AWS services. This event history simplifies security analysis, resource change tracking, and troubleshooting.

For more information on AWS CloudTrail, please refer to the below URL:

*   [https://aws.amazon.com/cloudtrail/](https://aws.amazon.com/cloudtrail/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 46Incorrect**Domain:** Technology

Project team enhancing the security features of a banking application, requires implementing a threat detection service that continuously monitors malicious activities and unauthorized behaviors to protect AWS accounts, workloads, and data stored in Amazon S3\. Which AWS services should the project team select?

*   A. AWS Shieldwrong
*   B. AWS Firewall Manager
*   C. Amazon GuardDutyright
*   D. Amazon Inspector

###### Explanation:

**Answer: C**

*   **Option A is INCORRECT**. AWS Shield is a managed Distributed Denial of Service (DDoS) protection service that safeguards applications running on AWS.
*   **Option B is INCORRECT**. AWS Firewall Manager is a security management service that allows you to centrally configure and manage firewall rules across your accounts and applications in AWS Organization.
*   **Option C is CORRECT**. Amazon GuardDuty is a threat detection service that continuously monitors malicious activities and unauthorized behaviors to protect your AWS accounts, workloads, and data stored in Amazon S3.
*   **Option D is INCORRECT**. Amazon Inspector is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS.

 **Reference:**[](https://aws.amazon.com/guardduty/)

*   [https://aws.amazon.com/guardduty/](https://aws.amazon.com/guardduty/)
*   [https://aws.amazon.com/firewall-manager/](https://aws.amazon.com/firewall-manager/)
*   [https://aws.amazon.com/shield/](https://aws.amazon.com/shield/)
*   [https://aws.amazon.com/inspector/](https://aws.amazon.com/inspector/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 47Correct**Domain:** Technology

Which of the following are benefits of the AWS's Relational Database Service (RDS)? Choose the 2 correct answers from the options below.

*   A. Automated patches and backupsright
*   B. DB owner can resize the capacity accordinglyright
*   C. It allows you to store unstructured data
*   D. It allows you to store NoSQL data

###### Explanation:

Answer - A and B

The AWS Documentation mentions the following:

Amazon Relational Database Service (Amazon RDS) makes it easy to set up, operate, and scale a [relational database](https://aws.amazon.com/relational-database/) in the cloud. It provides cost-efficient and resizable capacity while automating time-consuming administration tasks such as hardware provisioning, database setup, patching and backups. It frees you to focus on your applications. So you can give them the fast performance, high availability, security and compatibility they need.

For more information on AWS RDS, please visit the URL:

*   [https://aws.amazon.com/rds/](https://aws.amazon.com/rds/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 48Incorrect**Domain:** Cloud Concepts

Which AWS product provides a unified user interface, enabling easy management of software development activities in one place, along with, quick development, build, and deployment of applications on AWS?

*   A. Amazon CodeGuru.
*   B. AWS CodeBuildwrong
*   C. AWS CodeArtifact
*   D. AWS CodeStarright

###### Explanation:

**Answer: D**

*   **Option A is INCORRECT**. Amazon CodeGuru is a developer tool powered by machine learning that provides intelligent recommendations for improving code quality and identifying an application’s most expensive lines of code.
*   **Option B is INCORRECT**. AWS CodeBuild is a fully managed continuous integration service that compiles source code, runs tests, and produces software packages that are ready to deploy.
*   **Option C is INCORRECT**. AWS CodeArtifact is a fully managed artifact repository service that makes it easy for organizations of any size to securely store, publish, and share software packages used in their software development process.
*   **Option D is CORRECT**. AWS CodeStar enables you to develop, build, and deploy applications on AWS quickly. AWS CodeStar provides a unified user interface, enabling you to manage your software development activities in one place easily.

**Reference:**[](https://aws.amazon.com/codeguru/)

*   [https://aws.amazon.com/codeguru/](https://aws.amazon.com/codeguru/)
*   https://aws.amazon.com/codeartifact/
*   [https://aws.amazon.com/codebuild/](https://aws.amazon.com/codebuild/)
*   [https://aws.amazon.com/codestar/](https://aws.amazon.com/codestar/?c=10&pt=8)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 49Correct**Domain:** Cloud Concepts

If you want to take a backup of an EBS Volume, what would you do?

*   A. Store the EBS volume in S3.
*   B. Store the EBS volume in an RDS database.
*   C. Create an EBS snapshot.right
*   D. Store the EBS volume in DynamoDB.

###### Explanation:

Answer - C

The AWS Documentation mentions the following:

You can back up the data on your Amazon EBS volumes to Amazon S3 by taking point-in-time snapshots.

For more information on EBS Snapshots, please visit the link:

*   [https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSSnapshots.html](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSSnapshots.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 50Incorrect**Domain:** Security0

Your Security Team has some security concerns about the application data stored on S3. The team requires you to introduce two improvements: (i) add “encryption at rest” and (ii) give them the possibility to monitor who has accessed the data and when the data have been accessed.

Which of the following AWS solution would you adopt to satisfy the requirement?

*   A. AWS Certificate Manager with CloudTrail.
*   B. Server-Side Encryption managed by S3 (SSE-S3) with CloudTrail.wrong
*   C. Server-Side Encryption managed by customer (SSE-C) with CloudTrail.
*   D. Server-Side Encryption managed by KMS (SSE-KMS) with CloudTrail.right

###### Explanation:

**Answer: D**

Amazon S3 is integrated with AWS CloudTrail, a service that provides a record of actions taken by a user, role, or an AWS service in Amazon S3. 

CloudTrail logs successful operations and attempted calls that failed, such as when the caller is denied access to a resource. Operations on KMS keys in other accounts are logged in both the caller account and the KMS key owner account.

*   **Option A is INCORRECT** AWS Certificate Manager is not a solution for encryption at rest. It is a service that lets you easily provision, manage, and deploy public and private Secure Sockets Layer/Transport Layer Security (SSL/TLS) certificates. Hence it is a solution for “encryption in transit”, not an “encryption at rest.”
*   **Option B is INCORRECT** because SSE-S3 does “encryption/decryption at rest”, but it does not offer monitoring capabilities (who/when encrypts/decrypts).
*   **Option C is INCORRECT** because SSE-C does “encryption/decryption at rest”, but it does not offer monitoring capabilities (who/when encrypts/decrypts).
*   **Option D is CORRECT** because SSE-KMS does “encryption/decryption at rest” and does offer monitoring capabilities. CloudTrail captures all API calls to AWS KMS as events, including calls from the AWS KMS console, AWS KMS APIs, the AWS Command Line Interface (AWS CLI), and AWS Tools for PowerShell.

**References:**

*   [https://docs.aws.amazon.com/kms/latest/developerguide/services-s3.html#sse](https://docs.aws.amazon.com/kms/latest/developerguide/services-s3.html#sse)
*   [https://docs.aws.amazon.com/kms/latest/developerguide/logging-using-cloudtrail.html](https://docs.aws.amazon.com/kms/latest/developerguide/logging-using-cloudtrail.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 51Incorrect**Domain:** Technology

Which of the following statements regarding Amazon Athena are accurate? Select TWO.

*   A. Amazon Athena queries data directly from Amazon S3 and there are no additional data storage commitments beyond the object storage.right
*   B. Amazon Athena is not suitable for complex analysis such as large joins, window functions and arrays.
*   C. Amazon Athena resources are allocated in accordance to processing and memory requirements prior to deployment.
*   D. Amazon Athena is compatible with data formats such as CSV, JSON, ORC, AVRO and Parquetright
*   E. Amazon Athena uses a variety of query languages including SQL, LDAP, JPQL as well as CQL.wrong

###### Explanation:

**Correct Answer – A, D**

Amazon Athena a serverless query service that does not need to build databases on dedicated Elastic Block Store (EBS) volumes. Instead, it builds tables from data read directly from Amazon S3 buckets. Amazon Athena does not store any of the data. The service is compatible with the regular data formats that include CSV, JSON, ORC, AVRO and Parquet.

[https://docs.aws.amazon.com/athena/latest/ug/what-is.html](https://docs.aws.amazon.com/athena/latest/ug/what-is.html)

*   **Option B is incorrect** because Amazon Athena can query Big Data, complex analysis such as large joins, window functions and arrays.
*   **Option C is incorrect** because Amazon Athena is serverless. Thus the service scales following the resource demands. No prior resource planning is necessary.
*   **Option E is incorrect** because Amazon Athena uses SQL only.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 52Correct**Domain:** Technology

An administrator is running a large deployment of AWS resources that are spread across several AWS Regions. They would like to keep track of configuration changes on all the resources and maintain a configuration inventory. What is the best service they can use?

*   A. AWS CloudFormation
*   B. Stacks and Templates
*   C. AWS Backup
*   D. AWS Configright

###### Explanation:

**Correct Answer – D**

AWS Config will meet the scenario requirements. The service allows the administrator to monitor and record configuration changes on AWS resources in their account. The service also allows the administrator to create a resource configuration inventory.

[https://aws.amazon.com/config/](https://aws.amazon.com/config/)

*   **Option A is incorrect** because AWS CloudFormation will allow the administrator to create templates of resources such as EC2 instances and RDS instances but not the actual configurations in these resources.
*   **Option B is incorrect** because Templates and Stacks form the basis of AWS CloudFormation. They aid in the automated deployment of whole environments but not the applications that run in them.
*   **Option C is incorrect** because AWS Backup is a fully managed service that allows the administrator to back up data in the cloud and on-premises. The service is not the most appropriate to monitor and record resource configuration changes.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 53Correct**Domain:** Technology

A company does not want to manage their database. Which of the following services is a fully managed NoSQL database provided by AWS?

*   A. AWS RDS
*   B. DynamoDBright
*   C. Oracle RDS
*   D. Elastic Map Reduce

###### Explanation:

Answer - B

DynamoDB is a fully managed NoSQL offering provided by AWS. It is now available in most regions for users to consume.

For more information on AWS DynamoDB, visit the below link:

*   [https://aws.amazon.com/dynamodb/](https://aws.amazon.com/dynamodb/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 54Correct**Domain:** Technology

Whilst working on a collaborative project, an administrator would like to record the initial configuration and several authorized changes that engineers make to the route table of a VPC. What is the best method to achieve this?

*   A. Use of AWS Configright
*   B. Use of VPC Flow Logs
*   C. Use of AWS CloudTrail
*   D. Use of an AWS Lambda function that is triggered to save a log file to an S3 bucket each time configuration changes are made.

###### Explanation:

**Correct Answer – A**

AWS Config can be used to keep track of configuration changes on AWS resources, keeping multiple date-stamped versions in a reviewable history. This makes it the best method to meet the scenario requirements.

[https://aws.amazon.com/config/](https://aws.amazon.com/config/)

*   **Option B is incorrect** because VPC flow logs will only capture IP traffic-related information passing through and from network interfaces within the VPC. VPC flow logs will not be able to capture configuration changes made to route tables.
    *   [https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html](https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html)
*   **Option C is incorrect** because AWS CloudTrail will capture identity access activity, event history into the AWS environment. Recording the actions and API calls are not best suited to keep a record of configurations.
    *   [https://aws.amazon.com/cloudtrail/](https://aws.amazon.com/cloudtrail/)
*   **Option D is incorrect** because using a Lambda function to write configuration changes might meet the requirements, but it would not be the best method. AWS Config can deliver what is needed with much less administrative input.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 55Correct**Domain:** Cloud Concepts

**Which of the following is a template that contains the software configuration to launch an ec2 instance?**

*   A. EBS Volumes
*   B. AMIright
*   C. EC2 Snapshot
*   D. EBS Snapshot

###### Explanation:

Answer – B

The AWS Documentation mentions the following

An Amazon Machine Image (AMI) provides the information required to launch an instance, which is a virtual server in the cloud. You specify an AMI when you launch an instance, and you can launch as many instances from the AMI as you need. You can also launch instances from as many different AMIs as you need.

For more information on Amazon Machine Images, please refer to the following link:

*   [https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 56Correct**Domain:** Security

Security and Compliance is a shared responsibility between AWS and the customer. Which amongst the below-listed options are AWS responsibilities? (Select TWO.)

*   A. Perform all the necessary security configuration and management tasks for Amazon Elastic Compute Cloud (Amazon EC2).
*   B. Patch management of the guest OS and applications
*   C. Security of the data in the AWS cloud
*   D. Security of the AWS cloudright
*   E. Patch management within the AWS infrastructureright

###### Explanation:

**Answer: D and E**

*   **Option A is INCORRECT** because Amazon Elastic Compute Cloud (Amazon EC2) is categorized as Infrastructure as a Service (IaaS). Hence this is the customer's responsibility.
*   **Option B is INCORRECT** because AWS is responsible for patching and fixing flaws within the infrastructure. But customers are responsible for patching their guest OS and applications.
*   **Option C is INCORRECT** as Security of the data in the cloud is the customer's responsibility.
*   **Option D is CORRECT** as security of the cloud is AWS’s responsibility.
*   **Option E is CORRECT**. AWS is responsible for patching and fixing flaws within the infrastructure.

**Reference:**[](https://aws.amazon.com/compliance/shared-responsibility-model/)

*   [https://aws.amazon.com/compliance/shared-responsibility-model/](https://aws.amazon.com/compliance/shared-responsibility-model/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 57Incorrect**Domain:** Cloud Concepts

Which of the following tools can be used to check service limits for resources launched within AWS Cloud Infrastructure?

*   A. AWS Config
*   B. AWS Trusted Advisorright
*   C. Amazon CloudWatch wrong
*   D. AWS CloudTrail

###### Explanation:

**Correct Answer: B**

AWS Trusted Advisor checks for service usage for all the resources within AWS Cloud and provides notifications.

*   **Option A is incorrect** as AWS Config can be used to audit, evaluate configurations of AWS resources. But it does not check service limits for resources.
*   **Option C is incorrect** as Amazon CloudWatch monitors AWS resources and applications on these resources. But it does not check service limits for resources.
*   **Option D is incorrect** as AWS CloudTrail is a logging service, recording activity made to AWS resources. But it does not check service limits for resources.

For more information on AWS Trusted Advisor, refer to the following URL:

*   [https://aws.amazon.com/premiumsupport/technology/trusted-advisor/](https://aws.amazon.com/premiumsupport/technology/trusted-advisor/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 58Correct**Domain:** Technology

Which of the following accurately describes a typical use case in which the AWS CodePipeline service can be utilized?

*   A. To compose code in an integrated development environment that enables developers to run, test and debug components of a dynamic microservice.
*   B. To compile and deploy a microservice onto Amazon EC2 instances or AWS Lambda functions.
*   C. To securely share code, collaborate on source code, version control and store binaries on an AWS fully-managed platform that scales seamlessly.
*   D. To orchestrate and automate the various phases involved in the release of application updates in-line with a predefined release model.right

###### Explanation:

**Correct Answer:  D**

The question is looking for a typical use case for AWS CodePipeline. Option D is the most appropriate because AWS CodePipeline is typically utilized when orchestrating and automating the various phases involved in the release of application updates in-line with a release model that the developer defines.

*   [https://aws.amazon.com/codepipeline/](https://aws.amazon.com/codepipeline/)
*   Option A is **INCORRECT** because composing code in an integrated development environment that enables developers to run, test, and debug components of a dynamic microservice is the typical AWS Cloud9 IDE function.
*   Option B is **INCORRECT** because compiling and deploying microservices on Amazon EC2 instances or AWS Lambda functions are the typical functions of AWS CodeDeploy.
*   Option C is **INCORRECT** because securely sharing code, collaborating on source code, version control and storing binaries on an AWS fully-managed platform describe the functions of CodeCommit.

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 59Correct**Domain:** Technology

Your organization has planned to decommission its data centers. You have a task to migrate hundreds of TB of archived data and 22 TB of active data to S3 and EFS, as per the designed solution. Which of the below service will be best suited for this task?

*   A. AWS Data Syncright
*   B. AWS Direct Connect
*   C. AWS Data Pipeline
*   D. AWS Migration Hub

###### Explanation:

**Answer: A**

*   **Option A** is **CORRECT**. AWS Data Sync is a simple and fast way to move huge amounts of data (hundreds of terabytes) between on-prem storage to S3, EFS, FSx.
*   **Option B** is **INCORRECT**. AWS Direct Connect is an offering that helps run workloads that are heavy on bandwidth in AWS. AWS Direct Connect enables private and dedicated connections between the on-premises network and AWS. AWS Data Sync could be used over the internet or Direct Connect.
*   **Option C** is **INCORRECT**. AWS Data Pipeline is a web service that facilitates data processing and movement between various AWS services (like compute and storage). Data pipeline also works well with data sources that are on-premise. In the given data migration scenario, data sync is a more apt choice.
*   **Option D** is **INCORRECT**. AWS Migration Hub is a service that facilitates discovery of the existing applications and IT assets and provides a view to better plan and track application migrations.

**Reference:**[](https://aws.amazon.com/datasync)

*   [https://aws.amazon.com/datasync](https://aws.amazon.com/datasync)/
*   [https://aws.amazon.com/directconnect/](https://aws.amazon.com/directconnect/)
*   [https://aws.amazon.com/datapipeline/](https://aws.amazon.com/datapipeline/)
*   [https://aws.amazon.com/migration-hub/](https://aws.amazon.com/migration-hub/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 60Correct**Domain:** Technology

To maximize user satisfaction, you are asked to improve the performance of the application for local and global users. As part of this initiative, you must monitor the application endpoint health and route traffic to the most appropriate application endpoint. Which service will you prefer to use?

*   A. Amazon Global Acceleratorright
*   B. Amazon DAX accelerator
*   C. Amazon S3 transfer acceleration
*   D. AWS Direct Connect

###### Explanation:

**Answer:** **A**

Global accelerator is a networking service that utilizes AWS global network to optimize the “user to application” path. The performance benefits realized by the use of the Global accelerator can be tested using a speed comparison tool provided by AWS.

Global accelerator differs from S3 transfer acceleration and DynamoDB accelerator.

S3 transfer acceleration, accelerates the transfers of files to the S3 bucket by utilizing edge locations.

Fully managed DynamoDB Accelerator (DAX) is a highly available in-memory cache for Dynamodb.

*   **Option A** is **CORRECT**. Refer to the explanation above.
*   **Option B** is **INCORRECT**. Refer to the explanation above.
*   **Option C** is **INCORRECT**. Refer to the explanation above.
*   **Option D** is **INCORRECT**. AWS Direct Connect is an AWS offering that simplifies setting up dedicated network connectivity between AWS and on-premises infrastructure.

**Reference: **

*   [https://aws.amazon.com/global-accelerator/](https://aws.amazon.com/global-accelerator/)
*   [https://aws.amazon.com/dynamodb/dax/](https://aws.amazon.com/dynamodb/dax/)
*   [https://docs.aws.amazon.com/AmazonS3/latest/dev/transfer-acceleration.html](https://docs.aws.amazon.com/AmazonS3/latest/dev/transfer-acceleration.html)
*   [https://aws.amazon.com/directconnect/](https://aws.amazon.com/directconnect/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 61Incorrect**Domain:** Security

Which AWS service offering uses machine learning and graph theory capability on automatically collected log data to help you conduct faster and efficient security investigations?

*   A. Amazon Macie
*   B. Amazon Detectiveright
*   C. AWS Artifact
*   D. Amazon GuardDutywrong

###### Explanation:

**Answer:** **B**

**Option A** is **INCORRECT**. Amazon Macie is a fully managed service from AWS that provides data security and privacy by utilizing Amazon’s machine learning and pattern matching capabilities.

**Option B** is **CORRECT**. Amazon Detective is a security service that uses machine learning capabilities on the automatically collected log data to help customers perform efficient and fast security investigations.

**Option C** is **INCORRECT**. AWS Artifact is a central resource for all the information about compliance. AWS artifact provides on-demand access to compliance reports at no additional cost.

**Option D** is **INCORRECT**. Amazon GuardDuty performs continuous monitoring to protect AWS account, S3 data and workloads from any malicious, unauthorized activities.

**Reference: **

*   [https://aws.amazon.com/macie/](https://aws.amazon.com/macie/)
*   [https://aws.amazon.com/detective/faqs/](https://aws.amazon.com/detective/faqs/)
*   [https://aws.amazon.com/artifact/](https://aws.amazon.com/artifact/)
*   [https://aws.amazon.com/guardduty/](https://aws.amazon.com/guardduty/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 62Correct**Domain:** Security

An administrator is tasked to configure privileges for the new joiners in the department. The admin is selectively granting privileges and ensuring that not all the team members can access all the resources.

Which principle is the administrator following?

*   A. Principle of privileged users
*   B. Least privilege of group principle
*   C. Best practices of permission advisory
*   D. Principle of least privilegeright

###### Explanation:

**Answer: D**

*   **Option A** is **INCORRECT**. This is not a valid option.
*   **Option B** is **INCORRECT**. This is not a valid option.
*   **Option C** is **INCORRECT**. This is not a valid option.
*   **Option D** is **CORRECT**. The administrator follows the “Principle of least privilege” as not all the privileges are granted to all the new joiners. The privileges are being selectively granted.

 **Reference:**

*   [https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 63Correct**Domain:** Cloud Concepts

You are asked to suggest an appropriate Amazon S3 storage class for “data with unknown/changing access pattern”. Which one would you suggest?

*   A. Amazon S3 Intelligent-Tieringright
*   B. Amazon S3 Standard
*   C. Amazon S3 Glacier
*   D. Amazon S3 Standard-Infrequent Access

###### Explanation:

**Answer:** **A**

*   **Option A** is **CORRECT**. Amazon S3 Intelligent-Tiering is best suited for data with “unknown/changing access pattern”.
*   **Option B** is **INCORRECT**. S3 standard is ideal for general-purpose storage of frequently accessed data.
*   **Option C** is **INCORRECT**. Amazon S3 Glacier is preferable for archival of data for a long term.
*   **Option D** is **INCORRECT**. Amazon S3 Standard-Infrequent Access is better suited for less frequently accessed, long-lived data.

**Reference:**[](https://aws.amazon.com/s3/storage-classes/)

*   [https://aws.amazon.com/s3/storage-classes/](https://aws.amazon.com/s3/storage-classes/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 64Incorrect**Domain:** Billing and Pricing

A “Member AWS account” in an AWS Organization (using consolidated billing) wants to receive a cost breakdown report (product-wise daily report) so that the analysis of cost and usage could be done.

Where can this report be configured to be delivered?

*   A. S3 bucket owned by the member account
*   B. S3 bucket owned by the master accountright
*   C. AWS Management Consolewrong
*   D. Amazon Athena

###### Explanation:

**Answer:** **B**

As the consolidated billing feature is being used in AWS organizations, the S3 bucket where the report could be configured to be received should be owned by the master account in the organization. Billing reports cannot be received in S3 buckets owned by member accounts. The report delivered to the S3 bucket owned by the master account could be ingested to Amazon Athena. After that, the data in the S3 bucket can be analyzed using standard SQL queries.

AWS Management Console is a centralized management and governance console for all the AWS products.

*   **Option A** is **INCORRECT**.
*   **Option B** is **CORRECT**.
*   **Option C** is **INCORRECT**.
*   **Option D** is **INCORRECT**.

**Reference:**

*   [https://docs.aws.amazon.com/cur/latest/userguide/what-is-cur.html](https://docs.aws.amazon.com/cur/latest/userguide/what-is-cur.html)
*   [https://aws.amazon.com/athena/](https://aws.amazon.com/athena/)
*   [https://aws.amazon.com/console/](https://aws.amazon.com/console/)

Ask our Experts<samp></samp>View QueriesDid you like this **Question?**‌‌‌Question 65Correct**Domain:** Cloud Concepts

Which AWS service allows:

1- Running Docker containers

2- Simple API calls to launch and stop container-based applications

*   A. AWS Docker Manager
*   B. AWS EKS
*   C. Amazon Elastic Container Serviceright
*   D. AWS Fargate

###### Explanation:

**Answer: C**

**AWS EKS (Elastic Kubernetes Service):** AWS EKS is a managed service that simplifies Kubernetes deployment on AWS by eliminating the need to install, operate, and/or maintain its own Kubernetes control plane.

**Amazon Elastic Container Service:** AWS ECS is a container management service that facilitates containers' management on the cluster, including running and stopping the containers. The container-based applications could be launched/stopped using simple API calls.

**AWS Fargate:** AWS Fargate is an “ECS and EKS compatible” serverless compute engine for containers.

*   **Option A is INCORRECT.** AWS Docker Manager is an invalid option.
*   **Option B is INCORRECT.**
*   **Option C is CORRECT.**
*   **Option D is INCORRECT.**

**Reference:**

*   [https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html](https://docs.aws.amazon.com/eks/latest/userguide/what-is-eks.html)
*   [https://docs.aws.amazon.com/AmazonECS/latest/developerguide/Welcome.html](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/Welcome.html)
*   [https://aws.amazon.com/fargate/](https://aws.amazon.com/fargate/)