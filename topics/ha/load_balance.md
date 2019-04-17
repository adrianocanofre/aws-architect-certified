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
[IMG]

With Cross Zone Load Balance  
[IMG]  


**What are path Patterns??**  

You can create a listener with rules to forward requests based on the URL path. This is know as path-base routing. If you are running microservices, you can route traffic to multiple beack-end services using path-based routing. For example, you can route general requests to one target  group and requests to render images to another target group.  

[IMG]


links:  
https://media.acloud.guru/aws-csa-2019/resource/05893768-d54d-ed3e-e69c-12be5814f3a2_6984f437-52a4-2585-eede-8fa8a5673fd0/aws-csa-2019-cc5ba723-e554-4b5e-8473-bae48d8d2375.pdf?Expires=1555638421&Signature=FalDq4xfhQfvRKg3fYSOaJlJmNaxijMS1INxxibPo+EyX0ucxrVUDN3XXTwjVh0E/wIVI6eVAbqnj973ZzZ7hi/m0Hd24oYWw5nks9bq5ph1VQ4rrhIoE9BAaT5ZyYxIKWgC+7qlf/Na6uPrAuQLyGIlBPSENSrVZ7glmxaDzEd8nkyA74UmtGQAIHBgzMHz05x4fOdRtn1zZFoHtquq3CWavL4W4pAPKdwVi0NLxRWB2/rDyXqKFFfA2OdrOrj+BbFYnGDPs7wW2ysOaHxj9cwegDWhpgcQgUOvEAOCRBLsoTl6t0GNZLJ7q0j46UcS5GCpj6csBPPW3O90LEbSBg==&Key-Pair-Id=APKAISLU6JPYU7SF6EUA

https://docs.aws.amazon.com/elasticloadbalancing/latest/classic/elb-backend-instances.html  

https://docs.aws.amazon.com/elasticloadbalancing/latest/userguide/what-is-load-balancing.html  
