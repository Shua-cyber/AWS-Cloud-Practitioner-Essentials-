# Module 9: Security 

## Overview
This module focuses on how AWS secures the cloud and how customers secure what they run in the cloud.  
You will learn about authentication, authorization, encryption, threat detection, incident response, and the AWS services that support security best practices.

---

## Key Concepts

| Concept | Description |
|--------|-------------|
| **Authentication** | Verifying who a user or system is. |
| **Authorization** | Determining what actions an authenticated entity is allowed to perform. |
| **Least Privilege** | Granting only the permissions required to perform a task. |
| **Shared Responsibility Model** | AWS secures the cloud; customers secure what’s in the cloud. |
| **Encryption at Rest** | Protecting stored data using encryption. |
| **Encryption in Transit** | Protecting data while it moves across networks. |
| **DDoS Attacks** | Attempts to overwhelm systems with traffic to disrupt services. |

---

## Authentication and Authorization

| Topic | Description |
|------|-------------|
| **Authentication** | Confirms identity using credentials, MFA, or federated identity. |
| **Authorization** | Uses policies to define permissions and access to resources. |
| **Benefit** | Prevents unauthorized access to enterprise data. |

---

## Shared Responsibility Model (Security)

| AWS Responsibilities | Customer Responsibilities |
|----------------------|---------------------------|
| Physical security of data centers | Identity and access management |
| Infrastructure security | Operating system & application security |
| Managed service protection | Data classification, encryption, monitoring |

---

## AWS Security Controls

| Control Type | Description |
|--------------|-------------|
| **Preventive** | Prevent security incidents (IAM, WAF). |
| **Detective** | Detect security events (GuardDuty, CloudTrail). |
| **Corrective** | Remediate issues (Systems Manager). |

---

## AWS Identity and Access Management (IAM)

| Feature | Purpose |
|--------|---------|
| **IAM** | Securely manage identities and access to AWS services and resources. |
| **IAM Users** | Individual identities within an AWS account. |
| **IAM Groups** | Collections of users with shared permissions. |
| **IAM Roles** | Temporary permissions for AWS services or trusted entities. |
| **IAM Policies** | JSON documents defining allowed or denied actions. |

---

## Root User Best Practices

| Best Practice | Description |
|---------------|-------------|
| Enable MFA | Adds strong protection to the root account |
| Use root sparingly | Only for account-level administrative tasks |
| Do not create access keys | Reduces risk of compromise |

---

## Identity & Least Privilege Services

| Service | Description |
|---------|-------------|
| **AWS IAM Identity Center** | Centralized workforce access with single sign-on (SSO). |
| **AWS Secrets Manager** | Secure storage and rotation of credentials and API keys. |
| **AWS Systems Manager** | Securely manage nodes across AWS and hybrid environments. |

---

## DDoS Protection

| Topic | Description |
|------|-------------|
| **DDoS Attacks** | Flood networks or applications to disrupt availability. |
| **AWS Protection** | Global infrastructure absorbs and mitigates attacks. |

---

## DDoS Defense Services

| Service | Purpose |
|---------|---------|
| **AWS Shield** | Protects against common and large-scale DDoS attacks. |
| **AWS WAF** | Filters traffic using web ACLs and IP rules. |

---

## Data Encryption

| Encryption Type | Description |
|------------------|-------------|
| **At Rest** | Encrypts stored data. |
| **In Transit** | Encrypts data moving across networks using TLS/SSL. |

---

## Encryption & Key Management

| Service | Purpose |
|---------|---------|
| **AWS KMS** | Create and manage cryptographic keys. |
| **AWS Certificate Manager (ACM)** | Manage SSL/TLS certificates for encryption in transit. |

---

## Data Protection & Classification

| Service | Description |
|---------|-------------|
| **Amazon Macie** | Discovers and protects sensitive data in Amazon S3. |

---

## Threat Detection & Vulnerability Management

| Service | Description |
|---------|-------------|
| **Amazon Inspector** | Detects vulnerabilities and security misconfigurations. |
| **Amazon GuardDuty** | Continuously monitors for malicious activity. |
| **Amazon Detective** | Investigates security issues with visual analysis. |
| **AWS Security Hub** | Aggregates and prioritizes security findings. |

---

## Incident Detection & Response

| Capability | AWS Services |
|------------|--------------|
| Detection | GuardDuty, Inspector |
| Investigation | Amazon Detective |
| Aggregation | AWS Security Hub |
| Remediation | AWS Systems Manager |

---

## AWS Security Documentation & Resources

| Resource | Purpose |
|---------|---------|
| **AWS Security Documentation** | Best practices and compliance guidance. |
| **AWS Well-Architected Framework (Security Pillar)** | Secure design principles. |
| **AWS Marketplace Security Tools** | Third-party security solutions. |

---

## Summary
In Module 9, you learned how authentication and authorization protect AWS environments, how responsibility for security is shared between AWS and customers, and how to apply the principle of least privilege.  
You explored AWS services for identity management, encryption, DDoS protection, threat detection, and incident response, helping build secure and resilient cloud environments.

