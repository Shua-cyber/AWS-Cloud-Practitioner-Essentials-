# Module 8: Introduction to AI & Machine Learning 

## Overview
This module introduces **artificial intelligence (AI)**, **machine learning (ML)**, **deep learning**, and **generative AI**, along with how AWS provides services to implement these technologies.  
You will also learn about ETL pipelines, data analytics, and the AWS AI/ML service stack, including pre-built AI services, SageMaker, and foundation models.

---

## Key Concepts

| Concept | Description |
|---------|-------------|
| **Artificial Intelligence (AI)** | Systems that perform tasks normally requiring human intelligence. |
| **Machine Learning (ML)** | Subset of AI where systems learn from data to make predictions or decisions. |
| **Deep Learning** | ML subset using multi-layer neural networks for complex pattern recognition. |
| **Generative AI** | Creates new content (text, images, audio, code) using AI models. |
| **ETL Pipelines** | Extract, Transform, Load pipelines for ingesting, processing, and storing data. |
| **Data Analytics** | Analyzing and visualizing data to extract insights. |
| **AWS AI/ML Stack Tiers** | Pre-built AI services, SageMaker for ML, and frameworks/infrastructure for deep learning. |

---

## AWS AI/ML Stack

| Tier | Description |
|------|-------------|
| **AI Services (Top Tier)** | Pre-built AI services for language, vision, search, and personalization. No ML expertise required. |
| **ML Services (Middle Tier)** | Amazon SageMaker for building, training, and deploying ML models. Requires some ML experience. |
| **ML Frameworks & Infrastructure (Bottom Tier)** | Deep learning AMIs, containers, and frameworks like PyTorch/TensorFlow for expert practitioners. |

---

## AWS AI Services

| Service | Description |
|---------|-------------|
| **Amazon Comprehend** | Extracts insights from text documents using NLP. |
| **Amazon Polly** | Converts text into lifelike speech. |
| **Amazon Transcribe** | Converts speech into text for transcription and search. |
| **Amazon Translate** | Automatically translates text into multiple languages. |
| **Amazon Kendra** | Enterprise search powered by NLP. |
| **Amazon Rekognition** | Identifies objects, faces, and activities in images and videos. |
| **Amazon Textract** | Extracts typed and handwritten text from documents. |
| **Amazon Lex** | Builds voice and text conversational interfaces. |
| **Amazon Personalize** | Adds personalized recommendations to applications. |

---

## AWS ML Development Services

| Service | Description |
|---------|-------------|
| **Amazon SageMaker AI** | Build, train, and deploy ML models without managing infrastructure. |
| **SageMaker JumpStart** | Deploy pre-trained ML solutions for vision, NLP, and tabular data with minimal effort. |

---

## AWS Generative AI Services

| Service | Description |
|---------|-------------|
| **Amazon Bedrock** | Access, fine-tune, and integrate foundation models via a single API. |
| **Amazon Q Business** | Answers questions using organizational data. |
| **Amazon Q Developer** | Accelerates development with AI-driven code recommendations. |

---

## AWS Data Ingestion Services

| Service | Description |
|---------|-------------|
| **Amazon Kinesis Data Streams** | Ingests terabytes of streaming data in real time. |
| **Amazon Data Firehose** | Delivers streaming data within seconds to S3, Redshift, OpenSearch, or analytics tools. |

---

## AWS Data Storage Services

| Service | Description |
|---------|-------------|
| **Amazon S3** | Highly durable object storage for data lakes, ML datasets, and backups. |
| **Amazon Redshift** | Petabyte-scale data warehouse for SQL analytics on structured and semi-structured data. |

---

## AWS Data Cataloging, ETL, and Big Data Services

| Service | Description |
|---------|-------------|
| **AWS Glue Data Catalog** | Centralized metadata repository for analytics services. |
| **AWS Glue** | ETL service for processing and preparing data at scale. |
| **Amazon EMR** | Managed clusters for big data frameworks like Apache Spark and Hadoop. |

---

## AWS Analytics & Visualization Services

| Service | Description |
|---------|-------------|
| **Amazon Athena** | Serverless SQL query engine for analyzing data in S3 and other sources. |
| **Amazon QuickSight** | BI service for interactive dashboards and data visualization. |
| **Amazon OpenSearch Service** | Real-time search, analytics, and log visualization with keyword or NLP queries. |

---

## ETL Pipeline Overview

| Phase | AWS Services & Purpose |
|-------|----------------------|
| **Ingestion** | Amazon Kinesis Data Streams, Amazon Data Firehose |
| **Processing** | AWS Glue, Amazon EMR, AWS Lambda |
| **Storage** | Amazon S3, Amazon Redshift, DynamoDB, RDS |
| **Visualization / Analytics** | Amazon QuickSight, Athena, SageMaker notebooks |

---

## Example Use Case

| Process | Description |
|---------|-------------|
| **Ingestion** | Company streams user activity into Kinesis. |
| **Processing** | AWS Glue cleans and transforms the data. |
| **Storage** | Data lands in S3 and Redshift. |
| **Delivery** | QuickSight dashboards visualize insights for stakeholders. |

---

## Summary
Module 8 covers AI, ML, deep learning, and generative AI, along with the AWS services that support them. You learned the three-tier AWS AI/ML stack, from pre-built AI services to SageMaker and deep learning frameworks.  
Generative AI, NLP, computer vision, and analytics services enable companies to build intelligent applications efficiently.  
ETL pipelines, storage, and visualization services illustrate how AWS supports end-to-end AI/ML data workflows, from ingestion to insights.

---
