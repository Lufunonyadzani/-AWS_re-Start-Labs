
---

# 🌐 Create Subnets and Allocate IP Addresses in an Amazon VPC

This repository contains my notes and steps from the **AWS VPC Subnetting Lab**, where I practiced creating a VPC, allocating subnets, and assigning IP addresses in a customer scenario.

---

## ✅ Lab Objectives

In this lab, I learned how to:

* ✔️ Summarize a customer networking scenario
* ✔️ Create an Amazon VPC using the AWS Management Console
* ✔️ Allocate private IP addresses for the VPC (~15,000 IPs)
* ✔️ Create a public subnet with at least 50 IP addresses
* ✔️ Verify and document the VPC and subnet configuration

---

## 🖥️ **Task 1: Investigate Customer Needs**

Customer request:

* Needs a VPC in the **192.x.x.x private range**
* Requires **~15,000 private IP addresses**
* Requires a **public subnet** with ≥ 50 IP addresses
* Needs basic connectivity (Internet Gateway, Public Route Table)

---

## 🗄️ **Task 2: Plan CIDR Blocks**

### 📌 Private IP Ranges (RFC 1918)

```
10.0.0.0 – 10.255.255.255
172.16.0.0 – 172.31.255.255
192.168.0.0 – 192.168.255.255 ← customer request
```

### 📌 VPC CIDR Block

* Requirement: ~15,000 IPs
* /18 provides 16,384 IPs → fits requirement

```
192.168.0.0/18
```

### 📌 Public Subnet CIDR Block

* Requirement: ≥ 50 IPs
* /26 provides 64 IPs → fits requirement

```
192.168.1.0/26
```

---

## 🛠️ **Task 3: Create the VPC**

### Step 1: Open AWS Console → Search for **VPC**

### Step 2: Launch VPC Wizard

Select: **VPC with a Single Public Subnet**

### Step 3: Configure Settings

| Setting            | Value             |
| ------------------ | ----------------- |
| VPC Name           | First VPC         |
| IPv4 CIDR          | 192.168.0.0/18    |
| IPv6 CIDR          | No IPv6           |
| Public Subnet CIDR | 192.168.1.0/26    |
| Availability Zone  | No Preference     |
| Subnet Name        | Public subnet     |
| Internet Gateway   | Enabled (default) |
| Route Table        | Auto-created      |

### Step 4: Create VPC


## ✅ Conclusion

You have now successfully:

* ✔️ Designed a VPC with private and public subnets
* ✔️ Allocated IP addresses based on customer requirements
* ✔️ Used AWS Management Console to create and verify VPC resources
* ✔️ Prepared a customer-friendly summary of your findings

---


Do you want me to do that next?
