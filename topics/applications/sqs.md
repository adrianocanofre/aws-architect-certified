# SQS  

SQS is a web service that gives  you access to a message queue that can be used to store messages while for a computer to process them.  
Amazon SQS is a distributed queue system that enables web service applications to quickly and reliably queue messages that one component inthe application generates to be consumed by another component. A queue is a temporary repository for messages that are awaiting processing.  

Using SQS, you can decouple the components of an application so they run independently, easing message management between components.  

Messages can contani up to 256kb of text in any format.


**Two types**:  

* Standard Queues(default)  
A stanard queue lets you have a nearly-unlimited number of transactions per second. Standard queues guarantee that a message is delivered at least once. However, occasionally, more than one copy of a message might be delivered out of order. Standard queues provide best-effort ordering which ensures that messages are generally delivered in the same order as they are sent.  

* FIFO(First-In-First-Out)  
FIFO queue complements the standard queue. The most important features of this queue type are FIFO delivery and exactly-once processing: The order in which messages are sent and received is strictly preserved and a message is delivered once and remains available until a consumer processes and deletes it; duplicated are not introduced into the queue.  
FIFO queues also support message groups that allow multiple ordered message groups within a single queue.  
FIFO queues are limited to 300 transactions per second(TPS), but have all the capabilities of standard queues.  

**SQS Key Facts**  
* SQS is pull-based, not pushed-based;  
* Messages are 256 KB in size;  
* Messages can be kept in the queue from 1 minute to 14 days;  
* Default retention period is 4 days;
* SQS guarantees that your messages will be processed at last once;  

**SQS Visibility Timeout**  
* Default Visibility Timeout is 30 seconds;  
* Increase it if your task takes >30 seconds;  
* Maximum is 12 hours;


#### Tips  

* SQS is a distributed message queueing system;  
* Allows you to decouple the components of an application so that they are independent;  
* Pull-based, not push-based;  
Standard Queues - best-effort ordering; message delivered at least once;  
* FIFO Queues - ordering strictly proserved, message delivered once, no duplicates. e.g. good for banking transactions which need to happen in strict order.  
* Visibility Timeout, for default is 30s, and max is 12 hours;  
* Short polling returned immediately even if no messages are in the queue;  
* Long polling  polls the queue periodically and only returns a response when a message is in the queue or the timeout is reached.  


[AWS Documentation](https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/sqs-how-it-works.html)

[NEXT - SWF](swf.md)
