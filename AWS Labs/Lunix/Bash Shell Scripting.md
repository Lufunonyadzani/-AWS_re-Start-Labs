
---

# Bash Shell Scripting Challenge Lab 

## Lab Objective

The purpose of this challenge lab is to demonstrate the ability to:

* Connect to an Amazon Linux EC2 instance using SSH
* Create a Bash script using automation
* Generate files dynamically without hard-coding values
* Validate results using Linux commands

---

##  Task Description

The Bash script must:

* Create **25 empty (0 KB) files**
* Use a **name + number** naming format
  Example: `lufuno1`, `lufuno2`, `lufuno3`, ...
* Automatically detect the **last existing file number**
* On each execution, the **next batch of 25 files** is created

---

##  Step 1: Create the Script File


create_files.sh
<img width="1366" height="768" alt="image 1" src="https://github.com/user-attachments/assets/f27ff630-5f00-4c43-854d-a635d5b14320" />


---

## Full Bash Script

<img width="1366" height="768" alt="image 2" src="https://github.com/user-attachments/assets/7764661f-5c7e-4eae-9528-a0e7a1879cb7" />

```

```
### Step 2: Make the Script Executable

<img width="1366" height="768" alt="image 3" src="https://github.com/user-attachments/assets/0f4f7dbc-0556-48e6-b768-aa807b4fd0be" />

```
```
### Step 3: Run the script (First Execution)

```bash
./create_files.sh
```
### Step 4:Validate with Long Listing
<img width="1366" height="768" alt="image 4" src="https://github.com/user-attachments/assets/ec9db643-4683-42db-aaca-8389d80b0a67" />


This confirms:

* File quantity
* File naming structure
* File size (0 KB)

---





## Key Concepts Demonstrated

* Bash scripting
* File automation
* Conditional logic
* Loops
* Linux file permissions
* Directory validation

---


