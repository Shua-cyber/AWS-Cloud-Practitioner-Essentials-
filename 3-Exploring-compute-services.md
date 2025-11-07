Module 3: Exploring Compute Services 
Overview

This module dives deeper into AWS compute options and explores how to choose the right service based on control, flexibility, and operational needs.
You’ll learn how to compare Amazon EC2, AWS Lambda, and container-based services like Amazon ECS, Amazon EKS, and AWS Fargate.

Key Concepts
What Are Compute Services?

Compute services provide the infrastructure and resources to run applications in the cloud.
Each service varies in how much you manage versus how much AWS manages for you.

Level of Control	Example Service	Description
Full Control	Amazon EC2	You manage instances, scaling, OS updates, and security.
Partial Control	ECS / EKS	You manage containers; AWS manages orchestration or infrastructure.
Minimal Control	AWS Lambda / Fargate	AWS manages scaling, patching, and server maintenance.
Amazon EC2 (Elastic Compute Cloud)
Overview

Amazon EC2 provides virtual machines (instances) that give you full control over your compute environment.
You can choose instance types, storage, and networking configurations to match your workload needs.

Key Features

Choose from hundreds of instance types for different use cases.

Use Elastic Load Balancing (ELB) and Auto Scaling for performance and cost efficiency.

Secure access with key pairs and security groups.

Pay-as-you-go or use Reserved / Spot Instances for savings.

Common Use Cases

Web servers and enterprise applications

Development and test environments

Big data processing

Legacy workloads requiring full OS control

AWS Lambda
Overview

AWS Lambda is a serverless compute service that runs your code automatically in response to events.
You don’t provision or manage servers — AWS handles scaling and fault tolerance.

How It Works

Upload your code and define a trigger (like S3, DynamoDB, or API Gateway).

Lambda executes your function only when triggered.

You pay only for the compute time used.

Common Use Cases

Process files automatically when uploaded to S3.

Run backend logic for APIs with API Gateway.

Automate routine system tasks.

Execute scheduled jobs via Amazon EventBridge.

Container-Based Compute

Containers package code and dependencies together, making apps portable and consistent across environments.
AWS offers multiple services to deploy and manage containers at scale.

Amazon ECS (Elastic Container Service)

A fully managed container orchestration service that integrates tightly with other AWS services.

Best For:

Running Docker containers

AWS-native container management

Simplifying microservice deployments

Amazon EKS (Elastic Kubernetes Service)

A managed Kubernetes service that runs Kubernetes control planes and nodes for you.

Best For:

Teams already using Kubernetes

Multi-cloud or hybrid architectures

Complex workloads needing Kubernetes ecosystem tools

AWS Fargate

A serverless compute engine for containers that works with ECS and EKS.

Best For:

Running containers without managing EC2 instances

Simplifying container scaling and infrastructure management

Choosing the Right Compute Option
Service	Management Model	Scalability	Ideal For
EC2	Full control	Manual or Auto Scaling	Legacy apps, full OS access
Lambda	Fully managed (serverless)	Automatic	Event-driven or microservices
ECS / EKS	Shared (you + AWS)	Auto or manual	Containerized workloads
Fargate	Fully managed	Automatic	Serverless containers
Elastic Beanstalk (Review)

Although covered earlier, AWS Elastic Beanstalk bridges the gap between full control (EC2) and serverless simplicity.
It automatically handles capacity provisioning, load balancing, and deployment — great for developers who just want to upload code.

Key Terms

Compute Instance: Virtual server that runs applications in the cloud.

AMI (Amazon Machine Image): Template for launching EC2 instances.

Container: Lightweight, portable application environment.

Orchestration: Automated management of containerized applications.

Serverless: No server management — AWS handles infrastructure behind the scenes.

Summary

In this module, you explored how AWS compute services range from manual management (EC2) to fully managed (Lambda, Fargate).
You also learned about container-based compute options (ECS, EKS) that combine scalability with control.

By understanding each model, you can choose the right compute service for your specific workload, balancing cost, flexibility, and automation.

Next Module ➡️

Module 4: Going Global – Learn about AWS’s global infrastructure, including Regions, Availability Zones, and Edge Locations, and how they help deliver resilient, low-latency applications worldwide.
