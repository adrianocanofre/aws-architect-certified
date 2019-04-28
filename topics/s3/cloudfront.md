# CloudFront  


**What is CDN?**  

A content delivery network(CDN) is a system of distributed servers(network) that deliver webpages and other web content to a user based on the geographic location of the user, the origin of the webpage and a content delivery server.  

![CDN](/imgs/cdn-example.png)   

**What is CloudFront?**  

It's can be used to deliver your entire website, including dynamic, static, streaming, and interactive content using a global network of edge locations. Requests for your content are automatically routed to the nearest  edge location, so content is delivered with the best possible performance.  

CloudFront is optimized to work with other Amazon Web Services, like S3, EC2, ELB and Route53. Amazon CloudFront also works seamlessly with any non-AWS origin server, which stores the original, definitive version of your files.  


### CloudFront - Key Terminology  

* **Edge Location**  - This is the location where content will be cached. This is separate to an AWS Region/AZ;  
* **Origin** - This is the origin of all the files that the CDN will distribute. This can be either an S3 Bucket, an EC2 Instance, an Elastic Load Balancer or Route53;  
* **Distribution** - This is the name given the CDN which consists of a collection of Edge Locations:  
  * **Web Distribution** - Typically used for websites;  
  * **RTMP** - Used for Media Streaming;  

![EDGE](/imgs/how-cloudfront-delivers-content.png)  


### Tips

* Edge locations are not just READ only, you can write to them too.(ie put an object on to them);  
* Objects are cached for the life of the TTL(Time to Live);  
* You can clear cached objects, but you will be charged;  

[NEXT - SnowBall](snowball.md) 
