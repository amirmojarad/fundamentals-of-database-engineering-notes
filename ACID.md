# ACID 

Here are some practices and notes on ACID concepts.

### What is ACID?
Atomicity is one of the ACID properties of database transactions, which ensure the reliability of transactions in a database management system (DBMS). The ACID properties are:

* **Atomicity** Ensures that a transaction is treated as a single unit, which either completes entirely or does not complete at all. If any part of the transaction fails, the entire transaction is rolled back, leaving the database in its previous state.
* **Consistency** Ensures that a transaction brings the database from one valid state to another, maintaining database invariants.
* **Isolation** Ensures that the execution of transactions concurrently does not affect their execution.
* **Durability** Ensures that once a transaction has been committed, it will remain so, even in the event of a system failure

## Atomacity
Atomicity ensures that a series of database operations are treated as a single unit. If any operation fails, the entire transaction is rolled back, ensuring that the database remains consistent. Using transactions, error handling, and savepoints in PostgreSQL allows you to manage atomicity effectively.
