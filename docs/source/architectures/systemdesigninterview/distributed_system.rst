Distributed Systems
===================================

**CORE CONCEPTS**

- Distributed System: A collection of interconnected computers that communicate and coordinate to achieve a common goal
- Scalability: Handling increased workload

  + Horizontal: Add more machines (nodes)
  + Vertical: Upgrade existing machines (e.g. CPU, RAM)

- Reliability: Functioning correctly despite failures
- Availability: Proportion of uptime
- Consistency: Agreement on data values across all nodes at a given time
- Partition Tolerance: Operating despite network splits
- CAP Theorem: (Pick two) Consistency, Availability, Partition Tolerance
- State Management: Data storage/synchronization across nodes (stateless/stateful)
- Data Partitioning: Dividing data for scalability (horizontal/vertical, hash/range-based)
- Replication Strategies: Copying data for fault tolerance
- (synchronous/asynchronous/quorum-based)
- Consistency Models: Trade-offs between data agreement and performance (strong/eventual/causal)
- Time and Order: Event ordering (Lamport timestamps/ vector clocks)
- Fault Tolerance: Handling failures gracefully (failover/redundancy)
- Concurrency Control: Managing simultaneous access (optimistic/pessimistic)

**ARCHITECTURES**

- Client-Server: Clients request services from servers
- Peer-to-Peer (P2P): Nodes act as both clients and servers
- Master-Slave: One master node coordinates, multiple slaves execute Microservices: System decomposed into small, independent services
- Event-Driven Architecture: Components communicate by reacting to events
- Service-Oriented Architecture (SOA): A collection of services that communicate with each other
- Lambda Architecture: A hybrid architecture for batch and real-time processing

**KEY TECHNOLOGIES**

- Container Orchestration: Kubernetes, Docker Swarm Service Discovery: Consul, etc
- API Gateways: Kong, Tyk, Apigee, AWS API Gateway Load Balancers: HAProxy, NGINX, Traefik, Amazon ELB
- Monitoring & Observability: Prometheus, Grafana
- Distributed Tracing: Zipkin, Jaeger Service Mesh: Istio, Linkerd
- Infrastructure as Code (laC): Terraform, Pulumi, CloudFormation Configuration Management: Ansible, Chef, Puppet Distributed Caches: Redis, Memcached
- Stream Processing: Apache Flink, Apache Spark Streaming Workflow Orchestration: Apache Airflow, Argo Workflows Job Schedulers: Quartz, Apache Oozie, Kubernetes CronJobs Cloud Providers: AWS, Azure, Google Cloud Platform Serverless Platforms: AWS Lambda, Azure Functions, Google Cloud Functions

**FALLACIES OF DISTRIBUTED COMPUTING**

- The network is reliable
- Latency is zero
- Bandwidth is infinite
- The network is secure
- Topology doesn't change
- There is one administrator
- Transport cost is zero
- The network is homogeneous

**COMMUNICATION**

- Remote Procedure Call (RPC): Call a function on a remote machine Message Passing: Asynchronous communication between nodes
- Message Queues (Point-to-Point): RabbitMQ, Amazon SQS
- Message Brokers (Publish-Subscribe): Kafka, Apache Pulsar
- REST: Query language for APls with fine-grained data fetching GraphQL: TLS/SSL, HTTPS, SSH
- gRPC: High-performance RPC framework using Protocol Buffers Webhooks: Automatic notifications sent when certain events occur

**COORDINATION & CONSENSUS**

- Consensus Algorithms: Paxos, Raft
- Distributed Locks: ZooKeeper, etcd
- Distributed Transactions: Two-phase commit (2PC)
- Leader Election: Choosing a coordinator node
- Gossip Protocol: Decentralized information dissemination

**DESIGN PRINCIPLES**

- Loose Coupling: Minimize component dependencies
- High Cohesion: Group related functionality together
- Abstraction: Hide implementation details
- Single Responsibility: Each component does one thing well Separation of Concerns: Divide system into distinct modules
- Statelessness: (Where possible) Avoid storing session data
- Idempotence: Operations can be repeated safely
- Eventual Consistency: Accept temporary inconsistency for availability and performance
- Fail-Fast: Detect and report errors quickly
- Circuit Breaker: Isolate failing components
- Retry Mechanisms: Automatically retry failed operations
- Asynchronicity: Design for non-blocking communication Timeouts/Deadlines: Set limits to prevent indefinite waits

**DATA MANAGEMENT**

Distributed Databases
- NoSQL: MongoDB, Cassandra, DynamoDB (flexible schema, scalable)
- NewSQL: CockroachDB, YugabyteDB (scalable with SQL-like features)
- Distributed File Systems

    + HDFS: For big data (Hadoop)
    + Ceph: Unified, distributed storage system

- Caching: Redis, Memcached (in-memory for speed)
- ACID: Atomicity, Consistency, Isolation, Durability (relational database guarantees)
- BASE: Basically Available, Soft state, Eventual consistency (NoSQL database characteristics)
- Data Partitioning: Distributing data across nodes (sharding, hashing, range partitioning)
- Replication Strategies: Copying data for fault tolerance