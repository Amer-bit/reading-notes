# Database
Database is a systematic collection of data. Databases support storage and  manipulation of data. Databases make data management easy.

There are many different types of databases. The best database for a specific organization depends on how the organization intends to use the data.

**Relational databases**. Items in a relational database are organized as a set of tables with columns and rows.

**Object-oriented databases**. Information in an object-oriented database is represented in the form of objects, as in object-oriented programming.

**Distributed databases**. A distributed database consists of two or more files located in different sites. The database may be stored on multiple computers, located in the same physical location, or scattered over different networks.

**Data warehouses**. A central repository for data, a data warehouse is a type of database specifically designed for fast query and analysis.

**NoSQL databases**. A NoSQL, or nonrelational database, allows unstructured and semistructured data to be stored and manipulated . *NoSQL databases grew popular* as *web applications became more common and more complex.*

**Graph databases**. A graph database stores data in terms of entities and the relationships between entities.

**OLTP databases**. An OLTP database is a speedy, analytic database designed for large numbers of transactions performed by multiple users.


# Data model
A data model refers to the logical inter-relationships and data flow between different data elements involved in the information world. It also documents the way data is stored and retrieved. Data models facilitate communication business and technical development by accurately representing the requirements of the information system and by designing the responses needed for those requirements. Data models help represent what data is required and what format is to be used for different business processes.

A data model can be concrete or abstract. It has the following main components:
Data types
Data items
Data sources
Event sources
Links
Data models are represented by the data modeling notation, which is often presented in the graphical format. Their main focus is to support and aid information systems by showing the format and definition of the different data involved. They also help prevent data redundancy. Information stored in data models is of great significance for businesses because it dictates the relationships between database tables, foreign keys and the events involved.

The three basic styles of data model are:

Conceptual data models
Physical data models
Logical data models

# CRUD
CRUD is an acronym for CREATE , READ , UPDATE , DELETE. They are the standard database command.

The CRUD cycle is designed for enhancing persistent storage, for instance with a database of records.
In modern software development, CRUD has transcended its origins as foundational functions of a database and now maps itself to design principles for dynamic application likes HTTP protocols, SQL.

**Principles of CRUD:**

**Create**: CREATE procedures to generate a new record in a database.

**Read/Retrieve**: READ procedures reads the data based on input parameters.

**Update**: UPDATE procedures modify the existing record in a database.

**Delete**: DELETE procedures deletes record in a database based on input parameter.

# Database schema
A database schema is an abstraction used to represent the storage of data in a database. It not only describes the organization of data but also represents the relationship between various tables in a database.

# Data sanitization
Data sanitization is the process of deliberately, permanently, and irreversibly removing or destroying the data stored on a memory device. A device that has been sanitized has no usable residual data and even advanced forensic tools should not ever be able recover erased data.

# Mongoose
Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node. js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.


#### Why would a developer choose to make data models?
Ensures that all data objects required by the database are accurately represented. Omission of data will lead to creation of faulty reports and produce incorrect results.
A data model helps design the database at the conceptual, physical and logical levels.
Data Model structure helps to define the relational tables, primary and foreign keys and stored procedures.
It provides a clear picture of the base data and can be used by database developers to create a physical database.
It is also helpful to identify missing and redundant data.
Though the initial creation of data model is labor and time consuming, in the long run, it makes your IT infrastructure upgrade and maintenance cheaper and faster.

#### What purpose do CRUD operations serve?
Maniplulating the data stored in the database

#### What kind of database is Postgres? What kind of database is MongoDB?
Postgres is an object-relational database and MongoDB is a document database(non-relational)

#### What is Mongoose and why do we need it?
Object Data Modeling (ODM) library for MongoDB and Node. js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB. we use because it has more abstraction over pure mongo and It also creates Model abstraction which makes it easier to work with, so it looks like you are working with just objects rather than pure data.


