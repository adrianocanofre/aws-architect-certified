# SNS(Simple Notification Service)  

SNS is a web service that makes it easy to set up operate, and send notifications from the cloud.  

It provides developers with a highly scalable, flexible and cost-effective capability to publish messages from an application and immediately deliver them to subscribers or other applications.  

SNS follows the "publish-subscribe" (pub-sub) messaging paradigm, with notifications being delivered to clients using a "push" mechanism that eliminates the need to periodically check or "pool" for new information and updates.  

With simple APIs requiring minimal up-front development effort, no maintenance or management overhead and pay-as-your-go pricing, SNS gives developers and easy mechanism to incorporate a powerful notification system with their applications.  

Push notifications to Apple, Google, Fire OS, and Windows devices, as well as Android devices in China with Baidu Cloud Push.  

Besides pushing cloud notifications directly to mobile devices, Amazon SNS can also deliver notifications by SMS text message or email, to Amazon Simple Queue Service(SQS) queues, or to any HTTP endpoint.  

To prevent messages from being lost, all messages published to Amazon SNS are stored redundantly across multiples availability zones.  

SNS allows you to group multiple recipients using topics. A topic is an "access point" for allowing recipients to dynamically subscribe for identical copies of the same notification.  

One topic can support deliveries to multiple endpoint types -- for example, you can group together IOS, Android, and SMS recipients, When you publish once to a topic SNS delivers appropriately formatted copies of your message to each subscriber.  


### SNS Benefits  

* Instantaneous, push-based delivery (no polling);  
* Simple APIs and easy integration with applications;  
* flexible message delivery over multiple transport protocols;  
* Inexpensive, pay-as-you-go model, with no up-front costs;  
* web-based AWS Management Console Offers the simplicity of a point-and-click interface;

### SNS vs SQS  

* Both messaging Services in AWS;  
* SNS - Push;  
* SQS - Polls (Pulls)  

### Pricing  

* User pay $0.50 per 1 million Amazon SNS Requests;  
* $0.06 per 100,000 Notification deliveries over HTTP;  
* $0.75 per 100 Notification deliveries over SMS;  
* $2.00 per 100,000 Notification deliveries over Email;  
