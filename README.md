# 🚀 AWS Three-Tier Architecture using CloudFormation

## 📌 Project Overview

This project demonstrates the design and deployment of a production-style Three-Tier Architecture on AWS using Infrastructure as Code (IaC) with AWS CloudFormation.

The solution provisions a complete cloud environment consisting of networking, compute, load balancing, database, monitoring, and security components. The entire infrastructure is deployed through a single CloudFormation template, enabling automated, repeatable, and scalable deployments.

---

## 🏗️ Architecture Components

### Networking Layer

* Custom VPC (10.0.0.0/16)
* Internet Gateway
* NAT Gateway
* Public Route Tables
* Private Route Tables
* Public Subnet 1 (10.0.1.0/24)
* Public Subnet 2 (10.0.2.0/24)
* Private Subnet 1 (10.0.11.0/24)
* Private Subnet 2 (10.0.12.0/24)

### Application Layer

* Application Load Balancer (ALB)
* Target Group
* HTTP Listener
* Auto Scaling Group
* Launch Template
* Amazon EC2 (t3.micro)

### Database Layer

* Amazon RDS MySQL 8.0
* DB Subnet Group
* Private Database Deployment
* Automated Backups

### Monitoring & Alerting

* Amazon CloudWatch
* CPU Utilization Monitoring
* SNS Alert Notifications

### Security Layer

* ALB Security Group
* EC2 Security Group
* RDS Security Group
* IAM Role
* IAM Instance Profile

---

## ⚙️ Technologies Used

* AWS CloudFormation
* Amazon VPC
* Amazon EC2
* Amazon RDS MySQL
* Elastic Load Balancer (ALB)
* Auto Scaling
* Amazon CloudWatch
* Amazon SNS
* IAM
* Amazon Linux 2023

---

## 🔄 Request Flow

User Request
↓
Application Load Balancer
↓
Auto Scaling EC2 Instances
↓
Private RDS MySQL Database
↓
CloudWatch Monitoring
↓
SNS Notifications

---

## 🎯 Key Features

✔ Infrastructure as Code (IaC)

✔ Automated Provisioning

✔ High Availability Architecture

✔ Auto Scaling Capability

✔ Load Balancing

✔ Secure Private Database

✔ Monitoring & Alerting

✔ Scalable Design

✔ Production-Oriented Deployment

✔ CloudFormation Automation

---

## 🔐 Security Implementation

* Public access restricted through ALB
* EC2 instances accessed only through security groups
* Database deployed in private subnets
* IAM roles used instead of hardcoded credentials
* Security group-based traffic control
* Network isolation through VPC design

---

## 📊 Monitoring Strategy

The environment includes CloudWatch alarms to monitor:

* CPU Utilization
* Resource Health
* Application Availability
* Infrastructure Performance

SNS notifications can be integrated with email alerts for operational visibility.

---

## 🚀 Deployment Steps

1. Login to AWS Console
2. Navigate to CloudFormation
3. Create Stack
4. Upload CloudFormation Template
5. Enter Stack Name
6. Review Configuration
7. Create Stack
8. Wait for CREATE_COMPLETE
9. Access Application using ALB DNS Name

---

## 📈 Project Outcomes

* Automated AWS infrastructure deployment
* Reduced manual configuration effort
* Improved scalability and availability
* Enhanced operational monitoring
* Demonstrated Infrastructure as Code best practices
* Production-ready cloud architecture implementation

---

## 💼 Skills Demonstrated

* AWS Cloud Architecture
* Infrastructure as Code (IaC)
* CloudFormation Template Development
* Network Design
* Load Balancing
* Auto Scaling
* Database Administration
* Monitoring & Alerting
* Cloud Security
* DevOps Practices

---

## 🎓 Learning Outcomes

Through this project, the following cloud engineering concepts were implemented and validated:

* VPC Design and Routing
* Multi-Tier Architecture
* High Availability Principles
* AWS Security Best Practices
* Infrastructure Automation
* Cloud Monitoring
* Auto Scaling Strategies
* Database Deployment
* Production Workload Design

---

## 👨‍💻 Author

Nitesh Vishwakarma

AWS Cloud | DevOps | Infrastructure as Code | CloudFormation | Automation | Monitoring | Security

---

⭐ If you found this project useful, consider starring the repository and sharing it with the cloud community.
