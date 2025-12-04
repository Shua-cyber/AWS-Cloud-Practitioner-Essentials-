Overview

This module introduces the core AWS storage services, the differences between storage types, and how AWS storage fits into the shared responsibility model. You will also explore Amazon S3, EBS, EFS, FSx, Storage Gateway, and Elastic Disaster Recovery (DR), along with hands-on tasks in the AWS Management Console.

Storage Types
Block Storage

Data stored in fixed-size blocks.

Low-latency and high-performance.

AWS Service: Amazon EBS

Use Cases: Databases, boot volumes, transactional workloads.

Object Storage

Data stored as objects with metadata.

Massively scalable, durable, accessible over HTTP.

AWS Service: Amazon S3

Use Cases: Backups, static websites, media storage, big data.

File Storage

Data stored in hierarchical directories.

Accessible over network file protocols.

AWS Services: Amazon EFS, Amazon FSx

Use Cases: Shared storage, home directories, enterprise app migrations.

AWS Shared Responsibility Model & Storage

AWS: Infrastructure security, durability guarantees, hardware.

Customer: Data protection, encryption, access controls, backup policies, lifecycle configurations.

Amazon EC2 Instance Store

Description: Temporary, high-performance block storage physically attached to the host.

Benefits: Extremely fast I/O.

Use Cases: Caches, temporary data, buffers.

Note: Data is lost when the instance stops or terminates.

Amazon EBS (Elastic Block Store)
What it is

Persistent block storage volumes for EC2.

Benefits

Highly available within an Availability Zone.

Snapshots, encryption, resizing.

Use Cases

Databases, boot volumes, critical app data.

EBS Snapshots

Incremental backups stored in S3.

Use cases: Backup, migration, DR, versioning.

Customer Responsibilities: Backup strategies, snapshot lifecycle configs.

Data Lifecycle

Snapshots → Policies using Amazon Data Lifecycle Manager automate creation, retention, and deletion.

Amazon S3 (Simple Storage Service)
Key Benefits

11 nines of durability.

Nearly unlimited scalability.

Multiple managed storage classes.

Fine-grained security features.

Security Features

IAM policies

Bucket policies

Access Control Lists (ACLs)

S3 Block Public Access

Encryption (SSE-S3, SSE-KMS, SSE-C)

Storage Classes

S3 Standard

S3 Standard-IA

S3 One Zone-IA

S3 Glacier Instant Retrieval

S3 Glacier Flexible Retrieval

S3 Glacier Deep Archive

Intelligent-Tiering

S3 Lifecycle Policies

Automate moving objects to cheaper classes.

Automate expiration and clean-up.

Reduce long-term storage costs.

Hands-On Skills

Navigate the AWS Management Console.

Create and configure an S3 bucket.

Upload files and folders.

Configure system-defined and user-defined metadata.

📁 Amazon EFS (Elastic File System)
Benefits

Fully managed, elastic, POSIX-compliant file storage.

Scales automatically with workload.

Storage Classes

Standard

Standard-IA

One Zone

One Zone-IA

EFS Lifecycle Policies

Automatic tiering to IA classes based on access frequency.

🏢 Amazon FSx

Managed high-performance file systems for enterprise workloads.

Available File Systems

FSx for Windows File Server

FSx for Lustre

FSx for NetApp ONTAP

FSx for OpenZFS

Use Cases

Windows applications, HPC, machine learning, enterprise migrations.

🏠 AWS Storage Gateway

Hybrid storage service bridging on-prem and cloud.

Gateway Types

File Gateway – NFS/SMB to S3

Volume Gateway – iSCSI block storage with backups to S3

Tape Gateway – Virtual tape library for backups

Use Cases

Hybrid cloud backup

On-prem caching

Migration to cloud storage

Elastic Disaster Recovery (DRS)

Continuous replication for fast failover.

Reduced downtime and data loss.

Use cases: Business continuity, migration, DR automation.

Real-World Scenarios

Companies may use:

S3 for backups, logs, static hosting.

EBS for application storage or databases.

EFS/FSx for shared storage across multiple EC2 instances.

Storage Gateway for hybrid access.

Elastic DR for disaster recovery and failover planning.
