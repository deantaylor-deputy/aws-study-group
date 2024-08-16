## 1.Placement group

**Q: What is an EC2 placement group?**

> [!note]- Answer
> An EC2 placement group is a logical grouping of instances within a single Availability Zone that influences how instances are placed on underlying hardware.

## 2. Placement group Types

**Q: What are the three types of placement groups in AWS EC2?.**

> [!note]- Answer
> The three types of placement groups are Cluster, Spread, and Partition

## 3. Placement group

**Q: Which placement group type is best for applications that need low network latency and high network throughput?**

> [!note]- Answer
> The Cluster placement group is best for applications requiring low latency and high network throughput

## 4. Placement group

**Q: What's the main benefit of a Spread placement group?**

> [!note]- Answer
> It places instances on distinct underlying hardware to reduce correlated failures.


## 5. Placement group

**Q: What is the maximum number of running instances that you can have in a single Partition placement group?**

> [!note]- Answer
> A single Partition placement group can have a maximum of 7 partitions per Availability Zone, with hundreds of EC2 instances per partition.


## 6.Elastic Network Interface

**Q: What is an ENI in AWS?**

> [!note]- Answer
> An Elastic Network Interface is a virtual network interface that you can attach to an EC2 instance.

## 7. Elastic Network Interface

**Q: Can you attach multiple ENIs to a single EC2 instance?**

> [!note]- Answer
> Yes, you can attach multiple ENIs to a single EC2 instance, depending on the instance type

## 8. Hibernation

**Q: What's the main advantage of hibernating an EC2 instance instead of stopping it?**

> [!note]- Answer
> Hibernation preserves the in-memory state (RAM) of the instance, allowing for faster startup and resumption of processes.

## 9. Public IP

**Q: What's the main advantage of hibernating an EC2 instance instead of stopping it?**

> [!note]- Answer
> When you stop an EC2 instance, it loses its public IP address. When you start the instance again, it is assigned a new public IP address. This means the public IP address of an EC2 instance can change over time.

## 8. Elastic IP

**Q: What's the main advantage of hibernating an EC2 instance instead of stopping it?**

> [!note]- Answer
> - It's static and doesn't change when you stop and start your instance.
> - You can easily remap it to another instance in case of instance failure.
> - You retain the IP address as long as you want, even if not associated with a running instance.
> - It allows for DNS stability in your applications.

