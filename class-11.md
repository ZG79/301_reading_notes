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
