# EBS  

### What is EBS?  

Elastic Block Store(EBS) provide persistent block storage volumes for use EC2 instances in the AWS cloud. Each Amazon EBS volume is automatically  replicated within its AZ to protect you from component failure, offering high availability and durability.  

##### 5 Different Types of EBS  

**General Purpose(SSD)**  

General purpose SSD(gp2) volumes offer cost-effective storage that is ideal for a broad range of workloads. These volumes deliver single-digit millisecond latencies and the ability to burst to 3,000  IOPS for extended periods of time.

**Provisioned IOPS SSD**  

Provisioned IOPS SSD (io1) volumes are designed to meet the needs of I/O-intensive workloads, particularly  database workloads, that are sensitive to storage performance and consistency.  

**Throughput Optimized HDD**  

Throughput Optimized HDD(st1) volumes provide low-cost magnetic storage that defines performance in terms of throughput rather than IOPS. This volume type is a good fit for large, sequential workloads such Amazon EMR, ETL, data warehouses, and log processing.  

**Cold Hard Disk Drive**  

Cold Hard Disck Drive(sc1) volumes provide low-cost magnetic storage that defines performance in terms of throughput rather than IOPS. With a lower throughput limit than st1, sc1 is a good fit ideal for large, sequential cold-data workloads. If you required infrequent access to your data and are looking to save costs, sc1 provides inexpensive block storage. Bootable sc1 volumes are not supported.  

**Magnetic**  

Magnetic volumes are backed by magnetic drives and are suited for workloads where data is accessed infrequently, and scenarios where low-cost storage for small volume sizes is important. These volumes deliver approximately 100 IOPS on average, with burst capability of up to hundreds of IOPS, and they can range in size from 1GIb to 1 Tib.

##### Compare EBS types  

![EBS Types](/imgs/ebs_volume_types.png)


[Amazon EBS Volume Types](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSVolumeTypes.html#EBSVolumeTypes_standard)
