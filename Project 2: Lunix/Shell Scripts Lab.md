

# Bash Shell Lab

## Overview

This lab demonstrates the use of Bash shell commands on an Amazon Linux EC2 instance. The objectives include:

* Creating and working with an alias for backing up directories
* Exploring and updating the `PATH` environment variable

---


## Steps Performed

### Task 1: Connect to EC2 Instance

* Download the `.pem` key file and set permissions:

  ```bash
  chmod 400 labsuser.pem
  ```
* SSH into the instance:

  ```bash
  ssh -i labsuser.pem ec2-user@<public-ip>
  ```
  <img width="1366" height="768" alt="image 1" src="https://github.com/user-attachments/assets/0f3774aa-2a2e-42d1-8d00-1f4266d9525c" />


### Task 2: Create Backup Alias

* Confirm the current directory:

  ```bash
  pwd
  ```
* Create a backup file:
    ```bash
  touch backup.sh
  ```
  
* changing the file privileges to make backup.sh be executable, :

  ```bash
   sudo chmod 755 backup.sh
  ```
*Running  backup.sh file:

  ```bash
  vi backup.sh

  ```

### Task 3: Editing the file
* By pressing i and enter:

  ```bash
   DAY="$(date +%Y_%m_%d)"                                                       
   BACKUP="/home/$USER/backups/$DAY-backup-CompanyA.tar.gz"                             
   tar -csvpzf $BACKUP /home/$USER/CompanyA  
  ```
  <img width="1366" height="768" alt="image 2" src="https://github.com/user-attachments/assets/98d158f1-067d-4c39-84f0-c59fd4f23484" />

* Run the script:

  ```bash
   backup.sh  ```
* Add the folder to `PATH` for easier execution:

  ```bash
  PATH=$PATH:/home/ec2-user/CompanyA/bin
  ```

---

## Key Learnings

* Aliases simplify repetitive tasks, like backups, in Bash.
* The `PATH` variable controls where Linux searches for executables.
* Scripts not in `PATH` require the full path to execute.
* `tar` can compress directories into `.tar.gz` archives for backup.

---
