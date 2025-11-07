# Module 3: Exploring Compute Services 🧩

---

## Overview
This module focuses on **modern compute services in AWS**, including containers, orchestration tools, and managed platforms. You’ll learn how services like **ECS**, **EKS**, **Fargate**, and **Elastic Beanstalk** simplify application deployment, scaling, and management.  

It also covers **Amazon Lightsail**, **AWS Batch**, and **AWS Outposts**, which extend compute flexibility to specific use cases and environments.

---

## Key Concepts

### What Are Containers?
Containers are **lightweight, portable packages** that include everything needed to run an application—code, runtime, and dependencies.  
AWS offers multiple services to **store, orchestrate, and run containers** efficiently.

| Term | Description |
|------|--------------|
| **Container** | A standardized unit of software that runs reliably across environments. |
| **Image** | A snapshot of a container’s file system used to launch instances of containers. |
| **Orchestration** | The process of automating deployment, scaling, and management of containerized applications. |

---

## Core Container Services

| Service | Description | Key Benefit |
|----------|--------------|--------------|
| **Amazon Elastic Container Registry (ECR)** | Fully managed container image registry for storing, managing, and deploying container images securely. | Simplifies image management with integrated security and scalability. |
| **Amazon Elastic Container Service (ECS)** | Fully managed container orchestration service that runs Docker containers on AWS. | Simplifies running and scaling containerized applications. |
| **Amazon Elastic Kubernetes Service (EKS)** | Fully managed Kubernetes service for running Kubernetes clusters on AWS and on premises. | Provides Kubernetes automation with deep AWS integration. |
| **AWS Fargate** | Serverless compute engine for running containers without managing servers or clusters. | Eliminates server management—pay only for container resources used. |

---

## AWS Elastic Beanstalk
**AWS Elastic Beanstalk** is a **Platform as a Service (PaaS)** that makes it easy to deploy, manage, and scale web applications.  

AWS handles the underlying infrastructure (servers, OS, scaling, load balancing), letting developers focus on code.

**Good for:** Developers who want to deploy applications quickly without managing servers.

**Common Use Cases:**
- Hosting web apps built in Python, Node.js, Java, or .NET  
- Automatically scaling and load balancing web environments  
- Rapid prototyping or staging environments  

---

## AWS Batch
**AWS Batch** efficiently runs **large-scale batch computing jobs** across AWS compute services.  

It automatically provisions compute resources and optimizes workload scheduling based on job requirements.

**Good for:** High-performance workloads that need to process large volumes of data, such as analytics, simulations, or scientific computing.

**Example Use Cases:**
- Image or video processing  
- Financial risk modeling  
- Genomics data analysis  

---

## Amazon Lightsail
**Amazon Lightsail** provides a **simplified cloud platform** for users who want to quickly deploy virtual private servers (VPS), containers, and databases.  

It offers predictable, low-cost pricing and preconfigured environments for small-scale applications.

| Feature | Description |
|----------|--------------|
| **VPS hosting** | Easily launch and manage virtual servers. |
| **Container support** | Run lightweight container workloads without deep AWS knowledge. |
| **Predictable pricing** | Fixed monthly cost for compute, storage, and data transfer. |

**Good for:** Small businesses, students, or developers needing an easy entry point into AWS.

---

## AWS Outposts
**AWS Outposts** extends AWS infrastructure and services to **on-premises** locations.  

It provides a **hybrid cloud** model, enabling local compute and data storage with consistent AWS tools and APIs.

**Good for:** Workloads requiring **low latency**, **local data processing**, or **data residency compliance**.

**Example Use Cases:**
- Real-time factory or hospital systems  
- Local analytics with data residency constraints  
- On-premises applications needing cloud integration  

---

## Choosing a Modern Application Strategy
AWS provides guidance through the **Decision Guide for Modern Application Strategy**, which helps organizations decide between **serverless** and **Kubernetes-based** approaches.

| Approach | Description | Best For |
|-----------|--------------|----------|
| **Serverless** | Automatically manages scaling, patching, and infrastructure (e.g., AWS Lambda, Fargate). | Teams focusing on agility, cost optimization, and minimal operations. |
| **Kubernetes (EKS)** | Provides full control of orchestration and configuration using Kubernetes tools. | Teams needing portability, customization, or hybrid/multi-cloud strategies. |

---

## Summary
AWS offers multiple compute services to match every application strategy:

- **Containers:** Managed through ECR, ECS, and EKS for flexible, scalable workloads.  
- **Serverless Compute:** Fargate and Lambda reduce management overhead.  
- **Application Management:** Elastic Beanstalk automates deployment and scaling.  
- **Specialized Compute:** Lightsail simplifies VPS hosting, AWS Batch handles large-scale processing, and Outposts extends AWS to on-prem environments.  
- **Modern App Strategy:** Choose serverless for simplicity or Kubernetes for control.

---

## Next Module ➡️
**Module 4: Storage Services** – Learn how AWS provides durable, scalable, and cost-effective storage solutions with services like S3, EBS, and Glacier.

