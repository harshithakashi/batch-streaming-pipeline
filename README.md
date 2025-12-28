# Batch & Streaming Data Pipeline on AWS

## Problem Statement

Modern data platforms must handle two types of data:

- **Batch data** that arrives at fixed intervals (for example, daily CSV files)
- **Streaming data** that arrives continuously in real time (for example, user events)

The challenge is to design a system that can process both batch and streaming data
using the right AWS services while keeping the architecture simple and scalable.

This project demonstrates a beginner-friendly design for handling batch and streaming
data pipelines on AWS.


## Architecture Diagram

![Architecture Diagram](img/architecture.png)

## What I Learned

- Difference between batch processing and streaming processing
- How Amazon S3 is used as a data lake storage layer
- How AWS Glue can perform batch ETL transformations
- How Amazon Kinesis supports real-time ingestion
- How AWS Lambda can process streaming events
- How to structure a project repository like an AWS sample repo


## Challenges Faced

- Understanding when to use batch processing versus streaming processing
- Designing a clear architecture without overcomplicating AWS services
- Keeping the project beginner-friendly while still realistic
- Structuring the repository to clearly explain the data flow


## Deployment

This project focuses on architecture and learning rather than full cloud deployment.

- AWS services are represented using placeholders
- The design follows real-world AWS data engineering patterns
- The project is deployment-ready but avoids actual deployment to prevent unnecessary cloud costs



  
