
# AWS re/Start – Project 1: EC2 Web Server

This project demonstrates how to launch, configure, monitor, resize, and terminate an Amazon EC2 instance.  
A User Data script deploys a simple Apache web server that displays **"Hello From Your Web Server!"**

---

## 📌 Task 1: Launching the EC2 Instance

Steps performed:

1. Launched an **Amazon Linux 2023** EC2 instance
2.   <img width="1366" height="768" alt="Screenshot_2025-11-24_15_37_00" src="https://github.com/user-attachments/assets/bcfd7624-69b3-444a-8e40-123184933289" />

3. Instance type: **t3.micro**  
4. Configured **termination protection**  
5. Did **not** use a key pair  
6. Used **Lab VPC**  
7. Created a **Web Server security group**  
8. Added User Data script:

```bash
#!/bin/bash
yum -y install httpd
systemctl enable httpd
systemctl start httpd
echo '<html><h1>Hello From Your Web Server!</h1></html>' > /var/www/html/index.html
