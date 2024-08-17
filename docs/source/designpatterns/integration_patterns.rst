Integration Patterns
===================================


**Extract, Transform, Load**

A process of extracting data from source systems, transforming it into a desired format or structure, and loading it into a target system, such as a data warehouse.

**Extract, Load, Transform**

A variation of ETL, where data is first loaded into the target system and then transformed leveraging the processing capabilities of modern data storage systems.

**Change data capture**

A technique for capturing and processing changes in source data, enabling incremental updates to target systems, & reducing the need for batch data transfers.

**Data Federation**

A technique for integrating data from disparate sources without physically moving or copying the data, providing a unified view of data across systems.

**Data Virtualization**

An approach that abstracts underlying data sources, enabling users and applications to access and manipulate data without needing to know its physical location.

**Data Replication**

The process of copying data from one database to another to ensure data availability, redundancy, and load balancing

**Data-Synchronization**

The process of keeping data in multiple locations or systems consistent and up-to-date by propagating changes
between systems.

**Data Preparation**

The process of cleaning, transforming, and enriching data to make it suitable for analysis, reporting, or further processing.

**Publish/Subscribe**

A messaging pattern that decouples data producers & consumers by using an intermediary to manage data distribution, enabling scalable & flexible data integration.

**Request/Reply**

A messaging pattern where a data consumer sends a request to a data producer & waits for a response, allowing for synchronous communication & data exchange.
