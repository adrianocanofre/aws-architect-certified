# AMI's  

An Amazon Machine Image (AMI) provides the information required to launch an instance. You must specify an AMI when you launch an instance. You can launch multiple instances from a single AMI when you need multiple instances with the same configuration. You can use different AMIs to launch instances when you need instances with different configurations.

**You can select your AMI based on:**  
* Region;  
* Operating System;  
* Architecture;  
* Launch Permissions;  
* Storage for the root device:  
  * Instance Store (EPHEMERAL STORAGE);  
  * EBS backed Volumes;  


### EBS vs Instances Sore Volumes  

All AMIs are categorized as either backed by  Amazon EBS or backed by instance store.  

For EBS: The root device for an instance launched from the AMI is an EBS volume created from an EBS snapshot.  

For Instance Store Volumes: The root device for an instance launched from the AMI is an instance store volume created from a template stored in S3.

[NEXT - Encrypted Device](encrypted_device.md)
