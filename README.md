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


--------------------------------- VOLUME --------------------------------------------------

When businesses have more data than they are able to process and analyze, they have a volume problem.

There are three broad classifications of data source types:

Structured data is organized and stored in the form of values that are grouped into rows and columns of a table.
Semistructured data is often stored in a series of key-value pairs that are grouped into elements within a file.
Unstructured data is not structured in a consistent way. Some data may have structure similar to semi-structured data but others may only contain metadata.

Amazon S3 concepts

Amazon S3 stores data as objects within buckets.

An object is composed of a file and any metadata that describes that file. To store an object in Amazon S3, you upload the file you want to store into a bucket. When you upload a file, you can set permissions on the object and add any metadata.

Buckets are logical containers for objects. You can have one or more buckets in your account and can control access for each bucket individually. You control who can create, delete, and list objects in the bucket. You can also view access logs for the bucket and its objects and choose the geographical region where Amazon S3 will store the bucket and its contents.


