
# Build Your VPC and Launch a Web Server – Lab README

## Lab Overview

This lab demonstrates how to design and deploy a **custom Virtual Private Cloud (VPC)** in AWS, configure **public and private subnets**, implement **routing and security**, and launch an **Amazon EC2 web server** inside the VPC. The goal is to create a secure, scalable network architecture that meets a **Fortune 100 customer’s requirements**.


---

##Lab Objectives

By completing this lab, I was able to:

* Create a custom Amazon VPC
* Create public and private subnets
* Configure route tables and subnet associations
* Create and configure a VPC security group
* Launch an EC2 instance inside a VPC
* Install and run a web server using user data

---


## Task 1: Create the VPC

The VPC was created using the **VPC Wizard** with the following configuration:
<img width="1366" height="768" alt="image 1" src="https://github.com/user-attachments/assets/ade46069-935d-4c07-af3b-2f8dfbfd28e5" />


---

##  Task 2: Create Additional Subnets

Two more subnets were created in a second Availability Zone:
<img width="1366" height="768" alt="image 2" src="https://github.com/user-attachments/assets/4c6c76ee-43f9-453a-8a45-6141f0c53eb7" />



## Task 3: Associate Route Tables

Subnet-to-route-table associations:
<img width="1366" height="768" alt="image 3" src="https://github.com/user-attachments/assets/21d45898-8343-43c8-be60-3808e651a29a" />



---

## Task 4: Create Security Group

A security group was created to allow **web traffic**:
<img width="1366" height="768" alt="image 4" src="https://github.com/user-attachments/assets/6207368e-143b-46a1-9037-5abfbe7a4590" />


---

## 🖥 Task 5: Launch the Web Server (EC2)

---

## ✅ Learning Outcomes

This lab strengthened my understanding of:

* VPC architecture design
* Public vs Private subnet usage
* Route table associations
* Internet Gateway vs NAT Gateway
* Security group configuration
* EC2 deployment inside a custom network
* Automated web server installation using User Data

---

