# EC2 Fundamentals Study Guide

## 1. AWS Budget Setup

**Q: Why is it important to set up an AWS budget when working with EC2 instances?**

> [!note]- Answer
> Setting up an AWS budget is important when working with EC2 instances because:
> - It helps monitor and control your AWS spending
> - You can set alerts for when you're approaching your budget limits
> - It prevents unexpected charges, especially when experimenting with different instance types or forgetting to terminate unused instances

## 2. EC2 Basics

**Q: What is Amazon EC2 and what are its key features?**

> [!note]- Answer
> Amazon EC2 (Elastic Compute Cloud) is a web service that provides resizable compute capacity in the cloud. Key features include:
> - Virtual computing environments, known as instances
> - Preconfigured templates for instances, called Amazon Machine Images (AMIs)
> - Various configurations of CPU, memory, storage, and networking capacity
> - Secure login information for instances using key pairs
> - Storage volumes for temporary data, known as instance store volumes
> - Persistent storage volumes using Amazon Elastic Block Store (EBS)
> - Multiple physical locations for resources, called Regions and Availability Zones

## 3. EC2 User Data

**Q: What is EC2 User Data and how can it be used when launching an EC2 instance?**

> [!note]- Answer
> EC2 User Data is a feature that allows you to run scripts when your instance launches. It can be used to:
> - Install software or utilities
> - Download and configure applications
> - Start services
> - Perform any other initialization tasks
> For example, you could use User Data to set up a web server automatically when the instance launches.

## 4. EC2 Instance Types

**Q: What are the main categories of EC2 instance types and what are they optimized for?**

> [!note]- Answer
> The main categories of EC2 instance types are:
> - General Purpose (e.g., T3, M5): Balanced compute, memory, and networking resources
> - Compute Optimized (e.g., C5): High-performance processors
> - Memory Optimized (e.g., R5): Fast performance for workloads that process large data sets in memory
> - Storage Optimized (e.g., I3, D2): High, sequential read/write access to large data sets on local storage
> - Accelerated Computing (e.g., P3, G4): Hardware accelerators, or co-processors

## 5. Security Groups

**Q: What are EC2 Security Groups and how do they function?**

> [!note]- Answer
> EC2 Security Groups act as a virtual firewall for EC2 instances. Key points:
> - They control inbound and outbound traffic
> - You can specify allow rules, but not deny rules
> - They are stateful - if you allow inbound traffic, the corresponding outbound traffic is automatically allowed
> - You can assign multiple security groups to an instance
> - Security groups are specific to a VPC

## 6. SSH Overview

**Q: What is SSH and why is it important for EC2 instances?**

> [!note]- Answer
> SSH (Secure Shell) is a protocol used to securely connect to EC2 instances. It's important because:
> - It provides a secure way to access your EC2 instances remotely
> - It allows you to run commands on your EC2 instances as if you were directly on the machine
> - It's the primary way to access Linux instances
> - For Windows instances, SSH can be used alongside or as an alternative to RDP (Remote Desktop Protocol)

## 7. EC2 Instance Connect

**Q: What is EC2 Instance Connect and how does it differ from traditional SSH?**

> [!note]- Answer
> EC2 Instance Connect is a simple and secure way to connect to your EC2 instances using Secure Shell (SSH):
> - It provides a browser-based SSH connection
> - No need to manage SSH keys locally
> - Uses AWS IAM policies for authentication
> - Works seamlessly with Amazon Linux 2 instances
> - Doesn't require opening inbound ports for SSH access

## 8. EC2 Instance Roles

**Q: What are EC2 Instance Roles and why are they useful?**

> [!note]- Answer
> EC2 Instance Roles are IAM roles that you can attach to EC2 instances. They are useful because:
> - They provide temporary security credentials to applications running on an EC2 instance
> - They eliminate the need to store AWS credentials in the instance
> - They are more secure than storing access keys on instances
> - They make it easier to manage permissions for applications on EC2 instances

## 9. EC2 Instance Purchasing Options

**Q: What are the main EC2 instance purchasing options?**

> [!note]- Answer
> The main EC2 instance purchasing options are:
> - On-Demand Instances: Pay for compute capacity by the second with no long-term commitments
> - Reserved Instances: Purchase instances for a 1 or 3 year term, offering significant discount
> - Savings Plans: Commit to a consistent amount of usage (measured in $/hour) for a 1 or 3 year term
> - Spot Instances: Bid on unused EC2 capacity, which can be significantly cheaper but may be interrupted
> - Dedicated Hosts: Physical EC2 servers dedicated for your use

## 10. Spot Instances & Spot Fleet

**Q: What are Spot Instances and Spot Fleet, and when would you use them?**

> [!note]- Answer
> Spot Instances are unused EC2 capacity that AWS sells at a discounted rate. Spot Fleet is a collection of Spot Instances and optionally On-Demand Instances.
> 
> You would use them:
> - For flexible start and end times
> - For applications feasible only at very low compute prices
> - For urgent need of large amounts of additional computing capacity
> - Spot Fleet helps you optimize for capacity or cost and automatically request resources across instance types to meet your needs