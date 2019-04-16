# API Gateway  

API Gateway is a fully managed service that makes it easy for developers to publish, maintain, monitor, and secure APIs at any scale. With a few clicks in the AWS Management Console, you can create API that acts as a "front door" for applications to access data, business logic, or functionality from your back-end services, such as applications running on EC2, code running on AWS Lambda, or any web application.

![CDN](/imgs/api-gw.png)   

**What can API Gateway DO?**  

* Expose HTTPS endpoint to define a RESTful API;  
* Serverless-ly connect to services like lambda & DynamoDB;  
* Send each API endpoint to a different target;  
* Low Cost & Efficient;    
* Scales Effortlessly;  
* Track and control usage by API key;  
* You can Throttle Requests to prevent attacks;  
* Connect to CloudWatch to log all requests;
* Maintain multiple versions of your API;  

**How DO I configure API Gateway?**  

* Define an API(container);  
* Define resources and nested resources(URL paths);  
* For each resource:  
  * Select supported HTTP methods (verbs);
  * Set security;  
  * Choose target(such as EC2, Lambda, DynamoDB, etc.);  
  * Set requests and response transformations;  

**How Do I deploy API Gateway?**  

* Deploy API to a stage:
  * Uses API Gateway domain, by default;
  * Can use custom domain;  
  * Now supports AWS Certificate Manager: Free SSL?TLS certs;  


### API Gateway Caching  

You can enable API caching in API Gateway to cache your endpoint's response. With caching, you can reduce the number of calls made to your endpoints and also improve the latency of the requests to your API. When you enable caching for a stage, API Gateway caches responses from your endpoint for a specified time-to-live(TTL) period, in seconds, API Gateway then responds to the requests by looking up the endpoint response from the cache instead of making a requests to your endpoint.  

![CDN](/imgs/api-gw-caching.png)

### Same Origin Policy  

In computing, the same-origin policy is an important concept in the web application security model. Under the policy, a web browser permits scripts contained in a first web page to access data in a second web page, but only if both web pages have the same origin.  

### CORS  

CORS is one way the server at the other end(not the client code in the browser) can relax the same-origin policy.  

Cross-origin resource sharing (CORS) is a mechanism that allows restricted resources on a web page to be requested from another domain outside the domain from which the first resource was served.   

**CORS in Action**

1 -  Browser makes an HTTP OPTIONS call for a URL;  
2.1 -  Server return a response that says: "These other domains are approved to GET this URL.";  
2.2-  ERROR -"Origin policy cannot be read at the remote resource?". You need to enable CORS on API Gateway.



### Exam Tips  

* Remember what API Gateway is at a High level;  
* API Gateway has caching capabilities to increase performance;  
* API Gateway is low cost and scales automatically;  
* You can throttle API Gateway to prevent attacks;  
* You can log results to CloudWatch;  
* If you are using Javascript/Ajax that uses multiple domains with API Gateway, ensure that you have enabled CORS on API Gateway;  
* CORS is enforced by the client;  

[API Gateway structure](https://docs.aws.amazon.com/apigateway/api-reference/)

[NEXT - Kinesis](kinesis.md)
