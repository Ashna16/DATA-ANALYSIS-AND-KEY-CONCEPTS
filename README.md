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


There are three broad classifications of data source types:

Structured data is organized and stored in the form of values that are grouped into rows and columns of a table.

Semistructured data is often stored in a series of key-value pairs that are grouped into elements within a file.

Unstructured data is not structured in a consistent way. Some data may have structure similar to semi-structured data but others may only contain metadata.
