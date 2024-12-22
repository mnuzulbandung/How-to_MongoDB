# **MongoDB**

## A. **Characteristics**
1. **Document-based**: MongoDB inputs JSON data and stores it as BSON (Binary JSON). It offers several key benefits, including:
    * **Non-Uniform Schema**: Each document can have its unique structure, accommodating different field types and varying numbers of fields within the same collection.
    * **Nested Structures**: Attributes can hold arrays or nested objects, eliminating the need for empty placeholders or additional relational tables.
    * **Dynamic Schema**: The schema can quickly adapt to changes, such as adding or removing fields, without affecting existing documents.
2. **Horizontal Scalability**: MongoDB scales out by using sharding to distribute data across multiple servers, with load balancers ensuring even traffic distribution. New servers can be added seamlessly without downtime.
3. **Replication**: MongoDB replicates data from the primary to secondary nodes for redundancy and high availability. A secondary is automatically promoted if the primary fails, ensuring uninterrupted operations.
4. **Data Query**: It provides advanced features for processing and analyzing data, making it possible to group, filter, and transform datasets effectively.
5. **Indexes**: It enable efficient data retrieval and enhance query performance by allowing the database to locate specific data without scanning the entire collection. These include index types such as a Single Field Index, Compound Index, Multikey Index, or Text Index.

## B. **Uses**:
* Industries requiring high availability and fault tolerance.
* Industries generating large volumes of diverse data.

## C. **Terminology**
* MongoDB Concepts: SQL Concepts
* Database: Database
* Collections: Tables
* Documents: Rows
* Fields: Columns
