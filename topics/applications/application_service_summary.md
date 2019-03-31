# Application Service Sumary  

**What is SQS?**  

SQS is a web service that gives you access to a message queue that can be used to store messages while waiting for a computer to process them.

**SQS Exam Tips**  
* SQS is pull based, not pushed base;  
* Messages are 256KB in size;  
* Messages can be kept in the queue from 1 minute to 14 days.(The default is 4 days);
* Visibility Time Out is the amount of time that the message is invisible in the SQS queue after a reader picks up that message. Provided the job is processed before the visibility time out expires, the message will then be deleted from the queue. If the job is not processed within that time, the message will become visible again and another reader will process it. This could result in the same message being delivered twice;   
* Visibility time out maximum is 12 hours;  
* SQS guarantees that your messages will be processed at least once;  
* SQS long polling is a way to retrieve messages from your Amazon SQS queues;
* Queues's can either be **standard** or **FIFO**;


**SWF vs SQS**  
* SQS has a retention period og 14 days, SWF up to 1 year for workflow executions;  
* Amazon SWF presents a task-oriented API, whereas Amazon SQS offers a message-oriented API;  
* Amazon SWF ensures that a task is assigned only once and is never duplicated. With Amazon SQS, you need to handle duplicated messages and may also need to ensure that a message is processed only once;  
* Amazon SWF keeps track of all the tasks and events in an application. With Amazon SQS, you nees to implment your own application-level tracking, especially if you application uses multiple queues;  

**SWF Actors**  
* Workflow Starters - An application that can initiate(start) a workflow. Could be your e-commerce website when placing an order a mobile app searching for bus times.  
* Deciders - Control the flow of activity tasks in a workflow execution. If something has finished in a workflow(or fails) a Decider decides what to do next.  
* Activity Workers - Carry out the activity tasks.  

**SNS Subscribers**  
HTTP, HTTPS, Email, Email-Json, SQS, Application, Lambda.  

**SNS vs SQS**  

* SNS - push;
* SQS - Polls(Pulls);  

**Elastic Transcoder**  


**Kinesis Streams**  
Kinesis Streams; Kinesis Firehose; Kinesis Analytics;  
