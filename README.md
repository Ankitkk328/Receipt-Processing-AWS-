Overview of Project ☁️

This project focuses on automating receipt processing using AWS services. Instead of manually handling receipts which can be time-consuming, error-prone, and difficult to scale—this system extracts structured data from receipts and stores it efficiently for record-keeping and auditing.

The architecture consists of:

1- Amazon S3: Stores uploaded receipt images and PDFs. [Storage]

2- Amazon Textract: Extracts text and structured data from scanned receipts. [AI/ML]

3- Amazon DynamoDB: Stores extracted receipt data in a structured format. [Database]

4- Amazon SES: Sends email notifications with extracted receipt details. [Messaging]

5- AWS Lambda: Automates the processing workflow for real-time execution. [Compute]

6- IAM Roles & Policies: Ensures secure access between services. [Security]


CLEAN UP 🗑️ (to avoid billing)

1. Delete S3 Bucket:

Remove all uploaded receipt files and then delete the bucket.

2. Stop Textract Processing: 

Ensure no further API calls are made to prevent extra costs.

3. Delete DynamoDB Table: 

Remove stored receipt data and then delete the table.

4. Disable SES Notifications: 

If SES was configured, remove verified email addresses.

5. Remove IAM Roles and Policies: 

Delete the IAM role created for the Lambda function.

NOTE: "Demo deployed on AWS (now offline to avoid charges)"

