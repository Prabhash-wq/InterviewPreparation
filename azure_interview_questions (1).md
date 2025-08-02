# Azure Interview Questions and Answers for 8+ Years Experienced Candidates

[...previous content retained...]

## Azure Storage Services

### Q34. What is Azure Storage? What are the types of Azure Storage?
**Answer:** Azure Storage is a scalable, durable, and secure cloud storage solution offered by Microsoft. It supports modern data storage scenarios such as big data analytics, backup, and archiving. Types include:
- **Blob Storage:** Optimized for storing massive amounts of unstructured data such as images, videos, backups, or logs. Example: Hosting images for a website.
- **File Storage:** Managed file shares accessible over SMB protocol. Example: Lift-and-shift legacy applications needing shared storage.
- **Queue Storage:** Message queuing for communication between distributed app components. Example: Handling background order processing.
- **Table Storage:** NoSQL store for structured key-value pairs. Example: User profile data for a web application.
- **Disk Storage:** Persistent storage for Azure VMs. Example: OS disk and data disk for a virtual machine.

### Q35. Explain Azure Blob Storage. Use case?
**Answer:** Azure Blob Storage allows storing large amounts of unstructured data like media files, logs, or backups. It's cost-effective and supports hot, cool, and archive tiers for data lifecycle management. 
**Use case:** Store backups of application logs or serve static assets (CSS, JS) in a web application.

### Q36. Explain Azure File Storage. Use case?
**Answer:** Azure Files offers fully managed file shares accessible via SMB or NFS. It's commonly used for lifting and shifting legacy apps to Azure.
**Use case:** Replace on-prem file servers with Azure Files for storing shared configuration files.

### Q37. Explain Azure Table Storage. Use case?
**Answer:** Table Storage is a NoSQL key-attribute store, good for storing large volumes of semi-structured data.
**Use case:** Storing IoT sensor data that doesn't require complex joins or relationships.

### Q38. Explain Azure Queue Storage. Use case?
**Answer:** Provides reliable message queuing for communication between components.
**Use case:** Web app queues user signup events for async processing.

### Q39. Format for Azure Queue messages?
**Answer:** Messages are Base64-encoded strings up to 64 KB each. They can be JSON or plain text.
**Example:** A message body like `{ "OrderId": "1234", "Status": "Pending" }`.

### Q40. What is Azure Disk Storage?
**Answer:** Used for attaching persistent, high-performance disks to Azure VMs. Comes in HDD or SSD flavors.
**Example:** Use Premium SSD for database VM to ensure fast IOPS.

### Q41. Types of Disk Storage?
**Answer:**
- **Premium SSD:** Ideal for I/O-intensive apps like databases.
- **Standard SSD:** Balanced option for general workloads.
- **Standard HDD:** Budget-friendly, good for dev/test or backups.

## Azure Database Services

### Q42. What is Azure SQL Database? Difference from SQL Server?
**Answer:** Azure SQL Database is a fully managed PaaS version of SQL Server that automates updates, patching, HA, and backups.
**Difference:** SQL Server is IaaS/on-prem; Azure SQL is PaaS with automatic maintenance.

### Q43. Difference between Azure SQL DB and SQL Managed Instance?
**Answer:**
- **SQL DB:** Single database or elastic pools; limited SQL Server features.
- **Managed Instance:** Near-complete SQL Server compatibility; suitable for migration.
**Example:** Use Managed Instance to lift-and-shift a legacy ERP system.

### Q44. What is Azure Cosmos DB? When to use?
**Answer:** A globally distributed NoSQL DB that supports multiple APIs (SQL, MongoDB, Cassandra). Ensures low latency and high availability.
**Use case:** E-commerce website needing global replication and low-latency access.

### Q45. What is NoSQL?
**Answer:** A non-relational database system optimized for scalability, performance, and flexible schema.
**Types:** Document, key-value, graph, column-family.

### Q46. NoSQL vs RDBMS?
**Answer:**
- **NoSQL:** Schema-less, horizontally scalable. Best for unstructured data (e.g., social feeds).
- **RDBMS:** Fixed schema, supports joins and transactions. Best for structured, relational data.

### Q47. When to use SQL vs Cosmos DB?
**Answer:**
- **SQL:** Use when you need ACID transactions, joins, and reporting.
- **Cosmos DB:** Use for globally distributed, high-throughput workloads like gaming or IoT.

## Azure Networking - Part 1

### Q48. What is a VNet?
**Answer:** A Virtual Network is a private, isolated section of the Azure cloud where resources like VMs communicate securely.
**Example:** Deploying a 3-tier app where frontend, backend, and DB are in separate subnets within a VNet.

### Q49. How do VMs in VNets get external access?
**Answer:** Via a Public IP address, NAT Gateway, or Load Balancer configured to forward traffic.

### Q50. Difference between Private IP and Public IP?
**Answer:**
- **Private IP:** Internal communication within VNet or on-prem via VPN/ExpressRoute.
- **Public IP:** Enables external access to Azure resources.

### Q51. What is Azure Load Balancer?
**Answer:** A Layer 4 (TCP/UDP) load balancer that distributes incoming traffic across multiple backend VMs.
**Use case:** Distribute HTTP traffic across multiple web servers.

### Q52. What is Application Gateway?
**Answer:** A Layer 7 load balancer for HTTP/HTTPS traffic. Supports SSL termination and Web Application Firewall (WAF).
**Use case:** Host multiple sites behind a single gateway using URL-based routing.

### Q53. When to use Load Balancer vs App Gateway?
**Answer:**
- **LB:** When you need simple port-based traffic distribution.
- **AG:** When you need SSL offload, WAF, or routing based on HTTP headers/URLs.

### Q54. Can they be used together?
**Answer:** Yes. For example, App Gateway can handle HTTPS traffic and forward it to internal Load Balancer for TCP-based services.

[...continued with the same structure for remaining sections...]

