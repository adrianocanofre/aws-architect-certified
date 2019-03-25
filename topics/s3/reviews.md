# Reviews  

**S3**  

* Remember that S3 is Object Based i.e. allows you to upload files;  
* Files can be from 0 Bytes to 5TB;  
* There is unlimited storage;  
* Files are stored in Buckets;  
* S3 is a universal namespace, that is, names must be unique globally;  
* Read after Write consistency for PUTS of new Objects;  
* Eventual Consistency for overwrite PUTS and DELETES(can take some time to propagate);  
* Remember the core fundamentals of S3:
  * Key(name);
  * Value(data);
  * Version ID;
  * Metadata;  
  * ACL;
* Object based storage only(For Files);  
* Not suitable to install an operating System on;  
* Write to S3 - HTTP 200 code for a successful write;


**Storage Tiers/Classes**  

* S3 Standard: 99,99% availability, 99,9999999999% durability, stored redundantly across multiple devices in multiple facilities, and is designed to sustain the loss of 2 facilities concurrently;  
* S3 - IA (Infrequently Accessed): For data that is accessed less frequently, but requires rapid access when needed. Lower fee that S3, but you are charged  a retrieval fee;
* S3 One Zone - IA: Want a lower-cost option for infrequently accessed data, but do not require the multiple **Availability Zone** data resilience;  
* Glacier: Very cheap, but used for archival only. Expedited, Standard or Bulk. A Standard retrieval time takes 3 - 5 hours.  

**Versioning**  

* Stores all versions of an Object  
* Great backup tool;  
* Once enabled, Versioning cannot be disabled, only suspended;  
* Integrate with Lifecycle rules;  
* Versioning's MFA Delete capability, which uses MFA, can be used to provide an additional layer of security;  
* Cross Region Replication, requires versioning enabled on the source bucket;  

**LifeCycle**  

* Can be used in conjunction with versioning;  
* Can be applied to current versions and previous versions;  
* Following actions can now be done;  
  * Transition to the standard - Infrequent Access Storage Class (128Kb and 30 days after the creation date);  
  * Archive to the Glacier storage Class(30 days after IA, if relevant);
  * Permanently Delete;  

**CloudFront**  

* Edge Location - location where content will be cached;  
* Origin - Origin of all the files that the CDN will distribute;  
* Distribution - Name given CDN which consists of a collection of Edge Locations;  
  * Web Distribution - Typically used for Websites;  
  * RTMP - Use for media Streaming;
* Edge locations are not READ only;  
* Cached for the life of the TTL(Time To Live);  
* You can clear the object, but you will be charged;  

**Security**  

* By default, all newly created buckets are PRIVATE;  
* Access control to your buckets using:  
  * Bucket Policies;
  * ACL;  
* S3 buckets can be configured to create access logs which log all requests made to the s3 bucket.  

**Encryption**  

* In Transit:  
  * SSL/TLS;  
* At Rest:  
  * Server Side Encryption:
    * S3 Managed Keys - SSE-S3;
    * AWS Key Management Service, Managed Keys - SSE-KMS;  
    * Server Side Encryption with customer Provided Keys - SSE-C;  
* Client Side Encryption;  

**Storage**  

* File Gateway - For flat files, stored directly on S3;  
* Volume Gateway:  
  * Stored Volumes;
  * Cached Volumes;  
* Gateway Virtual Tape Library (VTL)  
  * Used for backup and uses popular backup applications like NetBackup, Backup Exec, Veeam...

**Snowball**  

* Snowball;  
* Snowball Edge;  
* Snowmobile;  
* Understand what Snowball is;  
* Understand what Import Export is;  
* Snowball can:
  * Import to S3;
  * Export from S3;

**Transfer Acceleration**  

* Speed up transfers to S3 using **S3 transfer acceleration**;  
* This costs extra;  
* Greatest impact on people who are in far away location;  

**S3 Static Websites**  

* You can use S3 to host static websites;  
* Serverless;  
* Very cheap, scales automatically;
* STATIC only, cannot host dynamic sites;  
