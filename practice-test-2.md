Question 1Correct
Domain: Technology
Which of the following can be attached to EC2 Instances to store data?


A. Amazon Glacier
B. Amazon EBS Volumesright
C. Amazon EBS Snapshots
D. Amazon SQS
Explanation:
Answer – B

The AWS Documentation mentions the following on EBS Volumes:

An Amazon EBS volume is a durable, block-level storage device that you can attach to a single EC2 instance. You can use EBS volumes as primary storage for data that requires frequent updates, such as the system drive for an instance or storage for a database application.

For more information on EBS Volumes, please refer to the below URL:

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSVolumes.html
Ask our Experts
View Queries
Did you like this Question?

Question 2Correct
Domain: Technology
Which of the following networking component can be used to host EC2 resources in the AWS Cloud?


A. AWS Trusted Advisor
B. AWS VPCright
C. AWS Elastic Load Balancer
D. AWS Autoscaling
Explanation:
Answer - B

The AWS Documentation mentions the following on Amazon VPC:

Amazon Virtual Private Cloud (Amazon VPC) enables you to launch AWS resources into a virtual network that you've defined. This virtual network closely resembles a traditional network that you'd operate in your own data center, with the benefits of using the scalable infrastructure of AWS.

For more information on AWS VPC, please refer to the below URL:

https://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/VPC_Introduction.html
 

Ask our Experts
View Queries
Did you like this Question?

Question 3Incorrect
Domain: Technology
I have a web application that has been deployed to the AWS Mumbai region. My application soon becomes popular. Now there are users all over the world who would like to access it. If I use a CloudFront distribution for doing so, which statements are FALSE for CloudFront? (Select TWO.)


A. CloudFront uses the concept of Edge locations for caching and delivering content faster to its users.
B. CloudFront can help improve performance by using Keep-alive connections between the Edge locations &  the origin server.wrong
C. CloudFront does not cache dynamic content.right
D. CloudFront can use only S3 buckets as their Origin Server from where they can cache content.right
E. CloudFront can customize content at the Edge locations before delivering it to users.wrong
Explanation:
Answer: C, D

Option A is incorrect. CloudFront does use the concept of Edge locations for caching content that is requested by the user. When a user in the US requests for content in a web server hosted in the Mumbai region, CloudFront will initially check whether the content is available at the nearest edge location in the US region. If it is available, the content will be served directly from the Edge location. If not, CloudFront will request the Origin Server, get the content and cache it at the Edge location for serving future requests.


Option B is incorrect. Every HTTP connection runs on TCP/IP. For every HTTP connection to work, a TCP handshake has to be initially completed. Let’s consider the following 2 scenarios.
i). Two users without an Edge proxy – 1 Trip is 100ms

We can see here that the total turnaround time for both users is 400ms.



ii). Two users with a CloudFront Edge proxy

We can see here that for the first user, the total turnaround time is 400ms, while for the second user, the total turnaround time is 240ms(4x20 + 2x80 ). Instead of re-establishing a second handshake with the Origin, CloudFront leverages the Keep-alive session resulting in reduced latency.



Option C is CORRECT since we can use the Time To  Live (TTL) value to enable caching of dynamic content.
Option D is CORRECT. CloudFront has been opened to use Origin servers of your choice that can be S3 or a custom origin like EC2, ELB, etc...
Option E is incorrect. CloudFront has the ability to customize content at the Edge location before delivering it to its users. For example, a Lambda function (usually referred to as lambda@Edge) can use the following triggers Viewer Request, Origin Request, Origin Response, Viewer response that can be used for customizing the End User experience.
References:

https://docs.amazonaws.cn/en_us/AmazonCloudFront/latest/DeveloperGuide/Introduction.html
https://youtu.be/sQNONcj0cvc
Ask our Experts
View Queries
Did you like this Question?

Question 4Correct
Domain: Technology
Which of the following components of the Cloudfront service can be used to distribute content to users across the globe?


A. Amazon VPC
B. Amazon Regions
C. Amazon Availability Zones
D. Amazon Edge locationsright
Explanation:
Answer - D

The AWS documentation mentions the following:

Amazon CloudFront is a web service that speeds up distribution of your static and dynamic web content, such as .html, .css, .js, and image files, to your users. CloudFront delivers your content through a worldwide network of data centers called edge locations.

For more information on Amazon Cloudfront, please refer to the below URL:

http://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/Introduction.html
 

Ask our Experts
View Queries
Did you like this Question?

Question 5Correct
Domain: Billing and Pricing
Your company is planning to move to the AWS Cloud. You need to give a presentation on the cost perspective when moving existing resources to the AWS Cloud. Considering Amazon EC2, which of the following is an advantage from the cost perspective?


A. Having the ability of automated backups of the EC2 instance, so that you don’t need to worry about the maintenance costs.
B. The ability to choose low cost AMI’s to prepare the EC2 Instances.
C. The ability to only pay for what you use.right
D. Ability to tag instances to reduce the overall cost.
Explanation:
Answer - C

One of the advantages of EC2 Instances is the per-second billing concept. This is also given in the AWS documentation.

With per-second billing, you pay for only what you use. It takes the cost of unused minutes and seconds in an hour off of the bill. So, you can focus on improving your applications instead of maximizing usage to the hour especially if you manage instances running for irregular periods of time, such as dev/testing, data processing, analytics, batch processing and gaming applications.

For more information on EC2 Pricing, please refer to the below URL:

https://aws.amazon.com/ec2/pricing/
 

Ask our Experts
View Queries
Did you like this Question?

Question 6Correct
Domain: Security
Your company is planning to move to the AWS Cloud. Once it completely moves to the cloud, it wants to ensure that the right security settings are put in place. Which of the following tools are helpful? (Select TWO.)


A. AWS Inspectorright
B. AWS Trusted Advisorright
C. AWS Support
D. AWS Kinesis
Explanation:
Answer – A and B

The AWS documentation mentions the following

Trusted Advisor is a service to help you reduce cost, increase performance, and improve security by optimizing your AWS environment. Trusted Advisor provides real-time guidance to help you provision your resources following AWS best practices.

The AWS Inspector can inspect EC2 Instances against common threats.

For more information on the AWS Trusted Advisor, please refer to the below URL:

 

https://aws.amazon.com/premiumsupport/trustedadvisor/
https://docs.aws.amazon.com/inspector/latest/userguide/inspector_introduction.html
 

 

Ask our Experts
View Queries
Did you like this Question?

Question 7Correct
Domain: Technology
There is a requirement to collect important metrics from AWS RDS and EC2 Instances. Which AWS service would be helpful to fulfill this requirement?


A. Amazon CloudFront
B. Amazon CloudSearch
C. Amazon CloudWatchright
D. Amazon Config
Explanation:
Correct Answer – C

The AWS documentation mentions the following:

Amazon CloudWatch is a monitoring service for AWS cloud resources and the applications you run on AWS. You can use Amazon CloudWatch to collect and track metrics, collect and monitor log files, set alarms, and automatically react to changes in your AWS resources

For more information on AWS Cloudwatch, please refer to the URL below:

https://aws.amazon.com/cloudwatch/
 

Ask our Experts
View Queries
Did you like this Question?

Question 8Correct
Domain: Technology
I need to upload a large number of large-size objects from different Geographic locations to an S3 bucket. What is the best mechanism to do so in a fast & reliable way?


A. I can connect to an application running on AWS EC2 that is hosted in multiple regions using Route 53 & use latency based routing to upload files to the S3 bucket.
B. I can use a Direct Connect link from each of the Geographic location for transferring data quickly.
C. I can use S3 Transfer Acceleration from each Geographic location that will route the data from their respective Edge locations to S3.right
D. I can directly access the S3 bucket from the different locations & use a multi-part-upload for transferring huge objects.
Explanation:
Answer: C

Option A is incorrect since Route 53 latency routing only calculates latency between different endpoints based on the Internet traffic & location proximity rather than optimizing the network for fast data transfers.
Option B is incorrect since Direct Connect is used for very specific purposes like extreme security requirements for the data transfer. Also, establishing multiple Direct Connect infrastructures would be expensive from a cost standpoint.
Option C is CORRECT. The best way to address this scenario is to route the requests to the nearest CloudFront edge location from the different Geographic locations. Edge locations provide a fast network infrastructure bypassing much of the internet for delivering content to S3 destinations. Performance gains of nearly 50 - 500% can be observed while using S3 Transfer Acceleration.


Option D is incorrect. It is possible to use S3 endpoints directly for data transfer. But it will be impractical for situations where the Geographic location is significantly far away from the S3 destination introducing high latency while uploading large objects.
References:

https://medium.com/awesome-cloud/aws-amazon-s3-transfer-acceleration-overview-6baa7b029c27
https://docs.aws.amazon.com/AmazonS3/latest/dev/transfer-acceleration.html
Ask our Experts
View Queries
Did you like this Question?

Question 9Incorrect
Domain: Technology0
I have developed an application using AWS services that have been deployed to multiple regions to improve performance. How do I best achieve the optimal regional endpoint to increase the availability of your applications?


A. Use Route 53 latency based routing.
B. Use a CloudFront distribution.wrong
C. Use Global Accelerator.right
D. Use an endpoint of the application directly for accessing it that lies within a user’s Region.
Explanation:
Answer: C

Option A is incorrect. Route 53 latency-based routing helps select a region that may be relatively faster for the user to send traffic to based on certain factors like internet traffic and proximity to the user’s location. However, the actual route to the destination does not involve providing a fast network path for optimum performance, which is the prime requirement for the scenario. 
Option B is incorrect. CloudFront improves performance for both cacheable content (e.g., images, videos) and dynamic content (e.g., API, dynamic site delivery) using edge locations. Here we are talking about the optimal pathway to the regional endpoint, not caching the content. So CloudFront is not suitable. 
Option C is CORRECT. Global Accelerator uses the AWS global network to route traffic to the optimal regional endpoint based on health, client location, and policies that you configure, which increases the availability of your applications. Endpoints for standard accelerators can be Network Load Balancers, Application Load Balancers, Amazon EC2 instances, or Elastic IP addresses that are located in one AWS Region or multiple Regions.


Option D is incorrect since
The application may not be deployed in the Region that the user is trying to access.
There is no way to calculate latency even though there is proximity to the user’s region.
Availability will be restricted to AZ’s rather than Regions if regional endpoints, e.g., ELB’s are directly accessed.                    
References:

https://docs.aws.amazon.com/global-accelerator/latest/dg/what-is-global-accelerator.html
Ask our Experts
View Queries
Did you like this Question?

Question 10Correct
Domain: Billing and Pricing0
Which statement is accurate about AWS Budgets and Cost Explorer?


A. AWS Budgets uses the cost visualizations provided by AWS Cost Explorer to show the status of preset budgets and to provide forecasts of estimated costs.right
B. Both AWS Budgets and AWS Cost Explorer can be used to predict usage and to give recommended cost-optimization measures.
C. AWS Budgets will list the costs incurred over a period of time with a further breakdown by region and linked account.
D. Due to the sensitivity of billing and cost management information, with the AWS Cost Explorer and AWS Budgets services, it is not possible to view the information for multiple accounts.
Explanation:
Correct Answer – A

Under the Billing and Cost Management service in the AWS management service, it is possible to use the AWS Budgets and Cost Explorer to show the status of preset budgets and to provide forecasts of estimated costs.

https://aws.amazon.com/aws-cost-management/aws-cost-explorer/

Option B is incorrect because AWS Budgets does not provide cost-optimization recommendations.
Option C is incorrect because this feature is not provided by AWS budgets, rather it is provided by Cost Explorer.




Option D is incorrect because it is possible to view billing information for multiple AWS accounts as long as the administrator has lawful jurisdiction over them.
Ask our Experts
View Queries
Did you like this Question?

Question 11Correct
Domain: Cloud Concepts
When designing a system, you use the principle of “design for failure and nothing will fail”. Which of the following services/features of AWS can assist in supporting this design principle? Choose 3 answers from the options given below.


A. Availability Zonesright
B. Regionsright
C. Elastic Load Balancerright
D. Pay as you go
Explanation:
Answer – A, B and C

Each AZ is a set of one or more data centers. By deploying your AWS resources to multiple Availability zones, you are designing with failure in mind. So if one AZ were to go down, the other AZ’s would still be up and running. Hence your application would be more fault-tolerant.

For disaster recovery scenarios, one can move or make resources run in other regions.

And finally, one can use the Elastic Load Balancer to distribute load to multiple backend instances within a particular region.

For more information on AWS Regions and AZ’s, please refer to the below URL:

http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html
 

Ask our Experts
View Queries
Did you like this Question?

Question 12Correct
Domain: Cloud Concepts
While proposing AWS Cloud solution to a client as a value proposition, which of the following is not an advantage to use the AWS Cloud?


A. The AWS Cloud offers a pay-as-you-go model to trade Capital expense for Variable expense.
B. The AWS Cloud offers a Scale-on-demand model to eliminate wasted capacity.
C. The AWS Cloud gives complete control of Security to its users so that they can replicate their Data Center Security model on the Cloud.right
D. AWS Cloud frees  the users from spending time & money for maintaining their Data Centers.
Explanation:
Answer: C

Option A is incorrect. Instead of heavily investing in Data Centers & Servers for hosting their applications, clients can consume resources from the AWS Cloud, e.g., Compute, Storage, and only pay for the resources they have consumed. So Capital Expenditure (CAPEX) gets converted into Operational Expenditure (OPEX) while using a Cloud environment that results in Cost Efficiency for the client.
Option B is incorrect. The AWS Cloud model helps eliminating to guess infrastructure capacity needs by offering a Scale on Demand model. For example, during Christmas when there is a sudden increase in website traffic, additional resources (like EC2) can be created On-Demand (Scale- Up) to address the surge in traffic. Similarly, when the festival period goes away, the additional resources that were created can be terminated (Scale – Down) so that the user does not need to pay for idle resources.
Option C is CORRECT. AWS Cloud adopts a Shared Responsibility Model where Security & Compliance responsibility is shared between the Client & AWS. This shared responsibility security model helps relieve the client of operational burden as AWS operates, manages & controls the components from the host Operating System and Virtualization layer down to the physical security of its facilities (Data Center’s). The client can effectively manage the Security of his applications & the infrastructure in which it resides. AWS also helps customers to understand their robust controls in place to maintain security and compliance in the Cloud through their compliance certifications e.g., PCI DSS compliance.
Option D is incorrect. AWS Cloud allows clients to focus on their Projects that differentiate their business rather than maintaining infrastructure. AWS performs all the heavy lifting of maintaining facilities (Data Centers).
References:

https://d1.awsstatic.com/executive-insights/en_US/infographic-realizing-business-value-with-aws.pdf
https://youtu.be/Fl57qGYwdK4
Ask our Experts
View Queries
Did you like this Question?

Question 13Correct
Domain: Technology
You have a DevOps team in your current organization structure. They are keen to know if there is any service available in AWS which can be used to manage infrastructure as code. Which of the following can be met with such a requirement?


A. Using AWS Cloudformationright
B. Using AWS Config
C. Using AWS Inspector
D. Using AWS Trusted Advisor
Explanation:
Answer - A

The AWS documentation mentions the following.

AWS CloudFormation is a service that helps you model and set up your Amazon Web Services resources so that you can spend less time managing those resources and more time focusing on your applications that run in AWS. You create a template that describes all the AWS resources that you want (like Amazon EC2 instances or Amazon RDS DB instances). AWS CloudFormation takes care of provisioning and configuring those resources for you. You don't need to create and configure AWS resources individually and figure out what's dependent on what. AWS CloudFormation handles all of that.

For more information on AWS Cloudformation, please refer to the below URL:

https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html
 

Ask our Experts
View Queries
Did you like this Question?

Question 14Correct
Domain: Cloud Concepts
Which one of the following features does NOT belong to any Well-Architected Framework pillar in AWS?


A. It provides the ability to protect information, systems & assets.
B. It provides the ability to configure servers with much more CPU resources than required so that users do not need to maintain the CPU resources for a long time.right
C. It provides the ability to avoid or eliminate unneeded costs.
D. It provides the ability to recover from infrastructure or system failures.
Explanation:
Answer: B

The AWS Well architected framework is based on the five pillars – Security, Reliability, Performance efficiency, Cost Optimization & Operational Excellence.

Option A is incorrect since it belongs to the Security pillar of the AWS well architected framework.
Option B is CORRECT because configuring much more CPU resources than required is not appropriate in a cloud environment such as AWS. This method is not cost-efficient as well.
Option C is incorrect since it belongs to the Cost Optimization pillar of the AWS well architected framework.
Option D is incorrect since it belongs to the Reliability pillar of the AWS well architected framework.
References:

https://aws.amazon.com/architecture/well-architected/?wa-lens-whitepapers.sort-by=item.additionalFields.sortDate&wa-lens-whitepapers.sort-order=desc
https://aws.amazon.com/blogs/apn/the-5-pillars-of-the-aws-well-architected-framework/
Ask our Experts
View Queries
Did you like this Question?

Question 15Correct
Domain: Security
Which of the following is the responsibility of AWS according to the Shared Security Model? Choose 3 answers from the options given below.


A. Managing AWS Identity and Access Management (IAM)
B. Securing edge locationsright
C. Monitoring physical device securityright
D. Implementing service organization Control (SOC) standardsright
Explanation:
Answer – B, C and D

The responsibility of AWS includes the following.

1)      Securing edge locations

2)      Monitoring physical device security

3)      Implementing service organization Control (SOC) standards

For more information on AWS Shared Responsibility Model, please refer to the below URL:

https://aws.amazon.com/compliance/shared-responsibility-model/
 

Ask our Experts
View Queries
Did you like this Question?

Question 16Correct
Domain: Billing and Pricing
Your company has just started using the resources on the AWS Cloud. They want to get an idea of the costs being incurred so far for the resources being used. How can this be achieved?


A. By going to the Amazon EC2 dashboard. Here you can see the costs of the running EC2 resources.
B. By using the AWS Cost Explorer. Here you can see the running and forecast costs.right
C. By using the AWS Trusted Advisor dashboard. This dashboard will give you all the costs.
D. By seeing the AWS Cloud Trail logs.
Explanation:
The correct answer is Option B.

The AWS documentation mentions the following on AWS Cost Reports:

Cost Explorer is a free tool that you can use to view your costs. You can view data up to the last 12 months and 12 months forecast how much you are likely to spend for the next three months and get recommendations for what Reserved Instances to purchase.

For more information on AWS Cost Reports, please refer to the below URL:

http://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/cost-explorer-what-is.html
 

Ask our Experts
View Queries
Did you like this Question?

Question 17Correct
Domain: Security
By default who has complete administrative control over all resources in the respective AWS account?


A. AWS Support Team
B. AWS Account Ownerright
C. AWS Security Team
D. AWS Technical Account Manager (TAM)
Explanation:
Correct Answer: B

Option A is incorrect. AWS Support provides a mix of tools and technology, people, and programs designed to proactively help you optimize performance, lower costs, and innovate faster. 
Option B is correct. The entire control of data within an AWS account is with the Account Owner.
Option C is incorrect. The Security Specialist team is a customer-facing role where we get to talk to customers about the security, identity, and compliance of AWS. We help enable customers to securely and compliantly adopt the AWS Cloud.
Option D is incorrect. A technical account manager provides technical support to customers before and after a sale. The technical account manager will work with the client to build strong relationships and ensure customer satisfaction.
For more information on AWS Account identifiers, please refer to the below URL:
https://docs.aws.amazon.com/general/latest/gr/root-vs-iam.html
https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_accounts_create.html
Ask our Experts
View Queries
Did you like this Question?

Question 18Correct
Domain: Cloud Concepts
Your design team is planning to design an application that will be hosted on the AWS Cloud. One of their main non-functional requirements is given below:

Reduce inter-dependencies so failures do not impact other components.
Which of the following concepts does this requirement relate to?
 

 


A. Integration
B. Decouplingright
C. Aggregation
D. Segregation
Explanation:
Answer – B

The entire concept of decoupling components ensures that the different components of applications can be managed and maintained separately. If all components are tightly coupled, the entire application would go down when one component goes down. Hence it is always a better practice to decouple application components.

For more information on a decoupled architecture, please refer to the below URL:

http://whatis.techtarget.com/definition/decoupled-architecture
 

Ask our Experts
View Queries
Did you like this Question?

Question 19Correct
Domain: Cloud Concepts
Which of the following can be used to increase the fault tolerance of an application?


A. Deploying resources across multiple edge locations
B. Deploying resources across multiple VPC’s
C. Deploying resources across multiple Availability Zonesright
D. Deploying resources across multiple AWS Accounts
Explanation:
Answer – C

Each AZ is a set of one or more data centers. By deploying your AWS resources to multiple Availability zones, you are designing with failure in mind. So if one AZ were to go down, the other AZ’s would still be up and running. Hence your application would be more fault-tolerant.

For more information on AWS Regions and AZ’s, please refer to the below URL:

http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Concepts.RegionsAndAvailabilityZones.html
 

Ask our Experts
View Queries
Did you like this Question?

Question 20Correct
Domain: Security
Which of the following security requirements are managed by AWS? Select 3 answers from the options given below.


A. Password Policies
B. User permissions
C. Physical securityright
D. Disk disposalright
E. Hardware patchingright
Explanation:
Answer – C, D and E

As per the Shared Responsibility Model, the Patching of the underlying hardware and physical security of AWS resources is the responsibility of AWS.

For more information on AWS Shared Responsibility Model, please refer to the below URL-

https://aws.amazon.com/compliance/shared-responsibility-model/
Disk disposal-

 

Storage Device Decommissioning: When a storage device has reached the end of its useful life, AWS procedures include a decommissioning process designed to prevent customer data from being exposed to unauthorized individuals. AWS uses the techniques detailed in DoD 5220.22-M (“National Industrial Security Program Operating Manual “) or NIST 800-88 (“Guidelines for Media Sanitization”) to destroy data as part of the decommissioning process. All decommissioned magnetic storage devices are degaussed and physically destroyed in accordance with industry-standard practices.

 

For more information on Disk disposal, please refer to the below URL-

 

 

https://d0.awsstatic.com/whitepapers/aws-security-whitepaper.pdf
 

 

Ask our Experts
View Queries
Did you like this Question?

Question 21Correct
Domain: Cloud Concepts
Which of the following is not the pillars of AWS Well-Architected Framework?


A. Automationright
B. Cost Optimization
C. Reliability
D. Performance Efficiency
Explanation:
Correct Answer – A

 As per AWS Well-Architected Framework, the following are the 5 pillars:

· Operational Excellence

· Security

· Reliability

· Performance Efficiency

· Cost Optimization

Automation is not part of AWS Well-Architected Framework pillars.

Options B, C & D are incorrect as these are part of 5 Pillars of AWS Well-Architected Framework.
Reference:

https://docs.aws.amazon.com/wellarchitected/latest/framework/cost-bp.html
Ask our Experts
View Queries
Did you like this Question?

Question 22Correct
Domain: Billing and Pricing
Your company is planning to offload some of the batch processing workloads on to AWS. These jobs can be interrupted and resumed at any time. Which of the following instance types would be the most cost-effective to use for this purpose?


A. On-Demand
B. Spotright
C. Full Upfront Reserved
D. Partial Upfront Reserved
Explanation:
Answer – B

The AWS documentation mentions the following:

Spot Instances are a cost-effective choice if you can be flexible about when your applications run and if your applications can be interrupted. For example, Spot Instances are well-suited for data analysis, batch jobs, background processing, and optional tasks.

For more information on AWS Spot Instances, please refer to the below URL:

http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-spot-instances.html
 

Ask our Experts
View Queries
Did you like this Question?

Question 23Correct
Domain: Technology
Which service can be used to create steps required to automate build, test and deployments for a web application?


A. AWS CodeCommit
B. AWS CodePipelineright
C. AWS CodeDeploy
D. AWS CodeBuild
Explanation:
Correct Answer – B

AWS CodePipeline is a fully managed service that automates the release pipeline for application updates. For updates, it uses application code stored in AWS CodeCommit, performs testing using AWS CodeBuild, and uses AWS CodeDeploy for deployment.

Option A is incorrect as AWS CodeCommit is used to store deployment codes.
Option C is incorrect as AWS CodeDeploy is used for deployment of codes to resources.
Option D is incorrect as AWS CodeBuild is used to test and build application code.
For more information on AWS CodePipeline, refer to the following URL:

https://aws.amazon.com/codepipeline/faqs/
Ask our Experts
View Queries
Did you like this Question?

Question 24Correct
Domain: Billing and Pricing0
A manufacturing firm has recently migrated their application servers to the Amazon EC2 instance. The IT Manager is looking for the details of upcoming scheduled maintenance activities which AWS would be performing on AWS resources, that may impact the services on these EC2 instances.
Which of the following services can alert you about the changes that can affect resources in your account? 


A. AWS Organizations
B. AWS Personal Health Dashboardright
C. AWS Trusted Advisor
D. AWS Service Health Dashboard
Explanation:
Answer – B

AWS Personal Health Dashboard provides alerts for AWS services availability & performance which may impact resources deployed in your account. Customers get emails & mobile notifications for scheduled maintenance activities which might impact services on these AWS resources.   

Option A is incorrect as AWS Organizations do not provide any notifications for scheduled maintenance activities.

Option C is incorrect as AWS Trusted Advisor will provide notification on AWS resources created within the account for cost optimization, security, fault tolerance, performance, and service limits. It will not provide notification for scheduled maintenance activities performed by AWS on its resources.  

Option D is incorrect as Service Health Dashboard displays the general status of all AWS services & will not display scheduled maintenance activities.

For more information on the AWS Organizations, please refer to the below URL:

https://aws.amazon.com/premiumsupport/technology/personal-health-dashboard/
Ask our Experts
View Queries
Did you like this Question?

Question 25Correct
Domain: Security
Which of the following can be used as an additional security layer for the user name and password when logging into the AWS Console?


A. Multi-Factor Authentication (MFA)right
B. Secondary password
C. Root access privileges
D. Secondary user name
Explanation:
Answer – A

The AWS Documentation mentions the following:

AWS Multi-Factor Authentication (MFA) is a simple best practice that adds an extra layer of protection on top of your user name and password. 

For more information on the AWS MFA, please refer to the below URL:

https://aws.amazon.com/iam/details/mfa/
 

Ask our Experts
View Queries
Did you like this Question?

Question 26Correct
Domain: Technology
Which AWS Cloud service helps in the quick deployment of resources which can use different programming languages such as .Net and Java?


A. AWS Elastic Beanstalkright
B. AWS Elastic Compute Cloud (Amazon EC2)
C. AWS VPC
D. AWS SQS
Explanation:
Answer – A

The AWS Documentation mentions the following:

AWS Elastic Beanstalk is an easy-to-use service for deploying and scaling web applications and services developed with Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker on familiar servers such as Apache, Nginx, Passenger, and IIS.

For more information on enabling AWS Elastic beanstalk, please refer to the below URL:

https://aws.amazon.com/elasticbeanstalk/?p=tile
 

Ask our Experts
View Queries
Did you like this Question?

Question 27Correct
Domain: Cloud Concepts
Your company handles a crucial e-Commerce application. This application needs to have an uptime of at least 99.5%. There is a decision to move the application to the AWS Cloud. Which of the following deployment strategies can help build a robust architecture for such an application?


A. Deploying the application across multiple VPC’s
B. Deploying the application across multiple Regionsright
C. Deploying the application across Edge locations
D. Deploying the application across multiple subnets
Explanation:
Answer – B

The AWS Documentation mentions the following:

Businesses are using the AWS cloud to enable faster disaster recovery of their critical IT systems without incurring the infrastructure expense of a second physical site. The AWS cloud supports many popular disaster recovery (DR) architectures from “pilot light” environments that may be suitable for small customer workload data center failures to “hot standby” environments that enable rapid failover at scale. With data centers in Regions worldwide, AWS provides a set of cloud-based disaster recovery services that enable rapid recovery of your IT infrastructure and data.

For more information on enabling AWS Disaster Recovery, please refer to the below URL:

https://aws.amazon.com/disaster-recovery/
 

Ask our Experts
View Queries
Did you like this Question?

Question 28Incorrect
Domain: Billing and Pricing
Your company is moving a large application to AWS using a set of EC2 instances. A key requirement is reusing existing server-bound software licensing. Which of the following options is the best for satisfying the requirement?


A. EC2 Dedicated Instanceswrong
B. EC2 Reserved Instances
C. EC2 Dedicated Hostsright
D. EC2 Spot Instances
Explanation:
Answer: C

Option A is INCORRECT because despite instances run on a single-tenant hardware, AWS does not give visibility to sockets and cores required for reusing server bound licenses. AWS highlights this in the comparison table at the following link:
https://aws.amazon.com/ec2/dedicated-hosts/
Option B is INCORRECT because Reserved Instances are only a purchasing option and there’s no way to control the hardware where these instances are running on.
Option C is CORRECT because instances run on a dedicated hardware where AWS gives visibility of physical characteristics. AWS documentation mentions this with the following sentence:  “...Dedicated Host gives you additional visibility and control over how instances are placed on a physical server, and you can consistently deploy your instances to the same physical server over time. As a result, Dedicated Hosts enable you to use your existing server-bound software licenses and address corporate compliance and regulatory requirements.”
Option D is INCORRECT because Spot Instances are only a purchasing option.
Diagram: none

References:

AWS documentation explains the possibility of reusing server bound license:

https://aws.amazon.com/ec2/dedicated-hosts/
Ask our Experts
View Queries
Did you like this Question?

Question 29Correct
Domain: Technology
You are planning on deploying a video-based application onto the AWS Cloud. Users across the world will access these videos. Which of the below services can help efficiently stream the content to the users across the globe?


A. Amazon SES
B. Amazon Cloudtrail
C. Amazon CloudFrontright
D. Amazon S3
Explanation:
Answer – C

The AWS Documentation mentions the following:

Amazon CloudFront is a web service that gives businesses and web application developers an easy and cost-effective way to distribute content with low latency and high data transfer speeds. Like other AWS services, Amazon CloudFront is a self-service, pay-per-use offering, requiring no long term commitments or minimum fees. With CloudFront, your files are delivered to end-users using a global network of edge locations.

For more information on CloudFront, please visit the link:

https://aws.amazon.com/cloudfront/
 

Ask our Experts
View Queries
Did you like this Question?

Question 30Incorrect
Domain: Technology
Using Content Delivery Network (CDN), an administrator would like to serve varying types of content based on the viewer’s browser cookies. Which is the most appropriate serverless technique that can be used to achieve this?


A. AWS CodeCommit
B. AWS Lambda@Edgeright
C. AWS CodeStarwrong
D. AWS Cloud9
Explanation:
Correct Answer – B

AWS Lambda@Edge is a serverless service that makes it possible to run event-triggered functions on Edge Locations within the AWS Content Delivery Network. Using AWS CloudFront, an administrator can introduce decision-making and compute processing closer to the viewer’s location. Thereby it improves on their browsing experience.

https://aws.amazon.com/lambda/edge/

Option A is INCORRECT because AWS CodeCommit is inappropriate in addressing the scenario. It is a service that allows for the management of software development versions and software development assets. These include binary files, documents and source code.
Option C is INCORRECT because AWS CodeStar is a service used to manage software development projects. It is not the appropriate Option for the scenario. CodeStar project makes it possible to develop, build and deploy applications.
Option D is INCORRECT because it is not the best solution though it can be used in the scenario to write, run and deploy code. It is an integrated development environment (IDE) that can accommodate various runtimes. Since the Lambda@Edge is best suited to meet the requirements of the scenario, this makes this Option incorrect.
Ask our Experts
View Queries
Did you like this Question?

Question 31Incorrect
Domain: Cloud Concepts
For the AWS Shared Responsibility Model, which of the following responsibilities is NOT a part of shared controls by both customer and AWS?


A. Patch Management
B. Configuration Management
C. Global infrastructure that runs AWS Cloud services.right
D. Trainingwrong
Explanation:
Correct Answer – C

The global AWS infrastructure including the hardware, software, networking, and facilities is the responsibility of AWS, not the responsibility of the Customer.

Option A is incorrect. AWS is responsible for patching resources within AWS infrastructure, while customers are responsible for patching guest OS and applications.
Option B is incorrect. AWS is responsible for configuring resources within AWS infrastructure, while customers are responsible for configuring their guest OS, databases and applications.
Option D is incorrect. AWS trains for AWS employees while the customer is responsible for training employees within their organizations.
For more information on the Shared responsibility model, refer to the following URL:

https://aws.amazon.com/compliance/shared-responsibility-model/
Ask our Experts
View Queries
Did you like this Question?

Question 32Correct
Domain: Billing and Pricing
There is a requirement to host EC2 Instances in the AWS Cloud, wherein the utilization is for a duration of more than 3 years. Which of the following would you utilize to minimize the costs?


A. Reserved instancesright
B. On-demand instances
C. Spot instances
D. Regular instances
Explanation:
Answer – A

When you have instances that will be used continuously and throughout the year, the best option is to buy reserved instances. By buying reserved instances, you are actually allocated an instance for the entire year or the duration you specify with a reduced cost.

For more information on Reserved Instances, please visit the link:

https://aws.amazon.com/ec2/pricing/reserved-instances/
 

Ask our Experts
View Queries
Did you like this Question?

Question 33Incorrect
Domain: Cloud Concepts
An administrator would like to check if the Amazon CloudFront identity is making access API calls to an S3 bucket where a static website is hosted. Where can this information be obtained?


A. Configuring Amazon Athena to run queries on the Amazon CloudFront distribution.
B. Check AWS CloudWatch logs on the S3 bucket.wrong
C. In the webserver, tail for identity access logs from the Amazon CloudFront identity.
D. In AWS CloudTrail Event history, look up access calls and filter for the Amazon CloudFront identity.right
Explanation:
Correct Answer – D

By viewing Event history in Amazon CloudTrail, the administrator can be able to access operational, access and activity logs for the past 90 days, to the S3 bucket that hosts the static website.

https://docs.aws.amazon.com/awscloudtrail/latest/userguide/view-cloudtrail-events-console.html

Option A is INCORRECT because Amazon Athena will need a specific data repository from which a database and table can be created in order to run queries. Data repositories can be a folder in an S3 bucket where logs are written to.
Option B is INCORRECT because AWS CloudWatch does not log access API calls from one resource to another. AWS CloudTrail can do this.
Option C is INCORRECT because it is not possible to access the underlying web server for CloudFront. It is fully managed by AWS.
Ask our Experts
View Queries
Did you like this Question?

Question 34Correct
Domain: Security0
Which of the following AWS services can be used to retrieve configuration changes made to AWS resources causing operational issues?


A. Amazon Inspector
B. AWS CloudFormation
C. AWS Trusted Advisor
D. AWS Configright
Explanation:
Correct Answer – D

AWS Config can be used to audit, evaluate configurations of AWS resources. If there are any operational issues, AWS config can be used to retrieve configurational changes made to AWS resources that may have caused these issues.

Option A is incorrect as Amazon Inspector can be used to analyze potential security threats for an Amazon EC2 instance against an assessment template with predefined rules. It does not provide historical data for configurational changes done to AWS resources.
Option B is incorrect as AWS CloudFormation provided templates to provision and configure resources in AWS.
Option C is incorrect as AWS Trusted Advisor can help optimize resources with AWS cloud with respect to cost, security, performance, fault tolerance, and service limits. It does not provide historical data for configurational changes done to AWS resources.
For more information on AWS Config, refer to the following URL:

https://docs.aws.amazon.com/config/latest/developerguide/WhatIsConfig.html
Ask our Experts
View Queries
Did you like this Question?

Question 35Correct
Domain: Technology
A company is deploying a two-tier, highly available web application to AWS. The application needs a storage layer to store artifacts such as photos and videos. Which of the following services can be used as the underlying storage mechanism?


A. Amazon EBS volume
B. Amazon S3right
C. Amazon EC2 instance store
D. Amazon RDS instance
Explanation:
Answer – B

Amazon S3 is the default storage service that should be considered for companies. It provides durable storage for all static content.

For more information on AWS S3, please visit the Link:

https://aws.amazon.com/s3/
Ask our Experts
View Queries
Did you like this Question?

Question 36Incorrect
Domain: Security
An organization runs several EC2 instances inside a VPC using three subnets, one for Development, one for Test and one for Production. The Security team has some concerns about the VPC configuration. It requires to restrict the communication across the EC2 instances using Security Groups.

Which of the following options is true for Security Groups?


A. You can change a Security Group associated to an instance if the instance state is stopped or running.right
B. You can change a Security Group associated to an instance if the instance state is stopped but not if the instance state is running.wrong
C. You can change a Security Group only if there are no instances associated to it.
D. The only Security Group you can change is the Default Security Group.
E. None of the above
Explanation:
Answer: A

Option A is CORRECT because the AWS documentation mentions it in the section called  “Changing an Instance’s Security Group” using the following sentence: “After you launch an instance into a VPC, you can change the security groups that are associated with the instance. You can change the security groups for an instance when the instance is in the running or stopped state.”
Option B, C, D and E are INCORRECT as a consequence of A.
Diagram: none

References:

https://docs.aws.amazon.com/en_pv/vpc/latest/userguide/VPC_SecurityGroups.html

Ask our Experts
View Queries
Did you like this Question?

Question 37Correct
Domain: Technology
Which of the below-mentioned services is equivalent to hosting virtual servers on an on-premises location?


A. AWS IAM
B. AWS Server
C. AWS EC2right
D. AWS Regions
Explanation:
Answer - C

The AWS Documentation mentions the following:

Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers.

For more information on AWS EC2, please refer to the following link:

https://aws.amazon.com/ec2/
 

Ask our Experts
View Queries
Did you like this Question?

Question 38Correct
Domain: Security
You have a set of EC2 Instances hosted on the AWS Cloud. The EC2 Instances are hosting a web application. Which of the following acts as a firewall to your VPC and the instances in it? Choose 2 answers from the options given below.


A. Usage of Security Groupsright
B. Usage of AWS Config
C. Usage of Network Access Control Listsright
D. Usage of the Internet gateway
Explanation:
Answer – A and C

The AWS Documentation mentions the following.

A security group acts as a virtual firewall for your instance to control inbound and outbound traffic.

A network access control list (ACL) is an optional layer of security for your VPC that acts as a firewall for controlling traffic in and out of one or more subnets. 

For more information on Security Groups, please refer to the following link:

 

https://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/VPC_SecurityGroups.html
 

For more information on Network Access Control Lists, please refer to the following link:

https://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/VPC_ACLs.html
 

Ask our Experts
View Queries
Did you like this Question?

Question 39Incorrect
Domain: Technology
Which of the following can be used to launch EC2 instances on the AWS Cloud?


A. EBS Volumes
B. EBS Snapshotswrong
C. Amazon Machine Imageright
D. Amazon VMware
Explanation:
Answer – C

The AWS Documentation mentions the following.

An Amazon Machine Image (AMI) provides the information required to launch an instance, which is a virtual server in the cloud. You specify an AMI when you launch an instance and you can launch as many instances from the AMI as you need. You can also launch instances from as many different AMIs as you need.

For more information on Amazon Machine Images, please refer to the following Link:

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html
 

Ask our Experts
View Queries
Did you like this Question?

Question 40Incorrect
Domain: Technology
Which of the below options cannot be used to upload archives to Amazon Glacier?


A. AWS Glacier API
B. AWS Consoleright
C. AWS Glacier SDK
D. AWS S3 Lifecycle policieswrong
Explanation:
Answer – B

Note that the AWS Console cannot be used to upload data onto Glacier. The console can only be used to create a Glacier vault which can be used to upload the data.

For more information on uploading data onto Glacier, please refer to the following link:
https://docs.aws.amazon.com/amazonglacier/latest/dev/uploading-an-archive.html
Option A - AWS Glacier API
AWS Glacier is a storage service optimized for infrequently used data or "cold data." This option is used for programmatically access Glacier and work with it. Due to this reason, this option is incorrect.
https://docs.aws.amazon.com/amazonglacier/latest/dev/amazon-glacier-api.html
 Option C - AWS Glacier SDK: SDK, i.e., Software Development Kit, is used to develop applications for Amazon S3 Glacier. It provides libraries that map to the underlying REST API and provide objects that you can easily use to construct requests and process responses. Due to this reason, it's not a valid answer to the asked question.
 https://docs.aws.amazon.com/amazonglacier/latest/dev/using-aws-sdk.html
Option D - AWS S3 Lifecycle Policies: S3 Lifecycle Policies allow you to automatically review objects within your S3 Buckets and have them moved to Glacier or have the objects deleted from S3.
https://docs.aws.amazon.com/AmazonS3/latest/user-guide/create-lifecycle.html
https://aws.amazon.com/glacier/faqs/
Ask our Experts
View Queries
Did you like this Question?

Question 41Correct
Domain: Billing and Pricing
Your company is planning to pay for an AWS Support plan. They have the following requirements as far as the support plan goes:

24x7 access to Cloud Support Engineers via email, chat & phone
Response time of less than 15 minutes for any business-critical system faults
Which of the following plans will suffice to keep in mind the above requirement?


A. Basic
B. Developer
C. Business
D. Enterpriseright
Explanation:
Answer – D

As per the AWS document, there is no critical support available for Basic, Developer and Business plans. 

Enterprise plan has critical support within 15 minutes. The question mentions less than 15 minutes for critical faults. Hence the correct answer is Enterprise. 

For more information on the support plans, please refer to the following Link:

https://aws.amazon.com/premiumsupport/compare-plans/
 

Ask our Experts
View Queries
Did you like this Question?

Question 42Correct
Domain: Technology
Which of the following are features of an edge location? Choose 3 answers from the options given below.


A. Distribute content to usersright
B. Cache popular contentsright
C. Distribute load across multiple resources
D. Used in conjunction with the Cloudfront serviceright
Explanation:
Answer – A, B and D

The AWS Documentation mentions the following.

Amazon CloudFront employs a global network of edge locations and regional edge caches that cache copies of your content close to your viewers. Amazon CloudFront ensures that end-user requests are served by the closest edge location.

Regional edge caches are CloudFront locations that are deployed globally, close to your viewers. They're located between your origin server and the POPs—global edge locations that serve content directly to viewers. As objects become less popular, individual POPs might remove those objects to make room for more popular content. 

For more information on Cloudfront and Edge locations, please refer to the following link:

https://docs.aws.amazon.com/AmazonCloudFront/latest/DeveloperGuide/HowCloudFrontWorks.html
 

Ask our Experts
View Queries
Did you like this Question?

Question 43Correct
Domain: Technology
Which of the following storage options provides the option of Lifecycle policies that can be used to move objects to archive storage.


A. Amazon S3right
B. Amazon Glacier
C. Amazon Storage Gateway
D. Amazon EBS
Explanation:
Answer – A

The AWS Documentation mentions the following

Lifecycle configuration enables you to specify the lifecycle management of objects in a bucket. The configuration is a set of one or more rules, where each rule defines an action for Amazon S3 to apply to a group of objects. These actions can be classified as follows:

·         Transition actions – In which you define when objects transition to another storage class. For example, you may choose to transition objects to the STANDARD_IA (IA, for infrequent access) storage class 30 days after creation, or archive objects to the GLACIER storage class one year after creation.

 ·         Expiration actions – In which you specify when the objects expire. Then Amazon S3 deletes the expired objects on your behalf.

 For more information on AWS Object Lifecycle management, please visit the Link:

https://aws.amazon.com/s3/
Ask our Experts
View Queries
Did you like this Question?

Question 44Incorrect
Domain: Technology
Which of the following features of Amazon RDS allows for better availability of databases? Choose the answer from the options given below.


A. VPC Peering
B. Multi-AZright
C. Read Replicaswrong
D. Data encryption
Explanation:
Answer – B

The AWS Documentation mentions the following.

If you are looking to use replication to increase database availability while protecting your latest database updates against unplanned outages, consider running your DB instance as a Multi-AZ deployment. 

For more information on AWS RDS, please visit the FAQ Link:

https://aws.amazon.com/rds/faqs/
 

Ask our Experts
View Queries
Did you like this Question?

Question 45Correct
Domain: Cloud Concepts
A client who has adopted AWS Cloud would like to ensure that his systems need to deliver continuous business value & improve supporting processes and procedures. Which design pillar will he need to focus for achieving this?


A. Reliability
B. Scalability
C. Automation
D. Operational Excellenceright
Explanation:
Correct Answer: D

Continuous business value is achieved with the ability to monitor existing running systems & improving processes and procedures by managing & automating changes. For eg in response to a saturation in CPU usage of an EC2 instance, a monitoring system like CloudWatch will automatically trigger a creation of a new instance though alarms. This will ensure that the system's capacity meets changing load demands. This is a part of the Operational Excellence pillar of the AWS well architected framework which focuses on running & monitoring systems to deliver business value

Option A is incorrect since the Reliability pillar focuses on the ability of the system to recover from infrastructure or service failures
Option B is incorrect since scalability is a by-product of monitoring solutions which provide the capability for infrastructure resources to cope with increase or decrease of capacity by adding or terminating resources when not needed.
Option C is incorrect since automation is the ability to induce certain systemic requirements like scalability, auto recovery using monitoring solutions. It helps in improving system’s stability & efficiency of an Organization
Option D is CORRECT. Refer to the above description for details
Diagram:



Reference:

https://aws.amazon.com/blogs/apn/the-5-pillars-of-the-aws-well-architected-framework/
Ask our Experts
View Queries
Did you like this Question?

Question 46Incorrect
Domain: Security
Which of the following encryption techniques is used by AWS KMS for integration with other AWS services?


A. RSA Encryption
B. AES Encryptionwrong
C. Triple DES Encryption
D. Envelope Encryptionright
Explanation:
Correct Answer – D

AWS KMS uses envelope encryption while integrating with other AWS services. In this encryption technique, data is encrypted by the data encryption key within that service. This data key is further encrypted using the customer master key (CMK) stored in AWS KMS.

Options A, B & C are incorrect as AWS KMS does not use these encryption techniques for integration with other AWS services.
For more information on AWS KMS, refer to the following URL:

https://aws.amazon.com/kms/features/
Ask our Experts
View Queries
Did you like this Question?

Question 47Incorrect
Domain: Technology
You are the architect of a custom application running inside your corporate data center. The application runs with some unresolved bugs that produce a lot of data inside custom log files generating time-consuming activities for the operation team responsible for analyzing them.

You want to move the application to AWS using EC2 instances. At the same time, you want to take the opportunity to improve logging and monitoring capabilities, but without touching the application code.

What AWS service should you use to satisfy the requirement?


A. AWS Kinesis Data Streams
B. AWS CloudTrailwrong
C. AWS CloudWatch Logsright
D. AWS Application Logs
Explanation:
Answer: C

Option A is INCORRECT because in order to feed a Data Streams from custom logs you have to change the application code. AWS documentation describes this with the following sentence: “To put data into the stream, you must specify the name of the stream, a partition key, and the data blob to be added to the stream.”
Option B is INCORRECT because it is not related to the scenario and custom log files.
Option C is CORRECT because AWS CloudWatch Logs has the capability to reuse existing application logs increasing efficiency in operation with the ability to generate on them metrics, alerts and analytics with AWS CloudWatch Logs Insight.
The application and custom log files are exactly as they were when the application was running on-prem. So you don’t need to change any piece of application code that makes them ingestible by AWS CloudWatch Logs.

AWS official documentation in the FAQ section highlights the reusing capability with the sentence “AWS CloudWatch Logs lets you monitor and troubleshoot your systems and applications using your existing system, application and custom log files… so, no code changes are required.”

You can also leverage CloudWatch Metrics, Alarms and Dashboards with Logs to get full operational visibility into your applications. This empowers you to understand your applications, make improvements, and find problems quickly. Thus you can continue to innovate rapidly.

Option D is INCORRECT because AWS Application Logs does not exist.
Diagram: none

References:

https://aws.amazon.com/cloudwatch/faqs/
Ask our Experts
View Queries
Did you like this Question?

Question 48Correct
Domain: Technology
Your company wants to move an existing Oracle database to the AWS Cloud. Which of the following services can help facilitate this move?


A. AWS Database Migration Serviceright
B. AWS VM Migration Service
C. AWS Inspector
D. AWS Trusted Advisor
Explanation:
Answer - A

The AWS Documentation mentions the following.

AWS Database Migration Service helps you migrate databases to AWS quickly and securely. The source database remains fully operational during the migration, minimizing downtime to applications that rely on the database. The AWS Database Migration Service can migrate your data to and from the most widely used commercial and open-source databases.

For more information on AWS Database migration, please refer to the below URL:

https://aws.amazon.com/dms/
 

Ask our Experts
View Queries
Did you like this Question?

Question 49Correct
Domain: Cloud Concepts
Which of the following features of AWS RDS allows you to reduce the load on the database while reading data?


A. Cross region replication
B. Creating Read Replicasright
C. Using snapshots
D. Using Multi-AZ feature
Explanation:
Answer – B

The AWS Documentation mentions the following:

You can reduce the load on your source DB Instance by routing read queries from your applications to the read replica. Read replicas allow you to elastically scale out beyond the capacity constraints of a single DB instance for read-heavy database workloads.

For more information on Read Replicas, please refer to the below URL:

https://aws.amazon.com/rds/details/read-replicas/
Ask our Experts
View Queries
Did you like this Question?

Question 50Correct
Domain: Cloud Concepts
Which of the following terms refers to a physical location around the world where data centers are located in AWS?


A. Sub zone
B. Data center
C. Regionright
D. Edge location
Explanation:
Answer – C

AWS has the concept of a Region, which is a physical location around the world where we cluster data centers. We call each group of logical data centers an Availability Zone. Each AWS Region consists of multiple, isolated, and physically separate AZ's within a geographic area. Unlike other cloud providers, who often define a region as a single data center, the multiple AZ design of every AWS Region offers advantages for customers.

For more information on Regions and Availability Zones in AWS, please refer to the below URL:

https://aws.amazon.com/about-aws/global-infrastructure/regions_az/
Ask our Experts
View Queries
Did you like this Question?

Question 51Correct
Domain: Cloud Concepts
A company wants to have a database hosted on AWS. As much as possible they want to have control over the database itself. Which of the following would be an ideal option for this?


A. Using the AWS DynamoDB service
B. Using the AWS RDS service
C. Hosting the database on an EC2 Instanceright
D. Using the Amazon Aurora service
Explanation:
Answer – C

If you want a self-managed database, that means you want complete control over the database engine and the underlying infrastructure. In such a case, you need to host the database on an EC2 Instance.

For more information on EC2 Instances, please refer to the below URL:

https://aws.amazon.com/ec2/
Ask our Experts
View Queries
Did you like this Question?

Question 52Correct
Domain: Security
On which of the following resources does Amazon Inspector perform network accessibility checks?


A. Amazon CloudFront
B. Amazon VPN
C. Amazon EC2 instanceright
D. Amazon VPC
Explanation:
Correct Answer – C

Amazon Inspector provides two types of packages. Network reachability rules package checks network accessibility checks on Amazon EC2 instance. Host assessment rules package checks vulnerabilities on Amazon EC2 instance.

Options A, B & D are incorrect as Amazon Inspector performs network accessibility checks on Amazon EC2 instance, not on Amazon CloudFront, Amazon VPN or Amazon VPC.
For more information on Amazon Inspector, refer to the following URL:

https://aws.amazon.com/inspector/faqs/
Ask our Experts
View Queries
Did you like this Question?

Question 53Correct
Domain: Cloud Concepts
Which of the following services helps to achieve the computing elasticity in AWS?


A. AWS RDS
B. VPC Endpoint
C. AWS EC2 Auto Scaling Groupright
D. Amazon S3
Explanation:
Answer – C

AWS EC2 Auto Scaling Group achieves the computing elasticity by scaling up/down the EC2 instances based on demand.

For more information on the AWS Autoscaling service, please refer to the below URL:

https://aws.amazon.com/autoscaling/
 

Ask our Experts
View Queries
Did you like this Question?

Question 54Correct
Domain: Cloud Concepts
To receive AWS Trusted Advisor Notifications, what actions are required from the customer end?


A. Open a ticket with AWS Support.
B. Set up Notification in Dashboardright
C. Set up Amazon Simple Notification Service
D. No action is required, all Notifications are sent automatically on a weekly basis.
Explanation:
Correct Answer – B

AWS Trusted Advisor Notification is an optional service that needs to be set up from the dashboard providing a list of recipients and selecting resource items for which status is required.

Option A is incorrect as opening an AWS support ticket is not required to receive AWS Trusted Advisor Notification.
Option C is incorrect as Amazon SNS is a separate service for push notifications. But it is not required to receive AWS Trusted Advisor Notification.
Option D is incorrect as you need to set up the notifications in the dashboard.
For more information on AWS Trusted Advisor, refer to the following URL:

https://aws.amazon.com/premiumsupport/faqs/?nc=sn&loc=6
Ask our Experts
View Queries
Did you like this Question?

Question 55Correct
Domain: Cloud Concepts
Why is Amazon DynamoDB service best-suited for implementation in mobile, Internet of Things (IoT) and gaming applications?


A. DynamoDB is a fully-managed database instance with no infrastructure overheads.
B. DynamoDB has a flexible data model and single-digit millisecond latency.right
C. Whilst in operation, DynamoDB instances are spread across at least three geographically distinct centers, AWS Regions.
D. DynamoDB supports eventual and strongly consistent reads.
Explanation:
Correct Answer – B

The use cases mentioned in the scenario have unstructured data in common. Therefore, the most appropriate attribute of Amazon DynamoDB is its flexible data model and single-digit millisecond latency.

https://aws.amazon.com/blogs/database/how-to-determine-if-amazon-dynamodb-is-appropriate-for-your-needs-and-then-plan-your-migration/

Option A is INCORRECT because being fully-managed and having no infrastructure overheads do not distinguish DynamoDB as the best-suited solution for the given use cases.
Option C is INCORRECT because the aspect of fault-tolerance, disaster recovery and high availability is also present in Amazon Relational Databases (RDS). This feature does not distinguish the service in accordance with the described use cases.
Option D is INCORRECT because this attribute of DynamoDB does not fully justify its exclusive choice over other instances when considered for implementation in the use cases mentioned in the question.
Ask our Experts
View Queries
Did you like this Question?

Question 56Incorrect
Domain: Billing and Pricing0
A client who is using AWS cloud services has multiple environments for the EC2 servers like DEV, QA, PROD respectively. The client would like to know billing details for each of these environments to make informed decisions related to saving costs. Using which of the following options the requirements can be achieved?


A. Consolidated billing
B. AWS Budgetswrong
C. AWS Cost allocation tagsright
D. AWS Organizations
Explanation:
Correct Answer: C

Cost allocation tags appear as additional columns in detailed billing reports. As an example, let's say an AWS Region has 50 EC2 instances running out of which 15 are DEV, 15 are QA & the remaining are PROD. While launching these instances, one can apply a tag named “env” providing value of DEV for 15 instances, QA for 15 instances and PROD for 20 instances. These tags then appear in a detailed billing report as columns which can be filtered based on the environment and the cost of a set of environment servers calculated easily

Option A is incorrect since consolidated billing is a feature that applies to scenarios where a client has multiple accounts and would like to receive one bill for all his accounts
Option B is incorrect since AWS Budgets are used for setting custom budgets budgeting costs to track costs and usage of resources & get alerted when actual or forecasted cost and usage exceeds the limits set for that budget
Option C is CORRECT. Refer above description for the same.
Option D is incorrect. AWS Organizations allows you to consolidate multiple AWS accounts into an Organization that can be centrally managed for billing. They can have Service Control Policies applied at the organization level that can override policies set up by IAM for individual accounts
Reference:

https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/cost-alloc-tags.html
Ask our Experts
View Queries
Did you like this Question?

Question 57Incorrect
Domain: Cloud Concepts
Which of the following does AWS perform on its behalf for EBS volumes to make it less prone to failure?


A. Replication of the volume across Availability Zoneswrong
B. Replication of the volume in the same Availability Zoneright
C. Replication of the volume across Regions
D. Replication of the volume across Edge locations
Explanation:
Answer – B

When you create an EBS volume in an Availability Zone, it is automatically replicated within that zone to prevent data loss due to the failure of any single hardware component.

For more information on EBS Volumes, please refer to the below URL:

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSVolumes.html
 

Ask our Experts
View Queries
Did you like this Question?

Question 58Incorrect
Domain: Technology
You are requested to expose your serverless application implemented with AWS Lambda to HTTP clients. ( using HTTP Proxy )

Which of the following AWS services can you use to accomplish the task? (Select TWO)


A. AWS Elastic Load Balancing (ELB)right
B. AWS Route53
C. AWS API Gatewayright
D. AWS Lightsailwrong
E. AWS Elastic Beanstalk
Explanation:
Answer: A and C

Option A is CORRECT because AWS documentation mentions that "Application Load Balancers now support invoking Lambda functions to serve HTTP(S) requests." This enables users to access serverless applications from any HTTP client, including web browsers.
Option B is INCORRECT because Route53 is a Domain Name System and not an HTTP proxy.
Option C is CORRECT because API Gateway + Lambda is a common pattern for exposing serverless functions via HTTP/HTTPS. AWS documentation mentions that "Creating, deploying, and managing a REST application programming interface (API) to expose backend HTTP endpoints, AWS Lambda functions, or other AWS services." 
Option D is INCORRECT because AWS Lightsail has a completely different goal. It is a service to speed up the provisioning of AWS resources.
Option E is INCORRECT because AWS Elastic Beanstalk has a completely different goal. It is a service that makes it easier for developers to deploy and manage applications in the AWS Cloud quickly. Developers simply upload their applications, then Elastic Beanstalk automatically handles the deployment details of capacity provisioning, load balancing, auto-scaling, and application health monitoring.
Diagram: none

References:

ELB:

https://aws.amazon.com/elasticloadbalancing/faqs/?nc=sn&loc=6
API Gateway:

https://aws.amazon.com/api-gateway/faqs/
Ask our Experts
View Queries
Did you like this Question?

Question 59Incorrect
Domain: Security0
You have an EC2 Instance in development that interacts with the Simple Storage Service. The EC2 Instance is going to be promoted to the production environment. Which of the following features should be used to grant the EC2 instance suitable permissions to access the Simple Storage Service?


A. IAM Users
B. IAM Roleswrong
C. IAM Groups
D. IAM Policiesright
Explanation:
Answer - D

The AWS Documentation mentions the following.

IAM policies are used to manage access in AWS by attaching them to IAM identities (users, groups of users, or roles) or AWS resources. A policy is an object in AWS that, when associated with an identity or resource, defines their permissions. AWS evaluates these policies when an IAM principal (user or role) makes a request.

An IAM role is an IAM identity that you can create in your account that has specific permissions. An IAM role is similar to an IAM user, in that it is an AWS identity with permission policies that determine what the identity can and cannot do in AWS.

An IAM user group is a collection of IAM users.

An IAM user is an entity that you create in AWS to represent the person or application that uses it to interact with AWS.

An IAM user with administrator permissions is not the same thing as the AWS account root user. 

For more information on IAM Roles, please refer to the below URL:

https://docs.aws.amazon.com/IAM/latest/UserGuide/id_groups.html
https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies.html
https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html
Ask our Experts
View Queries
Did you like this Question?

Question 60Correct
Domain: Cloud Concepts
A live online game uses DynamoDB instances in the backend to store real-time scores of the participants as they compete against each other from various parts of the world. Which data consistency option is the most appropriate to implement?


A. Strongly consistentright
B. Eventually consistent
C. Strong Eventual consistency
D. Optimistic consistency
Explanation:
Correct Answer – A

Since the gamers are from geographically distinct locations, the data will need to be immediately readable within a second as soon as it is written. Therefore strongly consistency is needed.

https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.ReadConsistency.html

 

Option B is INCORRECT because the scenarios outline that the participants of the game are live. It will not suffice if any of them get updates on scores in less than real-time.
Option C is INCORRECT because strong eventual consistency is not applicable in DynamoDB.
Option D is INCORRECT because only two data consistency models are available with the DynamoDB service. Optimistic consistency is not supported.
Ask our Experts
View Queries
Did you like this Question?

Question 61Correct
Domain: Security
Your company is planning to host a large e-commerce application on the AWS Cloud. One of their major concerns is Internet attacks such as DDoS attacks. Which of the following services can help mitigate this concern? Choose 2 answers from the options given below.


A. Cloudfrontright
B. AWS Shieldright
C. AWS EC2
D. AWS Config
Explanation:
Answer – A and B

The AWS Documentation mentions the following on DDoS attacks.

AWS Services for DDoS Attack Mitigation
AWS offers globally distributed, high network bandwidth and resilient services that, when used in conjunction with application-specific strategies, are key to mitigating DDoS attacks. For more information on how to leverage each of these services and details on how their various features help protect against DDoS attacks, see the whitepaper AWS Best Practices for DDoS Resiliency.

AWS Shield

 

AWS Shield is a managed DDoS protection service that is available in two tiers: Standard and Advanced. AWS Shield Standard applies always-on detection and inline mitigation techniques, such as deterministic packet filtering and priority-based traffic shaping, to minimize application downtime and latency. AWS Shield Standard is included automatically and transparently to your Elastic Load Balancing load balancers, Amazon CloudFront distributions, and Amazon Route 53 resources at no additional cost. When you use these services that include AWS Shield Standard, you receive comprehensive availability protection against all known infrastructure layer attacks. Customers who have the technical expertise to manage their own monitoring and mitigation of application layer attacks can use AWS Shield together with AWS WAF rules to create a comprehensive DDoS attack mitigation strategy.

AWS Shield Advanced provides enhanced DDoS attack detection and monitoring for application-layer traffic to your Elastic Load Balancing load balancers, CloudFront distributions, Amazon Route 53 hosted zones and resources attached to an Elastic IP address, such Amazon EC2 instances. AWS Shield Advanced uses additional techniques to provide granular detection of DDoS attacks, such as resource-specific traffic monitoring to detect HTTP floods or DNS query floods. AWS Shield Advanced includes 24x7 access to the AWS DDoS Response Team (DRT), support experts who apply manual mitigations for more complex and sophisticated DDoS attacks, directly create or update AWS WAF rules, and can recommend improvements to your AWS architectures. AWS WAF is included at no additional cost for resources that you protect with AWS Shield Advanced.

AWS Shield Advanced includes access to near real-time metrics and reports, for extensive visibility into infrastructure layer and application layer DDoS attacks. You can combine AWS Shield Advanced metrics with additional, fine-tuned AWS WAF metrics for a more comprehensive CloudWatch monitoring and alarming strategy. Customers subscribed to AWS Shield Advanced can also apply for a credit for charges that result from scaling during a DDoS attack on protected Amazon EC2, Amazon CloudFront, Elastic Load Balancing, or Amazon Route 53 resources. See the AWS Shield Developer Guide for a detailed comparison of the two AWS Shield offerings.

AWS WAF

 

AWS WAF is a web application firewall that helps protect web applications from common web exploits that could affect application availability, compromise security, or consume excessive resources. You can use AWS WAF to define customizable web security rules that control which traffic accesses your web applications. If you use AWS Shield Advanced, you can use AWS WAF at no extra cost for those protected resources and can engage the DRT to create WAF rules.

AWS WAF rules use conditions to target specific requests and trigger an action, allowing you to identify and block common DDoS request patterns and effectively mitigate a DDoS attack. These include size constraint conditions to block a web request based on the length of its query string or request body, and geographic match conditions to implement geo restriction (also known as geoblocking) on requests that originate from specific countries. For a complete list of conditions, see the AWS WAF Developer Guide. With AWS WAF, you can also create rate-based rules that automatically block requests from a single IP address if they exceed a customer-defined rate limit. One benefit of rate-based rules is that you can block requests from an IP address while it exceeds the threshold, and then automatically allow requests from that same client once they drop to an acceptable rate. This helps ensure that regular viewers are not held in a persistent block list. You can also combine the rate limit with conditions to trigger different actions for distinct scenarios.

Amazon Route 53

One of the most common targets of DDoS attacks is the Domain Name System (DNS). Amazon Route 53 is a highly available and scalable DNS service designed to route end users to infrastructure running inside or outside of AWS. Route 53 makes it possible to manage traffic globally through a variety of routing types, and provides out-of-the-box shuffle sharding and Anycast routing capabilities to protect domain names from DNS-based DDoS attacks.

Amazon CloudFront

Amazon CloudFront distributes traffic across multiple edge locations and filters requests to ensure that only valid HTTP(S) requests will be forwarded to backend hosts. CloudFront also supports geoblocking, which you can use to prevent requests from particular geographic locations from being served.

Elastic Load Balancing

Elastic Load Balancing automatically distributes incoming application traffic across multiple targets, such as Amazon Elastic Compute Cloud (Amazon EC2) instances, containers, and IP addresses, and multiple Availability Zones, which minimizes the risk of overloading a single resource. Elastic Load Balancing, like CloudFront, only supports valid TCP requests, so DDoS attacks such as UDP and SYN floods are not able to reach EC2 instances. It also offers a single point of management and can serve as a line of defense between the internet and your backend, private EC2 instances. Elastic Load Balancing includes the Application Load Balancer, which is best suited for load balancing of HTTP and HTTPS traffic and also directly supports AWS WAF.

VPCs and Security Groups

Amazon Virtual Private Cloud (Amazon VPC) allows customers to configure subnet routes, public IP addresses, security groups, and network access control lists in order to minimize application attack surfaces. You can configure load balancers and EC2 instance security groups to allow traffic that originates from specific IP addresses only, such as that from CloudFront or AWS WAF, protecting backend application components from a direct attack.

For more information on DDoS attack prevention, please refer to the below URL:

https://aws.amazon.com/answers/networking/aws-ddos-attack-mitigation/
 

Ask our Experts
View Queries
Did you like this Question?

Question 62Correct
Domain: Technology
A research team conducting its work in remote locations of the world, without internet access, wishes to leverage Amazon services for their storage. The team collects petabytes of information at a time. Which service will best meet to transfer the petabytes of information?


A. Amazon S3
B. Amazon Elastic Block Store (EBS)
C. Amazon S3 Glacier
D. AWS Snowballright
Explanation:
Correct Answer – D

The AWS Snowball service uses physical storage devices to transfer large amounts of data between Amazon Simple Storage Service (Amazon S3) and your onsite data storage location at faster-than-internet speeds. By working with AWS Snowball, you can save time and money. Snowball provides powerful interfaces that you can use to create jobs, track data, and track your jobs' status through to completion.

Snowball devices are physically rugged devices protected by the AWS Key Management Service (AWS KMS). They secure and protect your data in transit. 

https://docs.aws.amazon.com/snowball/latest/ug/whatissnowball.html

Option A is incorrect because Amazon S3 is the most suitable object storage when there is internet connectivity. In this scenario, there is none.
Option B is incorrect because Amazon EBS provides block level storage volumes suitable for operating systems, database instances and applications. For the research team to store data to detached EBS volumes (not attached to EC2 instances), they would need internet connectivity. In this scenario, the remote location does not have connectivity.
Option C is incorrect because S3 Glacier is used for infrequent access nor usage. It is unsuitable for this scenario.
Ask our Experts
View Queries
Did you like this Question?

Question 63Incorrect
Domain: Technology
Which of the following AWS services use serverless technology? Choose 2 answers from the options given below.


A. DynamoDBright
B. EC2
C. Simple Storage Serviceright
D. AWS Autoscalingwrong
Explanation:
Answer – A and C

The Simple Storage Service and DynamoDB are services where you don’t need to manage the underlying infrastructure.

For more information on AWS S3 and DynamoDB, please refer to the below URL:
https://aws.amazon.com/serverless/
https://aws.amazon.com/s3/
https://aws.amazon.com/dynamodb/
Ask our Experts
View Queries
Did you like this Question?

Question 64Correct
Domain: Cloud Concepts
Which of the following disaster recovery deployment mechanisms has the highest downtime?


A. Pilot light
B. Warm standby
C. Multi-Site
D. Backup and Restoreright
Explanation:
Answer – D

The below snapshot from the AWS Documentation shows the spectrum of the Disaster recovery methods. If you go to the further end of the spectrum you have the least time for downtime for the users.


 In most traditional environments, data is backed up to tape and sent off-site regularly. If you use this method, it can take a long time to restore your system in the event of a disruption or disaster.  
https://d1.awsstatic.com/whitepapers/aws-disaster-recovery.pdf
For more information on Disaster recovery techniques, please refer to the below URL:

https://aws.amazon.com/blogs/aws/new-whitepaper-use-aws-for-disaster-recovery/
Ask our Experts
View Queries
Did you like this Question?

Question 65Correct
Domain: Security
Which of the following services allows you to analyze EC2 Instances against pre-defined security templates to check for vulnerabilities?


A. AWS Trusted Advisor
B. AWS Inspectorright
C. AWS WAF
D. AWS Shield
Explanation:
Answer – B

The AWS Documentation mentions the following.

Amazon Inspector enables you to analyze the behavior of your AWS resources and helps you to identify potential security issues. Using Amazon Inspector, you can define a collection of AWS resources that you want to include in an assessment target. You can then create an assessment template and launch a security assessment run of this target.

For more information on AWS Inspector, please refer to the below URL:

https://docs.aws.amazon.com/inspector/latest/userguide/inspector_introduction.html
 