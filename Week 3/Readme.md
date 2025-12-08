# Week 3: Getting Started with AWS

## 📘 Introduction
This repository contains materials and code for **Project 2: Provisioning EC2, S3, RDS, and VPC**.  
The goal is to learn how to provision AWS resources using Infrastructure-as-Code (IaC) tools such as **Terraform** or **AWS CloudFormation**.  

By the end of this project, you will have hands-on experience deploying compute, storage, database, and networking resources in AWS to support an internal development tool.

---

## 🛠 Prerequisites
Before starting, ensure you have:
- An **AWS account** with appropriate permissions (IAM user/role with admin or infra privileges).
- Installed and configured **AWS CLI** (`aws configure`).
- Installed **Terraform** or **AWS CloudFormation**.
- Basic knowledge of networking concepts (subnets, route tables, security groups).
- Git installed for version control.

---

## 🎯 Project 2: Provisioning EC2, S3, RDS, VPC

### Objective
Provision AWS resources with code to support infrastructure needs.

### Learning Outcomes
- Deploy **EC2** instances for compute
- Configure **S3** buckets for storage
- Set up **RDS** for relational database services
- Design and manage **VPC** for networking

---

## 📂 Scenario
As an infrastructure engineer, you are tasked with provisioning compute and storage resources for an internal development tool.  
This involves:
- Automating the deployment of EC2 instances
- Creating secure and scalable S3 buckets
- Setting up RDS for persistent data storage
- Designing a VPC to ensure proper network segmentation and security

---

## 📑 Expected Deliverables
- Infrastructure-as-Code (IaC) scripts (Terraform or CloudFormation)
- Documentation of resource configurations
- Verification of deployed resources in AWS console

---

## 🚀 Steps to follow
1. **Set up IAM roles and permissions** for secure access.  
2. **Provision EC2 instances** with appropriate AMIs and instance types.  
3. **Create S3 buckets** with versioning and encryption enabled.  
4. **Deploy RDS** with proper backup and multi-AZ configuration.  
5. **Design VPC** with subnets, route tables, and security groups.  
6. **Test connectivity** between resources to validate the setup.  

---

## 📝 Points to Note
- Ensure all resources are tagged for easy identification.  
- Follow AWS best practices for security and cost optimization.  
- Document any issues or troubleshooting steps during provisioning.  
```
