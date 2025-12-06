
Perfect — here is your **professional, submission-ready `README.md`** for the **Bash Shell Scripting Challenge Lab**. You can paste this directly into your project or GitHub repository.

---

# 📘 Challenge Lab: Bash Shell Scripting Exercise

## 📌 Lab Overview

This challenge lab focuses on **Bash shell scripting and Linux file automation**. The goal of the lab is to connect to an Amazon Linux EC2 instance using **SSH**, write a **Bash script that automatically generates files**, and ensure that the script dynamically continues numbering without hardcoding values.

This lab builds practical skills in:

* Remote Linux access
* Bash scripting
* File system automation
* Looping and condition handling in shell scripts

---

## ✅ Lab Objectives

By completing this challenge, I was able to:

* Connect to an Amazon Linux EC2 instance using SSH
* Write a Bash script to automatically generate files
* Use automation to determine file numbering
* Validate output using Linux directory listing commands

---

## ⏱ Estimated Duration

**55 minutes**

---

## 🛠 Technologies & Tools Used

* Amazon EC2 (Amazon Linux)
* AWS Management Console
* SSH
* Bash Shell
* Linux File System Commands

---

## 🔐 Task 1: Connect to Amazon Linux EC2 Instance

The EC2 instance was accessed using SSH authentication with a key pair.

### 🔹 For macOS & Linux:

* `.pem` file was downloaded
* Permissions were set using `chmod 400`
* SSH command used:

```bash
ssh -i labsuser.pem ec2-user@<public-ip>
```

### 🔹 For Windows:

* `.ppk` file was downloaded
* PuTTY was used to establish the SSH connection

✅ Successful login confirmed access to the EC2 instance terminal.

---

## 🧠 Challenge Requirements

The Bash script was required to:

* Create **25 empty (0 KB) files**

* File naming format:

  ```
  <yourName><number>
  ```

  Example:

  ```
  lufuno1, lufuno2, lufuno3, ...
  ```

* Each new execution must:

  * Detect the **highest existing file number**
  * Automatically continue with the **next batch of 25 files**

* **No hardcoded numbers** allowed

* Must use **automation and logic**

* Results must be validated using:

  ```bash
  ls -l
  ```

---

## 🧪 Script Testing & Validation

The script was executed multiple times to verify:

* ✅ Files were created correctly
* ✅ Numbers continued automatically
* ✅ No duplicate filenames
* ✅ Each batch added **exactly 25 new files**

Directory contents were displayed using:

```bash
ls -l
```

✅ The output confirmed the correct number of files and proper naming format.

---

## ✅ Final Results

* Fully automated file creation achieved
* Dynamic numbering successfully implemented
* Script passed all validation tests

---

## ✅ Learning Outcomes

Through this lab, I gained practical experience in:

* Writing Bash automation scripts
* Implementing loops and dynamic variables
* Parsing file names and tracking numbering
* Using Linux commands to validate results
* Automating repetitive system tasks

---

## ✅ Lab Status

**✔ Successfully Completed**

---

If you want, I can also:

✅ Add the **exact Bash script** into this README
✅ Convert this into a **PDF or Word document**
✅ Add a **Screenshots & Evidence section**
✅ Create a **GitHub-ready version with markdown badges**

Tell me what you’d like to add next and I’ll format it for you.
