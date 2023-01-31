# Data abstraction
<img src ="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/5bf5e19a-d26e-4ae8-9cc4-08dbe2024a98/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20221214%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20221214T170214Z&X-Amz-Expires=86400&X-Amz-Signature=07ee16bc4d38e3e4af3928afcc7fce57e4c4a6e3d12a3590f50f5c02a5e51633&X-Amz-SignedHeaders=host&response-content-disposition=filename%3D%22Untitled.png%22&x-id=GetObject"/>

1. refers to the process of hiding irrelevant details from the user.
2. There are mainly three levels of data abstraction and we divide it into three levels in order to achieve ***Data Independence.*** 
3. Data Independence means users and data should not directly interact with each other. The user should be at a different level and the data should be present at some other level. By doing so, Data Independence can be achieved.

- View Level(External Schema)
    1. This level tells *the application about how the data should be shown to the user.* 
    2. ***Example:*** 
    If we have a login-id and password in a university system, then as a student, we can view our marks, attendance, fee structure, etc. 
    3. But the faculty of the university will have a different view. He will have options like salary, edit marks of a student, enter attendance of the students, etc. 
    4. So, both the student and the faculty have a different views. 
    5. By doing so, *the security of the system also increases.*

- Conceptual Level(Logic Level)
    1. This level *tells how the data is actually stored and structured*. 
    2. We have different data models by which we can store the data(You can read more about the different types of the data models from [here](https://afteracademy.com/blog/what-is-data-model-in-dbms-and-what-are-its-types)).
    3.  ***Example:*** Let us take an example where we use the relational model for storing the data. 
    4. We have to store the data of a student, the columns in the student table will be student_name, age, mail_id, roll_no etc. 
    5. We have to *define all these at this level while we are creating the database.* 
    6. Though the data is stored in the database but the structure of the tables like the student table, teacher table, books table, etc are defined here in the conceptual level or logical level.
    7.  Also, *how the tables are related to each other are defined here.*

- Physical Level(Internal Schema)
    1. tells us where the data is actually stored i.e. it *tells the actual location of the data* that is being stored by the user. 
    2. The Database Administrators(DBA) decide which data should be kept at which particular disk drive, 
    3. *how the data has to be fragmented,* where it has to be stored etc. 
    4. They decide if the data has to be *centralized or distributed.* 
    5. Though we see the data in the form of tables at the view level the data here is actually stored in the *form of files only.*
