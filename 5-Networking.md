# Module 5: Networking 

---

## Overview
This module introduces the **networking fundamentals** of AWS and explains how resources communicate securely within and outside the AWS Cloud.  
You’ll learn about **Virtual Private Clouds (VPCs)**, **subnets**, **gateways**, **VPNs**, and **Direct Connect**, as well as how **security groups**, **network ACLs**, and **DNS services** like **Route 53** and **CloudFront** keep data flowing safely and efficiently.

---

## Key Concepts

### What Is a Virtual Private Cloud (VPC)?
A **Virtual Private Cloud (VPC)** is a **logically isolated network** within the AWS Cloud where you can launch and manage AWS resources.  
It gives you full control over your networking environment — including IP addressing, subnets, routing, and security.

**Core Components of a VPC:**
- **Subnets**
- **Route Tables**
- **Internet Gateway**
- **Virtual Private Gateway**
- **Security Groups**
- **Network ACLs**

---

## Subnets
Subnets divide your VPC’s IP address range into smaller segments for better organization and security.

| Type | Description | Typical Use Case |
|------|--------------|------------------|
| **Public Subnet** | Connected to the internet through an internet gateway. | Web servers or resources that must be publicly accessible. |
| **Private Subnet** | Not directly connected to the internet. | Databases or internal services requiring isolation. |

---

## Internet Gateways and Routing
An **Internet Gateway (IGW)** allows communication between instances in your VPC and the internet.

- Each VPC can have only **one IGW** attached.
- The **Route Table** defines how network traffic is directed (e.g., to the internet or between subnets).

---

## Virtual Private Gateway (VGW)
A **Virtual Private Gateway** enables a **secure connection** between your on-premises network and your AWS VPC using a **VPN connection**.

**Good for:**  
Organizations needing encrypted, site-to-site communication between their data centers and AWS.

---

## VPN and Direct Connectivity Options

| Service | Description | Best For |
|----------|--------------|----------|
| **AWS Client VPN** | Allows individual users to securely connect to AWS resources from remote locations. | Remote employees accessing AWS privately. |
| **AWS Site-to-Site VPN** | Establishes an encrypted tunnel between on-prem networks and a VPC. | Secure hybrid connectivity between offices and AWS. |
| **AWS Direct Connect** | Provides a **dedicated physical connection** from your data center to AWS. | High-throughput, low-latency, or compliance-sensitive workloads. |
| **AWS PrivateLink** | Enables private connectivity between VPCs and AWS services without using the public internet. | Secure service-to-service communication within AWS. |

**Using VPN and Direct Connect Together:**  
You can combine both for **redundancy and high availability**, ensuring consistent network performance.

---

## Security in a VPC

### Security Groups (Stateful)
- Act as **virtual firewalls** for EC2 instances.  
- Evaluate traffic **based on rules** for inbound and outbound connections.  
- Because they’re **stateful**, return traffic is automatically allowed.

### Network Access Control Lists (Network ACLs) (Stateless)
- Control traffic at the **subnet level**.  
- Evaluate each packet **independently** (both inbound and outbound).  
- Must explicitly allow **return traffic**.

**Shared Responsibility Model:**  
- **AWS** secures the **infrastructure** of the VPC.  
- **You** configure and manage **security groups** and **network ACLs** within your VPC.

---

## Domain Name System (DNS) and Content Delivery

### What Is DNS?
**DNS (Domain Name System)** translates human-readable domain names (like `example.com`) into IP addresses computers use to communicate.

---

### Amazon Route 53
**Amazon Route 53** is AWS’s scalable DNS web service.

| Feature | Description |
|----------|--------------|
| **Domain Registration** | Register and manage domain names directly in AWS. |
| **DNS Routing** | Translate domain names into IP addresses for AWS resources. |
| **Health Checks** | Route traffic away from unhealthy endpoints automatically. |

**Use Cases:**
- Domain registration and routing for web apps.  
- Latency-based routing for multi-Region deployments.  
- Failover routing for disaster recovery setups.

---

### Amazon CloudFront
**Amazon CloudFront** is AWS’s **Content Delivery Network (CDN)** service.  
It uses **edge locations** around the world to cache and deliver content with low latency.

| Feature | Description |
|----------|--------------|
| **Global Edge Network** | Delivers content closer to users for faster performance. |
| **Integration** | Works with S3, EC2, and Route 53. |
| **Security** | Integrates with AWS Shield and WAF to protect against DDoS attacks. |

**Use Cases:**
- Accelerating website and video content delivery.  
- Protecting applications from network-level attacks.  
- Supporting multi-Region architectures with Route 53.

---

## Multi-Region Architecture
AWS supports **multi-Region architectures** for high availability, global performance, and disaster recovery.

- **CloudFront** handles global content distribution through edge locations.  
- **Route 53** directs users to the nearest or healthiest endpoint automatically.  

**Example:**  
A website hosted in both the US and Europe uses **Route 53** for routing and **CloudFront** for global caching, ensuring low latency for all users.

---

## Summary
AWS networking enables **secure, scalable, and flexible connectivity** across cloud and hybrid environments.  
With VPCs, subnets, gateways, and routing tools, you can design isolated networks and control traffic flow.  
Services like **VPN**, **Direct Connect**, **Route 53**, and **CloudFront** extend that connectivity globally and securely.

Understanding these tools helps you design resilient, high-performance cloud architectures that meet modern networking demands.

---

## Next Module ➡️
**Module 6: Storage** – Learn how AWS provides durable, scalable, and cost-effective storage solutions such as S3, EBS, and Glacier.
