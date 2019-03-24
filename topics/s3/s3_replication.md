# S3 Replication  

**What Does Amazon S3 Replicate?**  

Amazon s3 replicated only specific items in buckets that are configured for cross-region replication.  

### Tips  

* Versioning must be enabled on both the source and destination buckets;  
* Regions must be unique;  
* Files in an existing bucket are not replicated automatically. All subsequent updated files will be replicated automatically;  
* You cannot replicate to multiple buckets or use daisy chaning(at this time);  
* Delete markers are NOT replicated;  
* Deleting individual versions or delete markers will not be replicated;  
* Understand what Cross Region Replication is at a High Level;

[Replication rules](https://docs.aws.amazon.com/AmazonS3/latest/dev/crr-what-is-isnot-replicated.html)  
[CRR Monitor](https://aws.amazon.com/solutions/cross-region-replication-monitor/)  
[Region Codes](https://docs.aws.amazon.com/general/latest/gr/rande.html#s3_region)  
[CRR Configuration](https://docs.aws.amazon.com/AmazonS3/latest/dev/crr-add-config.html)  
[Lab]()
