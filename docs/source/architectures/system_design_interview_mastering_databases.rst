System Design Interview: Mastering Databases
===================================

**Types of Databases**

1. Relational Databases

Imagine a well-organized filing cabinet, with files sorted meticulously into distinct drawers and folders. That's a relational database for you.

Characteristics:

- Tables as the primary data storage unit.
- SQL is the querying language.
- Stellar for transactions, intricate queries, and ensuring data integrity.
- Abides by the ACID properties (more on this later).

Examples: PostgreSQL, MySQL, SQLite


2. NoSQL Databases

Visualize a brainstorming board studded with sticky notes, free for you to add or rearrange. This flexible approach embodies NoSQL databases.

Characteristics:

- Can be Key-Value, Document, Wide-Column, or even Graph-based
- Doesn't tie you down with a fixed schema.
- Adept at handling unstructured data.
- Perfect for scalability, swift changes, and straightforward queries.

Examples: MongoDB, Cassandra, Redis

3. In-Memory Databases

Picture a whiteboard used for swift calculations and momentary sketches. Quick and efficient, that's the essence of in-memory databases.

Characteristics:

- Blazing-fast data access, as everything's stored in memory.
- Typically employed for caching and storing session-related data.

Examples: Redis, MemoryDB


**ACID Properties**

- Atomicity: Transactions are binary; they either complete fully or don't execute at all.
- Consistency: Post any transaction, the database remains consistent.
- Isolation: Each transaction operates independently.
- Durability: Once data is committed, it's there for the long haul.

**Scaling Databases**

1. Vertical Scaling

- Increasing CPU Power
- Adding more RAM
- Adding more disk storage
- Upgrading Network

2. Horizontal Scaling

- Database Sharding
- Replication

**Boosting Database Performance**

1. Caching

Leverage caching to store frequent queries, using in-memory databases like Redis, enhancing performance manifold.

2. Indexing

Much like a book's index, database indexes on often-accessed columns can drastically improve retrieval times.

3. Query Optimization

``SELECT first_name, last_name
FROM Employees
WHERE department = 'Engineering'
ORDER BY last_name``

Streamline your queries, minimize joins, and always, always steer clear of the generic
``SELECT *.``

**CAP Theorem**

- Consistency
- Availability
- Partition
