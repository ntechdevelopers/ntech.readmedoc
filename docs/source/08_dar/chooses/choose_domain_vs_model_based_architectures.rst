Domain vs Model Based Architectures
===================================

Domain-based architecture focuses on structuring systems around specific domains or problem entities. This architecture is based on dividing large, complex systems into smaller, more manageable sub-systems, each responsible for a specific domain of expertise or business functionality. The product is divided based upon various domains and physical entities. This helps deal with the complexity of modern-day software by focusing on the core business domain and creating clear boundaries between different parts.  

1. Features of Domain Driven Design  

- Ubiquitous Language  
- Bounded Contexts  
- Entities and Value Objects  
- Repositories and Services  
- Domain Events Sourcing  
- Aggregates and Factories  
- Strategic Context Mapping  

Various domains are determined for any business functionality and then mapped against other domains to determine dependencies. Once we have defined a set of domains (can be 500+ in bigger systems) and their relationships (1000+ in large systems), we then deal with entities, repositories, and aggregates.  
Aggregates deal with various groups of domains required for a specific business feature. Repositories and Services are generally part of business logic and deal with business functionality and database connections. Factories are responsible for creating complex aggregates or entities. Domain events are events of actions or transactions for a given business feature. Domain-driven architectures are highly useful in finance, healthcare, retail, supply chain, e-commerce, transportation, and others.  

2. Model Based Architectures (MBA)  

In this architecture, abstract models of a system or its components are used as primary artifacts throughout the development process. These models are often designed to represent various aspects of the software at different levels of abstraction, helping various stakeholders from different disciplines to communicate, analyze, simulate, and ultimately generate the final system implementation. The use of models simplifies the understanding of complex systems and guides decision-making through a structured representation with clearly defined models and rules for any business functionality. Models can be in various forms such as code, domains, and systems. They define how a system is designed, implemented, and utilized. This architecture in any system provides consistency, traceability, flexibility, and extendibility.  

3. Various Types of Models  

- Structured Model (UML, Component, Class Diagrams)  
- Behavioral Model (UML, Sequence, Activity Diagrams)  
- Interaction Model (Sequence, Collaboration Diagrams)  
- Data Model (Entity Relationship, Data Flow Diagrams)  
- Deployment Model (Platform, Infra, UML Diagrams)  
- Simulation Model (Analysis, Verifications, Testing)  

4. Business Use Cases  

- Embedded Systems  
- Aerospace, Aviation  
- Automotive, Transportation  
- Retail, Supply Chain  
- Inventory, Vendor Management  
- E-Commerce Platforms  
- Financial Platforms  
- Healthcare Systems