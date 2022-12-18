# Introduction to RDBMS
## What is RDBMS
- A relational Database Management System (RDBMS) is an advanced version of a DBMS system. 
- RDBMS system also allows the organization to access data more efficiently than DBMS.
- RDBMS is a software system that is used to store only data which needs to be stored in the form of tables. 
- data is managed and stored in rows and columns which are known as tuples and attributes.

## Key differences
1. DBMS stores *data as a file* whereas in RDBMS, data is stored in *the form of tables.*
2. DBMS supports *single users*, while RDBMS supports *multiple users.*
3. DBMS *does not support client-server architecture* but RDBMS supports client-server architecture.
4. DBMS has l*ow software and hardware requirements* whereas RDBMS has higher hardware and software requirements.
5. In DBMS, *data redundancy is common* while in RDBMS, *keys and indexes do not allow data redundancy.*
6. [Differences](https://www.guru99.com/difference-dbms-vs-rdbms.html#:~:text=DBMS%20vs%20RDBMS%3A%20Difference%20between%20DBMS%20and%20RDBMS)
## Degrees of relations
### 1. One to One
1. In relational database design, a one-to-one (1:1) relationship exists when zero or one instance of entity A can be associated with zero or one instance of entity B,
2. and zero or one instance of entity B can be associated with zero or one instance of entity A. (abbreviated 1:1)
### 2. Many to Many
1. Many-to-Many relationship in DBMS is a relationship between more than one instance of an entity with more than one instance of another entity i.e. both the entities can have many relationships between each other.
### 3. One to Many
1. one-to-many (1:N) relationship exists when, for one instance of entity A, there exists zero, one, or many instances of entity B;
2. but for one instance of entity B, there exists zero or one instance of entity A

