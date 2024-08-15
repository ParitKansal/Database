# Database
---
## Introduction to DBMS

### Database
A **database** is a structured system where data is stored, accessed, updated, and managed efficiently.

### Database Management System (DBMS)
A **DBMS** is a system that includes:
- A **database**: Collection of interrelated data.
- A **set of programs**: To access, store, update, and delete the data.

![DBMS](https://i.ibb.co/kmNHLFL/dbms.png)

### Tasks of a DBMS
1. **Definition**: Defining data structures for storage.
2. **Insertion**: Adding new data.
3. **Updation**: Modifying existing data.
4. **Retrieval**: Fetching data.
5. **Administration**: Managing and maintaining the database.

### Disadvantages of DBMS
1. **Cost**: Requires investment in specialized hardware and software.
2. **Size**: Needs significant storage space and resources.
3. **Complexity**: Requires trained personnel.
4. **Higher Impact of Failure**: Failures can have significant consequences.

### Disadvantages of File Systems
1. **Data Redundancy**: Multiple copies of data.
2. **Difficulty in Accessing**: Need for custom programs for access.
3. **Data Isolation**: Difficult to extract data from different files.
4. **Integrity**: Challenges in applying constraints.
5. **Atomicity**: Issues with rollbacks if transactions fail.
6. **Concurrent Access**: Issues with multiple users accessing data.
7. **Security Problems**: Vulnerabilities in data security.

---

## Database Users

1. **Native Users**:
   - Use existing applications to interact with the database.
   - Examples: Online library systems, ticket booking systems, ATMs.

2. **Application Programmers**:
   - Develop applications that interact with the database using DML queries.
   - Languages: C, C++, Java.

3. **Sophisticated Users**:
   - Database developers who use SQL directly.
   - Examples: Scientists, engineers, analysts.

4. **Specialized Users**:
   - Develop complex database applications.

### Database Administrator (DBA)
- Manages both data and programs that access data.
- **Functions**:
  1. Schema definition.
  2. Storage structure and access methods.
  3. Schema and physical organization modification.
  4. Authorization control.
  5. Routine maintenance.

---

## Instance and Schema

### Instance
- The collection of information stored in the database at a specific moment.

### Schema
- The structural description of data.

---

## Three Schema Architecture

- Provides users with an abstract view of data.
- **Levels of Abstraction**:
  1. **Physical Level**:
     - Describes how data is physically stored.
  2. **Logical/Conceptual Level**:
     - Describes the design of the database, including data types and relationships.
  3. **View/External Level**:
     - Describes the part of the database that a particular user group interacts with.

![Three Schema Architecture](https://i.ibb.co/4SPTpMJ/three-level.png)

---

## DDL and DML

1. **Data Definition Language (DDL)**:
   - Defines the database schema.

2. **Data Manipulation Language (DML)**:
   - Handles data queries and modifications.
   - **Procedural DML**: Specifies what data is needed and how to get it.
   - **Non-Procedural DML**: Specifies what data is needed without specifying how to get it.

![DBMS Architecture1](https://i.ibb.co/tLsWczG/dbms-archi-1.png)

![DBMS Architecture2](https://i.ibb.co/HnqNg79/dbms-archi-2.png)


## Data Models

### Relational Model
- **Tables**: Represent data and relationships.
- **Attributes**: Columns in tables.
- **Record-based model**: Fixed-format records.

![Relational Model](https://i.ibb.co/jGJs7m9/rational-database.png)

### Entity-Relationship Model
- **Entities**: Basic objects with attributes.
- **Relationships**: Connections among entities.

### Hierarchical Model
- Data elements linked in a tree structure with a single root.

### Network Model
- Extension of hierarchical model with multiple parent-child relationships.

### Object-Oriented Model
- Overcomes shortcomings of other models by defining data in terms of objects and classes.

---

## Keys

- **Super Key**: All possible keys of a relation.
- **Candidate Key**: A key whose proper subset is not a key.
- **Primary Key**: Chosen candidate key for implementation.
- **Alternate Key**: Candidate keys not chosen as the primary key.
- **Foreign Key**: References a primary key in another table, ensuring referential integrity.

---
