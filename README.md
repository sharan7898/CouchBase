# CouchBase

![CouchBase](/images/logo1.png)


## Introduction to CouchBase

Couchbase Server is an open-source, distributed, multi-model NoSQL, JSON document database that is enhanced for interactive applications. 

It is also known as Membase. It was developed by Couchbase, Inc. and initially released in August 2010.

It is written using C++, Erlang, C, Go languages.

Its server is designed to provide us with easy-to-scale key-value or JSON document access with high sustained throughput and low latency.

These applications may help in serving many users by storing, creating, aggregating, retrieving, manipulating and presenting data. 

## Why CouchBase

CouchBase is widely  used for its feauters such as:-

* It is an open-source NoSQL database that provides us with a mechanism for storage and recovery of data which is modeled in means other than the tabular relations used in relational databases.

* It is useful as it is optimized for interactive applications.

* It has schema-free Data Schema.

* It has multiple data access paths to query and manage our JSON documents.

* It supports Declarative Query Language (N1QL) that extends ANSI SQL to JSON.

* It has predefined data types such as boolean, string, number, etc.

* The primary database model for Couchbase is Document Store.

* The secondary database model for Couchbase is Key-Value Store.

* It supports XML data format.

* In Couchbase, the partitioning can be done by Sharding.

* It has in-memory capabilities.

* It provides ACID transaction concepts.

* It also supports secondary indexes without any restrictions.

* It has functions and timers in JavaScript for Server-side scripts.

## Difference Between RDBMS VS CouchBase

**1.RDBMS**

RDBMS stands for Relational Database Management Systems. 

It is most popular database. In it data is store in the form of row that is in the form of tuple. 

It contain numbers of table and data can be easily access because data is store in the table.

![RDBMS](/images/RDBMS.png)

**2.CouchBase**

Couchbase Server is an open-source, distributed multi-model NoSQL document-oriented database software package that is optimized for interactive applications. 

It is also known as Membase. 

It was developed by Couchbase, Inc. and initially released on August 2010.

![CouchBasedata](/images/couchbase_data.jpg)

### RDBMS VS CouchBase

|S.No.	|                   RDBMS	              |                 Couchbase                            |
|-------|-----------------------------------------|------------------------------------------------------|
|1.	    |RDBMS is a relational database.	      |It is a non-relational and document-oriented database.| 
|2.	    |RDBMS is column-based.	                  |Couchbase is field-based.                             |
|3.     |It has a predefined schema.	          |It has a dynamic schema.                              |
|4.     |It is slower in comparison with Couchbase.|	Couchbase is faster than RDBMS.|
|5.     |It supports SQL query language only.      |It supports JSON query language.|
|6.     |RDBMS does not provide JavaScript client for querying.	|It provides a JavaScript client for querying.|
|7.     |RDBMS is not suitable for hierarchical data storage.|	Couchbase is suitable for hierarchical data storage.|
|8.     |RDBMS is vertically scalable.	            |Couchbase is horizontally scalable.|
|9.     |It supports complex joins.	                |It doesn’t support for complex joins.|



## Difference Between CouchBase VS CouchDataBase 

**1.CoucBase**

Couchbase Server is an open-source, distributed multi-model NoSQL document-oriented database software package that is optimized for interactive applications.

It is also known as Membase. 

It was developed by Couchbase, Inc. and initially released on August 2010.

![Couchbasedata](/images/couchbase_data.jpg)

**2.CouchDB**

Apache CouchDB is an open-source document-oriented NoSQL database that uses multiple formats and protocols to store, transfer, and process its data, it uses JSON to store data, JavaScript as its query language using MapReduce, and HTTP for an API.

It was developed by Apache Software Foundation and initially released in 2005. It is written in Erlang.

![cdb](/images/cdb.png)


### CouchBase vs CouchDB

|S.No.	|                 CouchBase               |                 CouchDB                              |
|-------|-----------------------------------------|------------------------------------------------------|
|1.| Developed by Couchbase, Inc. and initially released on August 2010.|Developed by Apache Software Foundation and initially released in 2005.|
|2.|Couchbase is written in C++, Erlang, C and Go languages. |	CouchDB is written in Erlang. |
|3.|Couchbase have predefined datatypes such as boolean, string, number, etc.|	In CouchDB there is no predefined datatypes.|
|4.|Couchbase supports secondary indexes.	|CouchDB supports secondary indexes via views only.|
|5.|Couchbase supports Declarative query language (N1QL) that extends ANSI SQL to JSON. |	CouchDB do not have SQL support.|
|6.|Couchbase supports ACID transactions.| CouchDB does not supports ACID transactions.|
|7.|Couchbase has in-memory capabilities.|	CouchDB does not have any in-memory capabilities.|

## Advantages of CouchBase

* **High Performance and Scalability**: Couchbase is designed for high-performance, low-latency applications. It utilizes an in-memory caching model that allows for fast data access. Additionally, Couchbase's distributed architecture enables seamless scalability, allowing you to easily add more nodes to handle increasing data and traffic.

* **Flexible Data Model**: Couchbase offers a flexible data model with support for JSON documents. This allows you to store and query structured, semi-structured, and unstructured data without the need for rigid schemas. The flexible data model is particularly beneficial for applications that have evolving data requirements or require schema-less storage.

* **Full-Text Search Capabilities**: Couchbase provides built-in full-text search functionality. This feature allows you to perform complex searches across your data without the need for external search engines. It supports features like fuzzy matching, term boosting, and relevance ranking, enabling powerful search capabilities within your application.

* **High Availability and Data Durability**: Couchbase ensures high availability and data durability through built-in data replication and automatic failover mechanisms. It replicates data across nodes, ensuring that even in the event of node failures, your data remains accessible and your application can continue to operate.

* **Mobile Integration**: Couchbase offers seamless integration with mobile platforms through its embedded database called Couchbase Lite. It allows you to build mobile applications with offline capabilities and real-time data synchronization. Changes made on mobile devices can be synchronized with the Couchbase Server when connectivity is available.

* **Multi-Cloud and Hybrid Cloud Support**: Couchbase supports deployment across multiple cloud providers and on-premises environments. This flexibility allows you to build hybrid cloud architectures and take advantage of multi-cloud strategies. Couchbase provides features like cross-data center replication and data tiering, enabling data distribution and efficient resource utilization.

## Installation 

First-time users can get Couchbase Server running simply and rapidly by using Docker. Once you install Docker, you can use a single command to download and install a pre-configured version of Couchbase Server Enterprise Edition on your computer.

**Install Couchbase Server**

Prerequisite
Ensure that you have Docker set up on your computer before proceeding to install Couchbase Server. Refer to the https://www.docker.com/get-docker for instructions to set up Docker.

**NOTE** : 
You may need administrative or root privileges on your computer to complete the installation.

Open a console window on your computer and enter the following command:

```

docker run -t --name db -p 8091-8096:8091-8096 -p 11210-11211:11210-11211 couchbase/server:enterprise-7.2.0


```

When you run the command, Docker downloads and installs Couchbase Server. You should see the following message once Couchbase Server is started in a Docker virtual environment:

```
Starting Couchbase Server -- Web UI available at http://<ip>:8091
and logs available in /opt/couchbase/var/lib/couchbase/logs

```

![install](/images/install.png)

From this point onward, don’t close the console while you’re using Couchbase Server; this terminates both Docker and Couchbase Server.

You must now configure the server and load the travel-sample dataset.

### Configure Couchbase Server

For simplicity when getting started, we will provision a single node cluster from the Web Console. The Web console can be accessed over the network at http://<machine-ip-address>:8091/ or http://<machine-hostname>:8091/. It can be accessed from the machine on which Couchbase Server was installed at http://localhost:8091.

Once you have connected, the Welcome screen appears:

![CB](/images/CB.png)

Click Setup New Cluster and provide a name for your cluster. For the purpose of getting started, set the full administrator credentials to Administrator and password.

![CB1](/images/CB1.png)

Accept the Terms and Conditions and click Finish with Defaults to complete configuration with default values. You can also choose to Configure Disk, Memory, Services to select only a subset of services for the purpose of this getting started.

![Cb2](/images/CB2.png)

When you have finished entering your configuration-details, click the Save & Finish button, at the lower right. This configures the server accordingly, and brings up the Couchbase Web Console Dashboard, for the first time.

![CB3](/images/CB3.png)

### Load the Sample Dataset

You must load the sample travel-sample dataset to work through the rest of the Getting Started topics.

On the initial screen of the Web Console Dashboard, click the link Sample Buckets.

![CB5](/images/CB5.png)

On the Sample Buckets screen, select the checkbox for travel-sample and then click Load Sample. The travel-sample dataset is now displayed under Installed Samples.


### Other Installations

1.[Installing the Couchbase Server Cluster](https://docs.couchbase.com/server/current/install/install-intro.html): Explains how to install Couchbase Server directly onto your host, without the use of Docker or any other virtual environment. This kind of direct install is very common for production-deployments, as well as development and testing activities.

2.[Create a Cluster](https://docs.couchbase.com/server/current/manage/manage-nodes/create-cluster.html): Provides a detailed explanation of how to provision a Couchbase Server-node, and thereby create a one-node Couchbase cluster. This is the procedure you will certainly use in production; as well as for testing different configurations. The available options include use of the Couchbase Server Web Console, the Couchbase REST API, and the Couchbase Command Line Interface.

3.[Couchbase Server Startup and Shutdown](https://docs.couchbase.com/server/current/install/startup-shutdown.html): Explains how to start and stop the server using the commands that are specific to your underlying platform.

## CouchBase  Server Architecture

![server](/images/server1.png)

### Explaination


Couchbase Server Cluster Architecture:

Couchbase Server is designed as a distributed NoSQL database system, and its cluster architecture provides scalability, high availability, and fault tolerance. Here's an overview of the key components and concepts in the Couchbase Server cluster architecture:

* **Cluster**:A Couchbase Server cluster is a group of interconnected nodes that work together as a unified system. The cluster provides the foundation for a Couchbase deployment and enables horizontal scalability and fault tolerance. Nodes within the cluster collaborate to store, manage, and distribute data.

* **Node**:A node in Couchbase Server represents an individual server instance within the cluster. Each node can be a physical or virtual machine with its own CPU, RAM, and storage resources. Nodes are responsible for storing and managing data, handling queries, and participating in data replication and distribution.

* **Data Distribution**:Couchbase employs a partitioning mechanism called vBuckets (Virtual Buckets) to distribute and manage data across the nodes in the cluster. Each vBucket represents a subset of the data within a bucket and is responsible for storing a portion of the documents. Data is distributed across the vBuckets to achieve load balancing, fault tolerance, and efficient data access.

* **Data Replication**:Data replication in Couchbase Server provides redundancy, high availability, and fault tolerance. Each document is replicated across multiple nodes in the cluster, ensuring that there are redundant copies of the data. Replication allows for failover in case of node failures and maintains data consistency and durability.

* **Failover and High Availability**:Couchbase Server supports automatic failover, which means that in the event of a node failure, the system automatically detects the failure and promotes a replica node to take over the failed node's responsibilities. This ensures high availability and continuous operation even in the presence of node failures. Failover is based on the concept of maintaining replica copies of data.

* **Rebalancing**:Rebalancing is the process of redistributing the data and workload across the nodes in the cluster. When adding or removing nodes from the cluster, Couchbase Server automatically rebalances the data to ensure an even distribution and optimal resource utilization. Rebalancing helps maintain performance, data distribution, and cluster stability.

* **Indexing and Querying**:Couchbase Server provides indexing and querying services to enable efficient data retrieval and querying. The Index Service allows you to create and manage indexes on specific fields or attributes within documents, facilitating faster querying. The Query Service allows executing SQL-like queries using the N1QL query language to retrieve and manipulate data.

* **Memory and Disk Storage**:Couchbase Server utilizes memory for caching frequently accessed data, indexes, and control structures. Memory caching improves read and write performance. Disk storage is used for long-term data persistence, ensuring data durability and availability even when the server is restarted or shut down.

* **Management and Monitoring**:Couchbase Server provides management and monitoring tools, including the Couchbase Web Console, command-line interface (CLI), REST API, and SDKs. These tools allow administrators to manage the cluster, configure settings, monitor performance, and perform administrative tasks.



## Data

* Couchbase Server saves data as items, each of which has a key and a value.

* Each item consists of a key and a value. Each key is unique within its bucket, and values can be either binary or JSON.

* **Keys** : Each value (binary or JSON) is identified by a unique key, defined by the user or application when the item is saved. The key is immutable: once the item is saved, the key cannot be changed.

Note that Couchbase also refers to an item’s key as its id.

* **Values** : The maximum size of a value is 20 MiB. A value can be either:

**Binary**: Any form of binary is acceptable. Note that a binary value cannot be parsed, indexed, or queried: it can only be retrieved by key.

**JSON**: A JSON value, referred to as a document, can be parsed, indexed, and queried. Each document consists of one or more attributes, each of which has its own value. An attribute’s value can be a basic type, such as a number, string, or Boolean; or a complex, such as an embedded document or an array.

* **Document Structure** : A sample JSON document is provided immediately below. Its contents are as follows:

```

{
  "a1" : number,
  "a2" : "string",
  "a3" : {
    "b1" : [ number, number, number ]
    },
  "a4" : [
    { "c1" : "string", "c2" : number },
    { "c1" : "string", "c2" : number }
  ]
}


```

1.a1 and a2 are attributes that respectively have a single number and a single string as their values.

2.a3 is an attribute whose value is an embedded document consisting of a single attribute, b1, whose own value is an array of three numbers.

3.a4 is an attribute whose value is an array of two documents, each document consisting an attribute (c1 or c2) whose own values are respectively a string and a number.

* **Sub-Documents** : A sub-document is an inner component of a JSON document. The sub-document is referred to by a path, which specifies attributes and array-positions.

The example given above includes the following paths:

a1, whose value is a number.

a3.b1, whose value is an array of numbers.

a3.b1[0], whose value is the first number in an array.

a4[1].c2, whose value is a number.

* **Metadata** : Metadata is automatically generated and stored for each item saved in Couchbase Server. For example, the following document, which contains airport-information, has been saved with the key airport_1306:

JSON

```
{
  "airportname": "Brienne Le Chateau",
  "city": "Brienne-le Chateau",
  "country": "France",
  "faa": null,
  "geo": {
    "alt": 381,
    "lat": 48.429764,
    "lon": 4.482222
  },
  "icao": "LFFN",
  "id": 1306,
  "type": "airport",
  "tz": "Europe/Paris"
}

```

Couchbase Server generates metadata in association with the document, when the document is saved. The metadata might be as follows:

JSON

```
{
  "meta": {
    "id": "airport_1306",
    "rev": "1-1526338d1bbb00000000000002000000",
    "expiration": 0,
    "flags": 33554432,
    "type": "json"
  },
  "xattrs": {}
}

```

The attributes within the metadata are:

1.meta: The attribute whose value is the standard metadata for the saved document, airport_1306.

2.id: The key of the saved document, which is airport_1306.

3.rev: The revision or sequence number. This value is for internal server-use only: it is used in the resolution of conflicts that occur when replicated documents are updated concurrently on different servers, representing the number of times the document has been mutated. For more information, see XDCR Conflict Resolution.

4.expiration: The expiration-time (or Time-To-Live) of the document. If non-zero, this determines the point at which the document is removed from the system. The value can be set either per-document, by means of Couchbase SDK APIs (which is referred to as TTL); or per bucket, by means of Couchbase Web Console, the Couchbase CLI, or the Couchbase REST API (which is referred to as Bucket TTL).

5.flags: Couchbase SDK-specific values that may be used to identify the type of data saved, or to specify formatting.

6.type: The type of the saved value, which in this case is json.

7.xattrs: Extended Attributes, which constitute a special kind of metadata, some of which is system-internal, some of which can optionally be written and read by user-applications.

### Data Model

1.**Documents versus Tables**

* The nature and value of the document data model is clarified by comparison with the relational. 

* To support an online flight-booking application, allowing users to search for flights by date, the relational model requires multiple tables — for flights, airlines, and schedules. The result may be as follows:

![tables](/images/relationalDataModel.png)


By contrast, the document model likely requires only a single document, which embeds an array of schedules for all flights between each of two airports:

![documents](/images/jsonDataModel.png)

* Thus, in the document model, each document can be highly self-contained. 

* This supports the rapid fulfillment of application-requests, and has important implications for both scalability and latency: one document can be replicated, or atomically changed, without other documents needing to be accessed; eradicating the need for complex inter-node coordination, and minimizing contention.

2.**Flexible, Dynamic Schema**


In the document model, a schema is the result of an application’s structuring of its documents: schemas are entirely defined and managed by applications. A document’s structure consists of its inner arrangement of attribute-value pairs.

Couchbase Server does not enforce uniformity: document-structures can vary, even across multiple documents that each contain a type attribute with a common value. This allows differences between objects to be represented with great efficiency. It also allows a schema to be progressively evolved by an application, as required: properties and structures can be added to the document, without other documents needing to be updated in the same way. (This flexibility is especially advantageous when the application itself is large and long-lived.)

3.**Querying with N1QL**: N1QL (pronounced "nickel") is a SQL-like query language provided by Couchbase. It allows you to perform complex queries, filtering, sorting, and aggregation operations on the JSON documents stored in Couchbase. N1QL provides a familiar SQL syntax with extensions to handle the flexible nature of JSON data.

## Buckets

In Couchbase, a bucket is a logical container that holds a collection of documents. It is a fundamental component of the data organization in Couchbase Server. Buckets allow you to group related data together and apply specific configurations and settings to that data.

Here are some key points to understand about buckets in Couchbase:

1.**Data Grouping**: Buckets are used to organize documents based on their data type, application, or any other logical grouping. For example, you might create separate buckets for user profiles, product catalogs, or session data. Each bucket represents a separate namespace for documents.

2.**Isolation and Security**: Buckets provide data isolation and security within Couchbase. Each bucket has its own set of access controls and permissions, ensuring that different applications or users can access only the data within their designated buckets. This allows for multi-tenancy and secure separation of data.

3.**Configuration Settings**: Each bucket can have its own configuration settings, including memory quota, replication factor, durability settings, and data eviction policies. These settings allow you to control how data is stored, replicated, and managed within each bucket.

4.**Memory Allocation**: Couchbase uses memory to cache frequently accessed data for faster retrieval. Each bucket has a specific memory quota, which determines the maximum amount of RAM that can be allocated to store and cache documents within that bucket.

5.**Replication and High Availability**: Buckets can be configured with a replication factor, which determines the number of copies of each document that should be stored across the Couchbase cluster. Replication provides data redundancy, high availability, and fault tolerance in case of node failures.

6.**Querying and Indexing**: Buckets can be indexed to optimize query performance. Indexes allow you to create efficient lookup structures on specific fields or attributes within the documents stored in the bucket. Indexing enables faster querying and filtering of data.

7.**Backup and Restore**: You can perform backup and restore operations at the bucket level. This allows you to create backups of specific buckets and restore them when needed, providing data recovery and disaster resilience capabilities.

**NOTE**: It's important to note that the resources allocated to a bucket, such as memory quota, affect the overall resource usage of the Couchbase cluster. Therefore, it's crucial to plan and allocate resources wisely to ensure optimal performance and scalability

### V Bucket

In Couchbase, a vBucket (short for "Virtual Bucket") is a partitioning mechanism used for distributing and managing data across the nodes in a Couchbase cluster. It is a logical representation of data partitioning within the cluster.


In Couchbase, a vBucket (short for "Virtual Bucket") is a partitioning mechanism used for distributing and managing data across the nodes in a Couchbase cluster. It is a logical representation of data partitioning within the cluster.

Here are key points to understand about vBuckets:

1.**Data Distribution**: Couchbase divides the data stored in a bucket into multiple vBuckets. Each vBucket represents a subset of the data within the bucket. The data is distributed across the nodes in the cluster based on the number of vBuckets.

2.**Consistent Hashing**: Couchbase employs a consistent hashing algorithm to determine which vBucket a document belongs to. The hashing algorithm takes the document's key as input and maps it to a specific vBucket. This ensures that documents with similar keys are likely to be stored on the same node.

3.**Fault Tolerance**: vBuckets play a crucial role in providing fault tolerance and high availability. Couchbase replicates each vBucket's data across multiple nodes, ensuring that there are redundant copies of the data. In the event of a node failure, the cluster can quickly recover by promoting the replicas of the affected vBuckets.

4.**Load Balancing**: vBuckets also facilitate load balancing within the cluster. As nodes are added or removed from the cluster, vBuckets are automatically redistributed across the available nodes, ensuring that data is evenly distributed and preventing hotspots or imbalanced resource utilization.

5.**Data Operations**: When performing data operations such as storing, retrieving, or updating documents, the vBucket mapping determines which node in the cluster is responsible for handling that operation. The client SDKs or APIs interact with the appropriate node based on the vBucket mapping for the given document's key.

6.**Flexibility and Scalability**: The use of vBuckets allows Couchbase to scale horizontally by adding or removing nodes from the cluster. As new nodes join, the vBuckets are automatically rebalanced across the cluster, maintaining data distribution and balancing the workload.

![vbucket](/images/vbucketToNodeMapping.png)

Overall, vBuckets provide a scalable and fault-tolerant mechanism for data distribution and management in a Couchbase cluster. By dividing the data into smaller partitions and replicating them across nodes, Couchbase ensures high availability, load balancing, and efficient data operations within the cluster.

### Compression

* In Couchbase, compression refers to the process of reducing the size of data before storing it in the database. Couchbase provides built-in compression functionality to help optimize storage efficiency and reduce network bandwidth usage.

* When compression is enabled in Couchbase, the database automatically compresses the data before storing it on disk. This helps to reduce the storage space required and can improve overall performance by reducing disk I/O and network bandwidth usage.

* The compression of data allows RAM and disk-space to be used with increased efficiency

* Couchbase uses a compression algorithm called Snappy by default. Snappy is a fast, lightweight, and widely used compression algorithm that provides a good balance between compression ratio and speed.

* Compression can be enabled or disabled at the bucket level during bucket creation or configuration using the Couchbase Management Console or programmatically via the Couchbase SDKs.

* It's important to note that compression in Couchbase is transparent to the application. The application doesn't need to handle compression or decompression explicitly; it's handled automatically by the Couchbase server. 

* The data is compressed when written to disk and automatically decompressed when retrieved by the application.

* The decision to use compression in Couchbase depends on factors such as data characteristics, storage requirements, network constraints, and performance considerations. Careful evaluation and testing should be performed to determine the optimal compression configuration for your specific use case.

* Compression is available only in Couchbase Enterprise Edition, and can be applied only to Couchbase and Ephemeral buckets. Compression applies to both binary and JSON items

## Scopes and Collections

**Collections**

* A collection is a logical container within a scope that holds a group of related documents.Up to 1000 collections can be created per cluster.

* Item-names must be unique within their collection.

* Collections provide a way to further partition data within a scope based on a specific category or type.

* Collections can be used to organize and manage data with finer granularity, allowing for more efficient querying and indexing within a scope.

* Each scope can have multiple collections, and each collection can contain multiple documents.

**Scopes**

* A scope is a mechanism for the grouping of multiple collections. Up to 1000 scopes can be created per cluster. Collection-names must be unique within their scope

* Scopes provide a way to group collections together based on a specific application or domain.

* Scopes can be used to separate and isolate different sets of collections within a bucket, allowing for better organization and management of data.

* Each bucket can have multiple scopes, and each scope can contain multiple collections.

![scopes](/images/Picture2.png)

### Benefits and Use Cases

1.**Logical Data Organization**: Scopes and collections enable you to organize data hierarchically based on different applications, modules, or data types within a bucket. This enhances the overall data structure and provides a more meaningful organization for data management.

2.**Data Isolation and Access Control**: Scopes and collections allow for fine-grained access control and isolation of data. You can set permissions at the scope or collection level, providing better control over data access for different applications or users.

3.**Improved Query Efficiency**: Scopes and collections enable more targeted querying and indexing within specific subsets of data. By partitioning data into collections, you can create more focused indexes, resulting in improved query performance and reduced index size.

4.**Reduced Index Maintenance**: With scopes and collections, you can create indexes on specific collections, reducing the index size and maintenance overhead compared to indexing the entire bucket.

5.**Simplified Application Development**: Scopes and collections provide a more intuitive and meaningful structure for application developers, allowing them to work with smaller subsets of data within a bucket and providing a more natural organization for application logic.

## Indexes
  
Couchbase Server indexes enhance the performance of query and search operations.

Indexes are used by certain services, such as Query, Analytics, and Search, as targets for search-routines. Each index makes a predefined subset of data available for the search.

The Query service relies on indexes provided by the Index service. The Search and Analytics services both provide their own indexes, internally.

Indexes, when well-designed, provide significant enhancements to the performance of search-operations.

**Indexes**

The following forms of index are available:

**Primary**

Provided by the [Index Service](https://docs.couchbase.com/server/current/learn/services-and-indexes/services/index-service.html), this is based on the unique key of every item in a specified collection. Every primary index is maintained asynchronously. A primary index is intended to be used for simple queries, which have no filters or predicates. For information on primary indexes, see Using [Indexes](https://docs.couchbase.com/server/current/learn/services-and-indexes/indexes/global-secondary-indexes.html).

**Secondary**

Provided by the [Index Service](https://docs.couchbase.com/server/current/learn/services-and-indexes/services/index-service.html), this is based on an attribute within a document. The value associated with the attribute can be of any type: scalar, object, or array.

A Secondary Index is frequently referred to as a Global Secondary Index, or GSI. This is the kind of index used most frequently in Couchbase Server, for queries performed with SQL++. For information on Global Secondary Indexes, see Using [Indexes](https://docs.couchbase.com/server/current/learn/services-and-indexes/indexes/global-secondary-indexes.html).

**Full Text**

Provided by the [Search Service](https://docs.couchbase.com/server/current/learn/services-and-indexes/services/search-service.html), this is a specially purposed index, which contains targets derived from the textual contents of documents within one or more specified keyspaces. Text-matches of different degrees of exactitude can be searched for. Both input and target text-values can be purged of irrelevant characters (such as punctuation marks or html tags). For information on how to create Full Text Indexes, see [Creating Indexes](https://docs.couchbase.com/server/current/fts/fts-creating-indexes.html).

**Analytics**

Provided by the [Analytics Service](https://docs.couchbase.com/server/current/learn/services-and-indexes/services/analytics-service.html), this is a materialized access path for the shadow data in an Analytics collection. Analytics indexes can be used to speed up Analytics selection queries and join queries. If changes in operational data result in corresponding modifications to shadow data, Analytics indexes are updated automatically. See the section on Using [Indexes](https://docs.couchbase.com/server/current/learn/services-and-indexes/indexes/global-secondary-indexes.html). in Couchbase Analytics.

**View**

Supports Couchbase [Views](https://docs.couchbase.com/server/current/learn/views/views-intro.html), with fields and information extracted from documents. Views are deprecated in Couchbase Server 7.0, and will be removed in a future release.


## Expiration

1.Time To Live (TTL) imposes a maximum lifespan on items within a bucket or a collection, and thus ensures the expiration of such items, once the specified period is complete.

2.It allows you to define an expiration time for a document, after which Couchbase automatically removes the document from the bucket. 

3.TTL is a non-negative integer-value, specified per bucket or per collection, that determines the maximum expiration time of individual items within the bucket or collection

4.if TTL is enabled, each newly created item lives for the number of seconds specified by TTL, following the item’s creation. 

5.After its expiration time is reached, the item will be deleted by Couchbase Server. Deleted items and their contents are no longer available access-attempts are treated as if the items never existed.

6.The maximum value for TTL is MAX32INT seconds (2147483648, or 68.096 years). The default value is 0, which indicates that TTL is disabled. If TTL is changed from the default, it is thereby enabled.

Whenever TTL is modified, items that existed prior to the modification:

* Remain subject to the previous TTL, if TTL was previously enabled.

* Remain subject to no TTL, if TTL was not previously enabled.

Items created or modified following the modification of TTL are subject to the modified TTL.

**NOTE**:  TTL can be established on collections: it cannot be established on scopes. TTL is only available in the Enterprise Edition of Couchbase Server.

### Expiration: Bucket, Collection, and Item

In cases where an item has a TTL, the item’s TTL may need to be modified, depending on the TTL of either its bucket or its collection:

* If an item resides within a collection that has no TTL, and the collection resides within a bucket that does have a TTL, the bucket’s TTL is used to determine whether and how the item’s TTL is modified.

* If an item resides within a collection that has its own TTL, and the collection resides within a bucket that has no TTL, the collection’s TTL is used to determine whether and how the item’s TTL is modified.

* If an item resides within a collection that has its own TTL, and the collection resides within a bucket that also has its own TTL, the bucket’s TTL is ignored, and only the collection’s TTL is used, to determine whether and how the item’s TTL is modified.

Determination of whether and how to modify the item’s TTL is as follows. If a new item’s TTL is:

* Above that of the bucket’s or the collection’s TTL, the item’s TTL is reduced to the value of the bucket’s or the collection’s TTL.

* Below that of the bucket’s or the collection’s TTL, the item’s TTL is left unchanged.

* 0, the item’s TTL is reset to the value of the bucket’s or the collection’s TTL.

## Memory and Storage

To facilitate high-speed data-access, Couchbase Server provides a caching layer and tunable disk I/O priorities.

In Couchbase, memory and storage are two important components that play distinct roles in the functioning and performance of the database system.

1. **Memory:**

Memory in Couchbase refers to the RAM (Random Access Memory) resources allocated to the database server. Couchbase utilizes memory in several ways:

* **Data Caching**: Couchbase caches frequently accessed data in memory to provide fast read and write operations. Storing data in memory reduces the need to fetch it from disk, leading to lower latency and improved performance.

* **Indexes**: Couchbase uses memory to store indexes, which are data structures that facilitate efficient querying of the data. Indexes help optimize query performance by providing quick access to specific fields or attributes within the documents.

* **Metadata and Control Structures**: Couchbase maintains various metadata and control structures in memory to manage and coordinate the distributed nature of the database system. This includes information about cluster topology, data partitioning, replication, and more.

The amount of memory allocated to Couchbase can be configured through settings such as memory quotas and cache configurations. Allocating an appropriate amount of memory is crucial for optimal performance and ensuring that frequently accessed data and indexes are stored in memory for fast access.

**2.Storage:**

Storage in Couchbase refers to the persistent storage medium where data is stored for long-term durability and availability. Couchbase supports different storage backends, including disk-based storage and solid-state drives (SSDs).

* **Disk Storage**: Couchbase stores data on disk, allowing for persistence even when the server is restarted or shut down. Disk storage provides durability and allows for storing larger datasets that may not fit entirely in memory.

* **Persistence Options**: Couchbase offers different persistence options, such as full persistence and memory-optimized persistence, which determine how data is written to disk and managed in conjunction with memory.

Disk storage is used for long-term storage and durability, while memory caching enhances performance by keeping frequently accessed data and indexes in memory for faster access. The combination of memory and disk storage in Couchbase provides a balance between performance and durability, catering to various use cases and data requirements.

It's important to allocate memory and configure storage appropriately based on the specific workload, dataset size, and performance requirements of your Couchbase deployment. Proper memory and storage management are crucial for achieving optimal performance, scalability, and durability in a Couchbase environment.

## Services

Couchbase provides several services that work together to offer a comprehensive NoSQL database solution. Each service in Couchbase serves a specific purpose and contributes to the overall functionality and performance of the database system. Here's an overview of the key services in Couchbase:

**Data Service**:The Data Service is responsible for storing and managing data within Couchbase. It handles operations related to data storage, retrieval, update, and deletion. The Data Service ensures high availability, fault tolerance, and data replication across nodes in the cluster.

**Index Service**:The Index Service enables efficient querying of data by creating and maintaining indexes. It allows you to create indexes on specific fields or attributes within documents, enabling faster data retrieval based on those indexed fields. The Index Service optimizes query performance and supports various indexing options to suit different use cases.

**Query Service**:The Query Service provides a powerful SQL-like query language called N1QL (pronounced "nickel") for querying and manipulating data in Couchbase. It allows you to perform complex queries, filtering, sorting, and aggregation operations on the data. The Query Service supports joins, subqueries, and a range of built-in functions to facilitate flexible and expressive querying.

**Full-Text Search Service**:The Full-Text Search Service offers powerful and efficient full-text search capabilities within Couchbase. It allows you to create search indexes on specific fields and perform advanced search operations, including keyword search, fuzzy matching, relevance ranking, and facets. The Full-Text Search Service enhances the search capabilities of Couchbase applications.

**Analytics Service**:The Analytics Service is designed for performing complex analytical queries and processing large volumes of data within Couchbase. It enables you to execute ad-hoc queries, aggregations, and transformations on large data sets using a SQL-based query language called N1QL for Analytics. The Analytics Service supports distributed processing and allows for real-time analytics on live data.

**Eventing Service**:The Eventing Service allows you to define and execute event-driven functions or business logic within Couchbase. It enables you to create functions that respond to changes in the data, such as document mutations, and trigger custom operations. The Eventing Service integrates with other Couchbase services and provides a flexible and extensible way to build reactive and event-driven applications.

**Management Service**:The Management Service encompasses various administrative and management features in Couchbase. It provides tools and interfaces for cluster management, configuration, monitoring, and troubleshooting. The Management Service includes the Couchbase Web Console, command-line interface (CLI), REST API, and SDKs for programmatic management and automation.

## CouchBase Capella

**Capella Overview**

* Couchbase Capella is the easiest way to use the Couchbase NoSQL database and its many services, from SQL-like querying to connecting to mobile devices at the edge with App Server.

* Capella offers sophisticated multi-model capabilities including JSON document query, relational data structures, key-value access, full-text search, and real-time analytics. Operational, transactional, and analytical workloads are all supported. 

* You can Access the data using one of 10 SDKs in conjunction with your favorite programming language.

* Capella’s built-in high-performance cache and memory-first architecture can deliver the same lightning-fast results for the millionth user as for the first. 

* Capella offers a familiar database experience with its SQL++ query language, which supports a wide range of advanced query syntax, ACID transactions across documents, and massive parallel processing analytic functionality

* As a database-as-a-service, Capella automates steps like setup, backups, scaling, upgrades, and ongoing management, so teams can drastically reduce their operational costs.

## Get Started with CouchBase Capella

Firstly You need to signup for CouchBase Capella in order to use the CouchBase Capella Services.Click on the link given below and signup 

https://cloud.couchbase.com/sign-up

Once you log into Capella, you probably see a screen similar to this one. 

![capella](/images/capella1.png)

you can see that your setup is completes and sample data has been preloaded for you. This data set is based on the travel industry and contains thousands of Json documents. In the bottom section you are presented with links for important next steps. Capella has been designed to make it as easy as possible to get started quickly.

Lets start with a document viewer. Couchbase is a document database which provides great flexibility and how data is structured.

![capella](/images/capella2.png)

Here we see a subset of documents organised in the Airline collection within the inventory scope. Scopes in collections are ways to virtually organise data that is extremely flexible. It can be used from multi tenant design or align to a relational model when migrating from an RDBMS.

Data is being retrieved behind the scenes via the Key Value Data service. Key Value access is the fastest method for retrieving data from Capella.

![capella](/images/capella-kv.png)

We can see the documents inside the collection. This is similar to seen the rows in a table, but you don't need to go all the way here just to see the documents of a collections. One can visit an option called Query.



### Query

Here in the above  Query lets say we need to select hotels in France using to travel-simple bucket limitng to 10. We execute the query in SQL++

```
SELECT * FROM 'travel-sample'.inventory.hotel WHERE country = 'France' limit 10

```

![capella3](/images/capella3.png)

The above query can be executed in different way by selecting the  Bucket to travel-sample and also selecting the inventory.

```

SELECT * FROM hotel WHERE country = 'France' limit 10

```

![capella4](/images/capella4.png)

One Can refer the video for Complete Capella Demo : https://www.youtube.com/watch?v=zY5qbr4NHRU&list=PLociSetSILasi-Y7oLdSi24S7xPtdyg-c&index=2

### Creating a bucket

Let's go back to Buckets and create a new one by clicking on Create new buckets. 

![bucket](/images/bucket.png)

Let us give the name User Profile ,and specify the memory quota for a buckets. For now let's specify 500 megabytes.

![bucket](/images/bucket1.png)

Click Create Bucket to Create a new bucket with the name user_profile having a memory of 500mb.

![bucket](/images/bucket2.png)

### Connecting App to our Bucket

Before we connect our app to our bucket with you need to do 2 things. Add our IP address to the Capella List and create the credentials to access our database.

Step 1: Go to connect tab in navigation

![cred](/images/cred.png)

Step 2 :  To Create an Permanent IP address click on the Allowed IP address as shown and then click
on Add Allowed IP button to create an Permanent IP. 

![cred](/images/cred4.png)

![cred](/images/cred5.png)

Step 3 :  create a database access credentials as shown in the image by specifiying the username and password.

![cred](/images/cred2.png)

![cred](/images/cred1.png)


### Connecting App from locally to Cluster

Step 1 : Connecting App from locally to Cluster using Springboot

* Go to the link https://github.com/couchbase-examples and select the java-springboot-quickstart
and Clone the Project locally in a folder. 

* Open the Project in STS and open Application.properties

Step 2 : Open the Application.properties and add the capella credentials as shown in the image

![host](/images/host1.png)

Step 3 : Run the Application file in the src/main/java then u will get an following output of Swagger-ui.

![host](/images/host2.png)

### Adding user 

* Expand the profile Controller in swagger output and click on try-it-out to add user  and Execute.

![user](/images/user.png)

* One can see that the Profile details we added is stored in user profile collection in the profileController.java file.

![user](/images/user1.png)

* Go to Capella and run the Query to ensure that the user has been added to the database.

![user](/images/user3.png)

### Add Collections

* Go to Buckets and click on the Bucket(user_profile) you have created.

![col](/images/col2.png)

* Click on the default scope or you can create an scope if you want.

![col](/images/col3.png)

* Click on the create collection and give the collection name which you want to give

![col](/images/col5.png)

### Adding Index

* Lets create an Index for a Collection, its a mandatory process in order to query the data

* Go to Query tab and execute the following Query 

![index](/images/index.png)

* Here you are creating an index for a product collection in the Scope for a Bucket user_profile.

* onceu execute the Query the index will be created.

![index](/images/index1.png)

### Creating an Entity

In Couchbase, an "entity" refers to a document or object that you want to store and manage within a bucket. It represents a piece of data that you want to persist in Couchbase.

* Go to STS and create a new class in the model called Product.

![entity](/images/entity.png)

* Create two attributes called pid and name and generate getter and setter methods.

![entity](/images/entity2.png)

* Copy the ProfileController in the controller and then paste it as a ProductController

* Change the Request mapping url to product

![entity](/images/entity3.png)

```

package org.couchbase.quickstart.controllers;

import static org.couchbase.quickstart.configs.CollectionNames.PRODUCT;

import java.util.Arrays;
import java.util.List;
import java.util.UUID;

import com.couchbase.client.core.error.DocumentNotFoundException;
import com.couchbase.client.core.msg.kv.DurabilityLevel;
import com.couchbase.client.java.Bucket;
import com.couchbase.client.java.Cluster;
import com.couchbase.client.java.Collection;
import com.couchbase.client.java.json.JsonObject;
import com.couchbase.client.java.query.QueryOptions;
import com.couchbase.client.java.query.QueryScanConsistency;
import com.couchbase.client.java.transactions.TransactionQueryOptions;
import com.couchbase.client.java.transactions.config.TransactionOptions;

import org.couchbase.quickstart.configs.DBProperties;
import org.couchbase.quickstart.models.Product;
import org.couchbase.quickstart.models.Profile;
import org.couchbase.quickstart.models.ProfileRequest;
import org.springframework.http.HttpStatus;
import org.springframework.http.MediaType;
import org.springframework.http.ResponseEntity;
import org.springframework.web.bind.annotation.CrossOrigin;
import org.springframework.web.bind.annotation.DeleteMapping;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.PathVariable;
import org.springframework.web.bind.annotation.PostMapping;
import org.springframework.web.bind.annotation.PutMapping;
import org.springframework.web.bind.annotation.RequestBody;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RequestParam;
import org.springframework.web.bind.annotation.RestController;

import io.swagger.annotations.ApiOperation;
import io.swagger.annotations.ApiResponse;
import io.swagger.annotations.ApiResponses;

@RestController
@RequestMapping("/api/v1/product")
public class ProductController {

    private Cluster cluster;
    private Collection profileCol;
    private DBProperties dbProperties;
    private Bucket bucket;

    public ProductController(Cluster cluster, Bucket bucket, DBProperties dbProperties) {
      System.out.println("Initializing profile controller, cluster: " + cluster + "; bucket: " + bucket);
        this.cluster = cluster;
        this.bucket = bucket;
        this.profileCol = bucket.collection(PRODUCT);
        this.dbProperties = dbProperties;
    }


    @CrossOrigin(value="*")
    @PostMapping(path = "/", produces = MediaType.APPLICATION_JSON_VALUE)
    @ApiOperation(value = "Create a product from the request")
    @ApiResponses({
            @ApiResponse(code = 201, message = "Created", response = Profile.class),
            @ApiResponse(code = 400, message = "Bad request", response = Error.class),
            @ApiResponse(code = 500, message = "Internal Server Error", response = Error.class)
    })
    public ResponseEntity<Product> save(@RequestBody final Product product) {
       

        try {
            profileCol.insert(product.getPid(), product);
            return ResponseEntity.status(HttpStatus.CREATED).body(product);
        } catch (Exception e) {
            return ResponseEntity.status(HttpStatus.INTERNAL_SERVER_ERROR).body(null);
        }
    }

   
}


```

U can copy the code and paste in the ProductController class.

**Note:** Do not forget to create a collection named called product in the CollectionNames.java

![entity](/images/entity5.png)

* The OutPut will have a Product controller where u can post product details.Once u have posted u can query to see the results.

![entity](/images/entity4.png)

### Importing a data

* One can Import the data of Json or CSV  format to the Bucket.

* If we go to the dataset in src/main/resources one can find that the data consisting of 10 users and 1 product.Lets import this data in Capella.

* Click on the import in the side-menu bar, and click import button to import your data 

![import](/images/import1.png)

* Select the Bucket and click next

![import](/images/import2.png)

* Select the File type as JSON and Format type as List and upload the document.

![import](/images/import3.png)

* Here Select as Custom Collection mapping.Enter the Collection Mapping Expression as **-default.%myCollectionName%** and in testing and mapping add one of the user collection for testing purposes.

![import](/images/import4.png)

The **-default.%myCollectionName%** defines the collection name will be the value of this my collection name attribute.

* Select the Custom Generation as we have given key in the document and give the Key Name Generator Expression as **%pid%** and in testing and mapping add one of the user collection for testing purposes.

![import](/images/import7.png)

* Click next for Configurations page click next and Click import for the Importing data.





