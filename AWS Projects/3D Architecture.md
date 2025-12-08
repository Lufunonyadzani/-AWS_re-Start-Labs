



# 🛒 AWS 3D E-Commerce Architecture Design  
**Course:** AWS re-Start Cloud Computing Programme  
**Cohort:** 06 October 2025 – 26 December 2025  
**Project:** 2  
**Date Given:** 01 December 2025  
**Date Due:** 05 December 2025  

---

## 📌 Project Introduction
We are a startup team designing a **next-generation 3D e-commerce platform** where customers can **view, rotate, and interact with 3D models** of products such as furniture, gadgets, and clothing before purchasing.

We selected **Amazon Web Services (AWS)** because it allows us to:
- Serve customers worldwide  
- Maintain high security  
- Scale during massive traffic spikes  
- Control infrastructure costs

---

## ✅ Project Requirements
The platform must:
- Be **available 24/7**
- Handle **huge traffic spikes** (e.g. Black Friday)
- Load **3D models extremely fast**
- Be **highly secure**
- Be **cost-optimized**

---

## 🏗️ AWS 3D E-Commerce Architecture Overview

### 🔧 Core AWS Services Used
| AWS Service | Purpose |
|-------------|---------|
| **Amazon S3** | Stores 3D models and product images |
| **Amazon CloudFront** | Delivers files from the nearest edge location |
| **Amazon EC2 (GPU)** | Renders and displays 3D models |
| **AWS Lambda** | Runs backend tasks without servers |
| **Amazon RDS** | Stores product, order, and customer data |
| **Amazon DynamoDB** | Handles shopping carts and fast-changing data |
| **Elastic Load Balancer (ELB)** | Distributes traffic across EC2 servers |
| **AWS Auto Scaling** | Automatically adjusts EC2 capacity |
| **Amazon Route 53** | Domain routing and automatic failover |
| **Amazon CloudWatch** | Monitoring and performance tracking |
| **AWS Trusted Advisor** | Cost, security, and performance recommendations |

---

## 🎯 Why Each Service Was Chosen
- **S3:** Secure, scalable, and low-cost storage for large 3D files  
- **CloudFront:** Global fast delivery of content  
- **EC2 (GPU):** Required for smooth 3D rendering  
- **Lambda:** Pay-per-use backend logic  
- **RDS:** Reliable relational database for transactions  
- **DynamoDB:** Ultra-fast NoSQL for carts and live data  
- **ELB:** Keeps the platform available during server failures  
- **Route 53:** Smart DNS with automatic failover  
- **CloudWatch & Trusted Advisor:** Monitoring and cost control  

---

## 🔍 How the Design Meets System Requirements

| Requirement | Solution |
|------------|----------|
| Always Online | Multi-Availability Zone design + Route 53 failover |
| Traffic Spikes | EC2 Auto Scaling + Serverless Lambda |
| Fast Performance | CloudFront CDN + GPU-Powered EC2 |
| Security | Encryption, IAM, WAF, GuardDuty |
| Cost Optimization | Lambda, Spot Instances, Auto Scaling, Trusted Advisor |

---

## ⚖️ Key Trade-Offs
- GPU EC2 instances offer speed but increase costs  
- Lambda functions may experience cold starts  
- CloudFront adds a monthly cost but ensures global speed  
- Managing both RDS and DynamoDB increases complexity but boosts performance  

---

## 👨‍🏫 What We Learned as a Team
- CDN caching is essential for 3D performance  
- Managed services reduce development workload  
- Auto Scaling prevents system crashes during high demand  
- Security must be built into the design from day one  
- CloudWatch is critical for real-time system health  

---

## 🏛️ AWS Well-Architected Framework Evaluation

| Pillar | Score | Reason |
|--------|--------|--------|
| Operational Excellence | 5/5 | Automated CI/CD pipelines |
| Security | 5/5 | IAM, Encryption, WAF, Cognito |
| Reliability | 5/5 | Multi-AZ deployments & backups |
| Performance Efficiency | 5/5 | CDN, GPU EC2, caching |
| Cost Optimization | 4.5/5 | Auto Scaling, Lambda, Spot Instances |
| Sustainability | 4/5 | Smart scaling and resource efficiency |

---

## ✅ Final Conclusion
Using **Amazon S3, CloudFront, EC2 (GPU), Lambda, RDS, DynamoDB, ELB, Route 53, and CloudWatch**, we designed a **modern 3D e-commerce platform** that is:

✔ Fast  
✔ Always Available  
✔ Secure  
✔ Cost-Effective  
✔ Scalable for global growth  

This architecture is suitable for **real-world enterprise-level 3D shopping platforms**.

---

## 📚 References
- AWS Well-Architected Framework – AWS Official Documentation  
- AWS General Documentation  

---




