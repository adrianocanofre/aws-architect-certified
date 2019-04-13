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
