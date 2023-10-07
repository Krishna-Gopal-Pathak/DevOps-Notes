## AWS Auto Scaling
- AWS Auto scaling is a service that monitors the application and automatically adds or remove compute resources depending on the actual uses or demand.
- AWS Auto Scaling uses Cloudwatch to monitor the application and raise alarm to scale up or down resources depending on application needs.
- EC2 Auto Scaling Group uses health check replacement and scaling policies.<br/>
**EC2 Auto Scaling Group**
- EC2 Auto Scaling Group maintains the instances and scales automatically.
  - Minimum Size [1]
  - Desired Capacity Size [2]
  - Maximum Size [4]<br/>

**EC2 Auto Scaling Policies / Types of Scaling Policies**
- Manual Scaling Policies
- Dynamic Scaling Policies
- Schedule Scaling Policies
- Predictive Scaling Policies

## Elastic Load Balancer:
- Routes incoming application traffic across instances automatically.<br/>

**Elastic Load Balancer Support Four Load Balancer:**
- Application Load Balancer
- Network Load Balancer 
- Classic Load Balancer
- Gateway Load Balancer

## Launch Configuration
- Launch Configuration is an instance configuration template in which we define configuration of an EC2 instance.
- AMI, Instance Type, Key Pair, IAM Role, Security Group.
- Launch Configuration is not editable.

## Launch Template
- Launch Template is similar to Launch Configuration.
- Create multiple version of Launch Template.

## EC2
- Elastic Compute Cloud
- EC2 provides secure, resizable compute in the cloud offering broadest choice of processor, storage, networking, OS and purchase model.

**Virtual Machine**
- Virtual Machine is the virtual environment that works like a computer within computer.


## Elements of EC2
**Instance:** <br/>
- Instance is an EC2 virtual machine.<br/>

**AMI:** <br/>
- Amazon machine image contain operating system and additional software needed to launch EC2 instance.<br/>

**Key Pair:** <br/>
- Helps to connect to your EC2 instances.<br/>
- Consist of Public key and Private Key.<br/>

**Security Group:** <br/>
- Security Group acts as a virtual firewall for EC2 instances to control inbound and outbound traffic.<br/>
 
**EC2 Tags** <br/>
- Tag is a label<br/>
- Consist of key and value<br/>
- Must be unique<br/>

**Inbound**<br/>
- Inbound means who can configure to your EC2 instances from outside<br/>

**Outbound** <br/>
- Outbound means what your EC2 instance can connect with.<br/>


**Instance Type**<br/>
- General Purpose Instance<br/>
- Compute Purpose Instance<br/>
- Memory Purpose Instance<br/>
- Storage Purpose Instance<br/>


**Subnet**<br/>
- Subnet is a range of IP address in your VPC.<br/>
- You need to provide at least two subnet to create VPC connection.<br/>
- Each subnet must belong to different availability zone.<br/>


**Public Subnet**<br/>
- It is a subnet that interact with internet and can be accessed through the internet.<br/>

**Private Subnet**<br/>
- It is a subnet that can not be reached from Internet.<br/>
- We can create AWS resources which are only used inside VPC for internal purpose.<br/>

**Internet Gateway**<br/>
- Acts as a gateway b/w VPC and Internet.

## Availability
- How long system is operational and able to deliver data upon request.

## Durability
- Data should not be lost or corrupted in long run.


## CDN in AWS
- Amazon cloudfront is a content delivery network service that speeds up the delivery of web content, images, videos and application by caching them in edge location.

## Caching 
- Store a copy of data in temporary or cache storage location so it can be accessed more quickly.

## IAM
- Identity Access Management.
- Ensure that right person has access to the right service or resources.

## Identity
- Identity is the ability to identify a unique user.

## Authentication
- Authentication is the process of recognizing a user's identity.

## Authorization
- Authorization is the process of giving someone the permission to access something



## IAM Policy
- IAM policy is an entity, when attached to identity and resources defines its permission.

## Types of IAM Policy
- Identity-Based Policy
  - AWS Managed Policy
  - Customer Managed Policy
- Resourced-Based Policy
- Inline Policy


## IAM Role
- IAM Role is like an IAM User attached with an IAM Policy that determines what a role can and cannot do in AWS.


## IAM Group
- IAM Group is a collection User and permission assigned to those user.
- For Example: You have a user group called Admin and give that group administrator permission. Any user in that group automatically has Admin group permission.


## IAM User
- IAM user is an identity within your AWS account that has specific permission for a single person or application.
- These permission define what user can do in AWS.
- IAM user can be used to grant access to AWS resources to people or resources.


## S3
- Simple Storage Service
- Allows to store,retreive,access, and backup any amount of data at any time from anywhere over the internet.


