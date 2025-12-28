# Batch & Streaming Data Pipeline

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
**Batch Flow (Simple Explanation)**

1. A sample CSV file (`scripts/sample_data.csv`) is uploaded to Amazon S3 (Landing Zone).
2. An AWS Glue ETL job reads the CSV from S3.
3. Glue cleans and transforms the data.
4. The transformed data is written to:
   - Amazon S3 (Curated Zone) OR
   - Amazon RDS for analytics and reporting.

### Streaming Pipeline

In the streaming pipeline, data is processed in real time.

Events are sent to an Amazon Kinesis stream.
AWS Lambda consumes the stream and processes each event.
The processed data is stored in Amazon S3 or Amazon RDS.
