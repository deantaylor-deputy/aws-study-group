EC2 Placement Groups:

1. Q: What is an EC2 placement group? A: An EC2 placement group is a logical grouping of instances within a single Availability Zone that influences how instances are placed on underlying hardware.
2. Q: What are the three types of placement groups in AWS EC2? A: The three types of placement groups are Cluster, Spread, and Partition.
3. Q: Which placement group type is best for applications that need low network latency and high network throughput? A: The Cluster placement group is best for applications requiring low latency and high network throughput.
4. Q: What is the maximum number of running instances that can be launched in a Spread placement group? A: A Spread placement group can have a maximum of 7 running instances per Availability Zone.
5. Q: Can you move an existing instance into a placement group? A: No, you cannot move an existing instance into a placement group. You can launch a new instance into a placement group or create an AMI from your existing instance and launch a new instance from this AMI into a placement group.

Elastic Network Interfaces (ENIs):

1. Q: What is an Elastic Network Interface (ENI)? A: An ENI is a logical networking component in a VPC that represents a virtual network card and can be attached to an EC2 instance.
2. Q: How many ENIs can be attached to a single EC2 instance? A: The number of ENIs that can be attached to an EC2 instance depends on the instance type, but it typically ranges from 2 to 15.
3. Q: Can an ENI be detached from one EC2 instance and attached to another? A: Yes, an ENI can be detached from one EC2 instance and attached to another, as long as they are in the same Availability Zone.
4. Q: What happens to an ENI when its associated EC2 instance is terminated? A: By default, when an EC2 instance is terminated, any attached ENIs created during instance launch are also deleted. However, ENIs created separately and then attached to the instance are preserved.
5. Q: Can an ENI have multiple private IP addresses? A: Yes, an ENI can have multiple private IP addresses, including a primary private IP address and one or more secondary private IP addresses.