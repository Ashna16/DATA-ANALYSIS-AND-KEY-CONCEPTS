Reference : AWS Certification- Data Analytics Fundamentals


# DATA-ANALYSIS-AND-KEY-CONCEPTS

Fundamentals of Data Analysis:

Data analysis is the process of compiling, processing, and analyzing data so that you can use it to make decisions.
Analytics is the systematic analysis of data. Data analytics is the specific analytical process being applied.
Nowadays, the problem isn't finding the data but it is failing to do something with it.

Data is generated in many ways. The big question is where to put it all and how to use it to create value or generate competitive advantages. The challenges identified in many data analysis solutions can be summarized by five key challenges: volume, velocity, variety, veracity, and value.

COMPONENTS OF DATA ANALYSIS SOLUTION

1. Ingest/Collection : This includes collecting raw data from transactions,logs and IoT devices.These data can be structured or unstructured.
                       A good data analysis allows developers to ingest wide variety of data(Structured,unstructured) at any speed from batch
                       to streaming.

2. Store : A good data analysis solution should provide secure, scalable, and durable storage. This storage should include data stores 
           that can house structured, semistructured, and unstructured data.
           For example, data warehouses efficiently store structured analytical data, databases can store both structured and semistructured           
           data, and data lakes can store all three forms of data.
           
3. Process/analyze : First, data must be processed, transforming it to make the data more consumable. As part of the processing, the     
                     data will also be analyzed. This usually means sorting, aggregating, joining, and applying business logic to produce  
                     meaningful analytical data sets. The final step is to load this analytical data set into a new storage location,like a  
                     data lake, database, or data warehouse.
                     
4. Consume/ visualize : You have two ways to consume data: by querying or by using business intelligence (BI) tools. Querying produces results  
                        that are great for quick analysis by data analysts. Bl tools produce visualizations that are grouped into reports and
                        dashboards to help users explore data and determine the best actions to take.                     

                

The five main V's of data analysis are:

1. Volume
2. Velocity
3. Variety
4. Veracity
5. Value

![SQL COMMANDS](https://explore.skillbuilder.aws/files/a/w/aws_prod1_docebosaas_com/1661720400/cJszwHL05vRyqx_11yz-iA/tincan/c16bd0344c0123121a6326a58844db542da58ae5/assets/H-ZCOsPJEBEkarHL_9P-CzBBrUVLfpKCw.png)

Volume                             

Volume means the amount of data that will be ingested by the solution - the total size of the
data coming in. Solutions must work efficiently across distributed systems and be easily expandable in order to
accommodate spikes in traffic.

Velocity

Velocity means the speed of data entering a solution. Many organizations now require near
real-time ingestion and processing of data.The high velocity of data results in a shorter time
to analyze than traditional data processing can provide. Solutions must be able to manage this velocity
efficiently. Processing systems must be able to return results within an acceptable time frame.

Variety

Data can come from many different sources.Variety means the number of different sources
and the types of sources that the solution will use. Solutions need to be sophisticated enough to manage all the different types of data while
providing accurate analysis of the data.

Veracity

Veracity is the degree to which data is accurate,precise, and trusted. It is contingent on the integrity and trustworthiness of the data.
Solutions should be able to identify the common flaws in the data and fix them before the data is
stored. This is known as data cleansing. This process must be able to be completed within the time requirements of the solution, up to and
including real-time processing speeds.

Value
Value is the ability for a solution to extract meaningful information from the data that has been stored and analyzed. Solutions must be able to produce the right form of analytical results to inform business decision makers and stakeholders of insights using trusted reports and
dashboards.


------------------------------------------ VOLUME --------------------------------------------------------------------------------------------------------------------------------------------------

When businesses have more data than they are able to process and analyze, they have a volume problem.

There are three broad classifications of data source types:

Structured data is organized and stored in the form of values that are grouped into rows and columns of a table.
Semistructured data is often stored in a series of key-value pairs that are grouped into elements within a file.
Unstructured data is not structured in a consistent way. Some data may have structure similar to semi-structured data but others may only contain metadata.

Amazon S3 concepts

Amazon S3 stores data as objects within buckets.

An object is composed of a file and any metadata that describes that file. To store an object in Amazon S3, you upload the file you want to store into a bucket. When you upload a file, you can set permissions on the object and add any metadata.

Buckets are logical containers for objects. You can have one or more buckets in your account and can control access for each bucket individually. You control who can create, delete, and list objects in the bucket. You can also view access logs for the bucket and its objects and choose the geographical region where Amazon S3 will store the bucket and its contents.



DATA LAKES:

A data lake is a centralized repository that allows you to store structured, semistructured, and unstructured data at any scale.
Data lakes promise the ability to store all data for a business in a single repository. You can leverage data lakes to store large volumes of data instead of persisting that data in data warehouses. Data lakes, such as those built in Amazon S3, are generally less expensive than specialized big data storage solutions. That way, you only pay for the specialized solutions when using them for processing and analytics and not for long-term storage. Your extract, transform, and load (ETL) and analytic process can still access this data for analytics. 


DATA WAREHOUSE:

A data warehouse is a central repository of structured data from many data sources. This data is transformed, aggregated, and prepared for business reporting and analysis.
A data warehouse is a central repository of information coming from one or more data sources. Data flows into a data warehouse from transactional systems, relational databases, and other sources. These data sources can include structured, semistructured, and unstructured data. These data sources are transformed into structured data before they are stored in the data warehouse.

Data is stored within the data warehouse using a schema. A schema defines how data is stored within tables, columns, and rows. The schema enforces constraints on the data to ensure integrity of the data. The transformation process often involves the steps required to make the source data conform to the schema. Following the first successful ingestion of data into the data warehouse, the process of ingesting and transforming the data can continue at a regular cadence.


DATA MARTS:

A SUBSET OF A DATA WAREHOUSE
Data warehouses can be massive. Analyzing these huge stores of data can be confusing. Many organizations need a way to limit the tables to those that are most relevant to the analytics users will be performing.

A subset of data from a data warehouse is called a data mart. Data marts only focus on one subject or functional area. A warehouse might contain all relevant sources for an enterprise, but a data mart might store only a single department’s sources. Because data marts are generally a copy of data already contained in a data warehouse, they are often fast and simple to implement.

------------------------------------------ VELOCITY ----------------------------------------------------------------------------------------------------------------------------

When businesses need rapid insights from the data they are collecting, but the systems in place simply cannot meet the need, there's a velocity problem.

Data processing means the collection and manipulation of data to produce meaningful information. Data collection is divided into two parts, data collection and data processing.

Data processing may only need to be performed once a day, making results available the following morning, or it may need to be performed and made available immediately. This variance in the speed at which data processing must occur can be broken down into four categories.

SO BASICALLY :

1. BATCH PROCESSING :

 a. SCHEDULED: Scheduled batch processing represents data that is processed in a very large volume on a regularlyscheduled basis. For instance,  
               once a week or once a day. It is generally the same amount of data with each load, making these workloads predictable.

 b. PERIODIC: Periodic batch processing is a batch of data that is processed at irregular times. These workloads are often run once a certain   
              amount of data has been collected. This can make them unpredictable and hard to plan around.
 
 2. STREAM PROCESSING:
 
 a. NEAR REAL-TIME: Near real-time processing represents streaming data that is processed in small individual
                    batches. The batches are continuously collected and then processed within minutes of the data
                    generation.
 
 b. REAL TIME: Real-time processing represents streaming data that is processed in very small individual
               batches.The batches are continuously collected and then processed within milliseconds of the data
               generation.
               
               
![SQL COMMANDS](https://explore.skillbuilder.aws/files/a/w/aws_prod1_docebosaas_com/1661720400/cJszwHL05vRyqx_11yz-iA/tincan/c16bd0344c0123121a6326a58844db542da58ae5/assets/u7xQDkmAfXh2vSh2_Lb2teMDO_Qr5PqAo.png)


CHARACTERISTICS OF FOUR VELOCITIES ON COLLECTING AND PROCESSING DATA

COLLECTING DATA


Batch: Velocity is very predictable with batch processing. It amounts to large bursts of data transfer at scheduled intervals.

Periodic: Velocity is less predictable with periodic processing. The loss of scheduled events can put a strain on systems and must be considered.

Near real-time: Velocity is a huge concern with near real-time processing. These systems require data to be processed within minutes of the initial collection of the data. This can put tremendous strain on the processing and analytics systems involved.

Real-time: Velocity is the paramount concern for real-time processing systems. Information cannot take minutes to process. It must be processed in seconds to be valid and maintain its usefulness.

PROCESSING DATA

Batch and periodic: Once the data has been collected, processing can be done in a controlled environment. There is time to plan for the appropriate resources.

Near real-time and real-time: Collection of the data leads to an immediate need for processing. Depending on the complexity of the processing (cleansing, scrubbing, curation), this can slow down the velocity of the solution significantly. 


Data acceleration

Another key characteristic of velocity on data is data acceleration, which means the rate at which large collections of data can be ingested, processed, and analyzed. Data acceleration is not constant. It comes in bursts. Take Twitter as an example. Hashtags can become hugely popular and appear hundreds of times in just seconds, or slow down to one tag an hour. That's data acceleration in action. Your system must be able to efficiently handle the peak of hundreds of tags a second and the lows of one tag an hour. 


CHALLENGES OF VELOCITY:

1. Periodic velocity data ingest with batch processing

Imagine that a retail chain is trying to analyze point-of-sale (POS) data from its franchise stores. The stores are located all over the world. Each location transmits batches of data to the central data center periodically throughout the day. The customer prefers to hold the analysis of the datasets until 11:50 pm Eastern Standard Time. At this time, all datasets must be rapidly processed so that reports can be generated and delivered to branch managers across the world as soon as possible. The slower collection of data followed by a rapid processing requirement is a common challenge.

2. High-velocity data ingest with real-time processing

Imagine a media company that makes decisions based on click stream data gathered from social media. The sheer amount of data produced per second is huge. Collection must be fast enough to gather all data without missing anything. Once collected, this data must be processed just as fast in a continuous stream. The rapid collection of data followed by the rapid processing of data is a common signature of streaming analytics.


BATCH PROCESSING:

Batch processing is often thought of as a slow process. This is not the case. Batch processing must quickly and efficiently consume a huge amount of data all at once. This poses challenges that do not exist with stream processing.

Batch data processing provides companies with the ability to dive deep into the data they have collected to produce complex analytics that simply cannot be achieved using streaming analytics.

Batch processing is the execution of a series of programs, or jobs, on one or more computers without manual intervention. Data is collected into batches asynchronously. The batch is sent to a processing system when specific conditions are met, such as a specified time of day. The results of the processing job are then sent to a storage location that can be queried later as needed.

Batch processing is the execution of a series of programs, or jobs, on one or more computers without manual intervention. Data is collected into batches asynchronously. The batch is sent to a processing system when specific conditions are met, such as a specified time of day. The results of the processing job are then sent to a storage location that can be queried later as needed.

Amazon EMR and Apache Hadoop are used for Batch procesiing

Amazon EMR is a managed service for implementing Apache Hadoop workloads. In addition to running the Apache Hadoop framework, you can also run other popular distributed frameworks such as Apache Spark, HBase, Presto, and Flink in EMR. You have the added advantage of being able to interact with data in other AWS data stores such as Amazon S3 and Amazon DynamoDB. 

Amazon EMR notebooks provide a serverless development and collaboration environment for one-time querying and exploratory analysis. You can manipulate the data and generate data plots using rich graphical tools. Amazon EMR notebooks monitor your jobs and even help you debug code from the notebooks.
 
Apache Hadoop
Apache Hadoop is a scalable storage and batch data processing system. It uses commodity server hardware and provides fault tolerance through software. Hadoop complements existing data systems by simultaneously ingesting and processing large volumes of data, structured or not, from any number of sources, which enables deeper analysis than any one system can provide. These results can be delivered to any existing enterprise system for further use independent of Hadoop.

Hadoop is a platform that provides distinct modules:

1. Hadoop Common is the set of Java utilities and libraries that support the other Hadoop modules. These libraries help abstract the file system from the processing components. These Java files and scripts are required to start Hadoop.

2.Hadoop Distributed File System (HDFS) is the distributed file system that stores the data in a high-throughput environment of community nodes. This architecture ensures very high aggregate bandwidth access to application data.

3.Hadoop YARN is the resource management framework responsible for scheduling and executing processing jobs.

4.Hadoop MapReduce is a YARN-based system that allows for parallel processing of large data sets on the cluster.



STREAM PROCESSING :

There are many reasons to use streaming data solutions. In a batch processing system, processing is always asynchronous, and the collection system and processing system are often grouped together. With streaming solutions, the collection system (producer) and the processing system (consumer) are always separate. Streaming data uses what are called data producers. Each of these producers can write their data to the same endpoint, allowing multiple streams of data to be combined into a single stream for processing. Another huge advantage is the ability to preserve client ordering of data and the ability to perform parallel consumption of data. This allows multiple users to work simultaneously on the same data.

In stream processing, you use multiple services: one service to ingest the constant stream of data, one to process and analyze the stream, and one to load the data into an analytical data store if required. 



---------------------------------------------- VARIETY ---------------------------------------------------------------------

A data source can be just about anything—a folder on a file server, database, web page, and even a wearable device can be considered a data source. In each of these data sources, data is stored in a specific way. Some data sources use a schema to organize content and indexes to improve performance. Others organize data in a more flexible way and are called schemaless. Schemaless data sources still use indexes to improve performance. 

There are three types of data:

1. Structured Data: Structured data is stored in a tabular format, often within a database management system (DBMS). This data is organized based on a relational data model, which defines and standardizes data elements and their relation to one another. Data is stored in rows, with each row representing a single instance of a thing (for example, a customer). These rows are well understood due to the table schema, which explains what each field in the table represents. This makes structured data easy to query.

The downside to structured data is its lack of flexibility. Let’s say that you have decided you want to track the age of your customers. You must reconfigure the schema to allow for this new data, and you must account for all records that don’t have a value for this new field. It is not impossible, but it can be a very time-consuming process.


2. Semistructured data is stored in the form of elements within a file. This data is organized based on elements and the attributes that define them. It doesn't conform to data models or schemas. Semistructured data is considered to have a self-describing structure. Each element is a single instance of a thing, such as a conversation. The attributes within an element define the characteristics of that conversation. Each conversation element can track different attributes. This makes semistructured data quite flexible and able to scale to meet the changing demands of a business much more rapidly than structured data.

The trade-off is with analytics. It can be more difficult to analyze semistructured data when analysts cannot predict which attributes will be present in any given data set.

3. Unstructured data is stored in the form of files. This data doesn't conform to a predefined data model and isn't organized in a predefined manner. Unstructured data can be text-heavy, photographs, audio recordings, or even videos. Unstructured data is full of irrelevant information, which means the files need to be preprocessed to perform meaningful analysis. This can be done in many ways. For example, services can add tags to the data based on rules defined for the types of files. The data can also be cataloged to make it available to query services.


**Structured data is hot, immediately ready to be analyzed. 
Semistructured data is lukewarm—some data will be ready to go and other data may need to be cleansed or preprocessed. Unstructured data is the frozen ocean—full of exactly what you need but separated by all kinds of stuff you don’t need.**

**Flat File:**

Flat-file data generally resides in a worksheet or spreadsheet. This may not seem like a database, but it meets all of the basic requirements. This format provides a solid foundation for understanding some of the considerations when choosing a DBMS.

Drawbacks of Flat File: 
1. Duplicate Values
2. Ambigious Values
3. Relationship
4. Missing Data

**Relational databases**

Flat-file storage may not fit your structured data storage needs. The next logical step is to move to a more robust solution: a relational database.

A process known as normalization helps a business take flat-file data and turn it into a relational database. Normalization is a set of rules that work together to reduce redundancy, increase reliability, and improve the consistency of data storage.

A relational database is built to store structured data so it can be collected, updated, and queried easily. Relational databases rely on a series of structures, called tables, to hold the collected data. These tables are navigated using the structured query language, or SQL.

Logically, relational database tables group data based on a person, place, thing, or event related to that data. These groupings are referred to as entities. Each entity is stored as a table. 

A column, known as a field, is used to describe one attribute of the entity. A row, known as a record, in the table represents a single instance of an entity.

Relationships are created by first ensuring that every row in a table is unique. This is done by creating a primary key. This primary key value can then be used to create relationships between tables. A foreign key is a field that uses the values from a primary key in another table to define a record in the current table. This act is what builds the relationship. Some database engines can enforce this relationship to ensure that only values from the primary key can be used in the foreign key.


Types of information systems

There are two main ways—known as information systems—of organizing data within a relational database. The data can be organized to focus on the storage of transactions or the process of analyzing transactions.

Transactional databases are called online transaction processing (OLTP) databases. The data gathered by OLTP databases is often fed into another type of database that focuses on analyzing the transactional data. Online analytical processing (OLAP) databases gather data from OLTP systems for the purpose of organizing it for analytical operations.


OLTP:

Online transaction processing (OLTP) databases, often called operational databases, logically organize data into tables with the primary focus being on the speed of data entry. These databases are characterized by a large number of insert, update, and delete operations.

All decisions about the organization of data and storage of attributes is based on ensuring rapid data entry and updates. The effectiveness of an OLTP system is often measured by the number of transactions per second.

OLAP:

Online analytical processing (OLAP) databases, often called data warehouses, logically organize data into tables with the primary focus being the speed of data retrieval through queries. These databases are characterized by a relatively low number of write operations and the lack of update and delete operations.

All decisions about the organization of data and storage of attributes are based on the types of queries and other analytics that will be performed using the data. The effectiveness of an OLAP system is often measured by the response time of query results.
