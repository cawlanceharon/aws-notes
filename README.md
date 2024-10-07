# AWS Notes And Setup Guide

# 1. Amazon EC2 (Elastic Compute Cloud)
Purpose: Provides virtual servers for running applications.
Use case: Hosting your Node.js backend or microservices on EC2 instances with full control over the server environment.

# Guide
```
# Deploying Full Stack Apps to AWS EC2 with SQL Databases
https://www.sammeechward.com/deploying-full-stack-js-to-aws-ec2

For ubuntu
rsync -avz --exclude 'node_modules' --exclude '.git' --exclude '.env' \
-e "ssh -i ~/.ssh/ph-lance-virtual-windows.pem" \
. ubuntu@ec2-13-239-6-152.ap-southeast-2.compute.amazonaws.com:~/app

For Windows
scp -i ~/.ssh/ph-lance-virtual-windows.pem -r . ubuntu@ec2-13-239-6-152.ap-southeast-2.compute.amazonaws.com:~/app

Running the app
ssh -i "~/.ssh/ph-lance-virtual-windows.pem" ubuntu@ec2-13-239-6-152.ap-southeast-2.compute.amazonaws.com
```

# 2. AWS Lambda
Purpose: Serverless compute service that runs code in response to events.
Use case: Running Node.js functions without provisioning servers (great for event-driven architectures like APIs or background tasks).

# 3. Amazon S3 (Simple Storage Service)
Purpose: Scalable object storage.
Use case: Storing and serving static assets (like images, videos), backups, or even application logs for your Node.js application.

# Guide
```
# Simple tutorial
https://www.youtube.com/watch?v=MH01PNZLR98&t=8s

Project
https://github.com/cawlanceharon/event-driven-app
```

# 4. Amazon RDS (Relational Database Service)
Purpose: Managed relational databases like MySQL, PostgreSQL, and others.
Use case: Hosting relational databases for your Node.js application in a scalable and managed environment.

# 5. Amazon DynamoDB
Purpose: Fully managed NoSQL database service.
Use case: Storing non-relational data with low-latency performance (great for highly scalable applications using Node.js).

# 6. Amazon API Gateway
Purpose: API management and routing service.
Use case: Building and managing RESTful or WebSocket APIs that trigger your Node.js functions (especially when used with AWS Lambda).

# 7. Amazon SNS (Simple Notification Service)
Purpose: Pub/Sub messaging service.
Use case: Sending notifications or triggering events in a distributed system from your Node.js backend.

# 8. Amazon SQS (Simple Queue Service)
Purpose: Message queuing service.
Use case: Managing tasks asynchronously in a Node.js application, queuing up tasks like background jobs, and decoupling systems.

# 9. AWS Elastic Beanstalk
Purpose: Managed platform for deploying and scaling web applications and services.
Use case: Simplified deployment of Node.js applications without needing to manage the infrastructure (automatic scaling and monitoring included).

# 10. Amazon CloudWatch
Purpose: Monitoring and observability service.
Use case: Monitoring the performance and logs of your Node.js backend, including setting up alarms for various metrics (e.g., server CPU, memory usage).

# 11. AWS Secrets Manager
Purpose: Manages secrets like API keys, passwords, and database credentials.
Use case: Storing and securely managing sensitive configuration data for your Node.js backend.

# 12. Amazon CloudFront
Purpose: Content delivery network (CDN).
Use case: Distributing static and dynamic content from S3 or your backend services (Node.js APIs) globally with low-latency caching.

# 13. AWS Fargate (ECS or EKS)
Purpose: Serverless container service.
Use case: Running Node.js applications inside Docker containers without managing the underlying infrastructure (great for microservices or distributed systems).

# 14. Amazon ElastiCache
Purpose: Managed Redis and Memcached service.
Use case: Caching frequently used data to reduce latency and increase performance for your Node.js application.

# 15. AWS Step Functions
Purpose: Serverless orchestration of AWS services.
Use case: Managing workflows and automating long-running processes in a Node.js backend.
Using these services in combination can help you scale and manage your backend infrastructure efficiently when building Node.js applications on AWS.


