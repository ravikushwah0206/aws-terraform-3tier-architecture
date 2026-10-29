# aws-terraform-3tier-architecture


# AWS Multi-Tier Infrastructure Automation using Terraform

# 🚀 Project Overview
This project provisions a production-ready, highly available 3-tier web application architecture on AWS using **Terraform (Infrastructure as Code)**. It automates the deployment of secure networking components, compute layers, and database backends following AWS best practices.

---

# 🏗️ Architecture & Components
* Networking (VPC): Custom VPC with Public and Private Subnets across multiple Availability Zones for high availability.
* Security Groups: Strict ingress/egress firewall rules isolating the Web tier, Application tier, and Database tier.
* Compute Layer: Amazon EC2 instances launched via Auto Scaling Groups behind an Application Load Balancer (ALB).
* State Management: Terraform remote state backend configuration using Amazon S3 and DynamoDB for state locking.

---

## 🛠️ Tech Stack Used
* Cloud Provider: Amazon Web Services (AWS)
* Infrastructure as Code: Terraform (HCL, Modules, State Management)
* Version Control: Git & GitHub

---

## 📂 Project Structure
```text
├── main.tf          # Main resource configurations (VPC, EC2, ALB)
├── variables.tf     # Input variables for environment flexibility
├── outputs.tf       # Output values (Load Balancer DNS, Instance IPs)
├── provider.tf      # AWS provider and backend configurations
└── terraform.tfvars # Sensitive/Environment-specific variable values