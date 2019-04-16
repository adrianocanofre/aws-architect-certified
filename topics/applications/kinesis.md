# Kinesis  

Amazon Kinesis makes it easy to collect, process and analyze real-time, **streaming data** so you can get timely insights and react quick to new information. Kinesis makes it easy to load and analyze streaming data, and also providing the ability for you to build your own custom application for you business needs.  

**What is streaming data?**  

Streaming Data is data that is generated continuously by thousands of data sources, which typically send in the data records simultaneously, and in small sizes.  
* Purchases from online stores;  
* Stock Prices;  
* Game data(as the gammer plays);  
* Social network data;  
* Geospatial data;  
* IoT sensor data;    

### Kinesis Streams  

* Kinesis Streams consist of shards;  
  * The shards consist in 5 transactions per second for reads, up to a maximum total data read rate of 2 MB per second and up to 1,000 records per second for writes, up to a maximum total data write rate of 1 MB per second(including partition keys).
  * The data capacity of your stram is a function of the number of shards that you specify for the stream. The total capacity of the stream is the sum of the capacities os its shards.  

![Kinesis Streams](/imgs/kinesis-streams.png)https://docs.aws.amazon.com/streams/latest/dev/key-concepts.html

### Kinesis Firehose  

![Kinesis Streams](/imgs/kinesis-firehose.png)https://docs.aws.amazon.com/firehose/latest/dev/what-is-this-service.html
### Kinesis Analytics  


### Exam Tips  

* Know the difference between Kinesis Streams and Kinesis Firehose. You will given scenario questions and you must choose the most relevant service.  
* Understand what Kinesis Analytics is.  

[NEXT - Tips](tips.md)
