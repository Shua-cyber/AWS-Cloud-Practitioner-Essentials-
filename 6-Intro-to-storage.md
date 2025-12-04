# Module 6 – Intro to Storage

## Overview
In this module, you explore AWS storage types, core AWS storage services, lifecycle features, security responsibilities, and real-world cloud storage architectures.

---

## Storage Types

| Storage Type | Description | AWS Services | Common Use Cases |
|--------------|-------------|--------------|------------------|
| Block Storage | Data stored in fixed-size blocks; low-latency access | Amazon EBS, EC2 Instance Store | Databases, OS boot volumes, transactional apps |
| Object Storage | Data stored as objects with metadata; massively scalable | Amazon S3 | Backups, static websites, data lakes, analytics |
| File Storage | Shared file system with hierarchical structure | Amazon EFS, Amazon FSx | Distributed apps, enterprise workloads, HPC |

---

## Shared Responsibility Model (Storage)

| AWS Responsibility | Customer Responsibility |
|--------------------|-------------------------|
| Ensuring durability & availability of storage infrastructure | Data protection & access control (IAM, policies) |
| Securing hardware & global network | Encryption keys, bucket/object permissions |
| Maintaining AWS-managed services | Lifecycle policies, backup strategy, compliance |

---

## Block Storage Services

### EC2 Instance Store

| Feature | Summary |
|--------|---------|
| What it is | Temporary block storage physically attached to host |
| Benefits | Extremely high I/O performance |
| Limitations | Data lost on stop/terminate |
| Best For | Caches, buffers, ephemeral workloads |

---

### Amazon EBS

| Feature | Summary |
|--------|---------|
| What it is | Persistent block storage for EC2 |
| Benefits | High durability, encryption, resizing, snapshots |
| Best For | Databases, OS disks, production workloads |

#### EBS Snapshots

| Topic | Details |
|-------|---------|
| Purpose | Incremental backups stored in S3 |
| Benefits | Fast restore, cross-region copy, DR |
| Tools | Automated via Data Lifecycle Manager (DLM) |

#### EBS Lifecycle

| Phase | Description |
|-------|-------------|
| Volume | Live data attached to EC2 |
| Snapshot | Backup stored in S3 |
| Policies | Automate retention & cleanup |

---

## Object Storage Services

### Amazon S3

| Feature | Summary |
|--------|---------|
| What it is | Highly durable, scalable object storage |
| Security | IAM, bucket policies, ACLs, encryption, Block Public Access |
| Best For | Backup, archives, media storage, data lakes |

#### S3 Storage Classes

| Storage Class | Best Use Case |
|----------------|----------------|
| Standard | Frequently accessed data |
| Standard-IA | Long-lived but infrequently accessed data |
| One Zone-IA | Non-critical, infrequent access in 1 AZ |
| Intelligent-Tiering | Automatically optimizes cost |
| Glacier Instant Retrieval | Archive with sub-second access |
| Glacier Flexible Retrieval | Archive with minutes–hours access |
| Glacier Deep Archive | Lowest-cost long-term archival |

#### S3 Lifecycle Policies

| Purpose | Description |
|---------|-------------|
| Transition | Move objects between storage classes |
| Expiration | Delete objects after defined period |
| Pricing Impact | Reduces cost by optimizing storage tiers |

---

## File Storage Services

### Amazon EFS

| Feature | Summary |
|--------|---------|
| What it is | Fully managed, elastic NFS file system |
| Benefits | Scales automatically, multi-AZ |
| Best For | Shared workloads, lift-and-shift apps |

#### EFS Storage Classes

| Storage Class | Description |
|----------------|-------------|
| Standard | Multi-AZ storage |
| One Zone | Single-AZ, lower cost |
| IA (Infrequent Access) | Lower cost for infrequent data |

#### EFS Lifecycle

| Feature | Description |
|--------|-------------|
| Lifecycle Management | Automatically moves files to cost-effective storage |
| Pricing Impact | Reduces cost for cold data |

---

## Amazon FSx

| Type | Best For |
|------|----------|
| FSx for Windows File Server | Windows apps, SMB protocol |
| FSx for Lustre | HPC workloads |
| FSx for Ontap | NetApp workloads |
| FSx for OpenZFS | Linux apps needing ZFS |

---

## Hybrid Storage

### AWS Storage Gateway

| Gateway Type | Description |
|--------------|-------------|
| File Gateway | NFS/SMB interface to S3 |
| Volume Gateway | Block storage backed by S3 |
| Tape Gateway | Virtual tapes for backup apps |

---

## Disaster Recovery

### AWS Elastic Disaster Recovery (EDR)

| Feature | Summary |
|--------|---------|
| Purpose | Replicates on-premises or cloud workloads to AWS |
| Benefit | Fast recovery and business continuity |
| Use Case | DR, migration, resilience |

---

## Real-World Scenarios

| Scenario | Example AWS Service |
|----------|---------------------|
| Backup & archival | S3 + Glacier tiers |
| Database storage | EBS volumes |
| Shared storage for applications | EFS |
| Enterprise file systems | FSx |
| Hybrid cloud continuity | Storage Gateway |
