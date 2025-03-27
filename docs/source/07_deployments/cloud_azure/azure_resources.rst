Azure Resources
===================================

One of the best cloud providers that has huge depth of services for DevOps, Data Storage, Artificial Intelligence, Machine Learning, Data Analytics and Computation. Azure cloud can have any type of technical application (microservices, functions, systems, large products, platforms or monolithic monsters) deployed using any networking subnets with various security protocols, identity access management, ingress, outgress rules, traffic policies. 
Azure also has various types of computational deployments (virtual servers, clusters, containers) on any OS (Linux, Windows) for different programming languages, frameworks (Java, Spring .Net framework, Python, Go..) and using any type of data storage and messaging queues. Storage can be non relational and relational.
Azure also provides a huge benefit on DevOps offering tools for source code management, test pipelines, deployment mechanism and boards for user stories and tasks. Therefore, a lot of tools are replaced by Azure DevOps such as GitHut, JIRA, Jenkins and others. Azure also provides various other tools, services and products for data analytics, artificial intelligence and machine learning.
Other services provided by Azure are used for content delivery networks, virtual networks, identity access management, batch processing, monitoring (logging, observability), reporting and queues, topics for dealing with events, triggers and messages.
It also provides services for migration of application, data to Azure cloud and using other services, products from various other cloud providers through multi cloud products. Azure also has various services for mobile, web and digital development. Cloud native development encompassing whole software development Lifecyle is also provided by couple of services.

- Artificial Intelligence
- Data Analytics
- Blob, Vector, File Storage
- Messaging Queues
- Event Grids
- Content Delivery Networks
- Virtual Networks
- App Observability
- DevOps (Source, Code)
- DevOps (Boards, CI/CD)
- DevOps (Artifacts, Testing)
- Machine Learning
- Web Development
- Mobile Development
- Digital Transformation
- Automation & Batch Processing
- Non Relational Storage
- Relational Storage
- Various Types of Storage
- Access, Identity Mgmnt
- Firewalls, Security
- Serverless Functions
- Compute (Container, Servers)
- Key Vaults, Security Mgmnt
- API Management
- Disaster Recovery
- Migration To Cloud
- Enterprise Integration
- Middleware Platform
- DataOps Tools
- CloudNative Tools
- IoT Services

**What is an Azure Landing Zone?**  

When embarking on a cloud journey with Azure, one of the key concepts you will encounter is the Azure landing zone. But what exactly is it, and why should you care?  

An Azure landing zone is a well-architected environment that ensures your cloud infrastructure is scalable, secure, and efficient. It is built around key design principles that span across eight critical areas: Azure billing, identity and access management, resource organization, network topology and connectivity, security, management, governance, and platform automation and DevOps. These principles help in accommodating all application portfolios, whether you are migrating existing applications, modernizing them, or creating new innovations at scale.  

1. Architecture and Subscriptions   

The architecture of an Azure landing zone is modular and scalable, meaning it can grow with your needs. It uses subscriptions to isolate and scale both application resources and platform resources. Think of it like this: the application landing zones are where your specific apps live, while the platform landing zones provide the shared services those apps need to function smoothly.  

2. Platform vs. Application Landing Zones   

- **Platform Landing Zones**: These are subscriptions that provide shared services such as identity, connectivity, and management. By centralizing these services, you can improve operational efficiency and streamline management. Typically, these zones are managed by a central IT team.  
- **Application Landing Zones**: These are the individual subscriptions where your applications run. You can pre-provision these through code and assign policy controls to them via management groups. Depending on your needs, application landing zones can be managed by a central team, the application team, or a shared management model.  

3. Accelerators  

To make deployment easier, Azure provides landing zone accelerators. These are ready-made infrastructure-as-code solutions that help you set up your landing zones quickly and correctly. Whether you are using the Azure portal, Bicep, or Terraform, these accelerators can save you time and ensure best practices are followed.  

In summary, Azure landing zones offer a structured and efficient way to set up your cloud environment, ensuring it is ready to support your applications securely and at scale. By understanding and utilizing both platform and application landing zones, along with accelerators, you can streamline your cloud journey and focus on what truly matters—driving business value through innovation.

.. image:: ./imgs/azure_resources.jfif
  :width: 1000
  :alt: azure_resources.jfif