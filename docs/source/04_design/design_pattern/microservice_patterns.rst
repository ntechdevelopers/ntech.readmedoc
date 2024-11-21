Microservice Patterns  
===================================

1. API Gateway: 

- Entry point for microservices with cross-cutting concerns.  
- Handles security, rate limiting, and load balancing.  
- Utilizes tools like Spring Cloud Zuul or Spring Cloud Gateway.  

2. Service Discovery: 

- Allows services to find each other by name.  
- Manages dynamic IP changes caused by container spin-ups.  
- Implemented with Spring Cloud Eureka or Kubernetes service.  

3. Circuit Breaker:
 
- Prevents service failures by handling transient errors.  
- Offers fallback mechanisms or caches results.  
- Implemented using libraries like Hystrix or Resilient4J.  

4. Bulkhead:  

- Divides thread pools to isolate resources.  
- Prevents service failures from impacting others.  
- Implemented with Resilient4J for fault tolerance.  

5. CQRS (Command Query Responsibility Segregation): 

- Separates write and read operations for scalability.  
- Optimizes database tables differently.  

6. Event Driven Pattern:  

- Enables communication between services without coupling.  
- Uses event-driven messaging queues like RabbitMQ or Apache Kafka.  

7. Saga:  

- Manages distributed transactions scalably.  
- Offers Orchestration and Choreography options.  

8. Strangler Pattern:  

- Decomposes monolithic apps into microservices gradually.  
- Extracts features into separate microservices.  

9. Sidecar:  

- Attaches cross-cutting concern services alongside business services.  
- Deploys sidecar services in the same pod for seamless communication.  
- Utilizes tools like Envoy proxy.  

10. BFF (Backend for Frontend):  

- Customizes microservices for different platforms.  
- Optimizes performance based on platform requirements.  
- Ensures redundancy while avoiding resource waste.