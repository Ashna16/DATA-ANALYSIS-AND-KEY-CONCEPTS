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

![SQLCOMMANDS(https://explore.skillbuilder.aws/files/a/w/aws_prod1_docebosaas_com/1661724000/MqLpcokh7gF8mOODOyQYPA/tincan/c16bd0344c0123121a6326a58844db542da58ae5/assets/lUwzpHU8p_-NkdJE_LICrxU4Kipl21dTm.png)
