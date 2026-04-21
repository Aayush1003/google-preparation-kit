# System Design

System Design becomes increasingly important as you target L4, L5, and above roles. Google looks for candidates who can build large-scale, distributed systems that handle immense traffic, are highly available, and are fault-tolerant.

## High-Level Design (HLD)
You'll typically be asked to design an architecture for a well-known service (e.g., "Design YouTube, Design Google Drive, Design a Web Crawler").

### Core Concepts to Understand
- **Scalability:** Horizontal vs. Vertical Scaling.
- **Load Balancing:** Algorithms and approaches.
- **Caching:** Distributed caching (Redis, Memcached), CDN, eviction policies (LRU, LFU).
- **Databases:** Relational vs. NoSQL, Sharding, Replication, CAP Theorem, Eventual Consistency.
- **Message Queues:** Kafka, RabbitMQ, when to use asynchronous processing.
- **Microservices:** Service discovery, API Gateways.

### The System Design Framework
1. **Requirements Clarification:** Understand functional and non-functional requirements.
2. **Back-of-the-envelope Estimation:** Traffic, storage, and bandwidth estimates.
3. **System API Design:** Define the contracts.
4. **Data Model:** Choose the right database and schema.
5. **High-Level Design:** Draw the basic architecture.
6. **Detailed Design:** Deep dive into specific components or bottlenecks.
7. **Resolving Bottlenecks:** Address single points of failure, scaling, and fault tolerance.

## Low-Level Design (LLD) / Object-Oriented Design
Sometimes asked for L4/L3 roles. Focuses on writing modular, extensible code using Object-Oriented principles.
- Design Patterns (Singleton, Factory, Strategy, Observer)
- SOLID Principles
- Typical problems: Design a Parking Lot, Design an Elevator System.

## Resources
- ByteByteGo / Alex Xu's System Design Interview
- Grokking the System Design Interview
- Google Whitepapers (MapReduce, BigTable, Spanner) - *Highly recommended for senior roles.*
