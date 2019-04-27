# VPC  

Amazon Virtual Private Cloud(Amazon VPC) lets you provision a logically isolated section of the Amazon Web Service(AWS) Cloud where you can launch AWS resources in a virtual network that you define. You have complete control over your virtual networking  environment, including selection of your own IP address range, creation of subnets, and configuration of route tables and network gateways.  

You can easily customize the network configuration for your VPC. For example, you can create a public-facing subnet for your web servers that has access to the internet, and place your backend systems such as databases or application servers in a private-facing subnet with no internet access.  You can leverage multiple layers of security, including security groups and network access control list, to help control access to EC2 instances in each subnet.  

Additionally, you can create a Hardware Virtual Private Network(VPN) connection between your corporate datacenter and your VCP and leverage the AWS cloud as an extension of your corporate datacenter.  

![VPC](/imgs/vpc-diagram.png)  
https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html

**What can we do with a VPC?**

* Launch instances into a subnet of your choosing;  
* Assign custom IP address ranges in each subnet;  
* Configure route tables between subnets;  
* Create route tables between subnets;  
* Create internet gateway and attach it to our VPC;  
* Much better security control over your AWS resources;  
* Instance security groups;  
* Subnet network access control list (ACLS);  


**Default VPC vs Custom VPC**  

* Default VPC is user friendly, allowing you to immediately deploy instances;  
* All subnets in default VPC have a route out to the internet;  
* Each EC2 instances has both a public and private IP address;  

**VPC Peering**  

* Allows you to connect one VPC with another via a direct network route using private IP addresses;  
* Instances behave as if they were on the same private network;  
* You can peer VPC's with other AWS accounts as well as with other VPCs in the same account;  
* Peering is in a star configure: ie 1 central VPC peers with 4 others. NO TRANSITIVE PEERING;  
* You can peer between regions;  

![PEERING](/imgs/vpc-peering.png)  
https://aws.amazon.com/answers/networking/aws-multiple-region-multi-vpc-connectivity/

https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html

[NEXT - NAT](nat.md)
