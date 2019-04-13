# Aurora  

Amazon Aurora is a MySQl - Compatible, relation database engine that combines the speed and availability of high-end commercial databases with  the simplicity and cost-effectiveness of open source databases. Aurora  provides up to five times better performance than MySQL at a price point one tenth that of a commercial database while delivering similar performance and availability.  

About Aurora:  
* Start with 10GB, scales in 10GB increments to 64TB(storage Autoscaling);  
* Compute resources can scale up to 32vCPUs and 244GB of Memory;  
* 2 copies of your data is contained in each availability zine, with minimum of 3 availability zones. 6 copies of your data;  

### Scaling Aurora  

* Aurora is designed to transparently handle the loss of up to two copies of data without affecting database write availability and up to three copies without affecting read availability;  
* Aurora storage is also self-healing. Data blocks and disks are continuously scanned for errors and repaired automatically;  


### Types of Aurora Replicas  

* Aurora Replicas (currently 15);
* MySQL Read Replicas (currently 5);  

[IMG]


### Backups With Aurora  

* Automated backups are always enabled on Amazon Aurora DB Instances. Backups do not impact database performance;  
* You can also take snapshots with Aurora. This also does not impact on performance;  
* You can share Aurora Snapshots with other AWS accounts;  
