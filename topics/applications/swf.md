# SWF(Simple Workflow Service)  


SWF is a web service that makes it easy to coordinate work across distributed application components. Amazon SWF enables applications for a range of use cases, including media processing, web applications beck-ends, business process workflows, and analytics pipelines, to be designed as a coordination of tasks.  
Tasks represent invocations fo various processing steps in an application which can be performed by executable code, web service calls, human actions, and scripts.  

**SWF Workes**  

Workers are programs that interact with Amazon SWF to get tasks, process received tasks, and return the results.  

**SWF Decider**  

The decider is a program that controls the coordination of tasks, i.e. their ordering, concurrency, and scheduling according to the applications logic.  

**Workers & Deciders**  

The Workers and the deciders can run on cloud infrastructure, such as Amazon EC2, or on machines behind firewall. Amazon SWF brokers the interactions between workers and the decider. it allows the decider to get consistent views into the progress of tasks and to initiate new tasks in an ongoing manner.  

At the same time, Amazon SWF stores tasks, assigns them to workers when they are ready, and monitors their progress. It ensures that a task is assigned only once and is never duplicated. Since Amazon SWF maintains the applications state durably, workers and deciders don't have to keep track of execution state. They can run independently, and scale quickly.  

**SWF Domains**  

Your workflow and activity types and the workflow execution itself are all scoped to a domain. Domains isolate a set of types, executions, and task list from others within the same account.  

You can register a domain by using the AWS Management Console or by using the RegisterDomain action in the Amazon SWF API.  

The parameters are specified in JSON format.  

Maximum Workflow can be 1 year and the value is always measured in seconds.  

### SWF vs SQS  

* Amazon SWF presents a task-oriented API, whereas SQS offers a message-oriented API.  
* SWF ensures that a task is assigned only once and is never duplicated. With SQS, you need to ensure that a message is processed only once.  
* SWF keeps track of all the tasks and events in an application. With Amazon SQS, you need to implement your own application-level tracking, especially if your application uses multiples queues.


[Development Options](https://docs.aws.amazon.com/amazonswf/latest/developerguide/swf-welcome.htm)
