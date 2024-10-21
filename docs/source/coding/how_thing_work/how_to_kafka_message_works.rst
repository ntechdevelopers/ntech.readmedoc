How to Kafka Message Works
===================================

**What is Kafka?**

Apache Kafka is an open-source distributed streaming platform designed for building real-time data pipelines and streaming applications. Kafka operates as a distributed pub-sub message system, allowing applications to publish and subscribe to real-time or near-real-time data feeds.
Apache Kafka is a high-throughput, scalable, and fault-tolerant messaging system that facilitates communication between producers and consumers via message-based topics. It’s designed for distributed applications, ensuring high availability with automatic recovery, making it suitable for large-scale data systems. Kafka’s key components include:

1. **Kafka Broker**: A node in the Kafka cluster that stores and replicates messages.
2. **Kafka Producer**: Sends messages to Kafka topics.
3. **Kafka Consumer**: Retrieves messages from Kafka topics.

**Kafka Architecture**

Apache Kafka has four core APIs that shape its architecture:

1. **Kafka Producer API**: Allows an application to publish a stream of records to one or more Kafka topics.
2. **Kafka Consumer API**: Subscribes to one or more topics and processes the stream of records produced.
3. **Kafka Streams API**: Lets applications process and transform data streams from input topics to output topics efficiently.
4. **Kafka Connector API**: Enables the creation of reusable producers or consumers that connect Kafka topics with external systems, such as real-time database change capturing.

**Kafka Components**

Kafka’s messaging system is built upon the following components:

1. **Kafka Topic**: Kafka stores messages in Topics, which are partitioned for scalability and replicated for fault tolerance, ensuring reliability.
2. **Kafka Producer**: Publishes messages to a Kafka topic.
3. **Kafka Consumer**: Subscribes to a topic(s), reads, and processes messages from the topic(s).
4. **Kafka Broker**: Manages the storage of messages in the topic(s). A Kafka cluster consists of multiple brokers.
5. **Kafka Zookeeper**: Manages metadata for brokers and facilitates health checking and leadership elections.
6. **Kafka Partition**: Each partition is either a leader or a replica. The leader handles reads and writes, while replicas sync data and take over if the leader fails.

**Kafka Use Cases**

1. **Messaging**: Kafka can replace traditional message brokers due to its superior throughput, partitioning, replication, and fault tolerance.
2. **Event Sourcing**: Kafka’s ability to store large logs makes it ideal for event sourcing, capturing all changes to the application state as a sequence of events.

**How to Build Your Own Kafka**

1. Implement TCP Server

Start by creating a TCP server on port 9092 to handle client connections.

2. Parse Correlation ID

Extract the correlation ID from client requests and return it in responses to match requests correctly.

3. Parse API Version

Check the API version sent by the client. If unsupported, respond with error code 35 (UNSUPPORTED_VERSION).

4. Handle API Versions Requests

Respond with a list of API keys and versions supported by the broker to ensure compatibility with clients.

5. Support Sequential Requests

Handle multiple sequential requests from the same client over a single connection, ensuring responses match requests.

6. Support Concurrent Requests

Enable concurrent request handling to allow multiple clients to interact with the broker simultaneously.

7. Implement Describe Topic Partitions API

Provide metadata about topics and partitions or return an error for unknown topics.

8. Implement Fetch API

Create the ability to fetch messages by extracting the topic ID and partition, retrieving messages, and returning them to the client.


These steps guide you through building a simple Kafka-like broker focused on the protocol layer. While distributed components like replication, failover, and consumer groups are not included, this build lays the foundation for understanding how real-world Kafka systems operate.
