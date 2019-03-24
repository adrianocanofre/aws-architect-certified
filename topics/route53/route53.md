# Route53

## DNS 101

#### SOA(Start Of Authority)  
* The name  of the server that supplied the data for the zone;
* The admin of the zone;
* The current version of the data file;
* The default number of seconds for the time-to-live file on resource records;  

#### NS(Name Server)

NS stands for Name Server records. They are used by Top Level Domain servers to direct traffic to the Content DNS server which contains the authoritative DNS records.  

#### A (Address)  

The A record is used by a computer to translate the name of the domain to an IP address.  
Ex:  
> www.acloud.guro might pointo to 123.10.10.80

#### TTL  

The length that a DNS record is cached on either the Resolving Server or the users own local PC is equal to the value og th "time-to-live" in seconds.  

#### CNames( Canonical Name)  

A CNames can be used to resolve one domain name to another.  
Ex:  
> n.adrianocanofre.dev to mobile.adrianocanofre.dev

### Alias Records  

Alias records are used to map resource record sets in your hosted Zone to Elastic Load Balancers, CloudFront distrivutions, or s3 buckets that are configured as websites.  


#### Exam Tips

* ELBs do not have pre-defined IPv4 addresses; you resolve to them using a DNS name;  
* Difference between an Alias Record and a CNAME;  
* Each zone contains a single SOA record;  

## Routing Policies Available On AWS  

* Simple Routing  
* Weighted Routing  
* Latency-based Routing  
* Failover Routing
* Geolocation Routing
* Multivalue Answer Routing