# Bucket  

A bucket is owned by the AWS account that created it. By default, you can create up to 100 buckets in each of your AWS accounts. If you need additional buckets, you can increase your account bucket limit to a maximum of 1,000 buckets by submitting a service limit increase.  

Bucket ownership is not transferable; however, if a bucket is empty, you can delete it. After a bucket is deleted, the name becomes available to reuse, but the name might not be available for you to reuse for various reasons.


### Rules  

* After you create an S3 bucket, you can't change the bucket name, so choose the name wisely;  
* Bucket names:
  * Unique across S3;
  * East 3 and no more than 63 characters long;  
  * Not be formatted as an IP address;

[NEXT - S3 Version Control](s3_versioning.md)  
