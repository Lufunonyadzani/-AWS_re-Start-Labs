
# AWS re/Start – Project 1: EC2 Web Server

This project demonstrates how to launch, configure, monitor, resize, and terminate an Amazon EC2 instance.  
A User Data script deploys a simple Apache web server that displays **"Hello From Your Web Server!"**

---

## 📌 Task 1: Launching the EC2 Instance

Steps performed:

1. Launched an **Amazon Linux 2023** EC2 instance  
2. Instance type: **t3.micro**  
3. Configured **termination protection**  
4. Did **not** use a key pair  
5. Used **Lab VPC**  
6. Created a **Web Server security group**  
7. Added User Data script:

```bash
#!/bin/bash
yum -y install httpd
systemctl enable httpd
systemctl start httpd
echo '<html><h1>Hello From Your Web Server!</h1></html>' > /var/www/html/index.html
