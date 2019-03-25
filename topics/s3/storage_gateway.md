# Storage Gateway  

Storage gateway is a service that connects on-premises software application with cloud-based storage to provide seamless and secure integration between an organization's on-premises IT environment  and AWS storage infrastructure. The service enables you to securely store data to the AWS cloud for scalable and cost-effective storage.  

Storage Gateway's software appliance is available for download as a virtual machine (VM) image that you install on a host in your datacenter. Storage gateway support either VMware ESXI or Microsoft Hyper-V. Once you've install your gateway and associated it with your AWS account through the activation process, you can use the AWS Management Console to create the storage gateway option that is right for you.  


### Types of storage Gateway  

**File Gateway(NFS)**  
Files are stored  as objects in your S# buckets, accessed through a Network File System (NFS) mount point. Ownership, permissions, and timestamps are durably stored in S# in the user-metadata of the object associated with the file. Once objects are transferred to S3, they can be managed as native S3 objects, and bucket policies such as versioning, lifecycle management, and cross-region replication apply directly to object stored in your bucket.   

[File manage img]  

**Volumes Gateways(ISCSI)**  

The volume interface presents your application with disk volumes using the ISCSI block protocol.  

* Stored Volumes;  
  Stored volumes let you sore your primary data locally, while asynchronously backing up that data to AWS. Stored volumes provide your on-premises applications with low-latency access to their entire datasets, while providing durable, off-site backups. You can create storage volumes and mount then as ISCSI devices from your on-premises application servers.  

  [IMG]

* Cached Volumes;  
  Cached volumes let you use s3 as your primary data storage while retaining frequently accessed data locally in your storage gateway. Cached volumes minimize the need to scale your on-premises storage infrastructure, while still providing your applications with low-latency access to their frequently accessed data. You can create storage volumes up 32 TiB in size and attach to them as ISCSI devices from your on-premisse application servers.  

  [IMG]

**Tape Gateway(VTL)**  

Tape Gateway offers a durable, cost-effective solution to archive your data in the AWS Cloud.  The VTL interface it provides lets you leverage your existing tape-based backup application infrastructure to store data on virtual tape cartridges that you create on your  tape gateway. Each tape gateway is preconfigured with  a media changer and tape drives, which ate available to your existing client backup applications as ISCSI devices. You add tape cartridges as you need to archive your data. Supported by NetBackup, Backup Exec, Veeam etc.  

[IMG]  

### Tips  

* File Gateway - For flat, files, stored directly on S3;  
* Volume Gateway:  
  * Stored Volumes - Entire Dataset is stored on site and is asynchronously backup up to S3;  
  * Cached Volumes - Entire Dataset is stored on S3 and the most frequently accessed data is cached on site;  
* Gateway Virtual Tape Library(VTL):  
  * Used for backup and uses popular backup applications like NetBackup, Backup Exec, Veeam etc.  

[NEXT - Snowball](snowball.md)  
