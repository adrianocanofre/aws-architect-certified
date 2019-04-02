# EC2(Elastic Computer Cloud)   

EC2 is a web service that provides resizable compute capacity in the cloud. EC2 reduces the time required to obtain and boot new server instances to minutes, allowing you to quickly scale capacity, both up and down, as your computing requirements change.  

### EC2 Pricing Models  

* On Demand  
> Allows you to pay a fixed rate by the hour(or by second) with no commitment.  

  * Users that want the low cost and flexibility of EC2 without any up-front payment or long-term commitment.  
  * Applications with short term, spiky, or unpredictable workloads that cannot be interrupted.  
  * Applications being developed or tested on Amazon EC2 for the first time.  

* Reserved  
> Provides you with a capacity reservation, and offer a significant discount on the hourly charge for an instance. Contract Terms are 1 year or 3 Year terms.  

  * Applications with steady state or predictable usage;  
  * Applications that require reserved capacity;  
  * User able to make upfront payments to reduce their total computing cost even further;  

  * Pricing Types:  
    * Standard Reserved;  
    > These offer 75% off on demand instances, The more you pay up front and the longer the contract, the greater the discount.  

    * Convertible Reserved;  
    > These offer up to 54% off on demand capability to change the attributes of the RI as long as the exchange results in the creation of Reserved Instances of equal or greater value.  

    * Scheduled Reserved;  
    > These are available to launch within the time windows you reserve. This option allows you match your capacity reservation to a predictable recurring schedule that only requires a fraction of a day, a week, or a month.  

* Spot  
> Enable you to bid whatever price you want for instance capacity, providing for even greater savings if your applications have flexible start and end times.  

  * Application that have flexible start and end times;
  * Applications that are only feasible at very low compute prices;  
  * User with urgent computing needs for large amounts of additional capacity;  

* Dedicated Hosts  
> Physical EC2 server dedicated for your use. Dedicated hosts can help you reduce costs by allowing you to use your existing server-bound software licenses.  

  * Useful for regulatory requirements that may not support multi-tenant virtualization;  
  * Great for licensing which does not support multi-tenancy or cloud deployments;  
  * Can be purchased On-Demand(hourly);  
  * Can be purchased as a Reservations for up 70% off the On-Demand price;


### EC2 Types  

|Family| Speciality | Use case |
|:------:|:------------:|:---------:|
| F1 | Field Programmable<br/> gate array| Genomics research, financial analytics, real-time video<br/> processing, big data, etc. |
| I3| High Speed Storage| NoSQL DBs, Data warehousing, etc.|
| G3| Graphics Intensive| Video Encoding, 3D Applications Streaming|
| H1|  High Disk Throughput|  MapReduce-based workloads, distributed file systems such as HDFS and MapR-FS|
| T3| Lowest cost, General purpose| Web servers, small DBs|
| D2| Dense Storage| Fileservers/Data Warehousing/Hadoop|
| R5| Memory Optimized| Memory intensive Apps/DBs|
| M5| General Purpose| Application service|
| C5| Compute Optimized|  CPU Intensive Apps/DBs|  
| P3| Graphics/General Purpose GPU| Machine Learning, Bit Coin Mining etc|
| X1| Memory Optimized| SAP HANA/ Apache Spark|
| Z1D| High compute capacity and a high memory footprint| Ideal for electronic design automation (EDA) and certain relational db workloads with high per-core licensing etc.|
| A1| Arm-based workloads|  Scale-out workloads such as web servers.|
| U-6TB1| Bare Metal| Bare metal capabilities that eliminate virtualization overhead| 

**Memorization**  
**F** for FPGA, **I** for IOPS, **G** for graphics, **H** for high Disk Throughput, **T** for cheap general purpose(think T2micro), **D** for Density, **R** for RAM, **M** for Main choice for general purpose apps, **C** for compute, **P** for graphics(Pics), **X** for extreme memory, **Z** for extreme memory and CPU, **A** for Arm-based workloads, **U** Bare Metal.
