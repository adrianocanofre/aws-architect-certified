# Security & Encryption  


### Security  

* By default, all newly created buckets are **PRIVATE**;  
* You can setup access controll to your buckets using:
  * Bucket Policies;
  * ACL(Acces Control List);
* S3 buckets can be configured to create access logs which log all requests made to the S3 bucket. This can be done to another bucket;  

### Encryption  

* In transit:  
  * SSL/TLS;  
* At Rest:  
  * Server Side Encryption:  
    * S3 Managed Keys - **SSE-S3**;
    * Aws Key Management Service, Managed Keys - **SSE-KMS**;  
    * Server Side Encryption with Customer Provided Keys - **SSE-C**;  
* Client Side Encryption;  


[NEXT - S3 Version Control](s3_versioning.md)  
