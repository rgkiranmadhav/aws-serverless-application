aws-serverless-application
Serverless AWS registration system using S3, API Gateway, Lambda, and RDS MySQL.

# AWS Serverless Registration System

## Project Overview

This project demonstrates the implementation of a **serverless user registration system on AWS**, using Amazon S3, Amazon API Gateway, AWS Lambda, and Amazon RDS (MySQL).

The application provides a static registration website hosted on Amazon S3, where users can submit their registration details. The submitted data is transferred through API Gateway to an AWS Lambda function, which processes the request, validates the input, and stores the registration details in an RDS MySQL database.

The architecture follows a serverless approach by using managed AWS services, reducing the need for traditional server management and supporting a scalable application design.

## Architecture Flow

User → Amazon S3 → API Gateway → AWS Lambda → Amazon RDS (MySQL)

## Application Workflow

1. The user accesses the registration website hosted on Amazon S3.
2. The user enters registration details through the frontend form.
3. The frontend sends an HTTPS request containing JSON data to Amazon API Gateway.
4. API Gateway triggers the AWS Lambda function.
5. Lambda validates the input and processes the registration request.
6. Lambda establishes a database connection and stores the data in Amazon RDS MySQL.
7. The registration information is stored in the database for future access.

## AWS Services Used

* **Amazon S3:** Hosts the static registration website.
* **Amazon API Gateway:** Receives and manages HTTP API requests.
* **AWS Lambda:** Processes registration requests and executes backend logic.
* **Amazon RDS (MySQL):** Stores user registration data.
* **AWS IAM:** Manages access permissions for AWS resources.
* **AWS Certificate Manager (ACM):** Supports certificate management where configured.

## Key Features

* Serverless backend architecture
* Static website hosting
* API-based communication
* Lambda-based request processing
* MySQL database integration
* Separation of frontend and backend components

## Key Learnings

* Understanding serverless architecture on AWS
* Integrating S3 with API Gateway and Lambda
* Connecting AWS Lambda with RDS MySQL
* Working with HTTP requests and JSON data
* Managing AWS services and IAM permissions

## 🖼️ Architecture Diagram

![AWS Serverless Registration System](architecture.png)

