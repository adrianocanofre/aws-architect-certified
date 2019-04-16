#### Exam Tips

* Route53 is Amazon's DNS Service;   
* ELBs do not have pre-defined IPv4 addresses; you resolve to them using a DNS name;  
* Difference between an Alias Record and a CNAME;  
* Each zone contains a single SOA record;  
* Given the choice, always choose an Alias Record over a CNAME;  
* It can take up to 3 days to register depending on the circumstances;  
* Common DNS Types:  
  * SOA Records;  
  * NS Records;  
  * A Records;  
  * CNAMES;
  * MX Records;  
  * PTR Records;  
* Routing Policies:  
  * Simple Routing;  
  * Weighted Routing;  
  * Latency-based Routing;  
  * Failover Routing;  
  * Geolocation Routing;  
  * Geoproximity Routing(Traffic Flow Only);  
  * Multivalue answer Routing;  
* Health Checks:  
  * You can set health checks on individual record sets;  
  * If a record set fails a health check it will be removed from Route53 until it passes the health check;  
  * You can set SNS notifications to alert you if a health check is failed;  

[NEXT - VPC](../vpc/overview.md)
