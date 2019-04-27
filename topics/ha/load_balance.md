# Load Balance  



**Types**  

* Application Load Balance  
> Are best suited for load balancing of HTTP/HTTPS traffic. They operate at layer 7 and are application-awerw. They are intelligent, and you can create advanced request routing, sending specified requests to specific web servers.  

* Network Load Balance  
> are the best suited for load balancing of TCP port traffic where extreme performance is required. Operating at the connection level (Layer 4), Network Load Balance are capable of handling millions of requests per second, while maintaining ultra-low latencies. Use for extreme performance.  

* Classic Load Balance  
> Are the legacy ELB. You can load Balance HTTP/HTTPS applications and use Layer 7-specific features, such as X-Forwarded and sticky sessions. You can also use strict Layer 4 load Balancing for applications that rely purely on the TCP protocol.




###  Sticky Sessions   

Classic load Balancer routes each request independently to the registered EC2 instance. This ensures that all requests from the user during the session are sent to the same instance.  
You can enable Sticky Sessions form Application Load Balancers as well, but the traffic will be sent to at the Target Group Level.  


No Cross Zone Load Balance  
![VPC](/imgs/no-cross.png)  
https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/how-elastic-load-balancing-works.html

With Cross Zone Load Balance  
![VPC](/with/no-cross.png)  
https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/how-elastic-load-balancing-works.html

**What are path Patterns??**  

You can create a listener with rules to forward requests based on the URL path. This is know as path-base routing. If you are running micro services, you can route traffic to multiple back-end services using path-based routing. For example, you can route general requests to one target  group and requests to render images to another target group.  



links:  
https://docs.aws.amazon.com/elasticloadbalancing/latest/classic/elb-backend-instances.html  

https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/what-is-load-balancing.html  
