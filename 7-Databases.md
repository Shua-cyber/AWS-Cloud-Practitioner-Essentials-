# Module 7: Databases 🗄️

## Overview
This module introduces AWS database services, the differences between relational and NoSQL databases, and how AWS manages database operations through fully managed services like **Amazon RDS**, **DynamoDB**, **Aurora**, and more.  
You will also explore caching, graph databases, backups, and the shared responsibility model for databases.

---

## Key Concepts

### Shared Responsibility Model for AWS Databases
| Area | Responsibility |
|------|----------------|
| **Infrastructure Security** | AWS manages the underlying hardware, patches, scaling, and maintenance. |
| **Customer Data & Access Control** | Customers manage schema, data encryption choices, user permissions, and database configurations. |
| **Backups & Availability (Managed Services)** | AWS automates backups and replication for services like RDS and DynamoDB. Customers configure retention and restore options. |

### Relational vs. NoSQL Databases
| Type | Description | Use Cases |
|------|-------------|-----------|
| **Relational (SQL)** | Structured, table-based storage with relationships and fixed schemas. | Financial apps, inventory, e-commerce, traditional enterprise workloads. |
| **NoSQL** | Flexible schema, highly scalable, designed for performance at scale. | Gaming, ad tech, IoT, real-time analytics. |

---

## AWS Database Services

### Amazon RDS (Relational Database Service)
| Feature | Description |
|--------|-------------|
| **Type** | Managed relational database service. |
| **Supports** | MySQL, PostgreSQL, MariaDB, Oracle, SQL Server. |
| **Benefits** | Automated backups, patching, snapshots, Multi-AZ replication, monitoring. |
| **Use Cases** | Traditional applications requiring SQL, high availability, and managed operations. |

### Amazon Aurora
| Feature | Description |
|--------|-------------|
| **Type** | High-performance relational database compatible with MySQL and PostgreSQL. |
| **Performance** | Up to 5× faster than MySQL and 3× faster than PostgreSQL. |
| **Benefits** | Distributed, fault-tolerant storage; auto-scaling; automated replication. |
| **Use Cases** | High-performance, scalable relational workloads. |

### Amazon DynamoDB (NoSQL)
| Feature | Description |
|--------|-------------|
| **Type** | Fully managed NoSQL key-value and document database. |
| **Performance** | Millisecond latency at any scale. |
| **Benefits** | Serverless, auto-scaling, global tables, built-in security. |
| **Use Cases** | Gaming, IoT, mobile apps, high-traffic workloads. |

### Amazon ElastiCache
| Feature | Description |
|--------|-------------|
| **Type** | Managed in-memory caching service for Redis and Memcached. |
| **Benefits** | Millisecond response times, reduces load on databases, accelerates application performance. |
| **Use Cases** | Session stores, caching layers, real-time leaderboards, high-throughput apps. |

### Amazon DocumentDB (with MongoDB compatibility)
| Feature | Description |
|--------|-------------|
| **Type** | Managed document database service compatible with MongoDB APIs. |
| **Benefits** | Scalable, fully managed, highly available. |
| **Use Cases** | Content management, catalogs, user profiles. |

### Amazon Neptune
| Feature | Description |
|--------|-------------|
| **Type** | Fully managed graph database service. |
| **Purpose** | Supports highly connected datasets using graph queries. |
| **Use Cases** | Knowledge graphs, fraud detection, social networking, recommendation engines. |

### AWS Backup
| Feature | Description |
|--------|-------------|
| **Type** | Centralized backup service for AWS workloads. |
| **Benefits** | Automated, policy-driven backups for RDS, DynamoDB, EFS, EC2, etc. |
| **Use Cases** | Compliance, disaster recovery, centralized backup management. |

---

## Hands-On: What You Will Do
| Task | Description |
|------|-------------|
| **Create Amazon RDS Instance** | Use the console to launch a managed relational database. |
| **Query RDS MySQL** | Create tables and add values using SQL queries. |
| **Create a DynamoDB Table** | Add items and interact with the table. |
| **Scan a DynamoDB Table** | Retrieve data using console tools. |

---

## Summary
AWS provides a wide range of fully managed database services for relational, NoSQL, in-memory, document, and graph data models.  
By offloading maintenance tasks like backups, patching, scaling, and replication to AWS, you can focus on application development.  
Understanding the strengths of each database type — along with their use cases — helps ensure you design scalable, high-performance data architectures in the cloud.

---
