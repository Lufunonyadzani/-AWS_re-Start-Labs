# AWS re/Start Journey
Welcome to my **AWS re/Start Labs Repository**!  I'm Lufuno Nyadzani I’m someone who genuinely enjoys technology, especially anything related to cloud computing. Over time, this interest has grown into a clear career goal: becoming a Senior Solutions Architect. Completing my IT Diploma gave me the foundation to understand how systems work, but exploring cloud platforms is what truly sparked my ambition.

What draws me to the cloud is how it enables businesses to operate smarter and faster. The idea that you can design solutions that scale on demand, stay secure, and reduce complexity motivates me to keep learning. I want to be the kind of architect who creates systems that are not only technically strong but also make a real difference in how companies run.

This collection showcases my hands-on labs, exercises, and projects completed as part of the **AWS re/Start Cloud Practitioner Program**.Each lab demonstrates practical cloud computing, Linux, and networking concepts using **Amazon Web Services (AWS)** and related technologies.

---

## Program Overview

I completed the AWS re/Start program, a full-time, hands-on cloud training journey designed to build technical readiness for cloud-focused roles. Throughout the program, I gained both foundational and advanced skills across core AWS services, Linux systems, networking, security, automation, and modern cloud architectures.

---

## Topics Covered

<div style="display: flex; flex-wrap: wrap; gap: 30px; width: 100%;">

<!-- Linux Fundamentals -->
<div style="flex: 1; min-width: 350px;">
<h3> Linux Fundamentals</h3>
<ul>
<li>Introduction to Linux & CLI</li>
<li>File & Directory Management</li>
<li>Users & Groups</li>
<li>Editing Files & Permissions</li>
<li>Shell Commands & Scripting</li>
</ul>
</div>

<!-- Cloud Foundations -->
<div style="flex: 1; min-width: 350px;">
<h3>Cloud Foundations</h3>
<ul>
<li>Core Cloud Concepts</li>
<li>AWS Global Infrastructure</li>
<li>Shared Responsibility Model</li>
<li>Deployment Models</li>
</ul>
</div>

<!-- AWS Cloud Services -->
<div style="flex: 1; min-width: 350px;">
<h3>AWS Cloud Services</h3>
<ul>
<li>EC2: Virtual Servers</li>
<li>S3: Cloud Storage</li>
<li>IAM: Identity & Policies</li>
<li>CloudWatch: Logs & Metrics</li>
<li>VPC: Networking & Security</li>
</ul>
</div>

<!-- Python Programming -->
<div style="flex: 1; min-width: 350px;">
<h3> Python Programming</h3>
<ul>
<li>Variables & Data Types</li>
<li>Functions & Control Flow</li>
<li>File Handling</li>
<li>Modules & Packages</li>
<li>boto3 Introduction</li>
</ul>
</div>

<!-- Databases -->
<div style="flex: 1; min-width: 350px;">
<h3>Databases</h3>
<ul>
<li>SQL Basics</li>
<li>Relational vs NoSQL</li>
<li>Querying & Joins</li>
<li>Database Design</li>
</ul>
</div>

<!-- AWS Architecture -->
<div style="flex: 1; min-width: 350px;">
<h3>AWS Architecture</h3>
<ul>
<li>High Availability</li>
<li>Fault Tolerance</li>
<li>Scalability Principles</li>
<li>Well-Architected Framework</li>
</ul>
</div>

<!-- Servers -->
<div style="flex: 1; min-width: 350px;">
<h3> Servers</h3>
<ul>
<li>Compute Types</li>
<li>Server Configuration</li>
<li>Volume Management</li>
</ul>
</div>

<!-- Automated Deployments -->
<div style="flex: 1; min-width: 350px;">
<h3>Automated Deployments</h3>
<ul>
<li>Infrastructure as Code</li>
<li>CloudFormation Basics</li>
<li>Automated Pipelines</li>
</ul>
</div>

<!-- Machine Learning & Gen AI -->
<div style="flex: 1; min-width: 350px;">
<h3>Machine Learning & Generative AI</h3>
<ul>
<li>ML Concepts</li>
<li>AI/ML Use Cases</li>
<li>AWS GenAI Services</li>
</ul>
</div>

</div>

---

##  Repository Structure

Each lab or module has its own folder with relevant files, screenshots, and explanations.

[Project 1: EC2](https://github.com/Lufunonyadzani/-AWS_re-Start-Labs/tree/main/Project%201%3A%20EC2%20)
This project focuses on teaching the fundamental skills needed to work with Amazon EC2, guiding you through the full lifecycle of a cloud-based virtual server. You learn how to launch an EC2 instance, configure networking and storage, apply termination protection, and deploy a simple web server using a User Data script. The lab also emphasizes cloud security by showing how to update security groups to allow HTTP traffic, and introduces monitoring tools such as CloudWatch metrics and instance screenshots for troubleshooting. Finally, you practice scaling by resizing both the instance type and EBS volume, and learn how to properly terminate an instance after disabling termination protection.

[Project 2: Lunix](https://github.com/Lufunonyadzani/-AWS_re-Start-Labs/tree/main/Project%202%3A%20Lunix)
This lab focuses on teaching essential Bash shell and Linux command-line skills within an Amazon Linux EC2 environment. You learn how to securely connect to an EC2 instance using SSH, create useful command aliases, and perform a full folder backup using the tar utility. The project also explores how the PATH environment variable works, showing how Linux locates executables and how to add new directories to PATH so scripts can run from anywhere. By completing the tasks, you gain hands-on experience with navigation, permissions, environment variables, and basic automation—core skills needed for managing Linux servers and working effectively in cloud environments.

[Project 3: Database](https://github.com/Lufunonyadzani/-AWS_re-Start-Labs/tree/main/Project%203%3A%20Database)
The lab guides you through creating a new database named world, building a table called country, and examining its structure with queries such as SHOW DATABASES, SHOW TABLES, and SHOW COLUMNS. You also learn how to correct a mistake in the table schema using the ALTER TABLE command. Additional challenges include creating a new table and working with common data types. The final part of the lab teaches how to safely delete tables and databases using the DROP command, reinforcing the importance of understanding destructive operations.


[Project 4: Networking](https://github.com/Lufunonyadzani/-AWS_re-Start-Labs/tree/main/Project%204%3A%20Networking)This lab focuses on understanding public and private IP addressing within an AWS VPC by investigating a customer issue where one EC2 instance can access the internet while another cannot. As a cloud support engineer, I analyze the IP configuration of both instances and discover that instance A cannot reach the internet because it only has a private IP address, while instance B has a public IP that allows external connectivity and successful SSH access.


[Project 5: Python](https://github.com/Lufunonyadzani/-AWS_re-Start-Labs/tree/main/Project%205%3A%20IAM)
This lab introduces you to basic programming through Python and teaches you how to create and run your first Python script using the AWS Cloud9 IDE. After launching the lab environment and opening Cloud9, you create a new Python file, save it with a .py extension, and explore the terminal to verify available Python versions. You then write a simple print("Hello, World") statement to confirm that your Python environment is working correctly.


[Project 6: Security](https://github.com/Lufunonyadzani/-AWS_re-Start-Labs/tree/main/Project%206%3A%20Security)
This lab teaches you how to use Amazon Inspector to automatically scan AWS Lambda functions for vulnerabilities and remediate security findings in a real-world development scenario. Acting as a cloud engineer for AnyCompany, you activate Amazon Inspector, review its dashboard, and observe how it continuously analyzes Lambda functions, EC2 instances, and Amazon ECR images for outdated or vulnerable software. You explore Inspector findings, including severity levels, impacted resources, and CVE details pulled from the National Vulnerability Database.


 
---

## Learning Objectives

By the end of this program, I will be able to:
- Deploy and manage AWS EC2 instances  
- Configure and secure Linux environments  
- Monitor and scale cloud infrastructure  
- Automate tasks using Python  
- Apply best practices in cloud security and architecture  

---


## Connect with Me

- **GitHub:** [Lufunonyadzani](https://github.com/Lufunonyadzani/-AWS_re-Start-Labs/tree/main)  
- **LinkedIn:** *(https://www.linkedin.com/in/lufuno-nyadzani-333ba0316/)*  
- **Email:** *(Nyadzanil20@gmail.com)*  

---



