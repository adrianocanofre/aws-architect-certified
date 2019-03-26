# Tips&Tracks  

**Basic S3**  
* It is Object-based storage;  
* Files can be from 0 Bytes to 5 TB;  
* There is unlimited storage;
* Files are stored in Buckets(Buckets are folder inside the cloud);  
* S3 is a universal namespace. That is, names must be unique globally;  
* Read after write consistency for PUTS of new Objects;
* Eventual consistency for overwrite PUTS and DELETS(can take some time to propagate);  
* Object-based storage only (for files.);  
* Not suitable to install an operating system on.  
* When you upload a file to S3, you will receive a HTTP 200 code if the upload was successful;
* BY DEFAULT BUCKETS ARE PRIVATE AND ALL OBJECTS STORED INSIDE THEM ARE PRIVATE;
* You can turn on MFA Delete;  
* S3 Storage Classes/Tiers:  
  * S3 - durable, immediately available, frequently accessed;  
  * S3 IA - durable, immediately available, infrequently accessed;  
  * S3 One Zone IA - Even cheaper than IA, but only in one AZ(Availability Zone);  
  * Glacier - Archived data, where you can wait 3 - 5 hours before accessing;  
* S3 is A Simple Key-value Store;  
  * Key;  
  * Value;  
  * Version ID ;  
  * Metadata;  
  * Subresources:  
    * ACL;  
    * torrent;
