# Exam Tips

#### EC2 Tips  

* Termination Protection is turned off by default, you must turn it on;  
* On an EBS-backed instance, the **default action is for the root EBS volume to be deleted** when the instance is terminated;  
* EBS root volumes of your DEFAULT AMI's cannot be encrypted. You can also use a third party tool(such as bit locker etc) to encrypted the root volume, or this can be done when creating AMI's(lab to follow) in the AWS console or using the API;  
* Additional volumes can be encrypted;  


#### Security Group  

* All inbound traffic is blocked by default;  
* All Outbound traffic is allowed;  
* Changes to Security Groups take effect immediately;  
* You can have any number of EC2 instances within a security group;  
* You can have multiple security groups attached to EC2 Instances;  
* Security Groups are **STATEFUL**;  
* If you create an inbound rule allowing traffic in, that traffic is automatically allowed back out again;  
* You cannot block specific IP addresses using Security Groups, instead use Network Access Control List;  
* You can specify allow rules, but not deny rules;


#### Snapshots  

* Volumes exist on EBS. Think of EBS as a virtual hard disk;  
* Snapshots exist on S3. Think of snapshots as a photograph of the disk;  
* Snapshots are point in time copies of volumes;  
* Snapshots are incremental, this means that only the blocks that have changed since your last snapshot are moved to S3;   
* If this is your first snapshot, it may take some time to create;  
* To create a snapshot for EBS volumes, that serve as root devices, you should stop the instance before talking the snapshot;  
* However  you can take a snap while instances is running;  
* You can create AMI's from both Volumes and Snapshots;  
* You can change EBS volumes sizes on the fly, including changing the size and storage type;  
* Volumes will ALWAYS be in the same availability zone as the EC2 instance;  
* To move an EC2 volume from one AZ to another, take a snapshot of it, create an AMI from the snapshot and then use the AMI to launch the EC2 instance in a new AZ;  
* To move an EC2 volume from one region to another, take a snapshot of it create an AMI from the snapshot and then copy the AMI from on region to the other. Then use the copied AMI to launch the new EC2 instance in the new region;

#### IAM  

* Instance Store Volumes are sometimes called Ephemeral Storage;  
* Instance store volumes cannot be stopped. If the underlying host fails, you will lose your data;  
* EBS backed instances can be stopped. You will not lose the data on this instance if it is stopped;  
* You can reboot both, you will not lose your data;  
* By default, both ROOT volumes will be deleted on termination. However, with EBS volumes, you can tell AWS to keep the root device volume;


#### CloudWatch  

* CloudWatch is used for monitoring performance;  
* CloudWatch can monitor most of AWS as well as your applications that run on AWS;  
* CloudWatch with EC2 will monitor events every 5 minutes by default;  
* You can have 1 minute intervals by turning on detailed monitoring;  
* You can create CloudWatch alarms which trigger notifications;  
* CloudWatch monitors performance;  
* CloudTrail is all about auditing, monitor API call in the AWS platform;  
* Standard Monitoring = 5 minutes;  
* Detailed Monitoring  = 1 minute;

**What can I do with CloudWatch?**   

* Dashboard - Create awesome  dashboard to see what is happening with your AWS environment;  
* Alarms - Allows you to set Alarms that notify you when particular thresholds are hit;  
* Events - CloudWatch Events helps you to respond to state changes in your AWS resources;  
* Logs - CloudWatch logs helps you to aggregate, monitor, and store logs;  
