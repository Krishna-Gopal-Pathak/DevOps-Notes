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
