# Tips and Tracks  

* Readshift for Business Intelligence or Data Warehousing;  
* ElastiCache to speed up performance of existing databases(frequent identical queries);  
* RDS runs on virtual machines;  
* You cannot log in to these operating systems however;  
* RDS is not serverless;  
* Patching of the RDS Operating System and DB is Amazon's responsability;  
* Aurora Serverless is Serverless;  



### DynamoDB  

* Stored on SSD storage;  
* Spread across 3 geographically distinct datacenter;  
* Eventual Consistent Reads (default);
* Strongly  Consistent Reads;


### Redshift  

* Redshitf is used for business intelligence;  
* Available in only 1 AZ;  

### Backups  

* Enabled by default with a 1 day retention period;  
* Maximum retention period is 35 days;  
* Redshift always attempts to maintain at least three copies of your data (the original and replica on the compute nodes and a backups in Amazon S3);  
* Redshift can also asynchronously replicate your snapshots to S3 in another region for disaster recovery;  

### Aurora  

* 2 copies of your data is contained in each availability zone, with minimum of 3 availability zines. 6 copies of your data;  
* You can share Aurora Snapshots with other AWS accounts;  
* 2 types of replicas available. Aurora Replicas and MySQL replicas. Automated failover is only available with Aurora Replicas;  
* Aurora has automated backups turned on by default. You can also takes snapshots with Aurora. You can share these snapshots with other AWS accounts;  
