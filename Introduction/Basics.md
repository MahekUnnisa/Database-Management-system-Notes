#Basics
- ## What is Data?
    1. data is small units of information
    2. we can organize data to find it easier for future use
    3. Data can be organize into rows columns, tables or indexes to find easily..
- ## Database?
    1. Database is an organized collection of data to easily access and manage data.
    2. As said can be organised into rows, columns, tables etc.
    Database Handlers create a database in such a way that only a specific set of software can access a database.
    Today dynamic websites on the internet use modern databases.
    ex. MySQL, Postgres, Mongo/db ect.
    
    - Modern Dbs are operates by **Sql called Structured query language and** are managed by **DBMS called Database management System.**
    ## Types of Databases:
    - **1. Cloud database**
        1. allows you to manage, retrieve, and access your ordered or unordered data via a cloud platform. it is stored over the internet. ex.AWS.
        2. Also called DBaaS.
        - Advantages
            1. Lower costs
            2. increased accessibility
            3. Automated.

    - **2. NoSQL**
        1. NoSQL database is an approach to designing such databases that can accommodate a wide variety of data models. 
        2. NoSQL stands for "not only SQL." It is an alternative to traditional relational databases in which data is placed in tables, and data schema is perfectly designed before the database is built.
        - some types of DBS.
        - MongoDB, CouchDB, Cloudant **(Document-based)**
        - Memcached, Redis, Coherence **(key-value store)**
        - HBase, Big Table, Accumulo **(Tabular)**

    **Advantages of NOSQL**
    - **High Scalability**
        1. NoSQL can handle an extensive amount of data because of scalability. 
        2. If the data grows, the NoSQL database scale it to handle that data in an efficient manner.
    - **High Availability**
        1. NoSQL supports auto replication. 
        2. Auto replication makes it highly available because, in case of any failure, data replicates itself to the previous consistent state.

    **Disadvantages of NOSQL**
    - **Open source**
        NoSQL is an open-source database, so there is no reliable standard for NoSQL yet.
    - **Management challenge**
        Data management in NoSQL is much more complicated than relational databases. It is very challenging to install and even more hectic to manage daily.
    - **GUI is not available**
        GUI tools for NoSQL database are not easily available in the market.
    - **Backup**
    **3. Object Oriented databases**
        1. Object-oriented databases contain data in the form of objects and classes.
        2. Objects are the real-world entity, and types are the collection of objects.
        3. An object-oriented database is a combination of relational model features with object-oriented principles. 
        4. It is an alternative implementation to that of the relational model.
        - **Object-oriented programming properties**
            - Objects
            - Classes
            - Inheritance
            - Polymorphism
            - Encapsulation
        - **Relational database properties**
            - Atomicity
            - Consistency
            - Integrity
            - Durability
            - Concurrency
            - Query processing

    **4. Relational Database**
    1. The relational database model has two main terminologies called **instance and schema.**
    2. The instance is a table with rows or columns.
    Schema specifies the structure like the name of the relation, type of each column, and name.
    3. During this era others like OOmodel, Object-relational model were also introduced.

    **5. Graph Databases**
    1. A graph database is a NoSQL database. It is a graphical representation of data. It contains nodes and edges. 
    2. A node represents an entity, and each edge represents a relationship between two edges. Every node in a graph database represents a unique identifier.
    3. are beneficial for **searching for the relationship between data** because they highlight the relationship between relevant data.
    4. mostly used in **supply chain management**

    **Evolution of Databases**
    1. initially, databases were managed in a hierarchical model and file based model which causes lot of repetion and overwriting, and loss of data sometimes.
    2. Therefore to avoid it the first database was introduced by Honeywell which was managed by  DBMS called as **Integrated Data model(IDS).** - It was a network data model.
    3. It was difficult to manage and has a complex system which contributed to the design of relational Databases.
- ## What is DBMS?
the software which is used to store and retrieve the database. For example, Oracle, MySQL, etc.
- DBMS provides the interface to perform various operations like creation, deletion, modification, etc.
- DBMS allows the user to create their databases as per their requirement.
- DBMS accepts the request from the application and provides specific data through the operating system.
- DBMS contains a group of programs that acts according to the user's instruction.
- It provides security to the database

- ***Advantages***
    - Controls Redundancy
        stores all the data in a single database file,
    - Backup
    - Data Sharing
    - Multiple User Interfaces
- ***Disdavantages***
    - *Size*
        It occupies large disk space and large memory to run efficiently.
    - *Cost*
        DBMS requires a high-speed data processor and larger memory to run DBMS software, so it is costly.
    - *Complexity*
        DBMS creates additional complexity and requirements.

## ***Two-Tier Database Architecture***
1. In two-tier, the application logic is either buried inside the User Interface on the client or within the database on the server (or both). 
2. With two-tier client/server architectures, the user system interface is usually located in the user’s desktop environment and 
3. the database management services are usually in a server that is a more powerful machine that services many clients.
## ***Three-Tier Database Architecture***

1. In three-tier, the application logic or process lives in the middle-tier, 
2. it is separated from the data and the user interface. 
3. Three-tier systems are more scalable, robust and flexible. In addition, they can integrate data from multiple sources. In the three-tier architecture, a middle tier was added between the user system interface client environment and the database management server environment. 
4. There are a variety of ways of implementing this middle tier, such as transaction processing monitors, message servers, or application servers.

## Terms to know
- ***Instances***
    1. In simple words, it is the snapshot of the database taken at a particular moment. 
    2. It can also be described in a more significant way as the collection of the information stored in the database at that particular moment. 
    3. An instance can also be called the database state or current set of occurrences due to the fact that it is information that is present in the current state.
    4. Every time we update the state say we insert, delete or modify the value of the data item in the record, it changes from one state to other. At the given time, each schema has its own set of instances.
- ***Schema***
    1. It is the overall description or the design of the database specified during the database design. 
    2. The important thing to be remembered here is it should not be changed frequently. Basically, it displays the record types(entity), and names of data items(attribute) but not the relation among the files.
    3. The interesting point is the values in the schema might change but not the structure of the schema.
    4. Physical schema is hidden behind the logical schema and thus can be modified without affecting the application programs
    5. The database management system provides data definition language(DDL) and document schema definition language(DSDL) to specify both logical and physical schema.
- ***SubSchema***
    1. and the logical view of data as it appears to the application can be called as subschema.
    2. Well, it is interesting to note that it provides the users a window through which the user can view only that part of database which is of matter of interest to him. 
    3. It Identifies subset of areas, sets, records, data names defined in database that is of interest to him. 
    4. Thus a portion of database can be seen by application programs and different application programs has different view of data.