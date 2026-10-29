AWS S3 Event-Driven Automation Using Lambda

Project Overview

This project demonstrates event-driven automation using Amazon S3 and AWS Lambda.

Whenever a new file is uploaded to the configured S3 bucket, an S3 event notification automatically triggers a Lambda function. The function extracts the bucket name, uploaded file name, and event type, then records these details in Amazon CloudWatch Logs.

Technologies Used

* Amazon S3
* AWS Lambda
* Python
* AWS IAM
* Amazon CloudWatch
* GitHub

Architecture

File Upload
    |
    v
Amazon S3 Bucket
    |
    v
S3 Object-Created Event
    |
    v
AWS Lambda Function
    |
    v
Amazon CloudWatch Logs

Project Structure

AWS-S3-Event-Driven-Automation-Using-Lambda/
├── lambda_function.py
├── README.md
└── screenshots/

Implementation Steps

1. Created an Amazon S3 bucket with public access blocked.
2. Created an AWS Lambda function using Python.
3. Configured the Lambda execution role with basic CloudWatch logging permissions.
4. Created an S3 event notification for object-creation events.
5. Connected the event notification to the Lambda function.
6. Uploaded a test file to the S3 bucket.
7. Verified the event details in CloudWatch Logs.

Expected Result

When a new file is uploaded to the configured S3 bucket, the Lambda function logs the bucket name, uploaded file name, and event type.

Testing

Upload a new file to the configured S3 bucket after enabling the event notification.

Open the Lambda function’s CloudWatch logs to verify that the event was processed.

Screenshots

Screenshots demonstrating the S3 configuration, Lambda function, and CloudWatch logs are included in the screenshots folder.

Author

Pavan Yadav C