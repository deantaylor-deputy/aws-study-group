# EC2 Fundamentals Study Guide

## 1. EC2 Basics

**Q: What is Amazon EC2 and what is its primary purpose?**

> [!note]- Answer
> Amazon EC2 (Elastic Compute Cloud) is a web service that provides resizable compute capacity in the cloud. Its primary purpose is to make web-scale cloud computing easier for developers, allowing them to quickly spin up virtual servers, configure security and networking, and manage storage.

## 2. EC2 Instance Types

**Q: Name and briefly describe the main categories of EC2 instance types.**

> [!note]- Answer
> The main categories of EC2 instance types are:
> - General Purpose: Balanced compute, memory, and networking resources
> - Compute Optimized: High-performance processors
> - Memory Optimized: Fast performance for workloads that process large data sets in memory
> - Storage Optimized: High, sequential read/write access to large data sets on local storage
> - Accelerated Computing: Hardware accelerators, or co-processors

## 3. EC2 Pricing Models

**Q: What are the different pricing models available for EC2 instances?**

> [!note]- Answer
> EC2 offers several pricing models:
> - On-Demand Instances: Pay for compute capacity by the hour or second with no long-term commitments
> - Reserved Instances: Purchase instances for a 1 or 3 year term, offering significant discount
> - Spot Instances: Bid on unused EC2 capacity, which can be significantly cheaper but may be interrupted
> - Dedicated Hosts: Physical EC2 servers dedicated for your use

## 4. EC2 and VPC

**Q: How does EC2 interact with Amazon VPC?**

> [!note]- Answer
> EC2 instances are launched into a Virtual Private Cloud (VPC). The VPC provides a logically isolated section of the AWS Cloud where you can launch AWS resources. This allows you to:
> - Control your virtual networking environment
> - Select your own IP address range
> - Create subnets
> - Configure route tables and network gateways

## 5. EC2 Security Groups

**Q: What are EC2 Security Groups and how do they work?**

> [!note]- Answer
> Security Groups act as a virtual firewall for EC2 instances to control incoming and outgoing traffic. Key points:
> - They control inbound and outbound traffic
> - You can specify allow rules, but not deny rules
> - You can assign up to 5 security groups to an instance
> - They are stateful - if you allow inbound traffic, the corresponding outbound traffic is automatically allowed

## 6. EC2 User Data

**Q: What is EC2 User Data and how is it used?**

> [!note]- Answer
> EC2 User Data is a feature that allows you to run scripts when your instance launches. It can be used to:
> - Install software or utilities
> - Download necessary files from the internet
> - Anything else that can be accomplished through a script

## 7. EC2 Instance Storage

**Q: What are the different types of storage options available for EC2 instances?**

> [!note]- Answer
> EC2 instances have several storage options:
> - Instance Store: Temporary block-level storage physically attached to the host computer
> - EBS (Elastic Block Store): Persistent block-level storage volumes
> - EFS (Elastic File System): Fully managed file storage service
> - S3 (Simple Storage Service): Object storage service, accessible from EC2 instances

## 8. EC2 Load Balancing

**Q: How does Elastic Load Balancing work with EC2?**

> [!note]- Answer
> Elastic Load Balancing automatically distributes incoming application traffic across multiple EC2 instances. It helps to:
> - Increase fault tolerance of your applications
> - Seamlessly handle varying loads of traffic
> - Improve availability and scalability of applications

## 9. EC2 Auto Scaling

**Q: What is EC2 Auto Scaling and why is it useful?**

> [!note]- Answer
> EC2 Auto Scaling helps ensure you have the correct number of EC2 instances available to handle the load for your application. It:
> - Automatically adds or removes EC2 instances according to conditions you define
> - Detects impaired EC2 instances and unhealthy applications, and replaces them
> - Provides better fault tolerance and availability

## 10. EC2 and IAM

**Q: How does IAM integrate with EC2?**

> [!note]- Answer
> IAM (Identity and Access Management) integrates with EC2 to provide:
> - Access control to EC2 resources
> - Creation of IAM roles that can be attached to EC2 instances, allowing secure access to other AWS services
> - Management of user permissions for starting, stopping, and terminating instances
> - Control over who can modify security groups, Elastic IP addresses, and other EC2 resources