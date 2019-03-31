# API Gateway  

API Gateway is a fully managed service that makes it easy for developers to publish, maintain, monitor, and secure APIs at any scale. With a few clicks in the AWS Management Console, you can create API that acts as a "front door" for applications to access data, business logic, or functionality from your back-end services, such as applications running on EC2, code running on AWS Lambda, or any web application.

[IMG] Como funciona api gateway

You can enable API caching in API Gateway to cache your endpoint's response. With caching, you can reduce the number of calls made to your endpoints and also improve the latency of the requests to your API. When you enable caching for a stage, API Gateway caches responses from your endpoint for a specified time-to-live(TTL) period, in seconds, API Gateway then responds to the requests by looking up the endpoint response from the cache instead of making a requests to your endpoint.  

[IMG] Como funciona caching


**What can API Gateway DO?**  

* Low Cost & Efficient;    
* Scales Effortlessly;  
* You can Throttle Requests to prevent attacks;  
* Connect to Cloudwatch to log all requests;  

**Same Origin Policy**  

In computing, the same-origin policy is an important concept in the web application security model. Under the policy, a web browser permits scripts contained in a first web page to access data in a second web page, but only if both web pages have the same origin.  

**CORS**  

CORS is one way the server at the other end(not the client code in the browser) can relax the same-orgin policy.  

Cross-orgin resource sharing (CORS) is a mechanism that allows restricted resources on a web page to be requested from another domain outside the domain from which the first resource was served.   

**ERROR**  
"Origin policy cannot be read at the remote resource?"  
You need to enable CORS on API Gateway.  


### Exam Tips  

* Remember waht API Gateway is at a High level;  
* API Gateway has caching capabilities to increase performanve;  
* API Gateway is low cost and scales automatically;  
* You can throttle API Gateway to prevent attacks;  
* You can log results to Cloudwatch;  
* IF YOU ARE USING JAVASCRIPT/AJAX that uses multiple domains with API Gateway, ensure that you have enabled CORS on API Gateway;

[API Gateway structure](https://docs.aws.amazon.com/apigateway/api-reference/)
