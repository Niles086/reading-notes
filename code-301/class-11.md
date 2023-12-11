# MongoDB and Mongoose

Fill in the chart below with five differences between SQL and NoSQL databases:

SQL Databases:

Data Structure:

SQL databases are table-based and follow a fixed schema. Each table represents an entity, and rows in the table represent records. Columns define the attributes of the records.
Scaling:

Scaling is typically done vertically by adding more power to the existing server. SQL databases may face limitations in horizontal scaling across multiple servers.
Query Language:

SQL (Structured Query Language) is the standard language for relational databases. It provides a powerful and standardized way to interact with and manipulate data, including support for complex queries and joins.
Schema:

SQL databases require a predefined schema, meaning the structure of the data must be defined before inserting data. Changes to the schema may require migrations.
ACID Properties:

SQL databases typically adhere to ACID properties (Atomicity, Consistency, Isolation, Durability), ensuring data integrity in transactions. Transactions are all-or-nothing, providing a reliable mechanism for handling complex operations.
NoSQL Databases:

Data Structure:

NoSQL databases can have various structures, such as document-based, key-value pairs, wide-column stores, or graph databases. They are schema-less, allowing for more flexibility in data modeling.
Scaling:

NoSQL databases are designed for horizontal scaling, making it easier to distribute data across multiple servers. This horizontal scaling capability is particularly beneficial for handling large amounts of data and traffic.
Query Language:

NoSQL databases use various query languages or APIs, depending on the type of database. Examples include MongoDB's query language for document databases or simple key-value lookups.
Schema:

NoSQL databases are schema-less or have a dynamic schema, allowing for flexibility in the data structure. This flexibility is advantageous in applications with evolving data requirements.
ACID Properties:

NoSQL databases may relax ACID properties for better performance and scalability. Instead, they might follow the CAP theorem (Consistency, Availability, Partition tolerance), allowing for trade-offs between consistency and availability during network partitions.

What kind of data is a good fit for an SQL database? Structured and well-defined data with complex relationships and transactions are suitable for SQL databases.
Give a real world example. Examples include:
Financial Systems: Recording transactions, managing accounts, and ensuring data consistency.
What kind of data is a good fit a NoSQL database? Unstructured or semi-structured data, where flexibility and scalability are more critical than maintaining strict relationships, is suitable for NoSQL databases. 
Give a real world example. Examples include:
Social Media Platforms: Storing user profiles, posts, and comments, where each user may have different attributes and data can be rapidly changing.
Which type of database is best for hierarchical data storage? NoSQL databases, particularly document-based ones like MongoDB, are well-suited for hierarchical data storage.
Which type of database is best for scalability? NoSQL databases are often preferred for scalability, especially in applications with high read and write loads, distributed systems, and large datasets.

## Videos

[sql vs nosql (Video)](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

What does SQL stand for?

SQL stands for "Structured Query Language."
What is a relational database?

A relational database is a type of database that organizes data into tables with rows and columns, establishing relationships between the tables. It follows the principles of the relational model proposed by Edgar Codd.
What type of structure does a relational database work with?

A relational database works with a tabular structure. It organizes data into tables, where each table consists of rows (records) and columns (attributes).
What is a ‘schema’?

A schema in the context of a relational database refers to the structure or blueprint that defines the organization of data in the database. It includes the tables, their fields, and the relationships between them.
What is a NoSQL database?

NoSQL (Not Only SQL) is a type of database that does not rely on the traditional relational database management system (RDBMS) structure. NoSQL databases are designed to handle unstructured or semi-structured data and can scale horizontally across multiple servers.
How does it work?

NoSQL databases work based on various models, such as document-based, key-value pairs, wide-column stores, or graph databases. They are schema-less or have a dynamic schema, allowing for more flexibility in data storage.
What is inside of a MongoDB database?

In MongoDB, data is stored in BSON (Binary JSON) format. The database contains collections, which are similar to tables in a relational database, and each collection consists of documents. Documents are JSON-like objects that can vary in structure within the same collection.
Which is more flexible - SQL or MongoDB? and why.

MongoDB is generally considered more flexible than traditional SQL databases. In MongoDB, documents within a collection can have different structures, allowing for more dynamic and evolving data models. SQL databases, being table-based and following a strict schema, are less flexible when it comes to accommodating changes in data structures.
What is the disadvantage of a NoSQL database?

One disadvantage of NoSQL databases is the potential lack of standardized query language across different types of NoSQL databases. Unlike SQL, which provides a standardized querying syntax, NoSQL databases may have different query languages or APIs, making it less uniform when working with various NoSQL systems. Additionally, some NoSQL databases may sacrifice certain ACID properties for performance and scalability, which might not be suitable for all use cases, particularly those requiring strict data consistency.