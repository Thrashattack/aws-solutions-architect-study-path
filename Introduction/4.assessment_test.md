# Assessment Test


- Test to verify the level of the student

## Logbook

- Mode: Study - You can see the awnsers after each question
- Order: Random 
- Questions: 39 
- Estimated Time: 78 minutes
- Started at: 17:10

--

# Question 1 of 39 
tb713081.AWSCSASG3E.at.37
Use V-O keys to navigate.True/false: CloudFormation stack names are case-sensitive.

A: True 
R: True 

You Answered Correctly!
Almost everything in CloudFormation is case sensitive. See [Chapter 14] for more information.

--

# Question 2 of 39 
tb713081.AWSCSASG3E.at.33
Use V-O keys to navigate.Use V-O keys to navigate.True/false: If versioning is enabled on an S3 bucket, applying encryption to an unencrypted object in that bucket will create a new, encrypted version of that object.

A: True 
R: True 

You Answered Correctly!
Applying encryption to an unencrypted object will create a new, encrypted version of that object. Previous versions remain unencrypted. See Chapter 12 for more information.

--

# Question 3 of 39 
tb713081.AWSCSASG3E.at.35
Use V-O keys to navigate.Use V-O keys to navigate.True/false: The EBS Lifecycle Manager can take snapshots of volumes that were once attached to terminated instances.

A: True 
R: True 

You Answered Correctly!
The EBS Lifecycle Manager can take scheduled snapshots of any EBS volume, regardless of attachment state. See Chapter 13 for more information.

--

# Question 4 of 39 
tb713081.AWSCSASG3E.at.23
Use V-O keys to navigate.Use V-O keys to navigate.You want to use Route 53 to send users to the application load balancer closest to them. Which of the following routing policies lets you do this with the least effort?


A. Latency routing
B. Geolocation routing
C. Geoproximity routing
D. Edge routing

A: A
R: C 

You Answered Incorrectly.
Geoproximity routing routes users to the location closest to them. Geolocation routing requires you to create records for specific locations or create a default record. See Chapter 8 for more information.
(I thought latency would require less effort, but the premise `low latency = closet to user` may not be true everytime)

--


# Question 5 of 39 
tb713081.AWSCSASG3E.at.03
Use V-O keys to navigate.Use V-O keys to navigate.Which of the following services is most useful for decoupling the components of a monolithic application?


A. SNS
B. KMS
C. SQS
D. Glacier


A: C
R: C 

You Answered Correctly!
Simple Queue Service (SQS) allows for event-driven messaging within distributed systems that can decouple while coordinating the discrete steps of a larger process. See Chapter 1 for more information.

-- 

# Question 6 of 39 
tb713081.AWSCSASG3E.at.12
Use V-O keys to navigate.Use V-O keys to navigate.True/false: The route table for a public subnet must have a default route pointing to an Internet gateway as a target.

A: False 
R: True 

You Answered Incorrectly.
The definition of a public subnet is a subnet that has a default route pointing to an Internet gateway as a target. Otherwise, it’s a private subnet. See Chapter 4 for more information.

(I missed the `public` here... Dammm)


--


# Question 7 of 39 
tb713081.AWSCSASG3E.at.19
Use V-O keys to navigate.True/false: EC2 sends instance memory utilization metrics to CloudWatch every five minutes.

A: True
R: False

You Answered Incorrectly.
EC2 doesn’t track instance memory utilization. See Chapter 7 for more information.

( I just thought it did)

--

# Question 8 of 39 
tb713081.AWSCSASG3E.at.07
Use V-O keys to navigate.Use V-O keys to navigate.Which S3 encryption option does not require AWS persistently storing the encryption keys it uses to decrypt data?


A. Client-side encryption
B. SSE-KMS
C. SSE-S3
D. SSE-C

A: A
R: D

You Answered Incorrectly.
With SSE-C you provide your own keys for Amazon to use to decrypt and encrypt your data. AWS doesn’t persistently store the keys. See Chapter 3 for more information.

( i dont know this encryption options)

--

# Question 9 of 39 
tb713081.AWSCSASG3E.at.04
Use V-O keys to navigate.Use V-O keys to navigate.An application you want to run on EC2 requires you to license it based on the number of physical CPU sockets and cores on the hardware you plan to run the application on. Which of the following tenancy models should you specify?


A. Dedicated host
B. Dedicated instance
C. Shared tenancy
D. Bring your own license

A: A
R: A

You Answered Correctly!
The dedicated host option lets you see the number of physical CPU sockets and cores on a host. See Chapter 2 for more information.


--

# Question 10 of 39 
tb713081.AWSCSASG3E.at.16
Use V-O keys to navigate.Use V-O keys to navigate.Which of the following steps does the most to protect your AWS account?


A. Deleting unused Identity and Access Management (IAM) policies
B. Revoking unnecessary access for IAM users
C. Rotating root access keys
D. Restricting access to S3 buckets
E. Rotating Secure Shell (SSH) key pairs

A: B
R: B

You Answered Correctly!
Revoking unnecessary access for IAM users is the most effective of the listed measures for protecting your AWS account. See Chapter 6 for more information.

--

# Question 11 of 39 
tb713081.AWSCSASG3E.at.20
Use V-O keys to navigate.Use V-O keys to navigate.You configured a CloudWatch alarm to monitor CPU utilization for an EC2 instance. The alarm began in the INSUFFICIENT_DATA state and then entered the ALARM state. What can you conclude from this?



A. The instance recently rebooted.
B. CPU utilization is too high.
C. The CPU utilization metric crossed the alarm threshold.
D. The instance is stopped.

A: C
R: C


You Answered Correctly!
The transition to the ALARM state simply implies that the metric crossed a threshold but doesn’t tell you what the threshold is. Newly created alarms start out in the INSUFFICIENT_DATA state. See Chapter 7 for more information.

( tricky i knew we couldn't conclude any of that by an alarm state transiction)

--

# Question 12 of 39 
tb713081.AWSCSASG3E.at.18
Use V-O keys to navigate.What is a difference between a token generated by the AWS Security Token Service (STS) and an IAM access key?


A. The token generated by STS can’t be used by an IAM principal.
B. An IAM access key is unique.
C. The token generated by STS can be used only once.
D. The token generated by STS expires.

A: C
R: D

You Answered Incorrectly.
STS tokens expire and IAM access keys do not. An STS token can be used more than once. IAM access keys and STS tokens are both unique. An IAM principal can use an STS token. See Chapter 6 for more information.

(I have a week experience with STS)


--

# Question 13 of 39 
tb713081.AWSCSASG3E.at.39
Use V-O keys to navigate.True/false: You can use either CodeDeploy or an AWS Systems Manager command document to deploy a Lambda application.

A: True
R: False

You Answered Incorrectly.
You can use CodeDeploy to deploy an application to Lambda or EC2 instances. But an AWS Systems Manager command document works only on EC2 instances. See Chapter 14 for more information.

( didnt knew it was only for ec2, i used it to deploy multiple docker instances on ec2)

--

# Question 14 of 39 
tb713081.AWSCSASG3E.at.11
Use V-O keys to navigate.True/false: An EC2 instance must be in a public subnet to access the Internet.

A: False
R: False

You Answered Correctly!
An EC2 instance can access the Internet from a private subnet provided it uses a NAT gateway or NAT instance. See Chapter 4 for more information.

--


# Question 15 of 39 
tb713081.AWSCSASG3E.at.13
Use V-O keys to navigate.Use V-O keys to navigate.Which of the following use cases is well suited for DynamoDB?


A. Running a MongoDB database on AWS
B. Storing large binary files exceeding 1 GB in size
C. Storing JSON documents that have a consistent structure
D. Storing image assets for a website

A: C
R: C

You Answered Correctly!
DynamoDB is a key-value store that can be used to store items up to 400 KB in size. See Chapter 5 for more information.

--


# Question 16 of 39 
tb713081.AWSCSASG3E.at.34
Use V-O keys to navigate.Use V-O keys to navigate.Which instance type will, if left running, continue to incur costs?

A: C
R: C

You Answered Correctly!
On-demand instances will continue to run and incur costs. Reserved instances cost the same whether they’re running or stopped. Spot instances will be terminated when the spot price exceeds your bid price. See Chapter 13 for more information.

--

# Question 17 of 39 
tb713081.AWSCSASG3E.at.02
Use V-O keys to navigate.Use V-O keys to navigate.True/false: AWS is responsible for managing the network configuration of your EC2 instances.

A: False
R: False

You Answered Correctly!
Customers are responsible for managing the network configuration of EC2 instances. AWS is responsible for the physical network infrastructure. See Chapter 1 for more information.


--

# Question 18 of 39 
tb713081.AWSCSASG3E.at.10
Use V-O keys to navigate.Use V-O keys to navigate.You created a Virtual Private Cloud (VPC) using the Classless Inter-Domain Routing (CIDR) block 10.0.0.0/24. You need to connect to this VPC from your internal network, but the IP addresses in use on your internal network overlap with the CIDR. Which of the following is a valid way to address this problem?


A. Remove the CIDR and use IPv6 instead.
B. Change the VPC’s CIDR.
C. Create a new VPC with a different CIDR.
D. Create a secondary CIDR for the VPC.

A: D
R: C


You Answered Incorrectly.
You can’t change the primary CIDR for a VPC, so you must create a new one to connect it to your internal network. See Chapter 4 for more information.


(never worked with cidr and vpc)


--

# Question 19 of 39 
tb713081.AWSCSASG3E.at.17
Use V-O keys to navigate.Use V-O keys to navigate.Which of the following can be used to encrypt the operating system of an EC2 instance?


A. AWS Secrets Manager
B. CloudHSM
C. AWS Key Management Service (KMS)
D. AWS Security Token Service (STS)

A: B ??
R: C

You Answered Incorrectly.
KMS can be used to encrypt Elastic Block Store (EBS) volumes that store an instance’s operating system. See Chapter 6 for more information.

( i have alot to learn about encryption)

--

# Question 20 of 39 
tb713081.AWSCSASG3E.at.06
Use V-O keys to navigate.Use V-O keys to navigate.True/false: You can use a Quick Start Amazon Machine Image (AMI) to create any instance type.

A: False
R: True

You Answered Incorrectly.
A Quick Start AMI is independent of the instance type. See Chapter 2 for more information.

( i thought it was only on-demand)

--

# Question 21 of 39 
tb713081.AWSCSASG3E.at.15
Use V-O keys to navigate.Use V-O keys to navigate.True/false: Enabling point-in-time RDS snapshots is sufficient to give you a recovery point objective (RPO) of less than 10 minutes.

A: True
R: True

You Answered Correctly!
Enabling point-in-time recovery gives you an RPO of about five minutes. The recovery time objective (RTO) depends on the amount of data to restore. See Chapter 5 for more information.


--

# Question 22 of 39 
tb713081.AWSCSASG3E.at.38
Use V-O keys to navigate.Use V-O keys to navigate.Use V-O keys to navigate.Where might CodeDeploy look for the appspec.yml file? (Choose two.)


A. GitHub
B. CodeCommit
C. S3
D. CloudFormation

A: A, C
R: A, C

You Answered Correctly!
CodeDeploy looks for the appspec.yml file with the application files it is to deploy, which can be stored in S3 or on GitHub. See Chapter 14 for more information.

--

# Question 23 of 39 
tb713081.AWSCSASG3E.at.08
Use V-O keys to navigate.Use V-O keys to navigate.True/false: Durability measures the percentage of likelihood that a given object will not be inadvertently lost by AWS over the course of a year.

A: True
R: True

You Answered Correctly!
Durability corresponds to an average annual expected loss of objects stored on S3, not including objects you delete. Availability measures the amount of time S3 will be available to let you retrieve those objects. See Chapter 3 for more information.

--

# Question 24 of 39 
tb713081.AWSCSASG3E.at.31
Use V-O keys to navigate.Use V-O keys to navigate.Which of the following services can you deactivate on your account?


A. Security Token Service (STS)
B. CloudWatch
C. Virtual Private Cloud (VPC)
D. Lambda

A: A
R: A

You Answered Correctly!
You can deactivate STS for all regions except US East. See Chapter 12 for more information.

--

# Question 25 of 39 
tb713081.AWSCSASG3E.at.24
Use V-O keys to navigate.Use V-O keys to navigate.True/false: You can use an existing domain name with Route 53 without switching its registration to AWS.

A: True
R: True

You Answered Correctly!
Route 53 is a true DNS service in that it can host zones for any domain name. You can also register domain names with or transfer them to Route 53. See Chapter 8 for more information.

--


# Question 26 of 39 
tb713081.AWSCSASG3E.at.09
Use V-O keys to navigate.Use V-O keys to navigate.True/false: After uploading a new object to S3, there will be a slight delay (one to two seconds) before the object is available.

A: True
R: False

You Answered Incorrectly.
S3 uses a read-after-write consistency model for new objects, so once you upload an object to S3, it’s immediately available. See Chapter 3 for more information.

( maybe was my network delay at the time)

--

# Question 27 of 39 
tb713081.AWSCSASG3E.at.22
Use V-O keys to navigate.Use V-O keys to navigate.True/false: An EC2 instance in a private subnet can resolve an “A” resource record for a public hosted zone hosted in Route 53.

A: True
R: True

You Answered Correctly!
An EC2 instance in a private subnet still has access to Amazon’s private DNS servers, which can resolve records stored in public hosted zones. See Chapter 8 for more information.

-- 

# Question 28 of 39 
tb713081.AWSCSASG3E.at.27
Use V-O keys to navigate.Use V-O keys to navigate.True/false: EC2 Auto Scaling automatically replaces group instances directly terminated by the root user.

A: True
R: True

You Answered Correctly!
Auto Scaling always attempts to maintain the minimum group size or, if set, the desired capacity. See Chapter 10 for more information.

-- 

# Question 29 of 39 
tb713081.AWSCSASG3E.at.05
Use V-O keys to navigate.Use V-O keys to navigate.True/false: Changing the instance type of an EC2 instance will change its elastic IP address.

A: False
R: False

You Answered Correctly!
An elastic IP address will not change. A public IP address attached to an instance will change if the instance is stopped, as would happen when changing the instance type. See Chapter 2 for more information.

--

# Question 30 of 39 
tb713081.AWSCSASG3E.at.30
Use V-O keys to navigate.Use V-O keys to navigate.True/false: S3 cross-region replication uses transfer acceleration.

A: True
R: False

You Answered Incorrectly.
S3 cross-region replication transfers objects between different buckets. Transfer acceleration uses a CloudFront edge location to speed up transfers between S3 and the Internet. See Chapter 11 for more information.
 
( why not use between them? )

--

# Question 31 of 39 
tb713081.AWSCSASG3E.at.25
Use V-O keys to navigate.You’re designing an application that takes multiple image files and combines them into a video file that users on the Internet can download. Which of the following can help you quickly implement your application in the fastest, most highly available, and most cost-effective manner?


A. EC2 spot fleet
B. Lambda
C. Relational Database Service (RDS)
D. Auto Scaling

A: B
R: B

You Answered Correctly!
Lambda is a highly available, reliable, “serverless” compute platform that runs functions as needed and scales elastically to meet demand. EC2 spot instances can be shut down on short notice. See Chapter 10 for more information.

--

# Question 32 of 39 
tb713081.AWSCSASG3E.at.26
Use V-O keys to navigate.Use V-O keys to navigate.You’re using EC2 Auto Scaling and want to implement a scaling policy that adds one extra instance only when the average CPU utilization of each instance exceeds 90 percent. However, you don’t want it to add more than one instance every five minutes. Which of the following scaling policies should you use?


A. Simple
B. Step
C. Target tracking
D. PercentChangeInCapacity

A: B
R: A

You Answered Incorrectly.
A simple scaling policy changes the group size and then has a cooldown period before doing so again. Step scaling policies don’t have cooldown periods. Target tracking policies attempt to keep a metric at a set value. PercentChangeInCapacity is a simple scaling adjustment type, not a scaling policy. See Chapter 10 for more information.

(step doenst coldown 😥 )

-- 

# Question 33 of 39 
tb713081.AWSCSASG3E.at.21
Use V-O keys to navigate.Use V-O keys to navigate.Where do AWS Config and CloudTrail store their logs?


A. S3 buckets
B. CloudWatch Logs
C. CloudTrail Events
D. DynamoDB
E. Amazon Athena

A: B
R: A

You Answered Incorrectly.
Both store their logs in S3 buckets. See Chapter 7 for more information.

( i imagined, just thouht it could have been updated)

--

# Question 34 of 39 
tb713081.AWSCSASG3E.at.36
Use V-O keys to navigate.Use V-O keys to navigate.Which of the following lets you spin up new web servers the quickest?


A. Lambda
B. Auto Scaling
C. Elastic Container Service
D. CloudFront

A: C
R: C

You Answered Correctly!
Elastic Container Service lets you run containers that can launch in a matter of seconds. EC2 instances take longer. Lambda is “serverless,” so you can’t use it to run a web server. CloudFront provides caching but isn’t a web server. See Chapter 13 for more information.

-- 

# Question 35 of 39 
tb713081.AWSCSASG3E.at.14
Use V-O keys to navigate.Use V-O keys to navigate.True/false: You can create a DynamoDB global secondary index for an existing table at any time.

R: True
A: True

You Answered Correctly!
You can create a global secondary index for an existing table at any time. You can create a local secondary index only when you create the table. See Chapter 5 for more information.

-- 

# Question 36 of 39 
tb713081.AWSCSASG3E.at.29
Use V-O keys to navigate.Use V-O keys to navigate.Which of the following is not an AWS service?


A. CloudFormation
B. Puppet
C. OpsWorks
D. Snowball

A: B
R: B

You Answered Correctly!
Puppet is a configuration management platform that AWS offers via OpsWorks but is not itself an AWS service. See Chapter 11 for more information.

-- 

# Question 37 of 39 
tb713081.AWSCSASG3E.at.32
Use V-O keys to navigate.Use V-O keys to navigate.Which of the following services can alert you to malware on an EC2 instance?


A. AWS GuardDuty
B. AWS Inspector
C. AWS Shield
D. AWS Web Application Firewall

A: A
R: A

You Answered Correctly!
GuardDuty looks for potentially malicious activity. Inspector looks for vulnerabilities that may result in compromise. Shield and Web Application Firewall protect applications from attack. See Chapter 12 for more information.

--

# Question 38 of 39 
tb713081.AWSCSASG3E.at.01
Use V-O keys to navigate.Use V-O keys to navigate.True/false: The Developer Support plan provides access to a support application programming interface (API).

A: True
R: False

You Answered Incorrectly.
The Business plan offers access to a support API, but the Developer plan does not. See Chapter 1 for more information.

( only used sdk )

-- 

# Question 39 of 39 
tb713081.AWSCSASG3E.at.28
Use V-O keys to navigate.Use V-O keys to navigate.Which ElastiCache engine can persistently store data?


A. MySQL
B. Memcached
C. MongoDB
D. Redis

A: D
R: D

You Answered Correctly!
ElastiCache supports Memcached and Redis, but only the latter can store data persistently. See Chapter 11 for more information.

--



# Yay that is done 


- Assessment Results
  - Grade: 59
- Assessment Perfomance
  - Correct: 23
  - Incorrect: 16
  - Skipped: 0
  