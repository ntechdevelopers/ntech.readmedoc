System Design Core Concept
===================================

The core concepts of system design pertain to the essential principles and components necessary for constructing scalable, efficient, and maintainable systems. Presented below are the major concepts:

**Scalability**:  
The capacity of a system to accommodate heightened demands, either by vertical scaling (enhancing the resources of a single machine) or horizontal scaling (augmenting the number of machines).

**Load balancing**:  
Allocating incoming network traffic among several servers to prevent any single server from becoming overloaded.

**Caching**:  
The practice of storing frequently used data in temporary storage, such as in-memory cache, to diminish access time and enhance performance.

**Database design**:  
Selecting between relational (SQL) and non-relational (NoSQL) databases according to data architecture, interrelations, and scalability requirements.

**Data partitioning (sharding)**:  
Dividing a database into smaller, more manageable segments to share the load across different servers and enhance performance.

**Concurrency**:  
Managing numerous requests concurrently without conflicts or delays, generally via techniques like multithreading, asynchronous processing, or distributed queues.

**Availability and fault tolerance**:  
Guaranteeing a system's functionality despite failures. This may encompass redundancy, failover mechanisms, and the architecture of distributed systems.

**Consistency**:  
Maintaining uniformity of data throughout the system, typically accomplished by stringent database regulations or distributed consensus protocols.

**Latency and throughput**:  
Reducing delay (latency) and enhancing the volume of requests a system can handle within a specified timeframe (throughput).

**Security**:  
Safeguarding the system against harmful incursions using encryption, authentication, authorization, and routine upgrades to mitigate vulnerabilities.

**Microservices architecture**:  
Segmenting an application into smaller, autonomous services that interact via a network, with each service accountable for a distinct business function.

**Monitoring and observability**:  
Employing tools and methodologies to assess system performance, identify concerns promptly, and investigate the underlying causes of failures or bottlenecks.
