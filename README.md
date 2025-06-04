# AWS-Global-Accelerator-with-VPC-Networking-project
This project demonstrates the use of **AWS Global Accelerator** to route traffic between multiple EC2 instances in different regions (Mumbai &amp; Frankfurt) through **VPCs, Route Tables, Subnets**, and **Internet Gateways**.

## 📌 Project Goal

To provide **low-latency access** to a web application hosted across AWS regions using Global Accelerator, ensuring:
- High availability
- Geo redundancy
- Fast failover

---

## 🏗️ Architecture Overview

### ✅ Key Components:
- **AWS Global Accelerator**
- **2 VPCs**: `ap-south-1 (Mumbai)` and `eu-central-1 (Frankfurt)`
- **EC2 Instances** in each region
- **Internet Gateway**
- **Elastic Load Balancer (ELB)**
- **Subnets & Route Tables**
- **Public IP Mapping**

---

## 🌐 How It Works

1. Global Accelerator maps a **static IP** to nearest healthy region.
2. ELB in each region forwards request to local EC2.
3. VPCs are isolated with proper CIDR ranges (`21.0.0.0/16` and `31.0.0.0/16`).
4. Route Tables manage traffic flow to/from EC2 and Internet Gateway.

---

## 🚀 Why This Matters

- Ensures **global availability** of apps with minimal latency.
- Demonstrates mastery of AWS core networking.
- Relevant for **DevOps / Cloud Engineer roles**.

---

## ⚙️ Tech Stack

- AWS EC2
- VPC / Subnetting
- Internet Gateway
- AWS Global Accelerator
- Load Balancer (ELB)
