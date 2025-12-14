
# AWS re/Start – Project 1: EC2 Web Server

This project demonstrates how to launch, configure, monitor, resize, and terminate an Amazon EC2 instance.  
A User Data script deploys a simple Apache web server that displays **"Hello From Your Web Server!"**

---

## Task 1: Launching the EC2 Instance

Steps performed:

1. Launching an **Amazon Linux 2023** EC2 instance
The setup involves creating one instance using the Amazon Linux 2023 AMI 2023.9.2, with a t2.micro instance type, a new     security group for firewall settings, and an 8 GB storage volume. 
4.   <img width="1366" height="768" alt="image 1" src="https://github.com/user-attachments/assets/5ea4724a-7184-4c5a-b60e-b9a1cc06c209" />


5. Changing Instance type: **t3.micro**
6. <img width="1366" height="768" alt="Image 2" src="https://github.com/user-attachments/assets/ed8c41d4-d499-4139-b878-880787881889" />

7. Configured **Networking**
 The instance is being configured to use a specific VPC identified as vpc-04586a50d92607c0f, with the subnet set to “No preference,” meaning AWS will automatically select a default subnet in any availability zone. 
9. <img width="1366" height="768" alt="image 3" src="https://github.com/user-attachments/assets/ec672d3f-500a-4997-b1c5-f096f0386bd7" />

7.Configuring storage
8. <img width="1366" height="768" alt="image 4" src="https://github.com/user-attachments/assets/4b0b6350-49e2-4f8b-8d9d-7ee8e4020026" />

9. Adding User Data script:
10. <img width="1366" height="768" alt="image 5" src="https://github.com/user-attachments/assets/d1073605-9d8a-4227-a014-62347ad74c6a" />

