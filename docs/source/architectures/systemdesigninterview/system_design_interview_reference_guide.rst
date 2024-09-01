System Design Interview Reference Guide
===================================

**Interview Framework**

- Step 1 (10 min): Understand the Problem Collect requirements, resolve ambiguities, understand constraints.
- Step 2 (10 min): Conceptual Design Create high-level architecture diagram, show components' interactions.
- Step 3 (10 min): Detailed Analysis Examine system components, data flow, protocols, interactions.
- Step 4 (10 min): Enhance the Design Identify improvements in scalability, reliability, maintainability.
- Step 5 (10 min): Conclusion Review requirements, discuss trade-offs, answer remaining questions.

**API Design Choices**

- REST: Building Scalable APIs using standard HTTP Methods.
- GraphQL: Query Language for APIs, Allowing Clients to Request Specific data
- gRPC: High Performance Framework For Remote Procedure Calls, Using HTTP/2.

**Scalability**

- Replication: Creating multiple copies of data for redundancy and fast access
- Sharding: Dividing data into smaller chunks across multiple servers for better performance and parallel processing.
- Partitioning: Distributing incoming traffic evenly across multiple servers.
- Load Balancing: Splitting data across multiple databases to balance the load.

**Messaging Patterns**

- Synchronous: Immediate response required, direct client-server interaction (e.g., HTTP).
- Async Messaging: Queue-based, no immediate response needed
- Publish-Subscribe: Event-driven, multiple subscribers receive same message

**Caching**

- In-memory Cache: Latency- In-memory cache is faster doesn't require a network request like distributed.
- Distributed Cache: 

    + Sharing data/ Consistency-data can be shared across machines with a distributed cache.
    + Availability- distributed cache is not affected by individual server failures

- Caching strategy

    + Write-through
    + Read-through
    + Write-around
    + Write-back

- Requested data

    + No. Items
    + Cache Miss & Hit
    + Disk & Memory Usage

- Eviction:

    + LRU (Least Recently Used)
    + LFU (Least Freq. used)
    + FIFO
    + MRU
    + Random Eviction Least Used
    + On-Demand Expiration
    + Garbage Collection