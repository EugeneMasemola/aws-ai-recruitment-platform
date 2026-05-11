# Architecture Overview

This project uses a cloud-native AWS architecture designed for availability, scalability, and security.

## Main Components

- Public subnets for internet-facing services
- Private subnets for application and database layers
- Application Load Balancer for traffic distribution
- EC2 or ECS Fargate for application hosting
- Amazon RDS MySQL for managed database storage
- CloudWatch for monitoring and alerts
- IAM roles and Security Groups for access control

## Security Design

The database is placed in private subnets and is not directly accessible from the internet. Access is controlled using Security Groups and IAM permissions.
