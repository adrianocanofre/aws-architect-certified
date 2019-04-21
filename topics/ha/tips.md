# HA Architecture  


### ELB  

* 3 different Types:  
  * Application Load Balancers;  
  * Classic Load Balancers;  
  * Network Load Balancers:  
* 504 Error means the gateway has timed out(app not responding within idle timeout period);  
* if you need the IPv4 address of your end user, look for the X-Forwarded-For header;   
* Instances monitored by ELB are reported as, **inService** or **OutofService**;  
* Health Checks check the instance health by talking to it;  
* Load Balance ha their own DNS name. You are never given an IP address;  
* Sticky Sessions enable your users to stick to the same EC2 instances. Can be useful if you are storing information locally to that instance;  
* Cross Zone Load Balance enables you to load balance across multiple availability zones;  
* Path patters allow you to direct traffic to different EC2 instances based on the URL contained in the requests;


### CloudFormation  

* Is a way to completely scripting your cloud environment;  
* Quick start is a bunch of CloudFormation templates already built by AWS Solutions Architects allowing you to create complex environment very quickly;  

### Elastic Beanstalk  

With Elastic Beanstalk , you can quickly deploy and manage application in the  AWS cloud without worrying about the infrastructure that runs those applications. You simply upload your application, and elastic Beanstalk automatically handles the details of capacity provisioning, ELB, autoscaling, and application health monitoring.

### Others  

* Use multiple AZ's and Multiple Regions where ever you can;  
* Know the difference between Multi-AZ and Read Replications for RDS;  
* Know the difference between scaling out and scaling up;  




https://d1.awsstatic.com/whitepapers/architecture/AWS-Operational-Excellence-Pillar.pdf  
https://d1.awsstatic.com/whitepapers/AWS_Cloud_Best_Practices.pdf
