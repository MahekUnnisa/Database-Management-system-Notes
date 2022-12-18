# Keys in RDBMS
## Different Types of Keys in RDBMS
### 1. Candidate key
- The minimal set of attributes that can uniquely identify a tuple is known as a candidate key. For Example, STUD_NO in STUDENT relation.
- It is a minimal *super* key.
- It is a super key with *no repeated data* is called a candidate key.
- The minimal set of attributes that can uniquely identify a record.
- It must contain unique values.
- It *can contain NULL values.*
- Every table *must have at least a single* candidate key.
- A table can have multiple candidate keys but only one primary key (the primary key cannot have a NULL value, so the candidate key with NULL value can’t be the primary key).
- The value of the Candidate Key is unique and non-null for every tuple.
- There *can be more than one candidate key in a relation*. For Example, STUD_NO is the candidate key for relation STUDENT.
- The candidate key can be simple (having only one attribute) or composite as well. For Example, {STUD_NO, COURSE_NO} is a composite candidate key for relation STUDENT_COURSE.
- No, of candidate keys in a Relation are nC(floor(n/2)),for example if a Relation have 5 attributes i.e. R(A,B,C,D,E) then total no of candidate keys are 5C(floor(5/2))=10.
### 2. Super Key
1. The set of attributes *that can uniquely identify a tuple* is known as Super Key. For Example, STUD_NO, (STUD_NO, STUD_NAME), etc.  
2. A super key *is a group of single or multiple keys* that identifies rows in a table. 
3. It *supports NULL* values. Example: SNO+PHONE is a super key.
4. Adding zero or more attributes to the candidate key generates the super key.
5. A candidate key is a super key but vice versa is not true.
### 3. Primary Key
1. There can be more than one candidate key in relation *out of which one can be chosen as the primary key.* 
2. For Example, STUD_NO, as well as STUD_PHONE, are candidate keys for relation STUDENT but STUD_NO can be chosen as the primary key (only one out of many candidate keys).
- It is a *unique* key.
- It can *identify only one tuple (a record) at a time.*
- It has *no duplicate values,* it has unique values.
- It *cannot* be NULL.
- Primary keys are not *necessarily to be a single column;* more than one the column can also be a primary key for a table.
- Eg:- STUDENT table SNO is a primary keySNO SNAME ADDRESS PHONE
### 4. Alternate Key
1. The *candidate key other than the primary key* is called an alternate key. 
2. For Example, STUD_NO, as well as STUD_PHONE both, are candidate keys for relation STUDENT but STUD_PHONE will be an alternate key (only one out of many candidate keys). It is a secondary key
- All the *keys which are not primary keys are called alternate keys.*
- It contains *two or more fields to identify two or more records*.
- These values are repeated.Eg:- SNAME, ADDRESS is Alternate keys
### 5. Foriegn Key
1. If an attribute can only take the values which are present as values of some other attribute, it will be a foreign key to the attribute to which it refers. 
2. The relation which is being referenced is called referenced relation 
3. and the corresponding attribute is called referenced attribute and 
4. the relation which refers to the referenced relation is called referencing relation and 
5. the corresponding attribute is called referencing attribute. 
6. The referenced attribute of the referenced relation should be the primary key to it. *For Example, STUD_NO in STUDENT_COURSE is a foreign key to STUD_NO in STUDENT relation.*
- It is a key it *acts as a primary key in one table* and *it acts as secondary key in another table.*
- It combines *two or more relations (table) at a time.*
- They act as a *cross-reference* between the tables.
- For example, DNO is a primary key in the DEPT table and a non-key in EMP
### 6. Secondary Key
1. Secondary Key is the key that has not been selected to be the primary key. *However, it is considered a candidate key for the primary key.*
2. Therefore, a candidate key not selected as a primary key is called secondary key. Candidate key is an attribute or set of attributes that you can consider as a Primary key.
3. **Note**: Secondary Key is not a Foreign Key.
4. ***Student_ID, Student_Enroll** and **Student_Email** are the candidate keys.* 
5. They are considered candidate keys since they can uniquely identify the student record. 
6. *Select any one of the candidate key as the primary key. Rest of the two keys would be Secondary Key.*