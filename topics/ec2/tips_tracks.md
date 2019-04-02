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
