
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

## 📍 Task 2: Create Additional Subnets

Two more subnets were created in a second Availability Zone:


## 📍 Task 3: Associate Route Tables

Subnet-to-route-table associations:


---

## 🔐 Task 4: Create Security Group

A security group was created to allow **web traffic**:

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

