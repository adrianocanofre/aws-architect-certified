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

A CNames can be used to resolve one domain name to another. A CNAME record assigns an Alias name to a Canonical Name.  
Ex:  
> n.adrianocanofre.dev to mobile.adrianocanofre.dev

### Alias Records  

Alias records are used to map resource record sets in your hosted Zone to Elastic Load Balancers, CloudFront distributions, or s3 buckets that are configured as websites.   
Alias Records provide a Route 53–specific extension to DNS functionality


## Routing Policies Available On AWS  

* Simple Routing  
* Weighted Routing  
* Latency-based Routing  
* Failover Routing
* Geolocation Routing
* Multivalue Answer Routing  

[More information about DNS record types](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/ResourceRecordTypes.html)


[NEXT - Routing Policies](policies.md)
