


---

# Monitor an EC2 Instance Using Amazon CloudWatch & SNS

## Lab Overview

This lab demonstrates how **logging and monitoring** work together to maintain system performance and security in AWS. Using **Amazon CloudWatch** and **Amazon SNS**, an alarm is created to monitor CPU usage on an EC2 instance. When the CPU utilization exceeds a defined threshold, an email notification is automatically sent.


---

## Objectives

By the end of this lab, I successfully:

* Created an Amazon SNS notification topic
* Configured a CloudWatch alarm
* Stress tested an EC2 instance
* Confirmed SNS email notification delivery
* Created a CloudWatch dashboard

---

##  AWS Services Used

* **Amazon EC2** – Virtual server used for stress testing
* **Amazon CloudWatch** – Monitoring and metrics
* **Amazon SNS (Simple Notification Service)** – Email alert notifications
* **AWS IAM** – Role for EC2 access via Session Manager

---

## Task 1: Configure Amazon SNS
The image shows the AWS Management Console with an Amazon SNS named MyCwAlarm that has been created successfully.

<img width="1366" height="768" alt="image 2" src="https://github.com/user-attachments/assets/21fdb75f-562f-40be-a774-7afaec4124d4" />


---

## Task 2: Create a  subscription
The screenshot shows the AWS console page for creating an SNS subscription where the Topic ARN is arn:aws:sns:us-west-2:351005276791:MyCWAlarm, the Protocol is set to Email, and the Endpoint is the email address nyadzran12@gmail.com; 

<img width="1366" height="768" alt="image 3" src="https://github.com/user-attachments/assets/c969f51c-7027-4fe9-84b3-a3582d98e3c5" />

---

## Task 3: Stress Test the EC2 Instance

<img width="1366" height="768" alt="image 4" src="https://github.com/user-attachments/assets/a16d5bca-d231-4597-aefa-e408468c375a" />

---

## Task 4: Create a CloudWatch Dashboard
<img width="1366" height="768" alt="image 5" src="https://github.com/user-attachments/assets/7702b59f-3faf-44ea-a11f-b7e5b19aa87a" />

---


---

## Conclusion

 This lab successfully demonstrated real-world cloud monitoring by:

* Automating CPU usage detection
* Triggering real-time email alerts
* Visualizing performance metrics
* Simulating a security incident


