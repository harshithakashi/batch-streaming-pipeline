# Batch & Streaming Data Pipeline (Beginner Friendly)

This project demonstrates a **simple end-to-end batch and streaming data pipeline on AWS**.
It is designed for **beginners** to understand how data flows through modern cloud systems.

---

## What this project shows

- How batch data is processed using **AWS Glue**
- How streaming data is processed using **Amazon Kinesis + AWS Lambda**
- How data is stored in **Amazon S3** and **Amazon RDS**
- How infrastructure is managed using **Terraform**
- Clear separation of batch and streaming pipelines

---

## Architecture (High Level)

### Batch Pipeline
Local CSV file  
→ Amazon S3 (Landing Zone)  
→ AWS Glue ETL Job  
→ Amazon S3 (Curated Zone) / Amazon RDS
