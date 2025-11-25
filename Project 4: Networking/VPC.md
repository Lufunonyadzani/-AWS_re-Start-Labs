
🌐 Create Subnets and Allocate IP Addresses in an Amazon VPC

This repository documents the steps, notes, and explanations from the AWS VPC Subnetting Lab, where a customer required assistance designing a VPC with specific IP requirements.

📌 Objectives

In this lab, I learned how to:

Understand customer networking requirements

Create an Amazon VPC

Allocate a correct CIDR block for ~15,000 private IP addresses

Create a public subnet with at least 50 IP addresses

Use the AWS Management Console to configure networking resources

Summarize findings and explain the solution like a cloud support engineer

🧑‍💼 Customer Scenario

A startup owner, Paulo Santos, opened a support ticket requesting help creating a VPC. Their requirements:

The VPC must use a 192.x.x.x private IPv4 range

Must support around 15,000 private IP addresses

Must include a public subnet with at least 50 IP addresses

Include basic components: VPC, Internet Gateway, Route Table, Public Subnet

🧠 CIDR Planning
✔ Private IP ranges (RFC 1918)

10.0.0.0 – 10.255.255.255 (10/8)

172.16.0.0 – 172.31.255.255 (172.16/12)

192.168.0.0 – 192.168.255.255 (192.168/16) ← customer wants this range

✔ VPC Requirement: ~15,000 IPs

A subnet calculator shows:

/18 = 16,384 IP addresses
Perfect for 15,000 usable IPs.

👉 Selected VPC CIDR:

192.168.0.0/18

✔ Public Subnet Requirement: ≥ 50 IPs

/26 = 64 IP addresses (62 usable)

👉 Selected Public Subnet:

192.168.1.0/26

🛠️ Task 1: Build the VPC
1. Open AWS Console → search VPC
2. Choose Launch VPC Wizard
3. Select VPC with a Single Public Subnet
4. Configure:
Setting	Value
VPC Name	First VPC
IPv4 CIDR	192.168.0.0/18
IPv6	No IPv6
Public Subnet CIDR	192.168.1.0/26
AZ	No Preference
Subnet Name	Public subnet
Internet Gateway	Enabled (default)
Route Table	Auto-created
5. Create VPC
