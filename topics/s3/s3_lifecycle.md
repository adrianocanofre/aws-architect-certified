# LifeCycle  



### LifeCycle Management  

* Can be used in conjunction with versioning;  
* Can be applied to current versions and previous versions;   
* S3 supports a waterfall model for transitioning between storage classes:  
  * Standard -> Standard_IA -> Intelligent_tiering -> OneZone_IA -> Glacier -> Deep_Archive;
* Following actions can now be done:
  * Transaction to the Standard - infrequent Access Storage Class(30 days after the creation date.);  
  * Archive to the Glacier Storage Class(30 days after IA, if relevant);  
  * Permanently Delete;  

[NEXT - Cross Region Replication](s3_replication.md)  
