# DBMS
## Introduction to DBMS

### Database
- **Definition**: A structured system where data is stored, accessed, updated, and managed efficiently.

### Database Management System (DBMS)
- **Components**:
  - **Database**: Collection of interrelated data.
  - **Set of Programs**: To access, store, update, and delete data.

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
2. **Difficulty in Accessing**: Custom programs needed for access.
3. **Data Isolation**: Difficult to extract data from different files.
4. **Integrity**: Challenges in applying constraints.
5. **Atomicity**: Issues with rollbacks if transactions fail.
6. **Concurrent Access**: Issues with multiple users accessing data.
7. **Security Problems**: Vulnerabilities in data security.

---

## Database Users

1. **Native Users**:
   - Use existing applications to interact with the database.
   - **Examples**: Online library systems, ticket booking systems, ATMs.

2. **Application Programmers**:
   - Develop applications interacting with the database using DML queries.
   - **Languages**: C, C++, Java.

3. **Sophisticated Users**:
   - Database developers using SQL directly.
   - **Examples**: Scientists, engineers, analysts.

4. **Specialized Users**:
   - Develop complex database applications.

### Database Administrator (DBA)
- **Functions**:
  1. Schema definition.
  2. Storage structure and access methods.
  3. Schema and physical organization modification.
  4. Authorization control.
  5. Routine maintenance.

---

## Instance and Schema

### Instance
- **Definition**: The collection of information stored in the database at a specific moment.

### Schema
- **Definition**: The structural description of data.

---

## Three Schema Architecture

- **Levels of Abstraction**:
  1. **Physical Level**: Describes how data is physically stored.
  2. **Logical/Conceptual Level**: Describes the database design, including data types and relationships.
  3. **View/External Level**: Describes the part of the database that a particular user group interacts with.

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

---

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
- Defines data in terms of objects and classes.

---

## Keys

- **Super Key**: All possible keys of a relation.
- **Candidate Key**: A key whose proper subset is not a key.
- **Primary Key**: Chosen candidate key for implementation.
- **Alternate Key**: Candidate keys not chosen as the primary key.
- **Foreign Key**: References a primary key in another table, ensuring referential integrity.

---

## ER Diagram Overview

### **Entities**
- **Strong Entity**: Can be uniquely identified.
- **Weak Entity**: Cannot be uniquely identified.

![Strong vs Weak Entity](https://techdifferences.com/wp-content/uploads/2016/12/Strong-Entity-Vs-Weak-Entity.jpg)

### **Entity Set**
- A set of entities with the same properties or attributes.

---

## **Types of Attributes**

| **Type**               | **Description**                                   | **Image**                                                                                                            |
|------------------------|---------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| **Simple**             | Cannot be divided further.                       | ![Simple](https://i.ibb.co/xJPxbDT/simple-1.png)                                                                     |
| **Composite**          | Can be divided into multiple attributes.         | ![Composite](https://i.ibb.co/znN9RPd/composite-1.png)                                                               |
| **Single Valued**      | Holds a single value.                            | ![Single Valued](https://i.ibb.co/xJPxbDT/simple-1.png)                                                              |
| **Multi-Valued**       | Can hold multiple values.                        | ![Multi Valued](https://i.ibb.co/c626nGF/multivales-1.png)                                                           |
| **Derived**            | Derived from other attributes.                   | ![Derived](https://i.ibb.co/QYtvSsk/primary-1.png)                                                                   |
| **Primary Key Attribute** | Uniquely identifies an entity.                   | ![Primary Key Attribute](https://i.ibb.co/59WM8w1/weak-1.png)                                                        |
| **Weak Key Attribute** | Part of a weak entity key.                       | ![Weak Key Attribute](https://i.ibb.co/S5NkLzS/derived-1.png)                                                        |

---

## **Strong and Weak Relationships**

| **Strong Relationship** | **Weak Relationship** |
|-------------------------|------------------------|
| ![Strong](https://i.ibb.co/znXBwtH/weak-relation-1.png)    | ![Weak](https://i.ibb.co/pf1Wsn4/strong-relation-1.png)                |

---

## **Degree of Relationship**

| **Degree** | **Type**          | **Image**                                                                                           |
|------------|-------------------|-----------------------------------------------------------------------------------------------------|
| 1          | **Unary (1 Degree)**       | ![Unary](https://media.geeksforgeeks.org/wp-content/uploads/20231030173427/unary.jpg)               |
| 2          | **Binary (2 Degrees)**     | ![Binary](https://media.geeksforgeeks.org/wp-content/uploads/20231030173529/binary.jpg)             |
| 3          | **Ternary (3 Degrees)**    | ![Ternary](https://media.geeksforgeeks.org/wp-content/uploads/20231030173612/tarnary.jpg)          |
| 4          | **N-Ary (n Degrees)**      | ![N-Ary](https://media.geeksforgeeks.org/wp-content/uploads/20231030173925/nary.jpg)               |

---

## **Relationship Constraints**

### **Mapping Cardinality**
- One to One
- One to Many
- Many to One
- Many to Many

### **Participation Constraints**
- **Total**: Each entity must be involved in at least one relationship instance.
- **Partial**: Not all entities are involved in relationship instances.

**Note**: Weak entities have a total participation constraint, meaning every instance must be associated with a strong entity.

---

## **Extended ER Features**

### **1. Specialization**
- **Top-Down Approach**

### **2. Generalization**
- **Bottom-Up Approach**

![Specialization vs Generalization](https://www.tutorialspoint.com/assets/questions/images/113346-1532408376.png)

### **3. Aggregation**
- Treating a relationship as a higher-level entity (abstract entity).

![Aggregation](https://i.ibb.co/B4f7K2v/aggeregation.png) 

---

## **Constraints**

| **Constraint**   | **Type**         | **Description**                                                                                       |
|------------------|------------------|-------------------------------------------------------------------------------------------------------|
| **Membership**   | **Attribute Defined** | Based on explicit attribute conditions. |
|                  | **User Defined** | Assigned manually by users.   |
| **Disjointness** | **Disjoint**        | An entity can belong to only one lower-level set. |
|                  | **Overlapping**     | An entity can belong to multiple lower-level sets. |
| **Completeness** | **Totalness**       | Every higher-level entity must belong to at least one lower-level set. |
|                  | **Partial**         | Some higher-level entities may not belong to any lower-level set. |

---

## **Integrity Constraints**

- **Domain Constraints**: Defines valid values for an attribute.
- **Entity Integrity

 Constraint**: Primary key value cannot be null.
- **Referential Integrity Constraints**: Foreign key must refer to a valid primary key or be null.
- **Key Constraint**: Primary key values must be unique.

---

## **Reduction of ER Diagrams to Tables**

| **Type**                              | **Description**                                  | **Image**                                                                                      |
|---------------------------------------|--------------------------------------------------|------------------------------------------------------------------------------------------------|
| 1. Weak Entity                        | ![Image 9](https://i.ibb.co/xXKgRjX/1-1.png)    |                                                                                                 |
| 2. Composite Attributes               | ![Image 8](https://i.ibb.co/n1pZ3RV/2-1.png)    |                                                                                                 |
| 3. Multi-Valued Attributes            | ![Image 7](https://i.ibb.co/9sHf14j/3-1.png)    |                                                                                                 |
| 4. Many-to-Many Relationship          | ![Image 6](https://i.ibb.co/7Y6GS0P/4-1.png)    |                                                                                                 |
| 5. One-to-Many Relationship           | ![Image 5](https://i.ibb.co/YR1sqpB/5-1.png)    |                                                                                                 |
| 6. Aggregation                        | ![Image 4](https://i.ibb.co/1QrspC9/6-1.png)    |                                                                                                 |
| 7. Unary One-to-Many Relationship     | ![Image 3](https://i.ibb.co/YLSnxc9/7-1.png)    |                                                                                                 |
| 8. Unary One-to-One Relationship      | ![Image 2](https://i.ibb.co/rpBvVmb/8-1.png)    |                                                                                                 |
| 9. Unary Many-to-Many Relationship    | ![Image 1](https://i.ibb.co/rmwpqR2/9-1.png)    |                                                                                                 |

---
