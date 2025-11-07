# Module 2: Compute in the Cloud 

## Overview
This module introduces **compute resources** in AWS — the engines that process workloads and run applications.  
You’ll learn how AWS provides flexible, scalable, and cost-efficient compute options through services like **Amazon EC2**, **AWS Lambda**, and **Elastic Beanstalk**.

---

## Key Concepts

### What Is Compute in AWS?
Compute resources provide the **processing power** required to run applications, perform calculations, and host workloads in the cloud.  
AWS compute services allow you to choose the right model — virtual machines, containers, or serverless — depending on your needs.

---

## Core Compute Services

| Service | Description | Key Benefit |
|----------|--------------|--------------|
| **Amazon EC2 (Elastic Compute Cloud)** | Virtual servers you can launch, configure, and scale on demand. | Full control over the OS, networking, and installed software. |
| **AWS Lambda** | Serverless compute service that runs code in response to events. | No servers to manage — pay only for compute time used. |
| **Amazon ECS (Elastic Container Service)** | Run and manage Docker containers at scale. | Simplifies container orchestration. |
| **Amazon EKS (Elastic Kubernetes Service)** | Managed Kubernetes service. | Deploy containerized applications with Kubernetes tools. |
| **AWS Elastic Beanstalk** | Platform as a Service (PaaS) for deploying web apps. | Automatically handles scaling and provisioning. |
| **AWS Fargate** | Serverless compute engine for containers. | Run containers without managing servers or clusters. |

---

## Interacting with EC2
| Name | Description | Key Benefit |
|----------|--------------|--------------|
| **AWS Management Console:** | Web interface for managing AWS services, offering quick access to services, search functionality, and simplified workflows. | Users who prefer a visual, easy-to-use interface for managing and configuring AWS services. |
| **AWS CLI:** | Manage multiple AWS services directly from the command line. Enables you to automate repetitive tasks using scripts. | Advanced users and developers who need to automate tasks, script actions. |
| **AWS SDK:** | Integrating AWS services into your applications by providing language-specific APIs. | Developers looking to integrate AWS services directly into applications using language-specific APIs. |

---

## EC2 Instance Concepts
- **Instance Type:** Defines CPU, memory, storage, and networking capacity (e.g., `t3.micro`, `m5.large`).
- **Amazon Machine Image (AMI):** Template for the OS and software configuration.
- **Instance Store & EBS:** Storage options for EC2 — instance store is temporary; EBS is persistent.
- **Security Groups:** Act as virtual firewalls controlling inbound and outbound traffic.
- **Elastic Load Balancing (ELB):** Distributes traffic across multiple EC2 instances.
- **Auto Scaling:** Automatically adjusts the number of instances to maintain performance and reduce cost.

---

## Serverless Computing
Serverless means you don’t provision or manage servers — AWS handles scaling, patching, and availability.

**Key Services:**
- **AWS Lambda:** Run code triggered by events (e.g., an image upload or API request).  
- **Amazon API Gateway:** Works with Lambda to expose REST APIs.  
- **AWS Step Functions:** Coordinate multiple serverless workflows.

---

## Elasticity and Scalability
- **Elasticity:** Automatically adjust capacity up or down based on demand.  
- **Scalability:** System’s ability to handle increased workload without performance degradation.  

These principles let AWS customers meet variable demand efficiently without manual intervention.

---

## Pricing Models for Compute
1. **On-Demand:** Pay by the hour or second; flexible and no commitment.  
2. **Savings Plans / Reserved Instances:** Commit to consistent usage for lower cost.  
3. **Spot Instances:** Use unused EC2 capacity for deep discounts (up to 90%), ideal for flexible workloads.  
4. **Dedicated Hosts:** Physical servers for compliance or licensing needs.
5. **Reserved Instances:** Get a savings of up to 75 percent by committing to a 1-year or 3-year term for predictable workloads using specific instance families and AWS Regions.
6. **Dedicated Instances:** Pay for instances running on hardware dedicated solely to your account. This option provides isolation from other AWS customers.

---

## Example Use Cases
- **Web Applications:** EC2 + Load Balancer + Auto Scaling for high availability.  
- **Event-Driven Apps:** S3 uploads trigger Lambda for serverless automation.  
- **Batch Processing:** Spot Instances handle large, flexible workloads cost-effectively.  
- **Containerized Services:** ECS or EKS for microservices architecture.

---

## Summary
Compute in AWS provides **flexible options** for running applications — from full control with EC2 to fully managed, event-driven solutions with Lambda.  
You can optimize for **cost, performance, and management effort** by choosing the right compute model.

---

## Next Module ➡️
**Module 3: Exploring Compute Services** – Dive deeper into scaling strategies, elasticity, and advanced compute capabilities in AWS.
