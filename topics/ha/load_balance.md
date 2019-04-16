# Load Balance  



**Types**  

* Application Load Balance  
> Are best suited for load balancing of HTTP/HTTPS traffic. They operate at layer 7 and are application-awerw. They are intelligent, and you can create advanced request routing, sending specified requests to specific web servers.  

* Network Load Balance  
> are the best suited for load balancing of TCP port traffic where extreme performance is required. Operating at the connection level (Layer 4), Network Load Balance are capable of handling millions of requests per second, while maintaining ultra-low latencies. Use for extreme performance.  

* Classic Load Balance  
> Are the legacy ELB. You can load Balance HTTP/HTTPS applications and use Layer 7-specific features, such as X-Forwarded and sticky sessions. You can also use strict Layer 4 load Balancing for applications that rely purely on the TCP protocol.
