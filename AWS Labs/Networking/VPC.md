
---

# Created Subnets and Allocate IP Addresses in an Amazon VPC

This repository contains my notes and steps from the **AWS VPC Subnetting Lab**, where I practiced creating a VPC, allocating subnets, and assigning IP addresses in a customer scenario.

---

##  Lab Objectives

In this lab, I learned how to:

* ✔️ Summarize a customer networking scenario
* ✔️ Create an Amazon VPC using the AWS Management Console
* ✔️ Allocate private IP addresses for the VPC (~15,000 IPs)
* ✔️ Create a public subnet with at least 50 IP addresses
* ✔️ Verify and document the VPC and subnet configuration

---

##  **Task 1: Investigate Customer Needs**

Customer request:

* Needs a VPC in the **192.x.x.x private range**
* Requires **~15,000 private IP addresses**
* Requires a **public subnet** with ≥ 50 IP addresses
* Needs basic connectivity (Internet Gateway, Public Route Table)

---

##  **Task 2: Plan CIDR Blocks**


###  VPC CIDR Block

* Requirement: ~15,000 IPs
* /18 provides 16,384 IPs → fits requirement

```
192.168.0.0/18
```

###  Public Subnet CIDR Block

* Requirement: ≥ 50 IPs
* /26 provides 64 IPs → fits requirement

```
192.168.1.0/26
```

---

##  **Task 3: Create the VPC**

### Step 1: Opened VPC on AWS Console 
<img width="1366" height="768" alt="image 1" src="https://github.com/user-attachments/assets/883ce441-39c2-4921-8cd3-935a8e924734" />


### Step 2: Setting name and CIDR Block**
he AWS VPC creation screen displays a configuration where the VPC is set to auto‑generate a name tag called “First VPC” with an IPv4 CIDR block of 192.168.0.0/16 and no IPv6 CIDR block selected.

<img width="1366" height="768" alt="image 2" src="https://github.com/user-attachments/assets/00f020bc-d09c-465a-9a7a-34fbf65ec105" />



### Step 3: Configure Settings
<img width="1366" height="768" alt="image 3" src="https://github.com/user-attachments/assets/277cc03b-3f7c-4539-8c8d-53ff95e91a56" />

### Step 4: Created VPC

<img width="1366" height="768" alt="image 4" src="https://github.com/user-attachments/assets/e80cfaea-8677-4477-9e72-b8fd13cd196f" />



##  Conclusion

I have now successfully:

* ✔️ Designed a VPC with private and public subnets
* ✔️ Allocated IP addresses based on customer requirements
* ✔️ Used AWS Management Console to create and verify VPC resources
* ✔️ Prepared a customer-friendly summary of your findings

---



