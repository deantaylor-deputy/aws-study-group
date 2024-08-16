

## 1. Public IP
> [!note]- Key Points
> - **Internet Access**: Allows instances to be reachable from the internet.
> - **Elastic IPs**: Static IPs that remain consistent across instance stops/starts.
> - **Assigned Automatically/Manually**: Can be automatically assigned or manually set with Elastic IPs.

## 2. Private IP
> [!note]- Key Points
> - **Internal Communication**: Used for communication within the VPC and not accessible from the internet.
> - **Stable within VPC**: Remain the same when instances are stopped and started within the VPC.

## 3.Placement group
> [!note]- Key Points
> Placement groups enhance performance, fault tolerance, and availability by controlling instance placement within AWS
> - **Cluster Placement Group**: Groups instances for low-latency, high-performance computing in a single Availability Zone.
> - **Partition Placement Group**: Spreads instances across partitions to improve fault tolerance and handle hardware failures.
> - **Spread Placement Group**: Distributes instances across distinct hardware to reduce the risk of correlated failures.

## 4. Elastic Network Interface
> [!note]- Key Points
> - **Additional Network Interfaces**: Allows multiple network interfaces per instance.
> - **Private/Public IPs**: Supports multiple private IPs and can be associated with public IPs.
> - **Security Groups**: Can be associated with one or more security groups.tolerance and handle hardware failures.
> - **Elastic IPs**: Can attach Elastic IPs for a static public IP address
> - **Persistence**: Can be detached and reattached to different instances, preserving network settings


## 5. Hibernate mode
> [!note]- Key Points
> - EC2 hibernation's key point is cost-saving while preserving instance state. It saves RAM to EBS, allowing quick resumption of work without paying for stopped compute time, only for storage.