# Routing Policy  

### Simple Route Policy  

This is the default routing policy when you create a new record set. this is most commonly used when you have a single resource that performs a given function for your domain.  

### Weighted Routing  

Weighted routing lets you associate multiple resources with a single domain name or subdomain name and choose how much traffic is routed to each resource. This can be useful for a variety of purposes, including load balancing and testing new versions of software.  

### Latency Routing  

Latency based routing allows you to route your traffic based on the lowest network latency for your end user. To use latency-based routing, you create a latency resource record set for the Amazon EC2(or ELB) resource in each region that host your website.  

### Failover Routing  

Failover routing policy are used when you want to create an active/passive set up. For exemple, you may want your primary site to be in EU-WEST-2 and your secondary  DR site in AP-SOUTHEAST-2.  
Route53 will monitor the health of your primary site using health check.  
A health check monitors the health of your end points.  

### Geolocation Routing  

Geolocation routing lets you choose where your traffic will be sent based on the geographic location of your users (ie the location from which DNS queries originate). For example, you might want all queries from Europe to be routed to an ELB load balancer in the Frankfurt region.   


###  Multivalue Answer Routing   

Multivalue answer routing lets you configure Route53 to return multiple values, such as IP addresses for your web servers, in response to DNS queries. You can specify multiple values for almost any record, but multivalue answer routing also lets you check the health of each resource, so Route 53 returns only values for healthy resources.  
This is similar to simple routing however it allows you to put **health checks** on each record set.   

[More information about policies](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html)
