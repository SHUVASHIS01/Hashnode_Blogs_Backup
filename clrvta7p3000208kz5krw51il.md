---
title: "Database Systems: Concepts, Principles, and Applications"
datePublished: Sat Jan 27 2024 08:30:05 GMT+0000 (Coordinated Universal Time)
cuid: clrvta7p3000208kz5krw51il
slug: database-systems-concepts-principles-and-applications
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1706344195615/626df186-d282-4948-b1fa-cc8cf4784031.jpeg
tags: databases, exploring-the-basics-of-data-science-a-beginners-guide

---

To know about Database systems we must learn some basic definitions. First of all, what is data? Simply, Known facts that can be recorded and have an implicit meaning are called data.

* **Database:** A collection of related data which is logically coherent and is built for a specific purpose.
    
* **Mini-world:** Some part of the real world's data is stored in a database. For example, student grades and transcripts at a university.
    
* **Database Management System (DBMS):** A software package/system that facilitates the creation and maintenance of a computerized database.
    
    * **Database system:** The DBMS software together with the data itself *(data+ DBMS)*. Sometimes, the applications are also included.
        
        ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706170285443/c29e8d63-d14d-46e5-a197-3436a252b539.png align="center")
        
        Examples of Databases
        

---

### Types of Databases and Database Applications

There are two types of Databases:

1. **Traditional:** Numeric and textual databases
    
2. **More recent:**
    
    ■ Multimedia databases
    
    ■ Geographic Information Systems (GIS)
    
    ■ Biological and genome databases
    
    ■ Data warehouses
    
    ■ Mobile databases
    
    ■ Real-time and active databases (used for machine learning)
    

Now the question arises how do we manage these data? There are **two** approaches to <mark>managing data</mark>:

1. **File-based approach:** The situation where data is stored in one or more separate computer files defined and managed by different application programs. Typically, for example, the details of customers may be stored in one file, orders in another, etc. Sharing the data among the programs is a big problem in this approach as this process is kind of analog.
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706171061149/853d47d2-5559-4395-905d-69ef08761300.png align="center")
    

**Database approach:** An approach in which data is collected and manipulated using specific software called Database Management System, and <mark>many programs share this data.</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706171287923/6649bbab-e080-458b-894f-6b378921ae5c.png align="center")

---

<mark>A simplified architecture for a database system:</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706171598991/0cd866a4-941a-4f03-8dcf-471c9cb31d5a.png align="center")

### Now we have to learn what a DBMS facilitates.

1. It defines a particular database in terms of its data types, structures, and constraints.
    
2. Constructs or loads the initial database contents on a secondary storage medium/device (SSD).
    
3. Manipulates the database:
    

■ Retrieval: Querying, generating reports

■ Modification: Insertions, deletions, and updates to its content

■ Accessing the database through Web applications

1. Processing and sharing by a set of concurrent users ***(more than one user utilizing a computer resource at the same time)*** and application programs – yet, keeping all data valid and consistent.
    
2. Provides protection or security measures to prevent unauthorized access.
    
3. “Active” processing to take internal actions on data.
    
4. Presents and visualizes data.
    
5. Maintain the database and associated programs over the lifetime of the database application.
    

### Main Characteristics of the Database Approach

1. **Self-describing nature of a database system:** A DBMS **catalog** stores the description of a particular database (e.g. data structures, types, and constraints). The description is called **meta-data**. This allows the DBMS software to work with different database applications.
    
2. **Insulation between programs and data:** Called **program-data independence**. Allows changing data structures and storage organization without having to change the DBMS access programs.
    
3. **Data abstraction:** A data model is used to hide storage details and present the users with a conceptual view of the database. Basically, hiding the data with something else. It is used for displaying multiple web pages specifically for multiple specific users.
    
4. **Support of multiple views of the data:** Each user may see a different view of the database, which describes **only** the data of interest to that user.
    
5. **Sharing of data and multi-user transaction processing:** Allowing a set of *concurrent users* to retrieve from and update the database. *Concurrency control* within the DBMS guarantees that each transaction is correctly executed or aborted. *The recovery subsystem* ensures each completed transaction has its effect permanently recorded in the database or if the transaction fails then the database rolls back to the last valid state. **OLTP** (Online Transaction Processing) is a major part of database applications; allows hundreds of concurrent transactions to execute per second.
    

### Advantages of Using the Database Approach

* Controlling redundancy in data storage and in development and maintenance efforts by sharing data among multiple users.
    
* Restricting unauthorized access to data. Only the DBA staff uses privileged commands and facilities.
    
* Providing storage structures (e.g. indexes) for efficient query processing and optimization of queries for efficient processing.
    
* Providing backup and recovery systems.
    
* Enforcing **integrity constraints** (Integrity Constraints are the protocols that a table's data columns must follow. These are used to restrict the types of information that can be entered into a table. This means that the data in the database is accurate, unique, and reliable) on the Database.
    

### Database Users

There are two types of Database users:

1. Those who use and control the database content, and those who design, develop and maintain database applications (called ***“Actors on the Scene”***).
    
2. Those who design and develop the DBMS software, related tools, and computer systems operators (called ***“Workers Behind the Scene”***).
    

### **Actors on the Scene**

There are 4 types of ATS. They are:

1. **Database administrator:** They usually decide who can access the database.
    
2. **Database designers:** Those who design the DBMS.
    
3. **Software engineers:** Those who create webpages or applications.
    
4. **End users (4 types):**
    
    ■ **Casual:** access the database occasionally when needed.
    
    ■ **Naïve or parametric:** they make up a large section of the end-user population, e.g. mobile app and social media users, constantly update and access the database.
    
    ■ **Sophisticated:** business analysts, scientists, engineers, and others thoroughly familiar with the system's capabilities.
    
    ■ **Stand-alone:** Mostly maintain personal databases using ready-to-use packaged applications.
    

### When not to use a DBMS

* High initial investment and the possible need for additional hardware.
    
* If the database and applications are simple, well-defined, and not expected to change.
    
* If access to data by multiple users is not required.
    
* In embedded systems (small robots) where a general-purpose DBMS may not fit in available storage.
    
* If there are stringent real-time requirements that may not be met because of DBMS overhead (e.g., telephone switching systems).
    
* If the database system is not able to handle the complexity of data because of modeling limitations (e.g., in complex genome and protein databases).
    
* If the database users need special operations not supported by the DBMS (e.g., GIS and location-based services).
    

---

### Data Models

A set of concepts to describe the ***structure*** of a database, the ***operations*** for manipulating these structures, and certain ***constraints*** that the database should obey. There are <mark>four</mark> types of data models:

1. **Conceptual (*high-level*, semantic) data models:** Provide concepts that are close to the way many users perceive data. Also called **entity-based** or **object-based** data models.
    
2. **Physical (*low-level*, internal) data models:** Provide concepts that describe details of how data is stored in the computer. These are usually specified in an ad-hoc manner through DBMS design and administration manuals.
    
3. **Implementation (*representational*) data models:** Provide concepts that fall between the above two, used by many commercial DBMS implementations (e.g. relational data models used in many commercial systems).
    
4. **Self-Describing Data Models:** Combine the description of data with the data values. Examples include XML, key-value stores, and some NOSQL systems.
    

### <mark>Database Schema versus Database State</mark>

**Database Schema:** The description of a database. Includes descriptions of the database structure, data types, and the constraints on the database. Depending on the schema a diagram (known as the schema diagram which is an ***illustrative*** display of a database schema.) is drawn to create the database. The database schema is also known as ***intentions***. The database schema changes very ***infrequently***. Example of a schema:-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706342472565/8521b88a-ab1b-4740-b03f-31c33f48b5d4.png align="left")

**Database State:** The actual data stored in a database at a ***particular moment in time***. This includes the collection of all the data in the database. Also called a database instance (or occurrence or snapshot). The database state ***changes every time*** the database is updated. Database State is also called ***extension***. Example of a database state:-

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706342684472/f7ca80cc-22ce-4bf2-ae7f-2ed3ed0bc52d.png align="left")

---

### <mark>Three-Schema Architecture</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1706342893510/1ab8fc2c-4283-408b-953d-fe6080a3a46c.png align="center")

The three-schema architecture defines DBMS into <mark>three</mark> levels:

1. **Internal schema** at the internal level to describe physical storage structures and access paths (e.g. indexes). Typically uses a ***physical*** data model.
    
2. **Conceptual schema** at the conceptual level to describe the structure and constraints for the whole database for a community of users. Uses a ***conceptual*** or an ***implementation*** data model.
    
3. **External schemas** at the external level to describe the various user views. Usually uses the same data model as the ***conceptual schema***.
    

### Data Independence

The ability to change the schema at one level without impacting the schema at the next higher level. **Two types** of data independence:

1. **Logical Data Independence:** If we change some data at the conceptual level there will be no impact on the external level. For example, adding a new column that is not shown in the app or changing the datatype which does not change the external view.
    
2. **Physical Data Independence:** If we change some data at the internal level there will be no impact on the conceptual level. For example, the internal schema may be changed when certain file structures are reorganized or new indexes are created to improve database performance.
    

### DBMS Languages

There are **two** types of DBMS languages:-

1. **Data Definition Language (DDL):** Used to define ***database schemas***. The DDL statement is used to identify the description of a schema construct and store the schema description in the DBMS catalog. <mark>Creating/Deleting a table, Adding columns, and Changing data types</mark> are examples that require DDL statements.
    
2. **Data Manipulation Language (DML):** Used to **manipulate data** by <mark>inserting, deleting, updating, and retrieving data</mark>. DML commands can be embedded in a general-purpose programming language such as Java. Two types of DML: high-level/non-procedural and low-level/procedural.