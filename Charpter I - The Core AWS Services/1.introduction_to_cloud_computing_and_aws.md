# Disclaimer

- Cloud is where technology innovation and growth happens. In this way this charper aims to introduce what is a cloud and how Amazon end of it works.
- This charpter will explore the basics:
  - That makes cloud computing different from other applications and client-server models
  - How the AWS platform provides secure and flexible virtual networked environments for your resources
  - How AWS provides such a high level of service reliability
  - How to access and manager your AWS-based resources
  - Where you can go for documentation and help with your AWS deployments

# Cloud computing and virtualization 

- Virtualization: thats the technology that lies at the core of all cloud operations.
- It lets you achieve the greatest value from a hardware.
- Cloud is  scalable, elastic and often cheap. 


## Scalability

- Scalable infrastructures can efficiently meet unexpected increases in demand by automatically adding resources. 
- This often means increase the number of running instances (virtual machines).

## Elasticity

- In the same way, you can scale down your infrastructure to meet low demand periods. Thats called elasticity.

## Cost Management

- The main pillar of cloud cost efficiency is the possibility to pay-on-demand instead having a fixed bill whenever you need to launch a new server. 
- This doenst guarantee that you will pay less everytime, but is definitely a more accurate way to manage your costs.
- Besides, once the need of scaling comes up, AWS can do that in a matter of minutes.
- The AWS TCO Calculator, provides a way to calculate the cost of your local infrastrucutre if they were aws services.

# The AWS Cloud

- As a Solutions Architect you will need to know all the core AWS services for the main categories, that are:
    - Cloud Computing
    - Networking
    - Storage
    - Database
    - Application Management
    - Security and Identity
    - Application Integration

## The core services by category: 


### Cloud Computing

- Elastic Compute Cloud (EC2): 
  - Ec2 Server inst ances provide virtual versions of the server you would run in your local data center.
  Ec2 instances can be provisioned with the CPU, memory, storage, and network interface profile to meet any
  application need, from a simple wb server to onme part of a cluster of instances providing an integrated multi=tiered
  fleed architecture. Since EC2 instances are virtual, they're resource-efficient and deploy nerly instantly.

- Lambda: 
  - Serveless application architectures like the one provided by Amazon's lambda service allow you to provide
  responsive public-facing services without the need for a server that's acctually running 24/7.
  Instead, network events, like consumer requests, can trigger the executio of a predefined cvode-based operation. 
  When the operation (wich can currently run for as long as 15 minutes) is complete, the Lambda event ends,
  and all resources automatically shut dowm.

- Auto Scaling:
  - Copies of running EC2 instances can be defined as image templates and automatically launched ( or scaled up ) when
  client demand can't be met by existing instances. As demaned drops, unused instances can be terminated ( or scaled down ).

- Elastic Load Balancing:
  - A load balancer is a network service that distributes traffic to multiple instances to do not overhealm a single web server.
  It can be used to provide high availability and scalability for your application. It can also be used to provide
  failover capability for your application.

- Elastic Beanstalk: 
  - A web application platform that provides a simple, cost-effective way to deploy, manage, and scale web applications.
  - It is a tool that automates the deployment of applications to Amazon's Elastic Compute Cloud (EC2) and Amazon's
  Elastic Load Balancing (ELB) services. (by copilot)
  - Beanstalk is a managed service that abstracts the provisioning of AWS compute and networking infra. You are required
  to do nothing more than pushing your application code , and Beanstalk automatically launches and manages
  all the necessary services in the background.


### Networking

- Virtual Private Cloud (VPC):
  - VPC's are highly configurable networking environments designed to host your EC2 (and RDS) instances. 
  You use VPC-based tools to secure and, if desired, isolate your instances by closely controlling inbound and
  outbound network access.

- Direct Connect: 
  - By purchasing fast and secure network connections to AWS through a third-party provider, you can use Direct
  Connect to establish an enhcnaced direct tunnel between your local data center or office and your AWS-based VPCs.

- Route 53: 
  - Its the AWS DNS service that lets you manage domain registration, record administration, routing protocols and health checks,
  which are all fully integrated with the rest of your AWS resources. 

- Cloud Front
  - Its the Amazon's distributed global content delivery network (CDN). When properly configured, a CloudFront distribution
  can store cached versions of your site's content at edge locations arount the world so that they can be delivered
  to customers on request with the gratest efficiency and lowest latency.


### Storage

- Simple Storage Service (S3):
  - S3 offers highly versatile, reliable, and inexpensive object sotrage that's great for data storage and backups.
  Its also commoly used as part of larger AWS production processes, including through the storage of script, teamplate, and log files.


- S3 Glacier:
  - A foog choice for when you need large data archives stored ceaply over the long term and can live with 
  retrieval delays measuring in the hours. Glacier's lifecycle management is closely integrated with S3.

- Elastic Block Store (EBS):
  - Ebs provides the persistent `virtual storage drivers` that host the operating system and working data of an EC2 instance.
  They're meant to mimic the function of the storage drivers and partitions attached to physical servers.

- Storage Gateway: 
  - It's the hybrid storage system that expose AWS cloud storage as a local, on-premises appliance. Storage gateway can be a great 
  tool for migration and data backup and as a part of disaster recovery operations.


### Database

- Relational Database Service (RDS)
  - RDS is a managed service that builds you a stable, secure and reliable database instance. You can run a variety of SQl 
  database engines on RDS, including MySQL, Microsoft SQL Server, Oracle, and Amazon's own Aurora. 

- DynamoDB:
  - It can be used for fast, flexible, highly scalable and managed nonrelations (NoSQL) database workloads


### Application Management 

- CloudWatch:
  - It can be set to monitor process performance and resource utilization and, whjen preset thresholds are met, either 
  send you a message or trigger an automated response. 

- CloudFormation:
  - This service enables you to use template files to define full and complex AWS deployments. The ability to script your use
  of any AWS resources makes it easier to automate, standardizing and speeding up the application launch process. 

- CloudTrail: 
  - It collects records of all your account's API events. This history is useful for account auditing and troubleshooting purposes. 

- Config
  - The Config service is designed to help you with change management and compliance for your AWS account. You first define a desired
  configuration state, and Config evaluates any future states against that ideal. When a configuration change ushes too far from
  the ideal baseline, you will be notified. 


### Security and Identity

- Identity and Access Management (IAM):
  - You use IAM to administrate user and programmatic access and authentication to your AWS account. Through the use of users,
  groups, roles, and policies, you can controll exactly who and what can access and/or work with any of your AWS resources.

- Key Management Service (KMS)
  - KMS is a managed service that allows you to administrate the creation and use of encryption keys to secure data used by and for any
  of your AWS resources.

- Directory Service:
  - For AWS environments that need to manage identities and relationships, Directory Service can integrate AWS resources with identity
  providers like Amazon Cognito and Microsoft AD domains.


### Application Integration

- Simple Notification Service (SNS):
  - Is a notification tool that can automate the publishing of alert topics to other services (to an SQS Queue or to trigger a Lambda function,
  for instance), to mobile devices or to recipients using email or SMS.

- Simple Workflow: 
  - Lets you coordinate a series of tasks that must be performed using a range of AWS services or even non-digital (meaning human) events.

- Simple Queue Service (SQS): 
  - Allows for event-driven messaging withing distributed systems that can decouple while coordinating the discrete steps of a larger process. 
  The data contained in your SQS messages will be reliably delivered, adding to the fault-tolerant qualities of an application.

- API Gateway:
  - This service enables you to create and manage secure and reliable APIs for your AWS-based applications


# AWS Platform Architecture

- AWS physical server are distributed along 21 gelocations that allow you to launch your applications geographically close to your end users. 
There ar 21 regions, besides the US government regions. Note that China regions requires specific protocols to access and authenticate. 









 
