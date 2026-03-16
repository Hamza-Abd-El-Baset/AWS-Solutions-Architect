# Scalable & Highly Available Web Infrastructure on AWS

## 📌 Project Overview
The primary objective of this project was to design and implement a scalable, highly available web application infrastructure on AWS. Following the **AWS Well-Architected Framework**, the goal was to create a fault-tolerant and secure environment capable of sustaining peak traffic periods while optimizing operational costs.

## 🏗️ Architecture Design
The infrastructure utilizes a multi-tier VPC design across multiple **Availability Zones (AZs)** to ensure high availability and eliminate single points of failure.

### Key Components:
* **Networking (VPC):** A custom VPC (10.0.0.0/16) featuring both **Public and Private subnets** to ensure proper network segmentation.
* **Compute:** **EC2 instances** managed by an **Auto Scaling Group** that adjusts capacity dynamically based on demand.
* **Traffic Management:** An **Application Load Balancer (ALB)** serves as the single point of entry, distributing traffic efficiently across healthy instances.
* **Security & Connectivity:** * **NAT Gateway:** Deployed in a public subnet to allow instances in private subnets to securely access the internet for updates.
    * **IAM Roles:** Granular permissions using IAM roles and policies to enforce the principle of least privilege.
* **Data Tier:** Highly available database configuration with **Primary and Standby** instances for synchronous replication.

## 📊 Cost Estimation & Planning
A critical phase of the project involved financial planning using the **AWS Pricing Calculator**.
* **Total Monthly Cost:** Estimated at **$127.16 USD**.
* **Total 12-Month Cost:** Estimated at **$1,525.92 USD**.
* Detailed planning ensured that resource selection aligned with both performance requirements and budget constraints.

## 🛠️ Implementation Phases
1. **Phase 1: Planning & Cost Estimation:** Defining objectives and resource budgeting.
2. **Phase 2: Functional Environment:** Setting up the core VPC networking and compute nodes.
3. **Phase 3: Decoupling:** Implementing architectural best practices to separate application components.
4. **Phase 4: High Availability:** Finalizing the Auto Scaling and Load Balancing configurations for maximum uptime.

## 📂 Project Assets
* **Cost Estimate URL:** [AWS Pricing Calculator Link](https://calculator.aws/#/estimate?id=f5d8666c1dcba245ec7d2c9ed917d1d2baf7d795).
