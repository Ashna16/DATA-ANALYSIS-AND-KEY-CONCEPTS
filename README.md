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

The collect component is where the services assemble data from many sources.
The store component stores data in repositories.
The process component is where services manipulate data into needed forms.
The consume component is where data is presented in the required formats.


WHAT ARE THE 5 V's OF DATA ANALYSIS?

Volume: 
Volume means the amount of data that will be ingested by the solution - the total size of the Data coming in. Solutions must work efficiently across distributed systems and be easily expandable in order to accommodate spikes in traffic.

Velocity : 
Velocity means the speed of data entering a solution. Many organizations now require near real-time ingestion and processing of data.
The high velocity of data results in a shorter time to analyze than traditional data processing can provide.
Solutions must be able to manage this velocity efficiently. Processing systems must be able to return results within an acceptable time frame.

Variety:
Data can come from many different sources.Variety means the number of different sources and the types of sources -
that the solution will use.
Solutions need to be sophisticated enough to manage all the different types of data while providing accurate analysis of the data.

Veracity : 
Veracity is the degree to which data is accurate, precise, and trusted. It is contingent on the integrity and trustworthiness of the data
Solutions should be able to identify the common flaws in the data and fix them before the data is stored. This is. known as data cleansing. This process must be able to be completed within the time requirements of the solution, up to and including real-time processing speeds.

Value :
Value is the ability for a solution to extract meaningful information from the data that has been stored and analyzed. Solutions must be
able to produce the right form of analytical results to inform business decision makers and stakeholders of insights using trusted reports and
dashboards.



THREE STEPS FOR DATA ANALYSIS SOLUTION:

1. Know where your data comes from

The majority of data ingested by data analysis solutions comes from existing on-premises databases and file stores. This data is often in a state where the required processing within the solution will be minimal.Streaming data is a source of business data that is gaining popularity. This data source is less structured. It may require special software to collect the data and specific processing applications to correctly aggregate and analyze it in near real-time.Public data sets are another source of data for businesses. These include census data, health data, population data, and many other datasets that help businesses understand the data they are collecting on their customers. This data may need to
be transformed so that it will contain only what the business needs.

2. Know the options for processing your data

There are many different solutions available for processing your data. There is no one-size-fits-all approach. You must carefully evaluate your business needs and match them to the services that will combine to provide you with the required results.
Throughout this course, we will cover the services that AWS offers for each of the components pictured below.

3. Know what you need to learn from your data

You must be prepared to learn from your data, work with internal teams to optimize efforts, and be willing to experiment.
It is vital to spot trends, make correlations, and run more efficient and profitabie businesses. It's time to put your data to work.




------------------------------------------------  VOLUME ---------------------------------------------------------------------------


There are three broad classifications of data source types:

Structured data is organized and stored in the form of values that are grouped into rows and columns of a table.

Semistructured data is often stored in a series of key-value pairs that are grouped into elements within a file, example the xml and json files. A very simple example of this can be the moves which one makes in the video games.

Unstructured data is not structured in a consistent way. Some data may have structure similar to semi-structured data but others may only contain metadata.

One way to deal with volume of data is by using Amazon S3

AWS has a storage service called Amazon Simple Storage Service, or Amazon S3 for short. This service is an object store, which means you can store just about any kind of discrete object in it. An object is how Amazon S3 refers to files. It’s a powerful service. It’s scalable and can grow to any size you need. It’s durable, meaning that your files will be there when you need them. It implements industry-leading scalability, security, and performance. People use Amazon S3 for websites, mobile applications, and data analytics, just to name a few use cases.

When you start using Amazon S3, you create buckets. They’re like file folders, only bigger, better organized, and with more security mechanisms. Next, you move data into the buckets. AWS gives you a lot of ways to do that, no matter how great the volume. You can even move exabytes in a single delivery.

There are three key ways that implementing Amazon S3 as your storage solution can improve your high-volume data analysis solution.

First, with Amazon S3, you can separate the way you store data from the way you process it. This is known as decoupling storage from processing. You may have separate buckets for raw data, temporary processing results, and final results.

Second is parallelization. With Amazon S3, you can access any of these storage locations from any process, in parallel, without negatively impacting other processes.
Finally, Amazon S3 becomes a central location to store analytical datasets, providing access for multiple analytic processes at the same time. This allows the solution to avoid the costly process of moving data between the storage system and processing system.


An object is composed of a file and any metadata that describes that file. To store an object in Amazon S3, you upload the file you want to store into a bucket. When you upload a file, you can set permissions on the object and add any metadata.

Buckets are logical containers for objects. You can have one or more buckets in your account and can control access for each bucket individually. You control who can create, delete, and list objects in the bucket. You can also view access logs for the bucket and its objects and choose the geographical region where Amazon S3 will store the bucket and its contents.

![SQL COMMANDS](https://explore.skillbuilder.aws/files/a/w/aws_prod1_docebosaas_com/1661378400/zgTyXzKSIeH_U9-IsY_l7A/tincan/c16bd0344c0123121a6326a58844db542da58ae5/assets/RSGn-ujAlWbihgr3_nCVTAu1gHj5zraGn.png)

Accessing your content
Once objects have been stored in an Amazon S3 bucket, they are given an object key. Use this, along with the bucket name, to access the object.

Below is an example of a URL for a single object in a bucket named doc, with an object key composed of the prefix 2006-03-01 and the file named AmazonS3.html.

![SQL COMMANDS](https://explore.skillbuilder.aws/files/a/w/aws_prod1_docebosaas_com/1661378400/zgTyXzKSIeH_U9-IsY_l7A/tincan/c16bd0344c0123121a6326a58844db542da58ae5/assets/Al_uS49WadqDYkVT_JlgrhfdoRaLOwsAS.png)

An object key is the unique identifier for an object in a bucket. Because the combination of a bucket, key, and version ID uniquely identifies each object, you can think of Amazon S3 as a basic data map between "bucket + key + version" and the object itself. Every object in Amazon S3 can be uniquely addressed through the combination of the web service endpoint, bucket name, key, and (optionally) version.

DATA LAKE


 A data lake is an architectural concept that helps you manage multiple data types from multiple sources, both structured and unstructured, through a single set of tools.
