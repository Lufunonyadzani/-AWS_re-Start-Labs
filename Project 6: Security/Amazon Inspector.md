
---

# Using Amazon Inspector for Vulnerability Assessment and Remediation

##  Lab Overview

In this lab, I use **Amazon Inspector** to scan AWS resources—specifically **AWS Lambda functions**—for security vulnerabilities. I activated the service, review findings, and remediate detected issues.

The development team at **AnyCompany** is building an application using AWS Lambda and needs an automated tool that scans for vulnerable software packages and insecure code. Amazon Inspector fits this requirement by:

* Continuously scanning Lambda functions after each deployment
* Automatically scanning EC2 instances and Amazon ECR images
* Providing detailed vulnerability insights and remediation steps

---

##  Objectives

After completing this lab, you will be able to:

* ✔️ Activate **Amazon Inspector**
* ✔️ Analyze and interpret vulnerability findings
* ✔️ Remediate vulnerabilities in AWS Lambda functions

---



---

---

#  Task 1: Activate Amazon Inspector




---

#  Task 2: Reviewing Inspected Resources



---

#  Task 3: Remediating Vulnerability Findings


1. In the AWS Console, search for **Lambda** and open it.
2. Select the **get-request** Lambda function.
3. Open the **requirements.txt** file.
4. Change this line:

   ```
   requests==2.20.0
   ```

   to:

   ```
   requests
   ```

   This installs the **latest version** of the package automatically.
5. Click **Deploy**.
6. After deployment, Amazon Inspector triggers a new scan.

---

##  Confirming the Remediation


---

## ✅ Lab Complete

You have successfully:

* Activated Amazon Inspector
* Reviewed Lambda vulnerabilities
* Remediated package vulnerabilities
* Verified the updated scan results

---

