🌐 Create Subnets and Allocate IP Addresses in an Amazon VPC

This repository contains notes and steps used during the AWS VPC Subnetting Lab, where I created a VPC, calculated CIDR ranges, and configured subnets based on a customer request.

✅ Objectives

Summarize the customer scenario

Create a VPC with the correct IPv4 CIDR block

Allocate private and public IP address ranges

Create a public subnet with at least 50 IPs

Use the AWS Management Console to configure VPC resources

Provide a walkthrough guide for the customer

🧑‍💼 Customer Scenario

A startup owner needs:

A VPC using the 192.x.x.x private range

At least 15,000 private IP addresses

A public subnet with ≥ 50 IP addresses

A simple VPC architecture with an Internet Gateway and one public subnet

📘 Private IP Ranges (RFC 1918)
10.0.0.0 – 10.255.255.255
172.16.0.0 – 172.31.255.255
192.168.0.0 – 192.168.255.255   ← customer wants this range

🧠 CIDR Planning
VPC needs around 15,000 IP addresses

Using the subnet calculator:

/18 = 16,384 total IPs → ✔ meets requirement

Chosen VPC CIDR Block

192.168.0.0/18

Public subnet needs at least 50 IPs

/26 = 64 total IPs (62 usable)

Chosen Public Subnet CIDR

192.168.1.0/26

🛠️ VPC Creation Steps
1. Open AWS Console → Search for VPC
2. Select Launch VPC Wizard
3. Choose:
VPC with a Single Public Subnet

4. Configure:
Setting	Value
VPC Name	First VPC
IPv4 CIDR	192.168.0.0/18
IPv6	No IPv6
Public Subnet CIDR	192.168.1.0/26
Availability Zone	No Preference
Subnet Name	Public subnet
Internet Gateway	Enabled
Route Table	Automatic
5. Click Create VPC
