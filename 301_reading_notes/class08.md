# SQL

## Database
A database is an organized collection of structured information, or data, typically stored electronically in a computer system. A database is usually controlled by a database management system (DBMS). Together, the data and the DBMS, along with the applications that are associated with them, are referred to as a database system, often shortened to just database.

Data within the most common types of databases in operation today is typically modeled in rows and columns in a series of tables to make processing and data querying efficient. The data can then be easily accessed, managed, modified, updated, controlled, and organized. Most databases use structured query language (SQL) for writing and querying data.

### Relational Database

A relational database uses SQL which is short for Structured Query Language. This is a fairly rigid and standard way of storing data using tables, columns and rows. Columns represent the data point to be stored and a row represents a record with data points per column that has been defined. These are defined in a table which is usually atomic in nature; this means that a table should really only store data records on one entity or object at a time. Eg. A Table Customers should ONLY be storing customer records.

When additional details are required, or data needs to be associated with a record from one table to another, then we have what we call relationships. A common key is established between the two (or more) tables and this is used for that association there after.

Popular Relational SQL Database Systems
1. Microsoft SQL Server
2. Oracle
3. MySQL / MariaDB
4. PostgreSQL
5. Microsoft Azure SQL

SQL is a programming language used by nearly all relational databases to query, manipulate, and define data, and to provide access control. SQL was first developed at IBM in the 1970s with Oracle as a major contributor, which led to implementation of the SQL ANSI standard, SQL has spurred many extensions from companies such as IBM, Oracle, and Microsoft. Although SQL is still widely used today, new programming languages are beginning to appear.

### Non-Relational NoSQL Database
Unlike its relational counterparts, no-sql databases allow far more flexibility and adaptability as you design your application. If your data requirements aren’t clear at the outset or if you’re dealing with massive amounts of unstructured data, you may not have the luxury of developing a relational database with clearly defined tables and relationships.

NoSQL databases are document-oriented. Instead of using tables, these documents allow us to store unstructured data in a single document. So a document could contain a customer's details, as well as all their orders to date, their favourites, etc. Thi is more intuitive and requires fewer hops across tables to find all the data relating to a customer. Note however that this results in a need for additional processing effort and more storage as the document sizes grow. The storage will not be as highly organized at with an Relational Database.

Popular Non-Relational No-SQL Databases
1. MongoDB
2. Oracle NoSQL
3. Apache CouchDB
4. Redis

