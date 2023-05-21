# SQL

Structured query language (SQL) is a programming language for storing and processing information in a relational database. A relational database stores information in tabular form, with rows and columns representing different data attributes and the various relationships between the data values. 
### What is SQL?
SQL is a domain-specific language used to query and manage data. It works by allowing users to query, insert, delete, and update records in relational databases. SQL also allows for complex logic to be applied through the use of transactions and embedded procedures such as stored functions or views.

### What is NoSQL?
NoSQL stands for Not only SQL. It is a type of database that uses non-relational data structures, such as documents, graph databases, and key-value stores to store and retrieve data. NoSQL systems are designed to be more flexible than traditional relational databases and can scale up or down easily to accommodate changes in usage or load. This makes them ideal for use in applications

### 5 differences between SQL and NoSQL
- SQL databases are relational, and NoSQL databases are non-relational.
- SQL databases use structured query language (SQL) and have a predefined schema. NoSQL databases have dynamic schemas for unstructured data.
- SQL databases are vertically scalable, while NoSQL databases are horizontally scalable.
- SQL databases are table-based, while NoSQL databases are document, key-value, graph, or wide-column stores.
- SQL databases are better for multi-row transactions, while NoSQL is better for unstructured data like documents or JSON

### What kind of data is a good fit for an SQL database? Give a real world example.

SQL databases are a good fit for data that is structured and relational, frequently updated. This means that the data is organized in a way that can be easily queried and manipulated. Since the ecommerce business need to have structured and updated order numbers and details, it's good fit to use SQL database.

### What kind of data is a good fit for an NoSQL database? Give a real world example.

NoSQL databases are a good fit for data that is not structured or relational. This means that the data does not fit neatly into a table, or that the relationships between different pieces of data are not well-defined. Since the social media posts and comments are unstructured it's good fit for NoSQL.

### Which type of database is best for hierarchical data storage?

Hierarchical data is a data structure in which data is organized in a tree-like structure. The data are stored as records which are connected to one another through links. NoSQL databases are a good choice for storing hierarchical data. NoSQL databases do not have a fixed schema, which means that they can store data in a variety of formats, including documents, key-value pairs, and graphs. MongoDB is one of the popular hierarchical data storages of NoSQL. 

### Which type of database is best for scalability?

NoSQL databases are generally more scalable than SQL databases. This is because NoSQL databases are designed to store and access data in a variety of formats, including documents, key-value pairs, and graphs. This makes NoSQL databases more flexible and adaptable to changes in data requirements.

- What does SQL stand for? Structured Query Language
- What is a relational database? Database that works certain way, like tables. 
- What type of structure does a relational database work with? SQL
- What is a ‘schema’? Strict path that decides which data goes where. 
- What is a NoSQL database? Has collections, documents. 
- How does it work? You don't have to follow schema. 
- What is inside of a MongoDB database? 
- Which is more flexible - SQL or MongoDB? and why. MongoDB is more flexible. 
- What is the disadvantage of a NoSQL database?


## 19 keypoints about NoSQL : 

NoSQL stands for "Not only SQL." It is a broad category of database systems that provide flexible, non-relational data storage solutions.

NoSQL databases are designed to handle large volumes of unstructured and semi-structured data, offering scalability, high performance, and horizontal scaling capabilities.

Unlike traditional relational databases, NoSQL databases do not use a fixed schema. They are schema-less or have a flexible schema, allowing for easy adaptation to changing data requirements.

NoSQL databases use a variety of data models, such as key-value, document, columnar, and graph. Each model is suited for different use cases and offers unique benefits.

Key-value stores are the simplest NoSQL databases, storing data as a collection of key-value pairs. They offer high performance for simple read/write operations and are often used for caching and session management.

Document databases store data in a semi-structured format, usually using JSON or XML. They provide flexibility for evolving data structures and are suitable for use cases like content management systems and real-time analytics.

Columnar databases organize data in columns rather than rows, making them efficient for handling large amounts of data and complex queries. They are commonly used for data warehousing and analytical workloads.

Graph databases model data using nodes and edges, representing relationships between entities. They excel in handling complex interconnections and are valuable for applications like social networks and recommendation systems.

NoSQL databases prioritize high availability and partition tolerance over consistency, as per the CAP theorem. This means that in the event of a network partition, they may sacrifice consistency to maintain availability and performance.

NoSQL databases often use distributed architectures and can be deployed across multiple servers or clusters. They provide horizontal scalability by adding more machines to the cluster, enabling efficient handling of large workloads.

ACID (Atomicity, Consistency, Isolation, Durability) properties, which are essential for transactional integrity, are often relaxed or not guaranteed in NoSQL databases. Instead, they may offer BASE (Basically Available, Soft-state, Eventually Consistent) properties, emphasizing availability and eventual consistency.

NoSQL databases offer flexible data replication and data partitioning strategies. Replication allows for data redundancy and fault tolerance, while partitioning enables distributing data across multiple nodes for better performance.

NoSQL databases are widely adopted in various industries, including e-commerce, social media, gaming, IoT, and big data analytics, due to their ability to handle large-scale, diverse, and real-time data.

NoSQL databases integrate well with modern application development frameworks and tools. Many NoSQL databases provide APIs, drivers, and libraries for popular programming languages, making it easier to work with them.

NoSQL databases can be complemented with traditional relational databases in a hybrid approach, often referred to as polyglot persistence. This allows for leveraging the strengths of both types of databases for different parts of an application.

NoSQL databases can have trade-offs in terms of data consistency and query flexibility. Developers need to carefully consider the specific requirements of their use case and choose the appropriate NoSQL database accordingly.

Common NoSQL databases include MongoDB, Couchbase, Cassandra, Redis, HBase, Neo4j, and DynamoDB. Each has its own strengths and weaknesses, so understanding their characteristics helps in selecting the right one for your needs.

NoSQL databases often provide horizontal scaling and fault tolerance through sharding, which involves dividing data into smaller subsets and distributing them across multiple nodes. Sharding can improve performance and handle increasing data volumes.

NoSQL databases can handle unstructured and semi-structured data
